# Comparing `tmp/ForestScience-0.0.5.tar.gz` & `tmp/ForestScience-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForestScience-0.0.5.tar", last modified: Thu Jul 13 04:20:44 2023, max compression
+gzip compressed data, was "ForestScience-0.0.6.tar", last modified: Thu Jul 13 04:23:02 2023, max compression
```

## Comparing `ForestScience-0.0.5.tar` & `ForestScience-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:20:44.632686 ForestScience-0.0.5/
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:20:44.475686 ForestScience-0.0.5/ForestScience/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14954 2023-07-13 04:20:41.000000 ForestScience-0.0.5/ForestScience/InventarioFlorestal.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-13 04:20:41.000000 ForestScience-0.0.5/ForestScience/__init__.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2689 2023-07-13 04:20:41.000000 ForestScience-0.0.5/ForestScience/_modidx.py
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:20:44.610688 ForestScience-0.0.5/ForestScience.egg-info/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1418 2023-07-13 04:20:44.000000 ForestScience-0.0.5/ForestScience.egg-info/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      399 2023-07-13 04:20:44.000000 ForestScience-0.0.5/ForestScience.egg-info/SOURCES.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 04:20:44.000000 ForestScience-0.0.5/ForestScience.egg-info/dependency_links.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       48 2023-07-13 04:20:44.000000 ForestScience-0.0.5/ForestScience.egg-info/entry_points.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 03:36:15.000000 ForestScience-0.0.5/ForestScience.egg-info/not-zip-safe
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-13 04:20:44.000000 ForestScience-0.0.5/ForestScience.egg-info/requires.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       14 2023-07-13 04:20:44.000000 ForestScience-0.0.5/ForestScience.egg-info/top_level.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11357 2023-07-13 03:11:19.000000 ForestScience-0.0.5/LICENSE
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestScience-0.0.5/MANIFEST.in
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1418 2023-07-13 04:20:44.630688 ForestScience-0.0.5/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      635 2023-07-13 04:10:57.000000 ForestScience-0.0.5/README.md
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      876 2023-07-13 04:20:41.000000 ForestScience-0.0.5/settings.ini
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-13 04:20:44.633688 ForestScience-0.0.5/setup.cfg
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestScience-0.0.5/setup.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:23:02.108260 ForestScience-0.0.6/
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:23:01.951259 ForestScience-0.0.6/ForestScience/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14954 2023-07-13 04:22:58.000000 ForestScience-0.0.6/ForestScience/InventarioFlorestal.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-13 04:22:58.000000 ForestScience-0.0.6/ForestScience/__init__.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2689 2023-07-13 04:22:58.000000 ForestScience-0.0.6/ForestScience/_modidx.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:23:02.086258 ForestScience-0.0.6/ForestScience.egg-info/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1418 2023-07-13 04:23:01.000000 ForestScience-0.0.6/ForestScience.egg-info/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      399 2023-07-13 04:23:01.000000 ForestScience-0.0.6/ForestScience.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 04:23:01.000000 ForestScience-0.0.6/ForestScience.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       48 2023-07-13 04:23:01.000000 ForestScience-0.0.6/ForestScience.egg-info/entry_points.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 03:36:15.000000 ForestScience-0.0.6/ForestScience.egg-info/not-zip-safe
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-13 04:23:01.000000 ForestScience-0.0.6/ForestScience.egg-info/requires.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       14 2023-07-13 04:23:01.000000 ForestScience-0.0.6/ForestScience.egg-info/top_level.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11357 2023-07-13 03:11:19.000000 ForestScience-0.0.6/LICENSE
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestScience-0.0.6/MANIFEST.in
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1418 2023-07-13 04:23:02.105257 ForestScience-0.0.6/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      635 2023-07-13 04:10:57.000000 ForestScience-0.0.6/README.md
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      876 2023-07-13 04:22:58.000000 ForestScience-0.0.6/settings.ini
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-13 04:23:02.109259 ForestScience-0.0.6/setup.cfg
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestScience-0.0.6/setup.py
```

### Comparing `ForestScience-0.0.5/ForestScience/InventarioFlorestal.py` & `ForestScience-0.0.6/ForestScience/InventarioFlorestal.py`

 * *Files identical despite different names*

### Comparing `ForestScience-0.0.5/ForestScience/_modidx.py` & `ForestScience-0.0.6/ForestScience/_modidx.py`

 * *Files identical despite different names*

### Comparing `ForestScience-0.0.5/ForestScience.egg-info/PKG-INFO` & `ForestScience-0.0.6/ForestScience.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestScience
-Version: 0.0.5
+Version: 0.0.6
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestScience
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ForestScience-0.0.5/LICENSE` & `ForestScience-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ForestScience-0.0.5/PKG-INFO` & `ForestScience-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestScience
-Version: 0.0.5
+Version: 0.0.6
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestScience
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ForestScience-0.0.5/README.md` & `ForestScience-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ForestScience-0.0.5/settings.ini` & `ForestScience-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ForestScience
 lib_name = ForestScience
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ForestScience
 nbs_path = nbs
 recursive = True
```

### Comparing `ForestScience-0.0.5/setup.py` & `ForestScience-0.0.6/setup.py`

 * *Files identical despite different names*

