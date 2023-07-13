# Comparing `tmp/gdocsync-0.0.3.tar.gz` & `tmp/gdocsync-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdocsync-0.0.3.tar", last modified: Mon Jul 10 05:42:02 2023, max compression
+gzip compressed data, was "gdocsync-0.0.4.tar", last modified: Thu Jul 13 03:15:53 2023, max compression
```

## Comparing `gdocsync-0.0.3.tar` & `gdocsync-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:42:02.503348 gdocsync-0.0.3/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.3/LICENSE
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-10 05:42:02.503411 gdocsync-0.0.3/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.3/README.rst
--rw-r--r--   0 peterdemin   (503) staff       (20)    21045 2023-07-10 04:49:41.000000 gdocsync-0.0.3/pyproject.toml
--rw-r--r--   0 peterdemin   (503) staff       (20)      751 2023-07-10 05:42:02.503681 gdocsync-0.0.3/setup.cfg
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:42:02.499909 gdocsync-0.0.3/src/
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:42:02.502425 gdocsync-0.0.3/src/gdocsync/
--rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.3/src/gdocsync/__init__.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      327 2023-07-10 05:21:38.000000 gdocsync-0.0.3/src/gdocsync/cli.py
--rw-r--r--   0 peterdemin   (503) staff       (20)       69 2023-07-10 05:17:11.000000 gdocsync-0.0.3/src/gdocsync/constants.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     2575 2023-07-10 05:12:07.000000 gdocsync-0.0.3/src/gdocsync/google_drive_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1311 2023-07-10 05:19:49.000000 gdocsync-0.0.3/src/gdocsync/johnny_decimal.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      549 2023-07-10 05:03:46.000000 gdocsync-0.0.3/src/gdocsync/pandoc_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.3/src/gdocsync/regexes.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      823 2023-07-10 05:09:34.000000 gdocsync-0.0.3/src/gdocsync/shelve_cache.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1020 2023-07-10 05:41:31.000000 gdocsync-0.0.3/src/gdocsync/sync.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      517 2023-07-10 05:02:15.000000 gdocsync-0.0.3/src/gdocsync/test_regexes.py
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:42:02.503238 gdocsync-0.0.3/src/gdocsync.egg-info/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-10 05:42:02.000000 gdocsync-0.0.3/src/gdocsync.egg-info/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      532 2023-07-10 05:42:02.000000 gdocsync-0.0.3/src/gdocsync.egg-info/SOURCES.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-10 05:42:02.000000 gdocsync-0.0.3/src/gdocsync.egg-info/dependency_links.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-10 05:42:02.000000 gdocsync-0.0.3/src/gdocsync.egg-info/entry_points.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       73 2023-07-10 05:42:02.000000 gdocsync-0.0.3/src/gdocsync.egg-info/requires.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-10 05:42:02.000000 gdocsync-0.0.3/src/gdocsync.egg-info/top_level.txt
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 03:15:53.132387 gdocsync-0.0.4/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.4/LICENSE
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 03:15:53.132456 gdocsync-0.0.4/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.4/README.rst
+-rw-r--r--   0 peterdemin   (503) staff       (20)    21045 2023-07-10 04:49:41.000000 gdocsync-0.0.4/pyproject.toml
+-rw-r--r--   0 peterdemin   (503) staff       (20)      757 2023-07-13 03:15:53.132707 gdocsync-0.0.4/setup.cfg
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 03:15:53.129832 gdocsync-0.0.4/src/
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 03:15:53.131513 gdocsync-0.0.4/src/gdocsync/
+-rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.4/src/gdocsync/__init__.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      333 2023-07-13 02:07:34.000000 gdocsync-0.0.4/src/gdocsync/cli.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)       69 2023-07-10 05:17:11.000000 gdocsync-0.0.4/src/gdocsync/constants.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     3262 2023-07-13 02:41:29.000000 gdocsync-0.0.4/src/gdocsync/docs_importer.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     3124 2023-07-13 02:23:07.000000 gdocsync-0.0.4/src/gdocsync/google_drive_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      348 2023-07-13 03:10:28.000000 gdocsync-0.0.4/src/gdocsync/html_cleaner.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1366 2023-07-13 02:31:07.000000 gdocsync-0.0.4/src/gdocsync/johnny_decimal.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      760 2023-07-13 02:09:05.000000 gdocsync-0.0.4/src/gdocsync/pandoc_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.4/src/gdocsync/regexes.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      823 2023-07-10 05:09:34.000000 gdocsync-0.0.4/src/gdocsync/shelve_cache.py
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 03:15:53.132287 gdocsync-0.0.4/src/gdocsync.egg-info/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      541 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/SOURCES.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/dependency_links.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/entry_points.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       78 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/requires.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/top_level.txt
```

### Comparing `gdocsync-0.0.3/LICENSE` & `gdocsync-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.3/PKG-INFO` & `gdocsync-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdocsync
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/peterdemin/gdocsync
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gdocsync-0.0.3/README.rst` & `gdocsync-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.3/pyproject.toml` & `gdocsync-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.3/setup.cfg` & `gdocsync-0.0.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdocsync
-version = 0.0.3
+version = 0.0.4
 author = Peter Demin
 author_email = peterdemin@gmail.com
 description = 
 long_description = file:README.rst
 url = https://github.com/peterdemin/gdocsync
 classifiers = 
 	Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
 	click
 	google-api-python-client
 	google-auth-httplib2
 	google-auth-oauthlib
