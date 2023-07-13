# Comparing `tmp/redlines-0.3.0.tar.gz` & `tmp/redlines-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redlines-0.3.0.tar", max compression
+gzip compressed data, was "redlines-0.4.0.tar", max compression
```

## Comparing `redlines-0.3.0.tar` & `redlines-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-10 14:46:40.787757 redlines-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2679 2023-05-10 14:46:40.787757 redlines-0.3.0/README.md
--rw-r--r--   0        0        0      611 2023-05-10 14:46:40.787757 redlines-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-10 14:46:40.787757 redlines-0.3.0/redlines/__init__.py
--rw-r--r--   0        0        0     7824 2023-05-10 14:46:40.787757 redlines-0.3.0/redlines/redlines.py
--rw-r--r--   0        0        0     3392 1970-01-01 00:00:00.000000 redlines-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-13 15:40:38.067880 redlines-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     4184 2023-07-13 15:40:38.067880 redlines-0.4.0/README.md
+-rw-r--r--   0        0        0      719 2023-07-13 15:40:38.067880 redlines-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-07-13 15:40:38.067880 redlines-0.4.0/redlines/__init__.py
+-rw-r--r--   0        0        0     1857 2023-07-13 15:40:38.067880 redlines-0.4.0/redlines/cli.py
+-rw-r--r--   0        0        0    10281 2023-07-13 15:40:38.067880 redlines-0.4.0/redlines/redlines.py
+-rw-r--r--   0        0        0     5017 1970-01-01 00:00:00.000000 redlines-0.4.0/PKG-INFO
```

### Comparing `redlines-0.3.0/LICENSE.txt` & `redlines-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redlines-0.3.0/README.md` & `redlines-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 The library gives a result of:
 
     The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog.
 
 Which is rendered like this:
 
-The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog.
+> The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog.
 
 ## Install
 
 ```shell
 pip install redlines
 ```
 
@@ -62,28 +62,51 @@
 
 assert (
         test.compare("The quick brown fox jumps over the dog.")
         == "The quick brown fox jumps over the <del>lazy </del>dog."
 )
 ```
 
+Redlines also features a simple command line tool `redlines` to visualise the differences in text in the terminal.
+
+```
+ Usage: redlines text [OPTIONS] SOURCE TEST                                                                                                                                                                                                   
+                                                                                                                                                                                                                                              
+ Compares the strings SOURCE and TEST and produce a redline in the terminal. 
+```
+
+### Custom styling in markdown
+
+By default, markdown output is styled in "red_green", like the following:
+
+> "The quick brown fox <span style='color:red;font-weight:700;text-decoration:line-through;'>jumps
+> over </span><span style='color:green;font-weight:700;'>walks past </span>the lazy dog."
+
+Set the `markdown_style` option in the constructor or compare function to change the styling.
+The available styles are "red"" and "none".
+
+You can also use css classes to provide custom styling by setting `markdown_style` as "custom_css".
+Insertions and deletions are now styled using the "redline-inserted" and "redline-deleted" CSS classes.
+You can also set your own CSS classes by specifying the name of the CSS class in the options "ins_class"
+and "del_class" respectively in the constructor or compare function.
+
 ## Uses
 
 * View and mark changes in legislation: [PLUS Explorer](https://houfu-plus-explorer.streamlit.app/)
 * Visualise changes after ChatGPT transforms a
   text: [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)
   Lesson 6
 
 ## Roadmap / Contributing
 
 Please feel free to post issues and comments. I work on this in my free time, so please excuse lack of activity.
 
 ### Nice things to do
 
-* Style the way changes are presented
+* <s>Style the way changes are presented</s>
 * Other than Markdown, have other output formats (HTML? PDF?)
 * Associate changes with an author
 * Show different changes by different authors or times.
 
 If this was useful to you, please feel free to [contact me](mailto:houfu@lovelawrobots.com)!
 
 ## License
```

### Comparing `redlines-0.3.0/pyproject.toml` & `redlines-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 [tool.poetry]
 name = "redlines"
