# Comparing `tmp/git_dl-0.0.1.tar.gz` & `tmp/git_dl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_dl-0.0.1.tar", last modified: Thu Jul 13 07:48:37 2023, max compression
+gzip compressed data, was "git_dl-1.0.0.tar", last modified: Thu Jul  6 13:16:21 2023, max compression
```

## Comparing `git_dl-0.0.1.tar` & `git_dl-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,12 @@
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
+drwxr-xr-x   0 tabish    (1000) tabish    (1000)        0 2023-07-06 13:16:21.542421 git_dl-1.0.0/
+-rw-r--r--   0 tabish    (1000) tabish    (1000)     1070 2023-06-19 17:16:05.000000 git_dl-1.0.0/LICENSE
+-rw-r--r--   0 tabish    (1000) tabish    (1000)      150 2023-07-06 13:16:21.542421 git_dl-1.0.0/PKG-INFO
+-rw-r--r--   0 tabish    (1000) tabish    (1000)     1146 2023-06-28 15:16:35.000000 git_dl-1.0.0/README.md
+drwxr-xr-x   0 tabish    (1000) tabish    (1000)        0 2023-07-06 13:16:21.542421 git_dl-1.0.0/git_dl.egg-info/
+-rw-r--r--   0 tabish    (1000) tabish    (1000)      150 2023-07-06 13:16:21.000000 git_dl-1.0.0/git_dl.egg-info/PKG-INFO
+-rw-r--r--   0 tabish    (1000) tabish    (1000)      179 2023-07-06 13:16:21.000000 git_dl-1.0.0/git_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 tabish    (1000) tabish    (1000)        1 2023-07-06 13:16:21.000000 git_dl-1.0.0/git_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 tabish    (1000) tabish    (1000)       42 2023-07-06 13:16:21.000000 git_dl-1.0.0/git_dl.egg-info/entry_points.txt
+-rw-r--r--   0 tabish    (1000) tabish    (1000)        7 2023-07-06 13:16:21.000000 git_dl-1.0.0/git_dl.egg-info/top_level.txt
+-rw-r--r--   0 tabish    (1000) tabish    (1000)       38 2023-07-06 13:16:21.542421 git_dl-1.0.0/setup.cfg
+-rw-r--r--   0 tabish    (1000) tabish    (1000)      303 2023-07-06 13:04:18.000000 git_dl-1.0.0/setup.py
```

### Comparing `git_dl-0.0.1/LICENSE` & `git_dl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_dl-0.0.1/README.md` & `git_dl-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 here link of folder should be modified as below
   https://github.com/microsoft/terminal/tree/main/.config
   should be modified as
   github.com microsoft terminal tree main .config
 
 
 3
-for hhljkl;'
+for hhlihhbjkl;'
 lkhkhghjkhklj:lhhwtesting this file is edited
  
 there is one more way to use it
 send post request to http://gitdl.onrender.com/get_add with {'url': "unmodified_url_of_the_folder"} 
 response of this will be text (say config)
 now send get to http://gitdl.onrender.com/download/{response_text} here response is config so url will be 
 http://gitdl.onrender.com/download/config -->
```

