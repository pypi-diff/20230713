# Comparing `tmp/magik-0.1.0.tar.gz` & `tmp/magik-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.1.0.tar", last modified: Tue Jul 11 16:07:28 2023, max compression
+gzip compressed data, was "magik-0.1.1.tar", last modified: Thu Jul 13 00:34:40 2023, max compression
```

## Comparing `magik-0.1.0.tar` & `magik-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-11 16:07:28.830141 magik-0.1.0/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-11 16:07:28.829923 magik-0.1.0/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2840 2023-07-11 14:25:41.000000 magik-0.1.0/README.md
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-11 16:07:28.825164 magik-0.1.0/magik.egg-info/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-11 16:07:28.000000 magik-0.1.0/magik.egg-info/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      600 2023-07-11 16:07:28.000000 magik-0.1.0/magik.egg-info/SOURCES.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-11 16:07:28.000000 magik-0.1.0/magik.egg-info/dependency_links.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       52 2023-07-11 16:07:28.000000 magik-0.1.0/magik.egg-info/entry_points.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      244 2023-07-11 16:07:28.000000 magik-0.1.0/magik.egg-info/requires.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       17 2023-07-11 16:07:28.000000 magik-0.1.0/magik.egg-info/top_level.txt
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-11 16:07:28.829060 magik-0.1.0/magik_prompt_sdk/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       34 2023-07-11 15:55:34.000000 magik-0.1.0/magik_prompt_sdk/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1301 2023-07-11 14:06:10.000000 magik-0.1.0/magik_prompt_sdk/cli.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      477 2023-07-11 13:50:13.000000 magik-0.1.0/magik_prompt_sdk/config.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      515 2023-07-11 13:26:16.000000 magik-0.1.0/magik_prompt_sdk/constants.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1392 2023-07-11 13:46:49.000000 magik-0.1.0/magik_prompt_sdk/deploy.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     7014 2023-07-11 15:55:38.000000 magik-0.1.0/magik_prompt_sdk/evaluators.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      746 2023-07-08 22:47:12.000000 magik-0.1.0/magik_prompt_sdk/generate.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1711 2023-07-08 22:46:41.000000 magik-0.1.0/magik_prompt_sdk/initialize.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-11 16:07:28.829337 magik-0.1.0/magik_prompt_sdk/logger/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-06 18:14:00.000000 magik-0.1.0/magik_prompt_sdk/logger/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.0/magik_prompt_sdk/matchers.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     4382 2023-07-11 15:55:33.000000 magik-0.1.0/magik_prompt_sdk/openai_helper.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     5733 2023-07-11 15:55:39.000000 magik-0.1.0/magik_prompt_sdk/run.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2992 2023-07-08 22:49:32.000000 magik-0.1.0/magik_prompt_sdk/sys_exec.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      299 2023-07-06 16:24:21.000000 magik-0.1.0/magik_prompt_sdk/utils.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-11 16:07:28.830207 magik-0.1.0/setup.cfg
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      834 2023-07-11 16:06:41.000000 magik-0.1.0/setup.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-13 00:34:40.831130 magik-0.1.1/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-13 00:34:40.831009 magik-0.1.1/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2840 2023-07-11 14:25:41.000000 magik-0.1.1/README.md
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-13 00:34:40.825345 magik-0.1.1/magik.egg-info/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      600 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/SOURCES.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/dependency_links.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       52 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/entry_points.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      246 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/requires.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       17 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/top_level.txt
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-13 00:34:40.830525 magik-0.1.1/magik_prompt_sdk/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       34 2023-07-11 15:55:34.000000 magik-0.1.1/magik_prompt_sdk/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1301 2023-07-11 14:06:10.000000 magik-0.1.1/magik_prompt_sdk/cli.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      477 2023-07-11 13:50:13.000000 magik-0.1.1/magik_prompt_sdk/config.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      515 2023-07-11 13:26:16.000000 magik-0.1.1/magik_prompt_sdk/constants.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1392 2023-07-11 13:46:49.000000 magik-0.1.1/magik_prompt_sdk/deploy.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     7014 2023-07-11 15:55:38.000000 magik-0.1.1/magik_prompt_sdk/evaluators.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      746 2023-07-08 22:47:12.000000 magik-0.1.1/magik_prompt_sdk/generate.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1711 2023-07-08 22:46:41.000000 magik-0.1.1/magik_prompt_sdk/initialize.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-13 00:34:40.830735 magik-0.1.1/magik_prompt_sdk/logger/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-06 18:14:00.000000 magik-0.1.1/magik_prompt_sdk/logger/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.1/magik_prompt_sdk/matchers.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     4382 2023-07-13 00:02:48.000000 magik-0.1.1/magik_prompt_sdk/openai_helper.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     5733 2023-07-11 15:55:39.000000 magik-0.1.1/magik_prompt_sdk/run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2992 2023-07-08 22:49:32.000000 magik-0.1.1/magik_prompt_sdk/sys_exec.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      299 2023-07-06 16:24:21.000000 magik-0.1.1/magik_prompt_sdk/utils.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-13 00:34:40.831162 magik-0.1.1/setup.cfg
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      834 2023-07-13 00:32:47.000000 magik-0.1.1/setup.py
```

### Comparing `magik-0.1.0/PKG-INFO` & `magik-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDK to write and run tests for your LLM app
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `magik-0.1.0/README.md` & `magik-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik.egg-info/PKG-INFO` & `magik-0.1.1/magik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDK to write and run tests for your LLM app
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `magik-0.1.0/magik.egg-info/SOURCES.txt` & `magik-0.1.1/magik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/cli.py` & `magik-0.1.1/magik_prompt_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/constants.py` & `magik-0.1.1/magik_prompt_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/deploy.py` & `magik-0.1.1/magik_prompt_sdk/deploy.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/evaluators.py` & `magik-0.1.1/magik_prompt_sdk/evaluators.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/generate.py` & `magik-0.1.1/magik_prompt_sdk/generate.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/initialize.py` & `magik-0.1.1/magik_prompt_sdk/initialize.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/logger/__init__.py` & `magik-0.1.1/magik_prompt_sdk/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/openai_helper.py` & `magik-0.1.1/magik_prompt_sdk/openai_helper.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/run.py` & `magik-0.1.1/magik_prompt_sdk/run.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/magik_prompt_sdk/sys_exec.py` & `magik-0.1.1/magik_prompt_sdk/sys_exec.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.0/setup.py` & `magik-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="magik",
-    version="0.1.0",
+    version="0.1.1",
     author="Magik Labs Team",
     author_email="hello@magiklabs.app",
     description="SDK to write and run tests for your LLM app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

