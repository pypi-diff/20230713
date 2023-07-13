# Comparing `tmp/imarkdown-1.1.0.tar.gz` & `tmp/imarkdown-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imarkdown-1.1.0.tar", last modified: Thu Jul 13 09:34:00 2023, max compression
+gzip compressed data, was "imarkdown-1.1.1.tar", last modified: Thu Jul 13 16:52:49 2023, max compression
```

## Comparing `imarkdown-1.1.0.tar` & `imarkdown-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.076101 imarkdown-1.1.0/
--rw-rw-rw-   0        0        0    17228 2023-07-13 09:34:00.075103 imarkdown-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    16366 2023-07-13 09:18:34.000000 imarkdown-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.046037 imarkdown-1.1.0/imarkdown/
--rw-rw-rw-   0        0        0      464 2023-07-12 09:17:55.000000 imarkdown-1.1.0/imarkdown/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.060212 imarkdown-1.1.0/imarkdown/adapter/
--rw-rw-rw-   0        0        0      476 2023-07-06 15:57:43.000000 imarkdown-1.1.0/imarkdown/adapter/__init__.py
--rw-rw-rw-   0        0        0     2939 2023-07-12 09:17:55.000000 imarkdown-1.1.0/imarkdown/adapter/aliyun_adapter.py
--rw-rw-rw-   0        0        0      835 2023-07-12 14:17:49.000000 imarkdown-1.1.0/imarkdown/adapter/base.py
--rw-rw-rw-   0        0        0      755 2023-07-09 06:11:27.000000 imarkdown-1.1.0/imarkdown/adapter/local_adapter.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.061115 imarkdown-1.1.0/imarkdown/client/
--rw-rw-rw-   0        0        0        0 2023-07-12 09:17:53.000000 imarkdown-1.1.0/imarkdown/client/__init__.py
--rw-rw-rw-   0        0        0     1371 2023-07-12 10:24:22.000000 imarkdown-1.1.0/imarkdown/config.py
--rw-rw-rw-   0        0        0      267 2023-07-06 13:32:07.000000 imarkdown-1.1.0/imarkdown/constant.py
--rw-rw-rw-   0        0        0    12736 2023-07-13 06:24:26.000000 imarkdown-1.1.0/imarkdown/converter.py
--rw-rw-rw-   0        0        0     9764 2023-07-12 10:45:20.000000 imarkdown-1.1.0/imarkdown/schema.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.065101 imarkdown-1.1.0/imarkdown/utils/
--rw-rw-rw-   0        0        0     2784 2023-07-12 10:45:20.000000 imarkdown-1.1.0/imarkdown/utils/__init__.py
--rw-rw-rw-   0        0        0      282 2023-07-06 15:57:43.000000 imarkdown-1.1.0/imarkdown/utils/cache.py
--rw-rw-rw-   0        0        0     1403 2023-07-02 17:09:48.000000 imarkdown-1.1.0/imarkdown/utils/singleton.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.053581 imarkdown-1.1.0/imarkdown.egg-info/
--rw-rw-rw-   0        0        0    17228 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2022-12-18 07:47:47.000000 imarkdown-1.1.0/license
--rw-rw-rw-   0        0        0       42 2023-07-13 09:34:00.076101 imarkdown-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1904 2023-07-13 09:00:03.000000 imarkdown-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.073104 imarkdown-1.1.0/tests/
--rw-rw-rw-   0        0        0     2379 2023-07-12 09:57:46.000000 imarkdown-1.1.0/tests/test_adapter.py
--rw-rw-rw-   0        0        0     2273 2023-07-12 09:17:55.000000 imarkdown-1.1.0/tests/test_image_converter.py
--rw-rw-rw-   0        0        0     2235 2023-07-12 09:21:39.000000 imarkdown-1.1.0/tests/test_md_file.py
--rw-rw-rw-   0        0        0     2957 2023-07-12 08:04:11.000000 imarkdown-1.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.721447 imarkdown-1.1.1/
+-rw-rw-rw-   0        0        0    17228 2023-07-13 16:52:49.720446 imarkdown-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16366 2023-07-13 10:10:10.000000 imarkdown-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.691455 imarkdown-1.1.1/imarkdown/
+-rw-rw-rw-   0        0        0      464 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.706447 imarkdown-1.1.1/imarkdown/adapter/
+-rw-rw-rw-   0        0        0      476 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/adapter/__init__.py
+-rw-rw-rw-   0        0        0     2939 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/adapter/aliyun_adapter.py
+-rw-rw-rw-   0        0        0      835 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/adapter/base.py
+-rw-rw-rw-   0        0        0      755 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/adapter/local_adapter.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.707446 imarkdown-1.1.1/imarkdown/client/
+-rw-rw-rw-   0        0        0        0 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/client/__init__.py
+-rw-rw-rw-   0        0        0     1371 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/config.py
+-rw-rw-rw-   0        0        0      267 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/constant.py
+-rw-rw-rw-   0        0        0    12736 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/converter.py
+-rw-rw-rw-   0        0        0     9764 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/schema.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.712448 imarkdown-1.1.1/imarkdown/utils/
+-rw-rw-rw-   0        0        0     2784 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/utils/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/utils/cache.py
+-rw-rw-rw-   0        0        0     1403 2023-07-13 10:10:10.000000 imarkdown-1.1.1/imarkdown/utils/singleton.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.699448 imarkdown-1.1.1/imarkdown.egg-info/
+-rw-rw-rw-   0        0        0    17228 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 16:52:49.000000 imarkdown-1.1.1/imarkdown.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2022-12-18 07:47:47.000000 imarkdown-1.1.1/license
+-rw-rw-rw-   0        0        0       42 2023-07-13 16:52:49.721447 imarkdown-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1940 2023-07-13 16:52:05.000000 imarkdown-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:49.718448 imarkdown-1.1.1/tests/
+-rw-rw-rw-   0        0        0     2379 2023-07-13 10:10:10.000000 imarkdown-1.1.1/tests/test_adapter.py
+-rw-rw-rw-   0        0        0     2273 2023-07-13 10:10:10.000000 imarkdown-1.1.1/tests/test_image_converter.py
+-rw-rw-rw-   0        0        0     2235 2023-07-13 10:10:10.000000 imarkdown-1.1.1/tests/test_md_file.py
+-rw-rw-rw-   0        0        0     2957 2023-07-13 10:10:10.000000 imarkdown-1.1.1/tests/test_utils.py
```

### Comparing `imarkdown-1.1.0/PKG-INFO` & `imarkdown-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imarkdown
-Version: 1.1.0
+Version: 1.1.1
 Summary: A practical Markdown image url converter
 Home-page: https://github.com/Undertone0809/imarkdown
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: Markdown,markdown,imarkdown,markdown converter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `imarkdown-1.1.0/README.md` & `imarkdown-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown/adapter/aliyun_adapter.py` & `imarkdown-1.1.1/imarkdown/adapter/aliyun_adapter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown/adapter/base.py` & `imarkdown-1.1.1/imarkdown/adapter/base.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown/adapter/local_adapter.py` & `imarkdown-1.1.1/imarkdown/adapter/local_adapter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown/config.py` & `imarkdown-1.1.1/imarkdown/config.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown/converter.py` & `imarkdown-1.1.1/imarkdown/converter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown/schema.py` & `imarkdown-1.1.1/imarkdown/schema.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown/utils/__init__.py` & `imarkdown-1.1.1/imarkdown/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown/utils/singleton.py` & `imarkdown-1.1.1/imarkdown/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/imarkdown.egg-info/PKG-INFO` & `imarkdown-1.1.1/imarkdown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imarkdown
-Version: 1.1.0
+Version: 1.1.1
 Summary: A practical Markdown image url converter
 Home-page: https://github.com/Undertone0809/imarkdown
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: Markdown,markdown,imarkdown,markdown converter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `imarkdown-1.1.0/imarkdown.egg-info/SOURCES.txt` & `imarkdown-1.1.1/imarkdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/license` & `imarkdown-1.1.1/license`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/setup.py` & `imarkdown-1.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 import setuptools
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="imarkdown",
-    version="1.1.0",
+    version="1.1.1",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A practical Markdown image url converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/imarkdown",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
-        "pydantic==1.10.0",
-        "cushy-storage"
-
+        "pydantic~=1.10.0",
+        "cushy-storage",
+        'broadcast-service==1.3.2',
     ],
     license="Apache 2.0",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

### Comparing `imarkdown-1.1.0/tests/test_adapter.py` & `imarkdown-1.1.1/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/tests/test_image_converter.py` & `imarkdown-1.1.1/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/tests/test_md_file.py` & `imarkdown-1.1.1/tests/test_md_file.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.1.0/tests/test_utils.py` & `imarkdown-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

