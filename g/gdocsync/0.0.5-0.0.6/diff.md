# Comparing `tmp/gdocsync-0.0.5.tar.gz` & `tmp/gdocsync-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdocsync-0.0.5.tar", last modified: Thu Jul 13 04:20:40 2023, max compression
+gzip compressed data, was "gdocsync-0.0.6.tar", last modified: Thu Jul 13 04:55:08 2023, max compression
```

## Comparing `gdocsync-0.0.5.tar` & `gdocsync-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:20:40.773572 gdocsync-0.0.5/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.5/LICENSE
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 04:20:40.773643 gdocsync-0.0.5/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.5/README.rst
--rw-r--r--   0 peterdemin   (503) staff       (20)    21043 2023-07-13 03:49:48.000000 gdocsync-0.0.5/pyproject.toml
--rw-r--r--   0 peterdemin   (503) staff       (20)      757 2023-07-13 04:20:40.773913 gdocsync-0.0.5/setup.cfg
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:20:40.769523 gdocsync-0.0.5/src/
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:20:40.772563 gdocsync-0.0.5/src/gdocsync/
--rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.5/src/gdocsync/__init__.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      333 2023-07-13 02:07:34.000000 gdocsync-0.0.5/src/gdocsync/cli.py
--rw-r--r--   0 peterdemin   (503) staff       (20)       69 2023-07-10 05:17:11.000000 gdocsync-0.0.5/src/gdocsync/constants.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     3262 2023-07-13 02:41:29.000000 gdocsync-0.0.5/src/gdocsync/docs_importer.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     3124 2023-07-13 02:23:07.000000 gdocsync-0.0.5/src/gdocsync/google_drive_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1055 2023-07-13 04:17:52.000000 gdocsync-0.0.5/src/gdocsync/html_cleaner.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1366 2023-07-13 02:31:07.000000 gdocsync-0.0.5/src/gdocsync/johnny_decimal.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      760 2023-07-13 02:09:05.000000 gdocsync-0.0.5/src/gdocsync/pandoc_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.5/src/gdocsync/regexes.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      823 2023-07-10 05:09:34.000000 gdocsync-0.0.5/src/gdocsync/shelve_cache.py
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:20:40.773462 gdocsync-0.0.5/src/gdocsync.egg-info/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      541 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/SOURCES.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/dependency_links.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/entry_points.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       78 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/requires.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/top_level.txt
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:55:08.387510 gdocsync-0.0.6/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.6/LICENSE
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 04:55:08.387569 gdocsync-0.0.6/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.6/README.rst
+-rw-r--r--   0 peterdemin   (503) staff       (20)    21043 2023-07-13 03:49:48.000000 gdocsync-0.0.6/pyproject.toml
+-rw-r--r--   0 peterdemin   (503) staff       (20)      757 2023-07-13 04:55:08.387844 gdocsync-0.0.6/setup.cfg
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:55:08.384156 gdocsync-0.0.6/src/
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:55:08.386654 gdocsync-0.0.6/src/gdocsync/
+-rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.6/src/gdocsync/__init__.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      393 2023-07-13 04:36:15.000000 gdocsync-0.0.6/src/gdocsync/cli.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)       68 2023-07-13 04:33:19.000000 gdocsync-0.0.6/src/gdocsync/constants.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     3262 2023-07-13 04:43:14.000000 gdocsync-0.0.6/src/gdocsync/docs_importer.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     3124 2023-07-13 02:23:07.000000 gdocsync-0.0.6/src/gdocsync/google_drive_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1365 2023-07-13 04:53:59.000000 gdocsync-0.0.6/src/gdocsync/html_cleaner.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1366 2023-07-13 02:31:07.000000 gdocsync-0.0.6/src/gdocsync/johnny_decimal.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      760 2023-07-13 04:39:53.000000 gdocsync-0.0.6/src/gdocsync/pandoc_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.6/src/gdocsync/regexes.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      824 2023-07-13 04:33:19.000000 gdocsync-0.0.6/src/gdocsync/shelve_cache.py
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:55:08.387400 gdocsync-0.0.6/src/gdocsync.egg-info/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      541 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/SOURCES.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/dependency_links.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/entry_points.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       78 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/requires.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-13 04:55:08.000000 gdocsync-0.0.6/src/gdocsync.egg-info/top_level.txt
```

### Comparing `gdocsync-0.0.5/LICENSE` & `gdocsync-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.5/PKG-INFO` & `gdocsync-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdocsync
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/peterdemin/gdocsync
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gdocsync-0.0.5/README.rst` & `gdocsync-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.5/pyproject.toml` & `gdocsync-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.5/setup.cfg` & `gdocsync-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdocsync
-version = 0.0.5
+version = 0.0.6
 author = Peter Demin
 author_email = peterdemin@gmail.com
 description = 
 long_description = file:README.rst
 url = https://github.com/peterdemin/gdocsync
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `gdocsync-0.0.5/src/gdocsync/docs_importer.py` & `gdocsync-0.0.6/src/gdocsync/docs_importer.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import os
 import shutil
 import tempfile
 import zipfile
 
 from .constants import CACHE_FILE_NAME
 from .google_drive_client import DriveClient, DriveFile, GoogleAuth
+from .html_cleaner import HTMLCleaner
 from .johnny_decimal import JohnnyDecimal
 from .pandoc_client import PandocClient
 from .shelve_cache import ShelveCache
-from .html_cleaner import HTMLCleaner
 
 
 class DocsImporter:
     def __init__(
         self,
         pandoc_client: PandocClient,
         drive_client: DriveClient,
```

