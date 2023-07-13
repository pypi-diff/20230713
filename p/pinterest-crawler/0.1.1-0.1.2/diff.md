# Comparing `tmp/pinterest-crawler-0.1.1.tar.gz` & `tmp/pinterest-crawler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinterest-crawler-0.1.1.tar", last modified: Thu Jul 13 06:46:24 2023, max compression
+gzip compressed data, was "pinterest-crawler-0.1.2.tar", last modified: Thu Jul 13 07:11:57 2023, max compression
```

## Comparing `pinterest-crawler-0.1.1.tar` & `pinterest-crawler-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:46:24.165295 pinterest-crawler-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-13 06:46:24.165295 pinterest-crawler-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:46:24.161295 pinterest-crawler-0.1.1/pinterest_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/pinterest_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/pinterest_crawler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/pinterest_crawler/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/pinterest_crawler/pinterest_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/pinterest_crawler/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:46:24.165295 pinterest-crawler-0.1.1/pinterest_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-13 06:46:24.000000 pinterest-crawler-0.1.1/pinterest_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-13 06:46:24.000000 pinterest-crawler-0.1.1/pinterest_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:46:24.000000 pinterest-crawler-0.1.1/pinterest_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 06:46:24.000000 pinterest-crawler-0.1.1/pinterest_crawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 06:46:24.000000 pinterest-crawler-0.1.1/pinterest_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 06:46:24.000000 pinterest-crawler-0.1.1/pinterest_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:46:24.165295 pinterest-crawler-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-13 06:46:13.000000 pinterest-crawler-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:11:57.893956 pinterest-crawler-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-13 07:11:57.893956 pinterest-crawler-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:11:57.893956 pinterest-crawler-0.1.2/pinterest_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/pinterest_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/pinterest_crawler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/pinterest_crawler/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/pinterest_crawler/pinterest_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/pinterest_crawler/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:11:57.893956 pinterest-crawler-0.1.2/pinterest_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-13 07:11:57.000000 pinterest-crawler-0.1.2/pinterest_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-13 07:11:57.000000 pinterest-crawler-0.1.2/pinterest_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:11:57.000000 pinterest-crawler-0.1.2/pinterest_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 07:11:57.000000 pinterest-crawler-0.1.2/pinterest_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:11:57.000000 pinterest-crawler-0.1.2/pinterest_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 07:11:57.000000 pinterest-crawler-0.1.2/pinterest_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:11:57.893956 pinterest-crawler-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-13 07:11:47.000000 pinterest-crawler-0.1.2/setup.py
```

### Comparing `pinterest-crawler-0.1.1/LICENSE.md` & `pinterest-crawler-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pinterest-crawler-0.1.1/pinterest_crawler/config.py` & `pinterest-crawler-0.1.2/pinterest_crawler/config.py`

 * *Files identical despite different names*

### Comparing `pinterest-crawler-0.1.1/pinterest_crawler/pinterest_crawler.py` & `pinterest-crawler-0.1.2/pinterest_crawler/pinterest_crawler.py`

 * *Files identical despite different names*

### Comparing `pinterest-crawler-0.1.1/pinterest_crawler/scraper.py` & `pinterest-crawler-0.1.2/pinterest_crawler/scraper.py`

 * *Files identical despite different names*

### Comparing `pinterest-crawler-0.1.1/setup.py` & `pinterest-crawler-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 pre_install()
 
 
 setup(
     name='pinterest-crawler',
-    version='0.1.1',
+    version='0.1.2',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=["pinterest_crawler"],
     setup_requires=[],
     url='https://github.com/SajjadAemmi/Pinterest-Crawler',
     license='',
     author='Sajjad Aemmi',
```

