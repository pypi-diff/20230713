# Comparing `tmp/pypi_download_pkg-0.2.1.tar.gz` & `tmp/pypi_download_pkg-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_download_pkg-0.2.1.tar", max compression
+gzip compressed data, was "pypi_download_pkg-0.2.2.tar", max compression
```

## Comparing `pypi_download_pkg-0.2.1.tar` & `pypi_download_pkg-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/LICENSE
--rw-r--r--   0        0        0      579 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/pypi_download_pkg/__init__.py
--rw-r--r--   0        0        0     4585 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/pypi_download_pkg/cli.py
--rw-r--r--   0        0        0      603 2023-07-13 10:23:55.024807 pypi_download_pkg-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 pypi_download_pkg-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-13 10:31:20.490031 pypi_download_pkg-0.2.2/LICENSE
+-rw-r--r--   0        0        0      579 2023-07-13 10:31:20.490031 pypi_download_pkg-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 10:31:20.490031 pypi_download_pkg-0.2.2/pypi_download_pkg/__init__.py
+-rw-r--r--   0        0        0     4239 2023-07-13 10:31:20.490031 pypi_download_pkg-0.2.2/pypi_download_pkg/cli.py
+-rw-r--r--   0        0        0      603 2023-07-13 10:31:20.490031 pypi_download_pkg-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 pypi_download_pkg-0.2.2/PKG-INFO
```

### Comparing `pypi_download_pkg-0.2.1/LICENSE` & `pypi_download_pkg-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_download_pkg-0.2.1/README.md` & `pypi_download_pkg-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pypi_download_pkg-0.2.1/pypi_download_pkg/cli.py` & `pypi_download_pkg-0.2.2/pypi_download_pkg/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,53 +39,51 @@
             re.compile("musllinux.*[_]i686[.]whl"),
         ]
 
 def is_linux(filename: str):
     return any((r for r in linux_regexes if re.search(r, filename)))
 
 def handle_package(pk: str, version: str, output_dir: str):
-    url = f"https://pypi.org/pypi/{pk}/json"
+    url = f"https://pypi.org/pypi/{pk}/{version}/json"
     r = requests.get(url)
     r.raise_for_status()
-    releases = r.json()["releases"]
-    for pkg_version, pkg_files in releases.items():
-        if pkg_version == version:
-            for fl in pkg_files:
-                if (
-                    fl["packagetype"] == "sdist"
-                    or fl["filename"].endswith("-none-any.whl")
-                    or is_linux(fl["filename"])
-                ):
-                    if not os.path.exists(os.path.join(output_dir, fl["filename"])):
-                        download_url = fl["url"]
-                        r = requests.get(download_url, stream=True)
-                        r.raise_for_status()
-                        os.makedirs(output_dir, exist_ok=True)
-                        with open(os.path.join(output_dir, fl["filename"]), 'wb') as f:
-                            for chunk in r.iter_content(chunk_size=1024):
-                                if chunk:
-                                    f.write(chunk)
-                        print("do " + fl["filename"])
-                    else:
-                        print("already done " + fl["filename"])
-                elif (
-                    "-macosx_" in fl["filename"]
-                    or "ppc64le." in fl["filename"]
-                    or fl["filename"].endswith("s390x.whl")
-                    or fl["filename"].endswith("win32.whl")
-                    or fl["filename"].endswith("win_amd64.whl")
-                    or fl["filename"].endswith("win_arm64.whl")
-                    or fl["filename"].endswith("win_arm32.whl")
-                    or fl["filename"].endswith("armv7l.whl")
-                    or re.search("armv[0-9]*[a-z]{0,3}.whl", fl["filename"])
-                ):
-                    print("ignoring " + fl["filename"])
-                else:
-                    print("not sure about " + fl["filename"] + ". Ignoring for now")
-                    print(fl["packagetype"])
+    pkg_files = r.json()["urls"]
+    for fl in pkg_files:
+        if (
+            fl["packagetype"] == "sdist"
+            or fl["filename"].endswith("-none-any.whl")
+            or is_linux(fl["filename"])
+        ):
+            if not os.path.exists(os.path.join(output_dir, fl["filename"])):
+                download_url = fl["url"]
+                r = requests.get(download_url, stream=True)
+                r.raise_for_status()
+                os.makedirs(output_dir, exist_ok=True)
+                with open(os.path.join(output_dir, fl["filename"]), 'wb') as f:
+                    for chunk in r.iter_content(chunk_size=1024):
+                        if chunk:
+                            f.write(chunk)
+                print("do " + fl["filename"])
+            else:
+                print("already done " + fl["filename"])
+        elif (
+            "-macosx_" in fl["filename"]
+            or "ppc64le." in fl["filename"]
+            or fl["filename"].endswith("s390x.whl")
+            or fl["filename"].endswith("win32.whl")
+            or fl["filename"].endswith("win_amd64.whl")
+            or fl["filename"].endswith("win_arm64.whl")
+            or fl["filename"].endswith("win_arm32.whl")
+            or fl["filename"].endswith("armv7l.whl")
+            or re.search("armv[0-9]*[a-z]{0,3}.whl", fl["filename"])
+        ):
+            print("ignoring " + fl["filename"])
+        else:
+            print("not sure about " + fl["filename"] + ". Ignoring for now")
+            print(fl["packagetype"])
 
 def execute(req_file: str, pkg_filter: Optional[List[str]], output_dir: str):
     if pkg_filter and len(pkg_filter) == 0:
         pkg_filter = None
 
     done_any = False
     all_deps = []
```

### Comparing `pypi_download_pkg-0.2.1/pyproject.toml` & `pypi_download_pkg-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypi-download-pkg"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["BMSuisse"]
 readme = "README.md"
 packages = [{include = "pypi_download_pkg"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pypi_download_pkg-0.2.1/PKG-INFO` & `pypi_download_pkg-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-download-pkg
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: BMSuisse
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

