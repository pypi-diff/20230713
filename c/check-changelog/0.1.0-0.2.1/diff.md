# Comparing `tmp/check_changelog-0.1.0-py3-none-any.whl.zip` & `tmp/check_changelog-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6090 bytes, number of entries: 9
+Zip file size: 6596 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      160 b- defN 16-Jan-01 00:00 check_changelog/__init__.py
--rw-rw-r--  2.0 unx     1084 b- defN 16-Jan-01 00:00 check_changelog/__main__.py
--rw-rw-r--  2.0 unx     5419 b- defN 16-Jan-01 00:00 check_changelog/changelog.py
+-rw-rw-r--  2.0 unx     1269 b- defN 16-Jan-01 00:00 check_changelog/__main__.py
+-rw-rw-r--  2.0 unx     6616 b- defN 16-Jan-01 00:00 check_changelog/changelog.py
 -rw-rw-r--  2.0 unx       21 b- defN 16-Jan-01 00:00 check_changelog/__version__.py
-?rw-------  2.0 unx       65 b- defN 16-Jan-01 00:00 check_changelog-0.1.0.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 check_changelog-0.1.0.dist-info/WHEEL
-?rw-------  2.0 unx     2855 b- defN 16-Jan-01 00:00 check_changelog-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 check_changelog-0.1.0.dist-info/licenses/LICENSE
-?rw-------  2.0 unx      775 b- defN 16-Jan-01 00:00 check_changelog-0.1.0.dist-info/RECORD
-9 files, 11569 bytes uncompressed, 4738 bytes compressed:  59.0%
+?rw-------  2.0 unx       65 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/WHEEL
+?rw-------  2.0 unx     3245 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/licenses/LICENSE
+?rw-------  2.0 unx      775 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/RECORD
+9 files, 13341 bytes uncompressed, 5244 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: check_changelog/changelog.py
 Comment: 
 
 Filename: check_changelog/__version__.py
 Comment: 
 
-Filename: check_changelog-0.1.0.dist-info/entry_points.txt
+Filename: check_changelog-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: check_changelog-0.1.0.dist-info/WHEEL
+Filename: check_changelog-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: check_changelog-0.1.0.dist-info/METADATA
+Filename: check_changelog-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: check_changelog-0.1.0.dist-info/licenses/LICENSE
+Filename: check_changelog-0.2.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: check_changelog-0.1.0.dist-info/RECORD
+Filename: check_changelog-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## check_changelog/__main__.py

```diff
@@ -14,15 +14,15 @@
 import logging
 import sys
 
 import pydevkit.log.config  # noqa: F401
 from pydevkit.argparse import ArgumentParser
 
 from . import __version__
-from .changelog import ChangelogError, check_changelog
+from .changelog import CLNotFoundError, CLSyntaxError, check_changelog
 
 log = logging.getLogger(__name__)
 
 
 def get_args():
     p = ArgumentParser(help=__doc__, version=__version__)
     p.add_argument(
@@ -37,16 +37,23 @@
     if unknown_args:
         log.warning("Unknown arguments: %s", unknown_args)
         sys.exit(1)
     try:
         text = open(args.file, "r").read()
         check_changelog(text)
         sys.exit(0)
-    except ChangelogError as exp:
-        log.error("%s:%d: %s", args.file, exp.lineno, exp.message)
+    except (CLSyntaxError, CLNotFoundError) as exp:
+        log.error(
+            "%s:%d: %s; got '%s'%s",
+            args.file,
+            exp.lineno,
+            exp.msg,
+            exp.content,
+            "; " + exp.msg_extra if exp.msg_extra else "",
+        )
     except Exception as exp:
         log.error("%s", exp)
     sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

## check_changelog/changelog.py

```diff
@@ -14,51 +14,102 @@
 logging.getLogger("markdown_it").setLevel(logging.INFO)
 
 
 class Tokens(list):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.idx = 0
+        self.lineno = 0
+        self.content = ""
 
     def get(self):
-        log.debug("token: %s", self[self.idx])
+        if self.is_empty():
+            return None
+        t = self[self.idx]
+        if log.getEffectiveLevel() == logging.DEBUG:
+            self.prn_token(t)
+        if t.map:
+            self.lineno = t.map[0]
+            self.content = t.content
         return self[self.idx]
 
     def next(self):  # noqa: A003
+        if self.is_empty():
+            return None
         self.idx += 1
         return self.get()
 
     def is_empty(self):
-        return self.idx == len(self)
+        return self.idx >= len(self)
 
     def consume_until(self, func):
         log.debug("consume_until")
         while True:
             t = self.get()
             self.next()
             if func(t):
                 return
 
+    def prn_token(self, t, lvl=0):
+        attrs = ["type", "tag", "map", "content"]
+        rc = {}
+        for a in attrs:
+            rc[a] = getattr(t, a, None)
+        log.debug("token[%d]: %s%s", self.idx, " " * lvl, rc)
+        if not t.children:
+            return
+        lvl += 2
+        for c in t.children:
+            self.prn_token(c, lvl)
+
 
 tokens = None
 
 
