# Comparing `tmp/safepull-2.0.3.tar.gz` & `tmp/safepull-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safepull-2.0.3.tar", last modified: Tue Jul 11 02:45:54 2023, max compression
+gzip compressed data, was "safepull-2.0.4.tar", last modified: Thu Jul 13 14:07:40 2023, max compression
```

## Comparing `safepull-2.0.3.tar` & `safepull-2.0.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:45:54.497826 safepull-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-11 02:45:43.000000 safepull-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-11 02:45:54.497826 safepull-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-11 02:45:43.000000 safepull-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-11 02:45:43.000000 safepull-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 02:45:54.501826 safepull-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:45:54.497826 safepull-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:45:54.497826 safepull-2.0.3/src/safepull/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 02:45:43.000000 safepull-2.0.3/src/safepull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 02:45:43.000000 safepull-2.0.3/src/safepull/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 02:45:43.000000 safepull-2.0.3/src/safepull/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-11 02:45:43.000000 safepull-2.0.3/src/safepull/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-11 02:45:43.000000 safepull-2.0.3/src/safepull/safepull.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:45:54.497826 safepull-2.0.3/src/safepull.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-11 02:45:54.000000 safepull-2.0.3/src/safepull.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 02:45:54.000000 safepull-2.0.3/src/safepull.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 02:45:54.000000 safepull-2.0.3/src/safepull.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 02:45:54.000000 safepull-2.0.3/src/safepull.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 02:45:54.000000 safepull-2.0.3/src/safepull.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 02:45:54.000000 safepull-2.0.3/src/safepull.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:40.820465 safepull-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-13 14:07:28.000000 safepull-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-13 14:07:40.816465 safepull-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-13 14:07:28.000000 safepull-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 14:07:28.000000 safepull-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:07:40.820465 safepull-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:40.816465 safepull-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:40.816465 safepull-2.0.4/src/safepull/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:28.000000 safepull-2.0.4/src/safepull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 14:07:28.000000 safepull-2.0.4/src/safepull/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-13 14:07:28.000000 safepull-2.0.4/src/safepull/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-13 14:07:28.000000 safepull-2.0.4/src/safepull/safepull.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:40.816465 safepull-2.0.4/src/safepull.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/top_level.txt
```

### Comparing `safepull-2.0.3/LICENSE` & `safepull-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `safepull-2.0.3/PKG-INFO` & `safepull-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safepull
-Version: 2.0.3
+Version: 2.0.4
 Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py
 License: MIT
 Project-URL: repository, https://github.com/import-pandas-as-numpy/safepull/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `safepull-2.0.3/README.md` & `safepull-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `safepull-2.0.3/pyproject.toml` & `safepull-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "safepull"
-version = "2.0.3"
+version = "2.0.4"
 description = "A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.10"
 dependencies = [
     "requests>=2.28.2,<2.32.0",
     "rich~=13.4.2",
```

### Comparing `safepull-2.0.3/src/safepull/models.py` & `safepull-2.0.4/src/safepull/models.py`

 * *Files identical despite different names*

### Comparing `safepull-2.0.3/src/safepull/safepull.py` & `safepull-2.0.4/src/safepull/safepull.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,41 +5,47 @@
 import tarfile
 from io import BytesIO
 from zipfile import ZipFile
 
 import requests
 from rich.console import Console
 
-from .exceptions import PackageNotFoundError
 from .models import Package
 
 HOST = "https://pypi.org"
 
 
 def query_package(package_title: str, version: str | None = None) -> Package:
     """Query PyPI for a package."""
     if version:
         response = requests.get(
             f"{HOST}/pypi/{package_title}/{version}/json",
             timeout=60,
-        ).json()
+        )
     else:
-        response = requests.get(f"{HOST}/pypi/{package_title}/json", timeout=60).json()
-    try:
-        my_package = Package.from_dict(response)
-    except KeyError as e:
-        raise PackageNotFoundError(package_title, version) from e
-    return my_package
+        response = requests.get(f"{HOST}/pypi/{package_title}/json", timeout=60)
+    response.raise_for_status()
+    return Package.from_dict(response.json())
 
 
 def unpack(byte_object: BytesIO, filename: str) -> None:
     """Unpack a compressed file into the CWD."""
     if filename.endswith(".tar.gz"):
         with tarfile.open(fileobj=byte_object) as sdist_tar:
-            sdist_tar.extractall(filter="data")
+            if hasattr(tarfile, "data_filter"):
+                sdist_tar.extractall(filter="data")
+            else:
+                print(
+                    "You do not have data filters enabled for your Python version.",
+                    "This is a security risk. Please update Python.",
+                    "For more information: https://directorytraversal.zip",
+                    sep="\n",
+                )
+                if input('To ignore this, enter "Y": ').upper() == "Y":
+                    sdist_tar.extractall()
     if filename.endswith((".whl", ".zip")):
         with ZipFile(byte_object) as whl_zip:
             whl_zip.extractall()
 
 
 def run() -> None:
     """Run the program."""
```

### Comparing `safepull-2.0.3/src/safepull.egg-info/PKG-INFO` & `safepull-2.0.4/src/safepull.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safepull
-Version: 2.0.3
+Version: 2.0.4
 Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py
 License: MIT
 Project-URL: repository, https://github.com/import-pandas-as-numpy/safepull/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