-version = "0.3.0"
+version = "0.4.0"
 description = "Compare text, and produce human-readable differences or deltas which look like track changes in Microsoft Word."
 authors = ["houfu <houfu@lovelawrobots.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/houfu/redlines"
 repository = "https://github.com/houfu/redlines"
 
 [tool.poetry.dependencies]
 python = "<4.0,>=3.8"
+rich = "^13.3.5"
+click = "^8.1.3"
+rich-click = "^1.6.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 pytest-sugar = "^0.9.4"
 pytest-cov = "^3.0.0"
 tox = "^3.24.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+redlines = 'redlines.cli:cli'
```

### Comparing `redlines-0.3.0/redlines/redlines.py` & `redlines-0.4.0/redlines/redlines.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import re
 
+from rich.text import Text
+
 # This regular expression matches a group of characters that can include any character except for parentheses
 # and whitespace characters (which include spaces, tabs, and line breaks) or any character
 # that is a parenthesis or punctuation mark (.?!-).
 # The group can also include any whitespace characters that follow these characters.
 # Breaking it down further:
 
 #    ( and ) indicate a capturing group
@@ -129,29 +131,71 @@
         matcher = SequenceMatcher(None, self._seq1, self._seq2)
         return matcher.get_opcodes()
 
     @property
     def output_markdown(self) -> str:
         """Returns the delta in Markdown format."""
         result = []
-        style = "red"
+
+        # default_style = "red_green"
+
+        md_styles = {
+            "ins": (
+                f"span style='color:green;font-weight:700;'",
+                "span",
+            ),
+            "del": (
+                f"span style='color:red;font-weight:700;text-decoration:line-through;'",
+                "span",
+            ),
+        }
 
         if self.options.get("markdown_style"):
             style = self.options["markdown_style"]
 
-        if style == "none":
-            md_styles = {"ins": ("ins", "ins"), "del": ("del", "del")}
-        elif "red":
-            md_styles = {
-                "ins": ('span style="color:red;font-weight:700;"', "span"),
-                "del": (
-                    'span style="color:red;font-weight:700;text-decoration:line-through;"',
-                    "span",
-                ),
-            }
+            if style == "none":
+                md_styles = {"ins": ("ins", "ins"), "del": ("del", "del")}
+            elif style == "red":
+                md_styles = {
+                    "ins": (
+                        f"span style='color:red;font-weight:700;'",
+                        "span",
+                    ),
+                    "del": (
+                        f"span style='color:red;font-weight:700;text-decoration:line-through;'",
+                        "span",
+                    ),
+                }
+            elif style == "custom_css":
+                ins_class = (
+                    self.options["ins_class"]
+                    if "ins_class" in self.options
+                    else "redline-inserted"
+                )
+                del_class = (
+                    self.options["del_class"]
+                    if "del_class" in self.options
+                    else "redline-deleted"
+                )
+
+                elem_attributes = {
+                    "ins": f"class='{ins_class}'",
+                    "del": f"class='{del_class}'",
+                }
+
+                md_styles = {
+                    "ins": (
+                        f"span {elem_attributes['ins']}",
+                        "span",
+                    ),
+                    "del": (
+                        f"span {elem_attributes['del']}",
+                        "span",
+                    ),
+                }
 
         for tag, i1, i2, j1, j2 in self.opcodes:
             if tag == "equal":
                 temp_str = "".join(self._seq1[i1:i2])
                 temp_str = re.sub("¶ ", "\n\n", temp_str)
                 # here we use '¶ ' instead of ' ¶ ', because the leading space will be included in the previous token,
                 # according to tokenizer = re.compile(r"((?:[^()\s]+|[().?!-])\s*)")
@@ -184,14 +228,40 @@
                     )
                     result.append("\n\n")
                 if len(splits) > 0:
                     result.pop()
 
         return "".join(result)
 
