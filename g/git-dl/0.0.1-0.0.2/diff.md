# Comparing `tmp/git_dl-0.0.1.tar.gz` & `tmp/git_dl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_dl-0.0.1.tar", last modified: Thu Jul 13 07:48:37 2023, max compression
+gzip compressed data, was "git_dl-0.0.2.tar", last modified: Thu Jul 13 08:08:09 2023, max compression
```

## Comparing `git_dl-0.0.1.tar` & `git_dl-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:48:37.293776 git_dl-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 07:48:26.000000 git_dl-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-13 07:48:37.293776 git_dl-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 07:48:26.000000 git_dl-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:48:37.289776 git_dl-0.0.1/git_dl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:48:26.000000 git_dl-0.0.1/git_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 07:48:26.000000 git_dl-0.0.1/git_dl/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:48:37.289776 git_dl-0.0.1/git_dl/data/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-13 07:48:26.000000 git_dl-0.0.1/git_dl/data/selector.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-13 07:48:26.000000 git_dl-0.0.1/git_dl/github_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:48:37.289776 git_dl-0.0.1/git_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-13 07:48:37.000000 git_dl-0.0.1/git_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-13 07:48:37.000000 git_dl-0.0.1/git_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:48:37.000000 git_dl-0.0.1/git_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 07:48:37.000000 git_dl-0.0.1/git_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 07:48:37.000000 git_dl-0.0.1/git_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 07:48:37.000000 git_dl-0.0.1/git_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:48:37.293776 git_dl-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-13 07:48:26.000000 git_dl-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:08:09.468437 git_dl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 08:07:59.000000 git_dl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-13 08:08:09.468437 git_dl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 08:07:59.000000 git_dl-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:08:09.468437 git_dl-0.0.2/git_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:07:59.000000 git_dl-0.0.2/git_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 08:07:59.000000 git_dl-0.0.2/git_dl/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:08:09.468437 git_dl-0.0.2/git_dl/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-13 08:07:59.000000 git_dl-0.0.2/git_dl/data/selector.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-13 08:07:59.000000 git_dl-0.0.2/git_dl/github_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:08:09.468437 git_dl-0.0.2/git_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-13 08:08:09.000000 git_dl-0.0.2/git_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-13 08:08:09.000000 git_dl-0.0.2/git_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:08:09.000000 git_dl-0.0.2/git_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 08:08:09.000000 git_dl-0.0.2/git_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 08:08:09.000000 git_dl-0.0.2/git_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 08:08:09.000000 git_dl-0.0.2/git_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:08:09.468437 git_dl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-13 08:07:59.000000 git_dl-0.0.2/setup.py
```

### Comparing `git_dl-0.0.1/LICENSE` & `git_dl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git_dl-0.0.1/PKG-INFO` & `git_dl-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_dl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cli app to download github repo folders
 Home-page: https://github.com/the-runtime/git_dl
 Author: the runtime
 Author-email: theruntime7@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `git_dl-0.0.1/README.md` & `git_dl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `git_dl-0.0.1/git_dl/github_downloader.py` & `git_dl-0.0.2/git_dl/github_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             t = data["branches"]
             fit(t)
             rel(t, master)
             master.append(t)
 
 
 def scrape(url):
-    e = Extractor.from_yaml_file('data/selector.yml')
+    e = Extractor.from_yaml_file('git_dl/data/selector.yml')
     headers = {
         'authority': 'www.github.com/',
         'pragma': 'no-cache',
         'cache-control': 'no-cache',
         'dnt': '1',
         'upgrade-insecure-requests': '1',
         'user-agent': 'Mozilla/5.0 (X11; CrOS x86_64 8172.45.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.64 Safari/537.36',
```

### Comparing `git_dl-0.0.1/git_dl.egg-info/PKG-INFO` & `git_dl-0.0.2/git_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-dl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cli app to download github repo folders
 Home-page: https://github.com/the-runtime/git_dl
 Author: the runtime
 Author-email: theruntime7@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `git_dl-0.0.1/setup.py` & `git_dl-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git_dl',
-    version='0.0.1',
+    version='0.0.2',
     author='the runtime',
     author_email='theruntime7@gmail.com',
     description='Cli app to download github repo folders',
     long_description='A longer description of your app',
     url='https://github.com/the-runtime/git_dl',
     packages=find_packages(),
     package_data={
```

