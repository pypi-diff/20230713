# Comparing `tmp/ladybug-geometry-polyskel-1.4.8.tar.gz` & `tmp/ladybug-geometry-polyskel-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-geometry-polyskel-1.4.8.tar", last modified: Fri Mar 10 22:30:19 2023, max compression
+gzip compressed data, was "dist/ladybug-geometry-polyskel-1.4.9.tar", last modified: Sat Mar 11 17:29:36 2023, max compression
```

## Comparing `ladybug-geometry-polyskel-1.4.8.tar` & `ladybug-geometry-polyskel-1.4.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19697 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel/polygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    28281 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel/polyskel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel/polysplit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/scripts/offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/scripts/offset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:30:19.000000 ladybug-geometry-polyskel-1.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/tests/polygraph_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/tests/polyskel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-03-10 22:29:16.000000 ladybug-geometry-polyskel-1.4.8/tests/polysplit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19697 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel/polygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28281 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel/polyskel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel/polysplit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-11 17:29:35.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-11 17:29:35.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 17:29:35.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-11 17:29:35.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-11 17:29:35.000000 ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/scripts/offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/scripts/offset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:29:36.000000 ladybug-geometry-polyskel-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/tests/polygraph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/tests/polyskel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-03-11 17:28:40.000000 ladybug-geometry-polyskel-1.4.9/tests/polysplit_test.py
```

### Comparing `ladybug-geometry-polyskel-1.4.8/.github/workflows/ci.yaml` & `ladybug-geometry-polyskel-1.4.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/.github/workflows/dependency-release.yaml` & `ladybug-geometry-polyskel-1.4.9/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/LICENSE` & `ladybug-geometry-polyskel-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/PKG-INFO` & `ladybug-geometry-polyskel-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-geometry-polyskel
-Version: 1.4.8
+Version: 1.4.9
 Summary: A library with poly skeleton methods using ladybug-geometry
 Home-page: https://github.com/ladybug-tools/ladybug-geometry-polyskel
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ladybug-geometry-polyskel-1.4.8/README.md` & `ladybug-geometry-polyskel-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/dev-requirements.txt` & `ladybug-geometry-polyskel-1.4.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/docs/_static/custom.css` & `ladybug-geometry-polyskel-1.4.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/docs/_templates/layout.html` & `ladybug-geometry-polyskel-1.4.9/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/docs/conf.py` & `ladybug-geometry-polyskel-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel/polygraph.py` & `ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel/polygraph.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel/polyskel.py` & `ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel/polyskel.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel/polysplit.py` & `ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel/polysplit.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel.egg-info/PKG-INFO` & `ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-geometry-polyskel
-Version: 1.4.8
+Version: 1.4.9
 Summary: A library with poly skeleton methods using ladybug-geometry
 Home-page: https://github.com/ladybug-tools/ladybug-geometry-polyskel
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ladybug-geometry-polyskel-1.4.8/ladybug_geometry_polyskel.egg-info/SOURCES.txt` & `ladybug-geometry-polyskel-1.4.9/ladybug_geometry_polyskel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/scripts/offset.py` & `ladybug-geometry-polyskel-1.4.9/scripts/offset.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/scripts/offset_test.py` & `ladybug-geometry-polyskel-1.4.9/scripts/offset_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/setup.py` & `ladybug-geometry-polyskel-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/tests/polygraph_test.py` & `ladybug-geometry-polyskel-1.4.9/tests/polygraph_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/tests/polyskel_test.py` & `ladybug-geometry-polyskel-1.4.9/tests/polyskel_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-polyskel-1.4.8/tests/polysplit_test.py` & `ladybug-geometry-polyskel-1.4.9/tests/polysplit_test.py`

 * *Files identical despite different names*