+    @property
+    def output_rich(self) -> Text:
+        """Returns the delta in text with colors/style for the console."""
+        console_text = Text()
+
+        for tag, i1, i2, j1, j2 in self.opcodes:
+            if tag == "equal":
+                temp_str = "".join(self._seq1[i1:i2])
+                temp_str = re.sub("¶ ", "\n\n", temp_str)
+                console_text.append(temp_str)
+            elif tag == "insert":
+                temp_str = "".join(self._seq2[j1:j2])
+                splits = re.split("¶ ", temp_str)
+                for split in splits:
+                    console_text.append(split, "green")
+            elif tag == "delete":
+                console_text.append("".join(self._seq1[i1:i2]), "red strike")
+            elif tag == "replace":
+                console_text.append("".join(self._seq1[i1:i2]), "red strike")
+                temp_str = "".join(self._seq2[j1:j2])
+                splits = re.split("¶ ", temp_str)
+                for split in splits:
+                    console_text.append(split, "green")
+
+        return console_text
+
     def compare(self, test: str | None = None, output: str = "markdown", **options):
         """
         Compare `test` with `source`, and produce a delta in a format specified by `output`.
 
         :param test: Optional test string to compare. If None, uses the test string provided during initialisation.
         :param output: The format which the delta should be produced. Currently, only "markdown" is supported
         :return: The delta in the format specified by `output`.
```

### Comparing `redlines-0.3.0/PKG-INFO` & `redlines-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: redlines
-Version: 0.3.0
+Version: 0.4.0
 Summary: Compare text, and produce human-readable differences or deltas which look like track changes in Microsoft Word.
 Home-page: https://github.com/houfu/redlines
 License: MIT
 Author: houfu
 Author-email: houfu@lovelawrobots.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Project-URL: Repository, https://github.com/houfu/redlines
 Description-Content-Type: text/markdown
 
 # Redlines
 ![Repository banner image](repository-open-graph.png)
 
 `Redlines` produces a Markdown text showing the differences between two strings/text. The changes are represented with
@@ -38,15 +41,15 @@
 
 The library gives a result of:
 
     The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog.
 
 Which is rendered like this:
 
-The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog.
+> The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog.
 
 ## Install
 
 ```shell
 pip install redlines
 ```
 
@@ -80,28 +83,51 @@
 
 assert (
         test.compare("The quick brown fox jumps over the dog.")
         == "The quick brown fox jumps over the <del>lazy </del>dog."
 )
 ```
 
+Redlines also features a simple command line tool `redlines` to visualise the differences in text in the terminal.
+
+```
+ Usage: redlines text [OPTIONS] SOURCE TEST                                                                                                                                                                                                   
+                                                                                                                                                                                                                                              
+ Compares the strings SOURCE and TEST and produce a redline in the terminal. 
+```
+
+### Custom styling in markdown
+
+By default, markdown output is styled in "red_green", like the following:
+
+> "The quick brown fox <span style='color:red;font-weight:700;text-decoration:line-through;'>jumps
+> over </span><span style='color:green;font-weight:700;'>walks past </span>the lazy dog."
+
+Set the `markdown_style` option in the constructor or compare function to change the styling.
+The available styles are "red"" and "none".
+
+You can also use css classes to provide custom styling by setting `markdown_style` as "custom_css".
+Insertions and deletions are now styled using the "redline-inserted" and "redline-deleted" CSS classes.
+You can also set your own CSS classes by specifying the name of the CSS class in the options "ins_class"
+and "del_class" respectively in the constructor or compare function.
+
 ## Uses
 
 * View and mark changes in legislation: [PLUS Explorer](https://houfu-plus-explorer.streamlit.app/)
 * Visualise changes after ChatGPT transforms a
   text: [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)
   Lesson 6
 
 ## Roadmap / Contributing
 
 Please feel free to post issues and comments. I work on this in my free time, so please excuse lack of activity.
 
 ### Nice things to do
 
-* Style the way changes are presented
+* <s>Style the way changes are presented</s>
 * Other than Markdown, have other output formats (HTML? PDF?)
 * Associate changes with an author
 * Show different changes by different authors or times.
 
 If this was useful to you, please feel free to [contact me](mailto:houfu@lovelawrobots.com)!
 
 ## License
```

