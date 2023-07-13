# Comparing `tmp/pypi_download_pkg-0.1.0.tar.gz` & `tmp/pypi_download_pkg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_download_pkg-0.1.0.tar", max compression
+gzip compressed data, was "pypi_download_pkg-0.2.1.tar", max compression
```

## Comparing `pypi_download_pkg-0.1.0.tar` & `pypi_download_pkg-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-05-23 12:07:55.905787 pypi_download_pkg-0.1.0/LICENSE
--rw-r--r--   0        0        0      236 2023-05-23 12:07:55.905787 pypi_download_pkg-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 12:07:55.905787 pypi_download_pkg-0.1.0/pypi_download_pkg/__init__.py
--rw-r--r--   0        0        0     4076 2023-05-23 12:07:55.905787 pypi_download_pkg-0.1.0/pypi_download_pkg/cli.py
--rw-r--r--   0        0        0      548 2023-05-23 12:07:55.905787 pypi_download_pkg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 pypi_download_pkg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/LICENSE
+-rw-r--r--   0        0        0      579 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/pypi_download_pkg/__init__.py
+-rw-r--r--   0        0        0     4585 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/pypi_download_pkg/cli.py
+-rw-r--r--   0        0        0      603 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 pypi_download_pkg-0.2.1/PKG-INFO
```

### Comparing `pypi_download_pkg-0.1.0/LICENSE` & `pypi_download_pkg-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_download_pkg-0.1.0/pypi_download_pkg/cli.py` & `pypi_download_pkg-0.2.1/pypi_download_pkg/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
 from typing import List, Optional
-
+import requests
 
 def get_deps(req_file: str):
     
     def parse_file(f):
         l = f.readline()
         while l is not None and l != "":
             if l and not l.strip().startswith("--"):
@@ -38,56 +38,67 @@
             re.compile("musllinux.*[_]x86[_]64[.]whl"),
             re.compile("musllinux.*[_]i686[.]whl"),
         ]
 
 def is_linux(filename: str):
     return any((r for r in linux_regexes if re.search(r, filename)))
 
-def execute(req_file: str, pkg_filter: Optional[List[str]], output_dir: str):
-    from pypi_simple import PyPISimple
+def handle_package(pk: str, version: str, output_dir: str):
+    url = f"https://pypi.org/pypi/{pk}/json"
+    r = requests.get(url)
+    r.raise_for_status()
+    releases = r.json()["releases"]
+    for pkg_version, pkg_files in releases.items():
+        if pkg_version == version:
+            for fl in pkg_files:
+                if (
+                    fl["packagetype"] == "sdist"
+                    or fl["filename"].endswith("-none-any.whl")
+                    or is_linux(fl["filename"])
+                ):
+                    if not os.path.exists(os.path.join(output_dir, fl["filename"])):
+                        download_url = fl["url"]
+                        r = requests.get(download_url, stream=True)
+                        r.raise_for_status()
+                        os.makedirs(output_dir, exist_ok=True)
+                        with open(os.path.join(output_dir, fl["filename"]), 'wb') as f:
+                            for chunk in r.iter_content(chunk_size=1024):
+                                if chunk:
+                                    f.write(chunk)
+                        print("do " + fl["filename"])
+                    else:
+                        print("already done " + fl["filename"])
+                elif (
+                    "-macosx_" in fl["filename"]
+                    or "ppc64le." in fl["filename"]
+                    or fl["filename"].endswith("s390x.whl")
+                    or fl["filename"].endswith("win32.whl")
+                    or fl["filename"].endswith("win_amd64.whl")
+                    or fl["filename"].endswith("win_arm64.whl")
+                    or fl["filename"].endswith("win_arm32.whl")
+                    or fl["filename"].endswith("armv7l.whl")
+                    or re.search("armv[0-9]*[a-z]{0,3}.whl", fl["filename"])
+                ):
+                    print("ignoring " + fl["filename"])
+                else:
+                    print("not sure about " + fl["filename"] + ". Ignoring for now")
+                    print(fl["packagetype"])
 
+def execute(req_file: str, pkg_filter: Optional[List[str]], output_dir: str):
     if pkg_filter and len(pkg_filter) == 0:
         pkg_filter = None
 
     done_any = False
     all_deps = []
-    with PyPISimple() as client:
-        for pkg, version in get_deps(req_file):
-            all_deps.append(pkg)
-            if pkg_filter and not pkg in pkg_filter:
-                continue
-            done_any = True
-            page = client.get_project_page(pkg)
-            for fl in page.packages:
-                if fl.version == version:
-                    if (
-                        fl.package_type == "sdist"
-                        or fl.filename.endswith("-none-any.whl")
-                        or is_linux(fl.filename)
-                    ):
-                        if not os.path.exists(os.path.join(output_dir, fl.filename)):
-                            client.download_package(fl, os.path.join(output_dir, fl.filename))
-                            print("do " + fl.filename)
-                        else:
-                            print("already done " + fl.filename)
-                    elif (
-                        "-macosx_" in fl.filename
-                        or "ppc64le." in fl.filename
-                        or fl.filename.endswith("s390x.whl")
-                        or fl.filename.endswith("win32.whl")
-                        or fl.filename.endswith("win_amd64.whl")
-                        or fl.filename.endswith("win_arm64.whl")
-                        or fl.filename.endswith("win_arm32.whl")
-                        or fl.filename.endswith("armv7l.whl")
-                        or re.search("armv[0-9]*[a-z]{0,3}.whl", fl.filename)
-                    ):
-                        print("ignoring " + fl.filename)
-                    else:
-                        print("not sure about " + fl.filename + ". Ignoring for now")
-                        print(fl.package_type)
+    for pkg, version in get_deps(req_file):
+        all_deps.append(pkg)
+        if pkg_filter and not pkg in pkg_filter:
+            continue
+        done_any = True
+        handle_package(pkg, version, output_dir)
     if not done_any and pkg_filter is not None:
         print("Could not find package: " + ", " .join(pkg_filter))
         print("Can be any of : " + ", ".join(all_deps))
 
 
 def cli():
     import argparse
```

### Comparing `pypi_download_pkg-0.1.0/pyproject.toml` & `pypi_download_pkg-0.2.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "pypi-download-pkg"
-version = "0.1.0"
+version = "0.2.1"
 description = ""
 authors = ["BMSuisse"]
 readme = "README.md"
 packages = [{include = "pypi_download_pkg"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-pypi-simple = "^1.1.0"
+python = "^3.10"
+requests = "^2.31.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 
 
 [tool.poetry.group.dev.dependencies]
@@ -20,8 +20,12 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
-download_linux_pkg = { callable = "pypi_download_pkg.cli:cli" }
+download_linux_pkg = { callable = "pypi_download_pkg.cli:cli" }
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+
```

