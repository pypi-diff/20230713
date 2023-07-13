# Comparing `tmp/pdm-packer-0.6.0.tar.gz` & `tmp/pdm_packer-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-packer-0.6.0.tar", last modified: Wed Mar 29 02:40:26 2023, max compression
+gzip compressed data, was "pdm_packer-0.6.1.tar", last modified: Thu Jul 13 04:01:17 2023, max compression
```

## Comparing `pdm-packer-0.6.0.tar` & `pdm_packer-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1059 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/LICENSE
--rw-r--r--   0        0        0     3846 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/README.md
--rw-r--r--   0        0        0     2585 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      277 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/src/pdm_packer/__init__.py
--rw-r--r--   0        0        0      521 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/src/pdm_packer/_compile_source.py
--rw-r--r--   0        0        0     4507 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/src/pdm_packer/command.py
--rw-r--r--   0        0        0     1844 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/src/pdm_packer/env.py
--rw-r--r--   0        0        0      135 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      722 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     4830 2023-03-29 02:40:16.364639 pdm-packer-0.6.0/tests/test_packer.py
--rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 pdm-packer-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3846 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/README.md
+-rw-r--r--   0        0        0     2629 2023-07-13 04:01:17.020003 pdm_packer-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/src/pdm_packer/__init__.py
+-rw-r--r--   0        0        0      521 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/src/pdm_packer/_compile_source.py
+-rw-r--r--   0        0        0     4337 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/src/pdm_packer/command.py
+-rw-r--r--   0        0        0     1844 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/src/pdm_packer/env.py
+-rw-r--r--   0        0        0      135 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      722 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     4823 2023-07-13 04:01:08.975912 pdm_packer-0.6.1/tests/test_packer.py
+-rw-r--r--   0        0        0     4612 1970-01-01 00:00:00.000000 pdm_packer-0.6.1/PKG-INFO
```

### Comparing `pdm-packer-0.6.0/LICENSE` & `pdm_packer-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-packer-0.6.0/README.md` & `pdm_packer-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm-packer-0.6.0/pyproject.toml` & `pdm_packer-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "pdm-packer"
 description = "A PDM plugin that packs your packages into a zipapp"
 authors = [
     { name = "Frost Ming", email = "mianghong@gmail.com" },
 ]
@@ -19,16 +19,17 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
-version = "0.6.0"
+version = "0.6.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/frostming/pdm-packer"
 Homepage = "https://github.com/frostming/pdm-packer"
@@ -41,15 +42,15 @@
 
 [tool.pdm.build]
 package-dir = "src"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=6.1",
-    "towncrier~=19.2",
+    "towncrier>=19.2",
     "pdm>=2.3",
     "parver>=0.3",
 ]
 
 [tool.pdm.scripts]
 release = "python -m tasks.release"
 test = "pytest tests/"
```

### Comparing `pdm-packer-0.6.0/src/pdm_packer/_compile_source.py` & `pdm_packer-0.6.1/src/pdm_packer/_compile_source.py`

 * *Files identical despite different names*

### Comparing `pdm-packer-0.6.0/src/pdm_packer/command.py` & `pdm_packer-0.6.1/src/pdm_packer/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,21 +84,17 @@
         if options.exe:
             output.chmod(output.stat().st_mode | stat.S_IEXEC)
         return output
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         def file_filter(name: str) -> bool:
             path = Path(name)
-            first = path.parts[0]
             last = path.name
             return not (
-                first.endswith(".dist-info")
-                or first.endswith(".egg")
-                or last.endswith(".egg-link")
-                or "__pycache__" in path.parts
+                "__pycache__" in path.parts
                 or options.no_py
                 and last.endswith(".py")
                 or not options.compile
                 and last.endswith(".pyc")
             )
 
         main = None
```

### Comparing `pdm-packer-0.6.0/src/pdm_packer/env.py` & `pdm_packer-0.6.1/src/pdm_packer/env.py`

 * *Files identical despite different names*

### Comparing `pdm-packer-0.6.0/tests/conftest.py` & `pdm_packer-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-packer-0.6.0/tests/test_packer.py` & `pdm_packer-0.6.1/tests/test_packer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,21 @@
             "project": {
                 "name": "test_app",
                 "version": "0.1.0",
                 "requires-python": ">=3.7",
                 "dependencies": ["requests==2.24.0"],
             },
             "build-system": {
-                "requires": ["pdm-pep517"],
-                "build-backend": "pdm.pep517.api",
+                "requires": ["pdm-backend"],
+                "build-backend": "pdm.backend",
             },
         }
     )
     project.pyproject.write()
-    invoke(["install"], obj=project)
+    invoke(["lock"], obj=project)
 
     return project
 
 
 def test_pack_env_all_non_editable(example_project):
     with PackEnvironment(example_project) as env:
         env.prepare_lib_for_pack()
@@ -66,17 +66,17 @@
     assert output.exists()
     assert f"#!{example_project.python.executable}".encode() in output.read_bytes()
 
     with zipfile.ZipFile(output) as zf:
         namelist = zf.namelist()
         assert "requests/__init__.py" in namelist
         assert "urllib3/__init__.py" in namelist
+        assert "requests-2.24.0.dist-info/METADATA" in namelist
         assert "app.py" in namelist
         assert not any(name.endswith(".pyc") for name in namelist)
-        assert not any(".dist-info" in name for name in namelist)
 
         main = [
             line.decode().rstrip()
             for line in zf.open("__main__.py")
             if not line.startswith(b"#")
         ]
         assert main == ["import app", "app.main()"]
```

### Comparing `pdm-packer-0.6.0/PKG-INFO` & `pdm_packer-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pdm-packer
-Version: 0.6.0
+Version: 0.6.1
 Summary: A PDM plugin that packs your packages into a zipapp
+Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
-Author-email: Frost Ming <mianghong@gmail.com>
-Requires-Python: >=3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Project-URL: Homepage, https://github.com/frostming/pdm-packer
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/frostming/pdm-packer
+Project-URL: Homepage, https://github.com/frostming/pdm-packer
+Requires-Python: >=3.7
+Requires-Dist: distlib>=0.3.4; sys_platform == "win32"
 Description-Content-Type: text/markdown
 
 # pdm-packer
 
 [![Tests](https://github.com/frostming/pdm-packer/workflows/Tests/badge.svg)](https://github.com/frostming/pdm-packer/actions?query=workflow%3Aci)
 [![pypi version](https://img.shields.io/pypi/v/pdm-packer.svg)](https://pypi.org/project/pdm-packer/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -138,8 +140,7 @@
 By default, zipapp is created with `.pyz` suffix. On Windows, if you have associted `.pyz` files with Python program, you can run the app by double-clicking the file in the explorer. But if you create the app with `--exe` turn on, you can have a .exe file on Windows and an **executable** file
 on Unix-like systems, so that the app can be executed without a `python` command prefixing it and
 no matter you assoicated the file exensition properly or not.
 
 ## Changelog
 
 See [CHANGELOG.md](https://github.com/frostming/pdm-packer/blob/main/CHANGELOG.md)
-
```