+class CLError(Exception):
+    def __init__(self, msg, token=None, msg_extra=""):
+        self.token = token
+        self.lineno = tokens.lineno
+        self.content = tokens.content
+        self.msg = msg
+        self.msg_extra = msg_extra
+        log.debug("%s: %d: %s", self.__class__.__name__, self.lineno, self.msg)
+
+    def __str__(self):
+        return self.msg
+
+
+class CLSyntaxError(CLError):
+    pass
+
+
+class CLNotFoundError(CLError):
+    pass
+
+
+class CLPartiallyFoundError(CLError):
+    pass
+
+
 def run(func, narg):
+    log.debug("func %s, narg %s", func, narg)
     count = 0
     while True:
         try:
             func()
-        except ChangelogError:
+        except CLSyntaxError:
             raise
-        except Exception:
+        except CLNotFoundError as exp:
             if narg == "?" or narg == "*":
                 return
             if narg == "+" and count > 0:
                 return
-            raise
+            if count == 0:
+                raise
+            raise CLPartiallyFoundError(exp.msg, exp.token) from exp
         count += 1
         if narg == "?":
             return
         if isinstance(narg, int) and count == narg:
             return
         if (narg == "+" or narg == "*") and count > len(tokens):
             return
@@ -74,32 +125,18 @@
     "h3": "heading",
     "ul": "bullet_list",
     "li": "list_item",
     "p": "paragraph",
 }
 
 
-class ChangelogError(Exception):
-    def __init__(self, token, msg, msg_extra=""):
-        if token.content:
-            msg += ": " + token.content
-        if msg_extra:
-            msg += "; " + msg_extra
-        self.message = msg
-        self.lineno = token.map[0] if token.map else -1
-        self.token = token
-
-    def __str__(self):
-        return self.message
-
-
 def do_item(tag, msg, validate):
     t = tokens.get()
-    if not (t.type == tag2type[tag] + "_open" and t.tag == tag):
-        raise Exception(msg)
+    if not (t and t.type == tag2type[tag] + "_open" and t.tag == tag):
+        raise CLNotFoundError(msg, t)
     if validate:
         validate(msg)
     tokens.consume_until(
         lambda x: x.tag == tag
         and x.type == tag2type[tag] + "_close"
         and x.level == t.level
     )
@@ -109,15 +146,16 @@
     log.debug("%s", func_name())
     msg = "expected 'Changelog'"
 
     def _validate(msg):
         t = tokens.next()
         log.info("title: %s", t.content)
         if t.content != "Changelog":
-            raise ChangelogError(t, "bad title", msg)
+            m1 = "bad title"
+            raise CLSyntaxError(m1, t, msg)
 
     do_item("h1", msg, _validate)
 
 
 def notes():
     log.debug("%s", func_name())
     do_item("p", "", None)
@@ -127,79 +165,86 @@
     log.debug("%s", func_name())
     msg = "expected '[Unreleased]' or '[ver] - YYYY-MM-DD'"
     msgr = "expected '[ver] - YYYY-MM-DD'"
 
     def _validate(msg):
         t = tokens.next()
         log.info("release: %s", t.content)
-        kids_no_unreleased = 3
-        kids_no_released = 4
+        kids_num_unreleased = 3
+        kids_num_released = 4
         if not (
-            len(t.children) >= kids_no_unreleased
+            len(t.children) >= kids_num_unreleased
             and t.children[0].type == "link_open"
             and t.children[0].attrs.get("href")
         ):
-            raise ChangelogError(t, "no link for release")
+            m1 = "no link for release"
+            raise CLSyntaxError(m1, t)
         rname = t.children[1].content
         log.debug("rname '%s'", rname)
         if rname is None:
-            raise ChangelogError(t, "bad release title", msg)
+            m1 = "bad release title"
+            raise CLSyntaxError(m1, t, msg)
 
         if rname == "Unreleased":
-            if len(t.children) != kids_no_unreleased:
-                raise ChangelogError(t, "bad release title", msg)
+            if len(t.children) != kids_num_unreleased:
+                m1 = "bad release title"
+                raise CLSyntaxError(m1, t, msg)
             return
-        if len(t.children) != kids_no_released:
-            raise ChangelogError(t, "bad release title", msg)
+        if len(t.children) != kids_num_released:
+            m1 = "bad release title"
+            raise CLSyntaxError(m1, t, msg)
         rdate = t.children[3].content
         log.debug("rdate '%s'", rdate)
         if not re.search("^ - \\d\\d\\d\\d-\\d\\d-\\d\\d$", rdate):
-            raise ChangelogError(t, "bad release date", msgr)
+            m1 = "bad release date"
+            raise CLSyntaxError(m1, t, msgr)
 
     do_item("h2", msg, _validate)
 
 
-def change_type():
+def change():
     log.debug("%s", func_name())