### Comparing `gdocsync-0.0.5/src/gdocsync/google_drive_client.py` & `gdocsync-0.0.6/src/gdocsync/google_drive_client.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.5/src/gdocsync/html_cleaner.py` & `gdocsync-0.0.6/src/gdocsync/html_cleaner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,38 @@
+from typing import Iterable
 from urllib.parse import parse_qs, urlparse
 
 from lxml import etree
 
 
 class HTMLCleaner:
     GOOGLE_TRACKING = "https://www.google.com/url"
+    BOLD_SELECTORS = [
+        '//span[@class="c1"]',
+        '//span[contains(@style,"font-weight:700")]',
+    ]
 
     def __call__(self, html_contents: str) -> str:
         htmlparser = etree.HTMLParser()
         tree = etree.fromstring(html_contents, htmlparser)
         etree.strip_elements(tree, "style")
         self._fix_spans(tree)
         self._fix_links(tree)
         return etree.tostring(tree, pretty_print=True).decode("utf-8")
 
     def _fix_spans(self, tree: etree.ElementTree) -> None:
-        for bold_span in tree.xpath('//span[@class="c1"]'):
-            bold_span.tag = 'b'
+        for bold_span in self._iter_bold_spans(tree):
+            bold_span.tag = "b"
             bold_span.text = bold_span.text.strip()
         etree.strip_tags(tree, "span")
 
+    def _iter_bold_spans(self, tree: etree.ElementTree) -> Iterable[etree.Element]:
+        for selector in self.BOLD_SELECTORS:
+            yield from tree.xpath(selector)
+
     def _fix_links(self, tree: etree.ElementTree) -> None:
         for link in tree.xpath("//a"):
             url = link.get("href")
             if not url or not url.startswith(self.GOOGLE_TRACKING):
                 continue
-            if real_url := parse_qs(urlparse(url).query).get("q", [''])[0]:
+            if real_url := parse_qs(urlparse(url).query).get("q", [""])[0]:
                 link.set("href", real_url)
```

### Comparing `gdocsync-0.0.5/src/gdocsync/johnny_decimal.py` & `gdocsync-0.0.6/src/gdocsync/johnny_decimal.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.5/src/gdocsync/pandoc_client.py` & `gdocsync-0.0.6/src/gdocsync/pandoc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
-import tempfile
 import subprocess
+import tempfile
 
 
 class PandocClient:
-    def convert_to_rst(self, source_bytes: bytes, target_path: str, extension: str = 'odt') -> str:
+    def convert_to_rst(self, source_bytes: bytes, target_path: str, extension: str = "odt") -> str:
         target_dir = os.path.dirname(target_path)
         with tempfile.TemporaryDirectory() as temp_dir:
             source_name = os.path.join(temp_dir, f"source.{extension}")
             with open(source_name, "wb") as f_in:
                 f_in.write(source_bytes)
             os.system(f"pandoc {source_name} -o {target_path} --extract-media {target_dir}")
```

### Comparing `gdocsync-0.0.5/src/gdocsync/shelve_cache.py` & `gdocsync-0.0.6/src/gdocsync/shelve_cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import contextlib
 import shelve
+
 from .constants import CACHE_FILE_NAME
 
 
 class ShelveCache:
     def __init__(self, cache_file_name: str) -> None:
         self._cache_file_name = cache_file_name
```

### Comparing `gdocsync-0.0.5/src/gdocsync.egg-info/PKG-INFO` & `gdocsync-0.0.6/src/gdocsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdocsync
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/peterdemin/gdocsync
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gdocsync-0.0.5/src/gdocsync.egg-info/SOURCES.txt` & `gdocsync-0.0.6/src/gdocsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

