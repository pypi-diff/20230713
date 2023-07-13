# Comparing `tmp/mathbib-0.7.3.tar.gz` & `tmp/mathbib-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.7.3.tar", max compression
+gzip compressed data, was "mathbib-0.7.4.tar", max compression
```

## Comparing `mathbib-0.7.3.tar` & `mathbib-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.3/LICENSE
--rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.3/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.3/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.3/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.3/mathbib/bibtex.py
--rw-r--r--   0        0        0     2844 2023-07-10 14:46:42.470944 mathbib-0.7.3/mathbib/citegen.py
--rw-r--r--   0        0        0    10823 2023-06-04 07:21:28.332360 mathbib-0.7.3/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.3/mathbib/partition.py
--rw-r--r--   0        0        0     9441 2023-06-04 07:04:03.110810 mathbib-0.7.3/mathbib/record.py
--rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.3/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.3/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.3/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.3/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.3/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.3/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.3/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.3/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.3/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     6688 2023-06-04 07:43:41.660653 mathbib-0.7.3/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.3/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.3/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.3/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.3/mathbib/term.py
--rw-r--r--   0        0        0      953 2023-07-10 14:47:12.088560 mathbib-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.4/LICENSE
+-rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.4/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.4/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.4/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.4/mathbib/bibtex.py
+-rw-r--r--   0        0        0     3326 2023-07-13 10:48:13.319332 mathbib-0.7.4/mathbib/citegen.py
+-rw-r--r--   0        0        0    10831 2023-07-13 10:33:28.789417 mathbib-0.7.4/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.4/mathbib/partition.py
+-rw-r--r--   0        0        0     9500 2023-07-13 10:44:15.098639 mathbib-0.7.4/mathbib/record.py
+-rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.4/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.4/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.4/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.4/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.4/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.4/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.4/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.4/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.4/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     6688 2023-06-04 07:43:41.660653 mathbib-0.7.4/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.4/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.4/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.4/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.4/mathbib/term.py
+-rw-r--r--   0        0        0      953 2023-07-13 10:48:54.865737 mathbib-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.4/PKG-INFO
```

### Comparing `mathbib-0.7.3/LICENSE` & `mathbib-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/README.md` & `mathbib-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/bibtex.py` & `mathbib-0.7.4/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/citegen.py` & `mathbib-0.7.4/mathbib/citegen.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Iterable, Final, Optional
     from .session import CLISession
+    from .record import KeyId
 
+from collections import defaultdict
 from itertools import chain
 from pathlib import Path
 import re
 
 from .record import ArchiveRecord
 from .term import TermWrite
 from .remote import KeyIdError
@@ -71,13 +73,25 @@
 
     citekeys = get_citekeys_from_paths(*paths)
 
     records_or_none = (
         citekey_to_record(session, citekey, session.alias) for citekey in citekeys
     )
 
-    return (record for record in records_or_none if record is not None)
+    out = [record for record in records_or_none if record is not None]
+
+    # check if there are multiple keys for the same record
+    multiple_citekeys: dict[KeyId, list[str]] = defaultdict(list)
+
+    for record in out:
+        multiple_citekeys[record.priority_key()].append(record.bib_id())
+
+    for priority_key, bib_ids in multiple_citekeys.items():
+        if len(bib_ids) > 1:
+            TermWrite.warn(f"Multiple citekeys for record '{priority_key}': {bib_ids}")
+
+    return out
 
 
 def generate_biblatex(session: CLISession, *paths: Path) -> str:
     """Generate the biblatex file associated with the citations inside a given file."""
     return session.bibtex_handler.write_records(get_file_records(session, *paths))
```

### Comparing `mathbib-0.7.3/mathbib/command.py` & `mathbib-0.7.4/mathbib/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,32 +76,32 @@
     metavar="TEXFILE",
 )
 alias_argument = click.argument("alias_name", type=str, metavar="ALIAS")
 
 
 @click.group()
 @click.version_option(prog_name="mbib (mathbib)")
-@click.option("--cache/--no-cache", "cache", default=True, help="Use local cache")
+@click.option("--cache/--no-cache", "cache", default=True, help="Use local cache.")
 @click.option(
-    "--remote/--no-remote", "remote", default=True, help="Access remote records"
+    "--remote/--no-remote", "remote", default=True, help="Use remote records."
 )
-@click.option("--debug/--no-debug", "debug", default=False, help="Debug mode")
+@click.option("--debug/--no-debug", "debug", default=False, help="Debug mode.")
 @click.option(
     "--alias",
     "-a",
     "alias_file",
     default=xdg_data_home() / "mathbib" / "alias.toml",
-    help="Alias file",
+    help="Use alias file.",
     type=click.Path(file_okay=True, dir_okay=False, readable=True, path_type=Path),
 )
 @click.option(
-    "--relation-file",
+    "--relation",
     "relation_file",
     default=xdg_data_home() / "mathbib" / "relations.json",
-    help="Alias file",
+    help="Use relation file.",
     type=click.Path(file_okay=True, dir_okay=False, readable=True, path_type=Path),
 )
 @click.pass_context
 def cli(
     ctx: click.Context,
     cache: bool,
     remote: bool,
```

### Comparing `mathbib-0.7.3/mathbib/partition.py` & `mathbib-0.7.4/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/record.py` & `mathbib-0.7.4/mathbib/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,27 +195,30 @@
             (
                 keyid.toml_record(warn=True)
                 for keyid in reversed(self.record.resolve().keys())
             ),
             {},
         )
 
+    def bib_id(self) -> str:
+        return str(self.keyid) if self.keyid.alias is None else self.keyid.alias
+
     def as_bibtex(self) -> dict:
         joint_record = self.as_joint_record()
 
         eprint_keyid = self.priority_key()
         eprint = {
             "eprint": eprint_keyid.identifier,
             "eprinttype": str(eprint_keyid.key),
         }
 
         captured = {k: v for k, v in joint_record.items() if k in CAPTURED}
 
         special = {
-            "ID": str(self.keyid) if self.keyid.alias is None else self.keyid.alias,
+            "ID": self.bib_id(),
             "ENTRYTYPE": joint_record["bibtype"],
         }
         local_bibtex = self.get_local_bibtex()
 
         if "authors" in local_bibtex.keys():
             special["author"] = " and ".join(local_bibtex.pop("authors"))
```

### Comparing `mathbib-0.7.3/mathbib/remote/__init__.py` & `mathbib-0.7.4/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/remote/arxiv.py` & `mathbib-0.7.4/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/remote/doi.py` & `mathbib-0.7.4/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/remote/error.py` & `mathbib-0.7.4/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/remote/isbn.py` & `mathbib-0.7.4/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/remote/ol.py` & `mathbib-0.7.4/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/remote/utils.py` & `mathbib-0.7.4/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/remote/zbl.py` & `mathbib-0.7.4/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/remote/zbmath.py` & `mathbib-0.7.4/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/request.py` & `mathbib-0.7.4/mathbib/request.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/resources/journal_abbrevs.json` & `mathbib-0.7.4/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/session.py` & `mathbib-0.7.4/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/mathbib/term.py` & `mathbib-0.7.4/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.3/pyproject.toml` & `mathbib-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [virtualenv]
 in-project = true
 
 [tool.poetry]
 name = "mathbib"
-version = "0.7.3"
+version = "0.7.4"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.7.3/PKG-INFO` & `mathbib-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.7.3
+Version: 0.7.4
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