-    msg = "expecting '### <Change Type>'"
-
-    def _validate(msg):
-        t = tokens.next()
-        log.info("change type: %s", t.content)
-        msg += "; got '%s'" % t.content
-        cnames = ["Added", "Changed", "Deprecated", "Removed", "Fixed", "Security"]
-        if t.content not in cnames:
-            raise ChangelogError(
-                t, "bad change type", "expected one of %s" % cnames
-            )
-
-    do_item("h3", msg, _validate)
+    msg = "expecting list item"
+    do_item("li", msg, None)
 
 
 def change_list():
     log.debug("%s", func_name())
     msg = "expecting unordered list"
 
     def _validate(msg):  # noqa: ARG001
         tokens.next()
         run(change, narg="+")
 
     do_item("ul", msg, _validate)
 
 
-def change():
+def change_type():
     log.debug("%s", func_name())
-    msg = "expecting list item"
-    do_item("li", msg, None)
+    msg = "expecting '### <Change Type>'"
+
+    def _validate(msg):
+        t = tokens.next()
+        log.info("change type: %s", t.content)
+        msg += "; got '%s'" % t.content
+        cnames = ["Added", "Changed", "Deprecated", "Removed", "Fixed", "Security"]
+        if t.content not in cnames:
+            m1 = "bad change type"
+            raise CLSyntaxError(m1, t, "expected one of %s" % cnames)
+
+    do_item("h3", msg, _validate)
 
 
 def change_block():
     log.debug("%s", func_name())
     run(change_type, narg=1)
-    run(change_list, narg="+")
+    try:
+        run(change_list, narg="+")
+    except CLNotFoundError as exp:
+        raise CLSyntaxError(exp.msg, exp.token) from exp
 
 
 def release():
     log.debug("%s", func_name())
     run(release_header, narg=1)
     run(notes, narg="*")
     run(change_block, narg="*")
@@ -213,8 +258,9 @@
 
     run(title, narg=1)
     run(notes, narg="*")
     run(release, narg="+")
 
     if tokens.is_empty() or tokens.get().tag == "hr":
         return
-    raise ChangelogError(tokens.get(), "out of context")
+    msg = "out of context"
+    raise CLSyntaxError(msg, tokens.get())
```

## check_changelog/__version__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.0'
+__version__ = '0.2.1'
```

## Comparing `check_changelog-0.1.0.dist-info/METADATA` & `check_changelog-0.2.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-changelog
-Version: 0.1.0
+Version: 0.2.1
 Summary: check that changelog conforms to 'Keep A Changelog' style
 Author-email: Anatoly Asviyan <aanatoly@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -26,29 +26,29 @@
 [![pkg - license][pkg-license]][pkg-link]
 
 ---
 
 check that changelog conforms to [Keep A Changelog][kacl] and
 [Common Changelog][ccl] styles.
 
-Main fetaures:
+Main features:
  * check that changelog conforms to [Keep A Changelog][kacl] style
- * allow release notes. Add them between release header and change list
+ * allow release notes. Add them between the release header and change list
    ([Common Changelog][ccl] addition)
 
    ```markdown
    ## [1.0.0] - 2023-05-05
    Release notes
 
    ### Added
     - add feature ...
    ```
 
  * allow custom footer to keep things from being verified. Useful for legal
-   notes, text used by other scripts, html comments etc
+   notes, text used by other scripts, HTML comments, etc
 
    ```markdown
    -----
    Linter will ignore this section.
    <!--- message for some script -->
    [my site]: http://mysite.com
    ```
@@ -61,20 +61,40 @@
 
 ## Installation
 
 ```sh
 pip install check-changelog
 ```
 
+## Usage
+From command line
+
+```sh
+# check CHANGELOG.md in a current dir
+check-changelog
+# check specific CHANGELOG.md
+check-changelog -f path/to/changelog.md
+```
+
+As a [pre-commit](https://pre-commit.com/) hook.
+Add this section to your `.pre-commit-config.yaml`
+
+```yml
+- repo: https://github.com/aanatoly/check-changelog
+  rev: '0.2.1'
+  hooks:
+    - id: check-changelog
+```
+
 ## Alternatives
-`check-changelog` is a minimalistic tool by design. It checks Changelog
+`check-changelog` is a minimalistic tool by design. It checks the Changelog
 structure and does nothing else.
 
-If you are looking for more, check [python-kacl][py-kacl]. It is feature-rich tool
-capable of linting, fixing errors and automating Changelog maintenance.
+If you are looking for more, check [python-kacl][py-kacl]. It is a feature-rich tool
+capable of linting, fixing errors, and automating Changelog maintenance.
 
 ## Development
 See [development](docs/devel.md) doc
 
 [kacl]: https://keepachangelog.com/en/ "Keep a Changelog"
 [ccl]: https://common-changelog.org/ "Common Changelog"
 [py-kacl]: https://gitlab.com/schmieder.matthias/python-kacl
```

## Comparing `check_changelog-0.1.0.dist-info/licenses/LICENSE` & `check_changelog-0.2.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

