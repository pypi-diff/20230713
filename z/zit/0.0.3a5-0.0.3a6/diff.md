# Comparing `tmp/zit-0.0.3a5.tar.gz` & `tmp/zit-0.0.3a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zit-0.0.3a5.tar", max compression
+gzip compressed data, was "zit-0.0.3a6.tar", max compression
```

## Comparing `zit-0.0.3a5.tar` & `zit-0.0.3a6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1018 2023-07-13 13:42:13.718007 zit-0.0.3a5/pyproject.toml
--rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.3a5/zit/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.3a5/zit/auth.py
--rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.3a5/zit/config.py
--rw-r--r--   0        0        0     8607 2023-07-10 18:46:59.264897 zit-0.0.3a5/zit/dashboard.py
--rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.3a5/zit/dataset/__init__.py
--rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.3a5/zit/dataset/build.py
--rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.3a5/zit/dataset/classification.py
--rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.3a5/zit/dataset/convert.py
--rw-r--r--   0        0        0     1701 2023-07-13 07:46:31.336264 zit-0.0.3a5/zit/dataset/detection.py
--rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.3a5/zit/dataset/factory.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.3a5/zit/dataset/keypoints.py
--rw-r--r--   0        0        0    15749 2023-07-10 23:17:00.512707 zit-0.0.3a5/zit/dataset/manager.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.3a5/zit/dataset/multilabel_classification.py
--rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.3a5/zit/dataset/segmentation.py
--rw-r--r--   0        0        0    12010 2023-07-07 20:00:48.386764 zit-0.0.3a5/zit/formula.py
--rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.3a5/zit/main.py
--rw-r--r--   0        0        0      753 2023-07-12 06:53:22.944703 zit-0.0.3a5/zit/routes/__init__.py
--rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.3a5/zit/routes/dataset/annotations.py
--rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.3a5/zit/routes/dataset/categories.py
--rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.3a5/zit/routes/dataset/images.py
--rw-r--r--   0        0        0     2358 2023-07-12 06:52:27.144711 zit-0.0.3a5/zit/routes/dataset/queries.py
--rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.3a5/zit/utils.py
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 zit-0.0.3a5/setup.py
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 zit-0.0.3a5/PKG-INFO
+-rw-r--r--   0        0        0     1018 2023-07-13 14:27:11.276967 zit-0.0.3a6/pyproject.toml
+-rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.3a6/zit/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.3a6/zit/auth.py
+-rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.3a6/zit/config.py
+-rw-r--r--   0        0        0     8607 2023-07-10 18:46:59.264897 zit-0.0.3a6/zit/dashboard.py
+-rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.3a6/zit/dataset/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.3a6/zit/dataset/build.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.3a6/zit/dataset/classification.py
+-rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.3a6/zit/dataset/convert.py
+-rw-r--r--   0        0        0     1773 2023-07-13 14:23:28.427050 zit-0.0.3a6/zit/dataset/detection.py
+-rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.3a6/zit/dataset/factory.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.3a6/zit/dataset/keypoints.py
+-rw-r--r--   0        0        0    15749 2023-07-10 23:17:00.512707 zit-0.0.3a6/zit/dataset/manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.3a6/zit/dataset/multilabel_classification.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.3a6/zit/dataset/segmentation.py
+-rw-r--r--   0        0        0    12010 2023-07-07 20:00:48.386764 zit-0.0.3a6/zit/formula.py
+-rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.3a6/zit/main.py
+-rw-r--r--   0        0        0      753 2023-07-12 06:53:22.944703 zit-0.0.3a6/zit/routes/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.3a6/zit/routes/dataset/annotations.py
+-rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.3a6/zit/routes/dataset/categories.py
+-rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.3a6/zit/routes/dataset/images.py
+-rw-r--r--   0        0        0     2358 2023-07-12 06:52:27.144711 zit-0.0.3a6/zit/routes/dataset/queries.py
+-rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.3a6/zit/utils.py
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 zit-0.0.3a6/setup.py
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 zit-0.0.3a6/PKG-INFO
```

### Comparing `zit-0.0.3a5/pyproject.toml` & `zit-0.0.3a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zit"
-version = "0.0.3a5"
+version = "0.0.3a6"
 description = "ZitySpace CLI tool"
 authors = ["Rui Zheng <rui@zityspace.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 PyYAML = "^6.0"
@@ -46,10 +46,10 @@
 
 [tool.isort]
 profile = "black"
 skip = ["dist"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.3a5"
+version = "0.0.3a6"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
```

### Comparing `zit-0.0.3a5/zit/auth.py` & `zit-0.0.3a6/zit/auth.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/config.py` & `zit-0.0.3a6/zit/config.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/dashboard.py` & `zit-0.0.3a6/zit/dashboard.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/dataset/convert.py` & `zit-0.0.3a6/zit/dataset/convert.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/dataset/detection.py` & `zit-0.0.3a6/zit/dataset/detection.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 from ..routes import build_default_router
 from ..utils import find_zit_root
 from .build import DatasetBuilder
 from .factory import DatasetFactory
 from .manager import Manager
 
 
+def abspath(path):
+    return os.path.abspath(path)
+
+
 class DetectionDatasetBuilder(DatasetBuilder):
     def __call__(self, **kwargs):
         zit_root = find_zit_root(Path.cwd())
 
-        image_source = str(zit_root / kwargs.get("image_source", "images"))
-        annotation_source = str(zit_root / kwargs.get("annotation_source", "annotations.csv"))
+        image_source = abspath(kwargs.get("image_source", str(zit_root / "images")))
+        annotation_source = abspath(kwargs.get("annotation_source", str(zit_root / "annotations.csv")))
 
         params = {
             "task": "detection",
             "image_source": image_source,
             "annotation_source": annotation_source,
         }
```

### Comparing `zit-0.0.3a5/zit/dataset/manager.py` & `zit-0.0.3a6/zit/dataset/manager.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/formula.py` & `zit-0.0.3a6/zit/formula.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/main.py` & `zit-0.0.3a6/zit/main.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/routes/__init__.py` & `zit-0.0.3a6/zit/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/routes/dataset/annotations.py` & `zit-0.0.3a6/zit/routes/dataset/annotations.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/routes/dataset/categories.py` & `zit-0.0.3a6/zit/routes/dataset/categories.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/routes/dataset/images.py` & `zit-0.0.3a6/zit/routes/dataset/images.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/zit/routes/dataset/queries.py` & `zit-0.0.3a6/zit/routes/dataset/queries.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a5/setup.py` & `zit-0.0.3a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'websocket-client>=1.5.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['zit = zit.main:app']}
 
 setup_kwargs = {
     'name': 'zit',
-    'version': '0.0.3a5',
+    'version': '0.0.3a6',
     'description': 'ZitySpace CLI tool',
     'long_description': 'None',
     'author': 'Rui Zheng',
     'author_email': 'rui@zityspace.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `zit-0.0.3a5/PKG-INFO` & `zit-0.0.3a6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zit
-Version: 0.0.3a5
+Version: 0.0.3a6
 Summary: ZitySpace CLI tool
 License: MIT
 Author: Rui Zheng
 Author-email: rui@zityspace.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

