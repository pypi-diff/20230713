# Comparing `tmp/giszhao-0.0.1.tar.gz` & `tmp/giszhao-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giszhao-0.0.1.tar", last modified: Sun Jul  9 19:12:06 2023, max compression
+gzip compressed data, was "giszhao-0.0.2.tar", last modified: Thu Jul 13 15:57:39 2023, max compression
```

## Comparing `giszhao-0.0.1.tar` & `giszhao-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yzhao233 (1622298973) 1024005267        0 2023-07-09 19:12:06.835957 giszhao-0.0.1/
--rw-r--r--   0 yzhao233 (1622298973) 1024005267     1067 2023-07-05 16:06:55.000000 giszhao-0.0.1/LICENSE
--rw-r--r--   0 yzhao233 (1622298973) 1024005267      122 2023-07-05 16:06:55.000000 giszhao-0.0.1/MANIFEST.in
--rw-r--r--   0 yzhao233 (1622298973) 1024005267     1109 2023-07-09 19:12:06.836009 giszhao-0.0.1/PKG-INFO
--rw-r--r--   0 yzhao233 (1622298973) 1024005267      387 2023-07-05 16:06:55.000000 giszhao-0.0.1/README.md
-drwxr-xr-x   0 yzhao233 (1622298973) 1024005267        0 2023-07-09 19:12:06.835273 giszhao-0.0.1/giszhao/
--rw-r--r--   0 yzhao233 (1622298973) 1024005267      124 2023-07-05 16:06:55.000000 giszhao-0.0.1/giszhao/__init__.py
--rw-r--r--   0 yzhao233 (1622298973) 1024005267      188 2023-07-05 16:06:55.000000 giszhao-0.0.1/giszhao/common.py
--rw-r--r--   0 yzhao233 (1622298973) 1024005267       19 2023-07-05 16:06:55.000000 giszhao-0.0.1/giszhao/giszhao.py
-drwxr-xr-x   0 yzhao233 (1622298973) 1024005267        0 2023-07-09 19:12:06.835821 giszhao-0.0.1/giszhao.egg-info/
--rw-r--r--   0 yzhao233 (1622298973) 1024005267     1109 2023-07-09 19:12:06.000000 giszhao-0.0.1/giszhao.egg-info/PKG-INFO
--rw-r--r--   0 yzhao233 (1622298973) 1024005267      276 2023-07-09 19:12:06.000000 giszhao-0.0.1/giszhao.egg-info/SOURCES.txt
--rw-r--r--   0 yzhao233 (1622298973) 1024005267        1 2023-07-09 19:12:06.000000 giszhao-0.0.1/giszhao.egg-info/dependency_links.txt
--rw-r--r--   0 yzhao233 (1622298973) 1024005267        1 2023-07-09 19:12:06.000000 giszhao-0.0.1/giszhao.egg-info/not-zip-safe
--rw-r--r--   0 yzhao233 (1622298973) 1024005267        8 2023-07-09 19:12:06.000000 giszhao-0.0.1/giszhao.egg-info/top_level.txt
--rw-r--r--   0 yzhao233 (1622298973) 1024005267        0 2023-07-05 16:06:55.000000 giszhao-0.0.1/requirements.txt
--rw-r--r--   0 yzhao233 (1622298973) 1024005267      390 2023-07-09 19:12:06.836213 giszhao-0.0.1/setup.cfg
--rw-r--r--   0 yzhao233 (1622298973) 1024005267     1701 2023-07-05 16:06:55.000000 giszhao-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:57:39.857802 giszhao-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 15:57:31.000000 giszhao-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-13 15:57:31.000000 giszhao-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-13 15:57:39.857802 giszhao-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 15:57:31.000000 giszhao-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:57:39.857802 giszhao-0.0.2/giszhao/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 15:57:31.000000 giszhao-0.0.2/giszhao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 15:57:31.000000 giszhao-0.0.2/giszhao/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:57:31.000000 giszhao-0.0.2/giszhao/giszhao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:57:39.857802 giszhao-0.0.2/giszhao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-13 15:57:39.000000 giszhao-0.0.2/giszhao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-13 15:57:39.000000 giszhao-0.0.2/giszhao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:57:39.000000 giszhao-0.0.2/giszhao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:57:39.000000 giszhao-0.0.2/giszhao.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 15:57:39.000000 giszhao-0.0.2/giszhao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:57:31.000000 giszhao-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 15:57:39.861802 giszhao-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-13 15:57:31.000000 giszhao-0.0.2/setup.py
```

### Comparing `giszhao-0.0.1/LICENSE` & `giszhao-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giszhao-0.0.1/PKG-INFO` & `giszhao-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giszhao
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a test pkg from Yun Zhao in Summer 2023.
 Home-page: https://github.com/zhaoyun1230/giszhao
 Author: Yun Zhao
 Author-email: zhaoyun1230@gmail.com
 License: MIT license
 Keywords: giszhao
 Classifier: Intended Audience :: Developers
```

### Comparing `giszhao-0.0.1/giszhao.egg-info/PKG-INFO` & `giszhao-0.0.2/giszhao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giszhao
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a test pkg from Yun Zhao in Summer 2023.
 Home-page: https://github.com/zhaoyun1230/giszhao
 Author: Yun Zhao
 Author-email: zhaoyun1230@gmail.com
 License: MIT license
 Keywords: giszhao
 Classifier: Intended Audience :: Developers
```

### Comparing `giszhao-0.0.1/setup.py` & `giszhao-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='giszhao',
     name='giszhao',
     packages=find_packages(include=['giszhao', 'giszhao.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zhaoyun1230/giszhao',
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

