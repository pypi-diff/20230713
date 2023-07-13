# Comparing `tmp/SPACEL-1.1.3.tar.gz` & `tmp/SPACEL-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPACEL-1.1.3.tar", last modified: Thu Jul 13 01:49:22 2023, max compression
+gzip compressed data, was "SPACEL-1.1.4.tar", last modified: Thu Jul 13 02:22:31 2023, max compression
```

## Comparing `SPACEL-1.1.3.tar` & `SPACEL-1.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:49:22.031698 SPACEL-1.1.3/
--rw-r--r--   0 xuhao      (501) staff       (20)     4009 2023-07-13 01:49:22.031336 SPACEL-1.1.3/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)     3708 2023-07-12 13:44:19.000000 SPACEL-1.1.3/README.md
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:49:21.939855 SPACEL-1.1.3/SPACEL/
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:49:21.970072 SPACEL-1.1.3/SPACEL/Scube/
--rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Scube/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.3/SPACEL/Scube/alignment.py
--rw-r--r--   0 xuhao      (501) staff       (20)    16402 2023-07-13 00:51:58.000000 SPACEL-1.1.3/SPACEL/Scube/gpr.py
--rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Scube/plot.py
--rw-r--r--   0 xuhao      (501) staff       (20)     6635 2023-07-12 13:05:31.000000 SPACEL-1.1.3/SPACEL/Scube/utils_3d.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:49:22.024994 SPACEL-1.1.3/SPACEL/Splane/
--rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Splane/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    15183 2023-07-11 12:20:57.000000 SPACEL-1.1.3/SPACEL/Splane/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Splane/graph.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:49:22.026611 SPACEL-1.1.3/SPACEL/Splane/kegra/
--rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Splane/kegra/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Splane/kegra/gnn.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Splane/kegra/gnn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Splane/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Splane/pygcn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4269 2023-07-13 01:47:26.000000 SPACEL-1.1.3/SPACEL/Splane/utils.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:49:22.030791 SPACEL-1.1.3/SPACEL/Spoint/
--rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Spoint/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.3/SPACEL/Spoint/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Spoint/data_augmentation.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Spoint/data_downsample.py
--rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Spoint/data_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Spoint/metrics.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Spoint/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/Spoint/spatial_simulation.py
--rw-r--r--   0 xuhao      (501) staff       (20)      226 2023-07-12 13:29:08.000000 SPACEL-1.1.3/SPACEL/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-13 01:47:44.000000 SPACEL-1.1.3/SPACEL/_version.py
--rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.3/SPACEL/setting.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:49:21.942088 SPACEL-1.1.3/SPACEL.egg-info/
--rw-r--r--   0 xuhao      (501) staff       (20)     4009 2023-07-13 01:49:21.000000 SPACEL-1.1.3/SPACEL.egg-info/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-13 01:49:21.000000 SPACEL-1.1.3/SPACEL.egg-info/SOURCES.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-13 01:49:21.000000 SPACEL-1.1.3/SPACEL.egg-info/dependency_links.txt
--rw-r--r--   0 xuhao      (501) staff       (20)      120 2023-07-13 01:49:21.000000 SPACEL-1.1.3/SPACEL.egg-info/requires.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-13 01:49:21.000000 SPACEL-1.1.3/SPACEL.egg-info/top_level.txt
--rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-13 01:49:22.031815 SPACEL-1.1.3/setup.cfg
--rw-r--r--   0 xuhao      (501) staff       (20)      908 2023-07-11 12:48:07.000000 SPACEL-1.1.3/setup.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.770411 SPACEL-1.1.4/
+-rw-r--r--   0 xuhao      (501) staff       (20)     4009 2023-07-13 02:22:31.769992 SPACEL-1.1.4/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)     3708 2023-07-12 13:44:19.000000 SPACEL-1.1.4/README.md
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.662074 SPACEL-1.1.4/SPACEL/
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.689779 SPACEL-1.1.4/SPACEL/Scube/
+-rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Scube/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.4/SPACEL/Scube/alignment.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    16402 2023-07-13 00:51:58.000000 SPACEL-1.1.4/SPACEL/Scube/gpr.py
+-rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Scube/plot.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6635 2023-07-12 13:05:31.000000 SPACEL-1.1.4/SPACEL/Scube/utils_3d.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.747946 SPACEL-1.1.4/SPACEL/Splane/
+-rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    15183 2023-07-11 12:20:57.000000 SPACEL-1.1.4/SPACEL/Splane/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/graph.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.763519 SPACEL-1.1.4/SPACEL/Splane/kegra/
+-rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/kegra/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/kegra/gnn.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/kegra/gnn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/pygcn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4269 2023-07-13 01:47:26.000000 SPACEL-1.1.4/SPACEL/Splane/utils.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.768054 SPACEL-1.1.4/SPACEL/Spoint/
+-rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.4/SPACEL/Spoint/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/data_augmentation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/data_downsample.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/data_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/metrics.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/spatial_simulation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      226 2023-07-12 13:29:08.000000 SPACEL-1.1.4/SPACEL/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-13 02:21:25.000000 SPACEL-1.1.4/SPACEL/_version.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/setting.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.664270 SPACEL-1.1.4/SPACEL.egg-info/
+-rw-r--r--   0 xuhao      (501) staff       (20)     4009 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/SOURCES.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/dependency_links.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)      108 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/requires.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/top_level.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-13 02:22:31.770517 SPACEL-1.1.4/setup.cfg
+-rw-r--r--   0 xuhao      (501) staff       (20)      885 2023-07-13 02:20:15.000000 SPACEL-1.1.4/setup.py
```

### Comparing `SPACEL-1.1.3/PKG-INFO` & `SPACEL-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPACEL
-Version: 1.1.3
+Version: 1.1.4
 Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
 Home-page: https://github.com/QuKunLab/SPACEL
 Author: Hao Xu
 Author-email: xuhaoustc@mail.ustc.edu.cn
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `SPACEL-1.1.3/README.md` & `SPACEL-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Scube/alignment.py` & `SPACEL-1.1.4/SPACEL/Scube/alignment.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Scube/gpr.py` & `SPACEL-1.1.4/SPACEL/Scube/gpr.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Scube/plot.py` & `SPACEL-1.1.4/SPACEL/Scube/plot.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Scube/utils_3d.py` & `SPACEL-1.1.4/SPACEL/Scube/utils_3d.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Splane/base_model.py` & `SPACEL-1.1.4/SPACEL/Splane/base_model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Splane/graph.py` & `SPACEL-1.1.4/SPACEL/Splane/graph.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Splane/kegra/gnn.py` & `SPACEL-1.1.4/SPACEL/Splane/kegra/gnn.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Splane/kegra/gnn_utils.py` & `SPACEL-1.1.4/SPACEL/Splane/kegra/gnn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Splane/model.py` & `SPACEL-1.1.4/SPACEL/Splane/model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Splane/pygcn_utils.py` & `SPACEL-1.1.4/SPACEL/Splane/pygcn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Splane/utils.py` & `SPACEL-1.1.4/SPACEL/Splane/utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Spoint/base_model.py` & `SPACEL-1.1.4/SPACEL/Spoint/base_model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Spoint/data_augmentation.py` & `SPACEL-1.1.4/SPACEL/Spoint/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Spoint/data_downsample.py` & `SPACEL-1.1.4/SPACEL/Spoint/data_downsample.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Spoint/data_utils.py` & `SPACEL-1.1.4/SPACEL/Spoint/data_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Spoint/metrics.py` & `SPACEL-1.1.4/SPACEL/Spoint/metrics.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Spoint/model.py` & `SPACEL-1.1.4/SPACEL/Spoint/model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/Spoint/spatial_simulation.py` & `SPACEL-1.1.4/SPACEL/Spoint/spatial_simulation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL/setting.py` & `SPACEL-1.1.4/SPACEL/setting.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/SPACEL.egg-info/PKG-INFO` & `SPACEL-1.1.4/SPACEL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPACEL
-Version: 1.1.3
+Version: 1.1.4
 Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
 Home-page: https://github.com/QuKunLab/SPACEL
 Author: Hao Xu
 Author-email: xuhaoustc@mail.ustc.edu.cn
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `SPACEL-1.1.3/SPACEL.egg-info/SOURCES.txt` & `SPACEL-1.1.4/SPACEL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.3/setup.py` & `SPACEL-1.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/QuKunLab/SPACEL",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=[
         "pip",
-        "rpy2==3.3.*",
         "squidpy",
         "scvi-tools",
         "scipy",
         "scikit-learn",
         "matplotlib",
         "seaborn",
         "scanpy",
```