+	lxml
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	gdocsync = gdocsync.cli:cli
```

### Comparing `gdocsync-0.0.3/src/gdocsync/google_drive_client.py` & `gdocsync-0.0.4/src/gdocsync/google_drive_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 ]
 
 
 @dataclass
 class DriveFile:
     drive_id: str
     name: str
-    md5: str = ""
 
 
 class GoogleAuth:
     _CREDENTIALS_PATH = os.path.expanduser("~/.gcp/credentials.json")
 
     def __init__(self, cache: ShelveCache) -> None:
         self._cache = cache
@@ -61,13 +60,29 @@
             DriveFile(drive_id=item["id"], name=item["name"])
             for item in self._service.files()  # pylint: disable=no-member
             .list(pageSize=100, fields="nextPageToken, files(id, name)")
             .execute()
             .get("files", [])
         ]
 
-    def download_doc(self, drive_file_id: str, mime_type="application/rtf") -> bytes:
+    def download_doc(self, drive_file_id: str, mime_type: str) -> bytes:
+        """Downloads the doc given drive file ID as bytes.
+
+        Supported mime types:
+
+        - Microsoft Word
+          application/vnd.openxmlformats-officedocument.wordprocessingml.document .docx
+        - OpenDocument application/vnd.oasis.opendocument.text .odt
+        - Rich Text application/rtf .rtf
+        - PDF application/pdf .pdf
+        - Plain Text text/plain .txt
+        - Web Page (HTML) application/zip .zip
+        - EPUB application/epub+zip .epub
+
+        Reference:
+        https://developers.google.com/drive/api/guides/ref-export-formats
+        """
         return (
             self._service.files()  # pylint: disable=no-member
             .export(fileId=drive_file_id, mimeType=mime_type)
             .execute()
         )
```

### Comparing `gdocsync-0.0.3/src/gdocsync/johnny_decimal.py` & `gdocsync-0.0.4/src/gdocsync/johnny_decimal.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,20 +26,23 @@
     @staticmethod
     def is_valid(name: str) -> bool:
         return bool(RE_JOHNNY_DECIMAL.match(name))
 
     def fit_path(self, base_dir: str) -> str:
         parent_dir_expr = os.path.join(base_dir, f"{self.category}*")
         parent_dir_candidates = glob.glob(parent_dir_expr)
-        filename = f"{self.index}{self.SLUG_DELIMITER}{self.slug}"
         if len(parent_dir_candidates) == 1:
             parent_dir = parent_dir_candidates[0]
-            return os.path.join(parent_dir, filename)
-        full_pattern = os.path.join(parent_dir_expr, filename)
+            return os.path.join(parent_dir, self.file_name)
+        full_pattern = os.path.join(parent_dir_expr, self.file_name)
         raise ValueError(
             f"Could not find unambiguous fit for {full_pattern}. "
             f"Candidates: {parent_dir_candidates}"
         )
 
     @property
+    def file_name(self) -> str:
+        return f"{self.index}{self.SLUG_DELIMITER}{self.slug}"
+
+    @property
     def slug(self) -> str:
         return RE_PUNCT.sub(self.SLUG_DELIMITER, self.name).lower()
```

### Comparing `gdocsync-0.0.3/src/gdocsync/shelve_cache.py` & `gdocsync-0.0.4/src/gdocsync/shelve_cache.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.3/src/gdocsync.egg-info/PKG-INFO` & `gdocsync-0.0.4/src/gdocsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdocsync
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/peterdemin/gdocsync
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gdocsync-0.0.3/src/gdocsync.egg-info/SOURCES.txt` & `gdocsync-0.0.4/src/gdocsync.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 src/gdocsync/__init__.py
 src/gdocsync/cli.py
 src/gdocsync/constants.py
+src/gdocsync/docs_importer.py
 src/gdocsync/google_drive_client.py
+src/gdocsync/html_cleaner.py
 src/gdocsync/johnny_decimal.py
 src/gdocsync/pandoc_client.py
 src/gdocsync/regexes.py
 src/gdocsync/shelve_cache.py
-src/gdocsync/sync.py
-src/gdocsync/test_regexes.py
 src/gdocsync.egg-info/PKG-INFO
 src/gdocsync.egg-info/SOURCES.txt
 src/gdocsync.egg-info/dependency_links.txt
 src/gdocsync.egg-info/entry_points.txt
 src/gdocsync.egg-info/requires.txt
 src/gdocsync.egg-info/top_level.txt
```

