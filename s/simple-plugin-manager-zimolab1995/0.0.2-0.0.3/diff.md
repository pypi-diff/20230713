# Comparing `tmp/simple_plugin_manager_zimolab1995-0.0.2.tar.gz` & `tmp/simple_plugin_manager_zimolab1995-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_plugin_manager_zimolab1995-0.0.2.tar", last modified: Thu Jul 13 12:03:34 2023, max compression
+gzip compressed data, was "simple_plugin_manager_zimolab1995-0.0.3.tar", last modified: Thu Jul 13 12:08:34 2023, max compression
```

## Comparing `simple_plugin_manager_zimolab1995-0.0.2.tar` & `simple_plugin_manager_zimolab1995-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 12:03:34.726060 simple_plugin_manager_zimolab1995-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-12 14:17:41.000000 simple_plugin_manager_zimolab1995-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      653 2023-07-13 12:03:34.726060 simple_plugin_manager_zimolab1995-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-12 14:16:25.000000 simple_plugin_manager_zimolab1995-0.0.2/README.md
--rw-rw-rw-   0        0        0      660 2023-07-13 12:03:06.000000 simple_plugin_manager_zimolab1995-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       95 2023-07-13 12:03:34.726060 simple_plugin_manager_zimolab1995-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-13 12:03:34.702080 simple_plugin_manager_zimolab1995-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:03:34.714075 simple_plugin_manager_zimolab1995-0.0.2/src/plugin_manager/
--rw-rw-rw-   0        0        0        0 2023-07-12 14:18:01.000000 simple_plugin_manager_zimolab1995-0.0.2/src/plugin_manager/__init__.py
--rw-rw-rw-   0        0        0      212 2023-07-13 11:05:22.000000 simple_plugin_manager_zimolab1995-0.0.2/src/plugin_manager/exceptions.py
--rw-rw-rw-   0        0        0    13468 2023-07-13 11:21:51.000000 simple_plugin_manager_zimolab1995-0.0.2/src/plugin_manager/manager.py
--rw-rw-rw-   0        0        0      865 2023-07-13 09:13:06.000000 simple_plugin_manager_zimolab1995-0.0.2/src/plugin_manager/plugin.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:03:34.722059 simple_plugin_manager_zimolab1995-0.0.2/src/simple_plugin_manager_zimolab1995.egg-info/
--rw-rw-rw-   0        0        0      653 2023-07-13 12:03:34.000000 simple_plugin_manager_zimolab1995-0.0.2/src/simple_plugin_manager_zimolab1995.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-07-13 12:03:34.000000 simple_plugin_manager_zimolab1995-0.0.2/src/simple_plugin_manager_zimolab1995.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 12:03:34.000000 simple_plugin_manager_zimolab1995-0.0.2/src/simple_plugin_manager_zimolab1995.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-13 12:03:34.000000 simple_plugin_manager_zimolab1995-0.0.2/src/simple_plugin_manager_zimolab1995.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-13 12:03:34.000000 simple_plugin_manager_zimolab1995-0.0.2/src/simple_plugin_manager_zimolab1995.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 12:08:34.094561 simple_plugin_manager_zimolab1995-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-12 14:17:41.000000 simple_plugin_manager_zimolab1995-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      653 2023-07-13 12:08:34.094561 simple_plugin_manager_zimolab1995-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-12 14:16:25.000000 simple_plugin_manager_zimolab1995-0.0.3/README.md
+-rw-rw-rw-   0        0        0      660 2023-07-13 12:08:09.000000 simple_plugin_manager_zimolab1995-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-07-13 12:08:34.094561 simple_plugin_manager_zimolab1995-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 12:08:34.074505 simple_plugin_manager_zimolab1995-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:08:34.085034 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/
+-rw-rw-rw-   0        0        0        0 2023-07-12 14:18:01.000000 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-07-13 11:05:22.000000 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/exceptions.py
+-rw-rw-rw-   0        0        0    13468 2023-07-13 11:21:51.000000 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/manager.py
+-rw-rw-rw-   0        0        0      865 2023-07-13 09:13:06.000000 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/plugin.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:08:34.094561 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/
+-rw-rw-rw-   0        0        0      653 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/top_level.txt
```

### Comparing `simple_plugin_manager_zimolab1995-0.0.2/LICENSE` & `simple_plugin_manager_zimolab1995-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_plugin_manager_zimolab1995-0.0.2/PKG-INFO` & `simple_plugin_manager_zimolab1995-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_plugin_manager_zimolab1995
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple plugin manager for python project
 Author-email: zimolab1995 <zimolab@aliyun.com>
 Project-URL: Homepage, https://gitee.com/zimolab1995/simple_plugin_manager
 Project-URL: Bug Tracker, https://gitee.com/zimolab1995/simple_plugin_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_plugin_manager_zimolab1995-0.0.2/pyproject.toml` & `simple_plugin_manager_zimolab1995-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple_plugin_manager_zimolab1995"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="zimolab1995", email="zimolab@aliyun.com" },
 ]
 description = "A simple plugin manager for python project"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simple_plugin_manager_zimolab1995-0.0.2/src/plugin_manager/manager.py` & `simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/manager.py`

 * *Files identical despite different names*

### Comparing `simple_plugin_manager_zimolab1995-0.0.2/src/plugin_manager/plugin.py` & `simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/plugin.py`

 * *Files identical despite different names*

### Comparing `simple_plugin_manager_zimolab1995-0.0.2/src/simple_plugin_manager_zimolab1995.egg-info/PKG-INFO` & `simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-plugin-manager-zimolab1995
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple plugin manager for python project
 Author-email: zimolab1995 <zimolab@aliyun.com>
 Project-URL: Homepage, https://gitee.com/zimolab1995/simple_plugin_manager
 Project-URL: Bug Tracker, https://gitee.com/zimolab1995/simple_plugin_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

