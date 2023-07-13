# Comparing `tmp/dpsim-1.1.0.tar.gz` & `tmp/dpsim-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpsim-1.1.0.tar", last modified: Sat Dec 10 09:56:36 2022, max compression
+gzip compressed data, was "dpsim-1.1.1.tar", last modified: Thu Jul 13 13:37:40 2023, max compression
```

## Comparing `dpsim-1.1.0.tar` & `dpsim-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-10 09:56:36.067836 dpsim-1.1.0/
--rw-r--r--   0 root         (0) root         (0)    16724 2022-12-10 09:56:27.000000 dpsim-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2692 2022-12-10 09:56:36.067836 dpsim-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2191 2022-12-10 09:56:27.000000 dpsim-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-10 09:56:36.067836 dpsim-1.1.0/dpsim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2692 2022-12-10 09:56:36.000000 dpsim-1.1.0/dpsim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      253 2022-12-10 09:56:36.000000 dpsim-1.1.0/dpsim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-10 09:56:36.000000 dpsim-1.1.0/dpsim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-10 09:56:36.000000 dpsim-1.1.0/dpsim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2022-12-10 09:56:36.000000 dpsim-1.1.0/dpsim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      277 2022-12-10 09:56:27.000000 dpsim-1.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-10 09:56:36.063836 dpsim-1.1.0/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-10 09:56:36.063836 dpsim-1.1.0/python/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-10 09:56:36.067836 dpsim-1.1.0/python/src/dpsim/
--rw-r--r--   0 root         (0) root         (0)      201 2022-12-10 09:56:27.000000 dpsim-1.1.0/python/src/dpsim/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12214 2022-12-10 09:56:27.000000 dpsim-1.1.0/python/src/dpsim/matpower.py
--rw-r--r--   0 root         (0) root         (0)      526 2022-12-10 09:56:36.067836 dpsim-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2508 2022-12-10 09:56:27.000000 dpsim-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:37:40.391788 dpsim-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)    16724 2023-07-13 13:37:33.000000 dpsim-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-07-13 13:37:40.391788 dpsim-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-07-13 13:37:33.000000 dpsim-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:37:40.391788 dpsim-1.1.1/dpsim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-07-13 13:37:40.000000 dpsim-1.1.1/dpsim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-13 13:37:40.000000 dpsim-1.1.1/dpsim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 13:37:40.000000 dpsim-1.1.1/dpsim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 13:37:40.000000 dpsim-1.1.1/dpsim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-13 13:37:40.000000 dpsim-1.1.1/dpsim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-13 13:37:33.000000 dpsim-1.1.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:37:40.391788 dpsim-1.1.1/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:37:40.391788 dpsim-1.1.1/python/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:37:40.391788 dpsim-1.1.1/python/src/dpsim/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-13 13:37:33.000000 dpsim-1.1.1/python/src/dpsim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12214 2023-07-13 13:37:33.000000 dpsim-1.1.1/python/src/dpsim/matpower.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-07-13 13:37:40.391788 dpsim-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-13 13:37:33.000000 dpsim-1.1.1/setup.py
```

### Comparing `dpsim-1.1.0/LICENSE` & `dpsim-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dpsim-1.1.0/PKG-INFO` & `dpsim-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dpsim
-Version: 1.1.0
+Version: 1.1.1
 Summary: dynamic real-time power system simulator
 Home-page: https://github.com/sogno-platform/dpsim
 Author: The DPsim Authors
 Author-email: mmirz@eonerc.rwth-aachen.de
 Project-URL: Bug Tracker, https://github.com/sogno-platform/dpsim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <img src="docs/images/dpsim.png" width=40 /> DPsim
 
 [![Build & Test CentOS](https://github.com/sogno-platform/dpsim/actions/workflows/build_test_linux_centos.yaml/badge.svg)](https://github.com/sogno-platform/dpsim/actions/workflows/build_test_linux_centos.yaml)
```

### Comparing `dpsim-1.1.0/README.md` & `dpsim-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dpsim-1.1.0/dpsim.egg-info/PKG-INFO` & `dpsim-1.1.1/dpsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dpsim
-Version: 1.1.0
+Version: 1.1.1
 Summary: dynamic real-time power system simulator
 Home-page: https://github.com/sogno-platform/dpsim
 Author: The DPsim Authors
 Author-email: mmirz@eonerc.rwth-aachen.de
 Project-URL: Bug Tracker, https://github.com/sogno-platform/dpsim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <img src="docs/images/dpsim.png" width=40 /> DPsim
 
 [![Build & Test CentOS](https://github.com/sogno-platform/dpsim/actions/workflows/build_test_linux_centos.yaml/badge.svg)](https://github.com/sogno-platform/dpsim/actions/workflows/build_test_linux_centos.yaml)
```

### Comparing `dpsim-1.1.0/python/src/dpsim/matpower.py` & `dpsim-1.1.1/python/src/dpsim/matpower.py`

 * *Files identical despite different names*

### Comparing `dpsim-1.1.0/setup.cfg` & `dpsim-1.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dpsim
-version = 1.1.0
+version = 1.1.1
 author = The DPsim Authors
 author_email = mmirz@eonerc.rwth-aachen.de
 description = dynamic real-time power system simulator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sogno-platform/dpsim
 project_urls =
```

### Comparing `dpsim-1.1.0/setup.py` & `dpsim-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         subprocess.check_call(
             ['cmake', '--build', '.', '--target', 'dpsimpy'] + build_args, cwd=self.build_temp
         )
 
 setup(
     packages=find_packages('python/src'),
     package_dir={"dpsim": "python/src/dpsim"},
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     setup_requires=[
         'pytest-runner',
         'wheel'
     ],
     tests_require=[
         'pytest',
         'pyyaml',
```

