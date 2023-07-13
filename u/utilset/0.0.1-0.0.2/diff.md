# Comparing `tmp/utilset-0.0.1.tar.gz` & `tmp/utilset-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilset-0.0.1.tar", last modified: Tue Feb 28 07:13:42 2023, max compression
+gzip compressed data, was "utilset-0.0.2.tar", last modified: Thu Jul 13 07:26:57 2023, max compression
```

## Comparing `utilset-0.0.1.tar` & `utilset-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 sai        (501) staff       (20)        0 2023-02-28 07:13:42.222761 utilset-0.0.1/
--rw-r--r--   0 sai        (501) staff       (20)     1060 2023-02-28 03:00:41.000000 utilset-0.0.1/LICENSE
--rw-r--r--   0 sai        (501) staff       (20)      597 2023-02-28 07:13:42.222393 utilset-0.0.1/PKG-INFO
--rw-r--r--   0 sai        (501) staff       (20)      174 2023-02-28 07:13:16.000000 utilset-0.0.1/README.md
--rw-r--r--   0 sai        (501) staff       (20)       38 2023-02-28 07:13:42.222856 utilset-0.0.1/setup.cfg
--rw-r--r--   0 sai        (501) staff       (20)      694 2023-02-28 07:02:34.000000 utilset-0.0.1/setup.py
-drwxr-xr-x   0 sai        (501) staff       (20)        0 2023-02-28 07:13:42.214110 utilset-0.0.1/tests/
--rw-r--r--   0 sai        (501) staff       (20)      300 2023-02-28 07:12:58.000000 utilset-0.0.1/tests/test_bitmap.py
--rw-r--r--   0 sai        (501) staff       (20)      291 2023-02-28 07:12:58.000000 utilset-0.0.1/tests/test_dict.py
--rw-r--r--   0 sai        (501) staff       (20)      281 2023-02-28 07:12:58.000000 utilset-0.0.1/tests/test_file.py
--rw-r--r--   0 sai        (501) staff       (20)      221 2023-02-28 07:12:58.000000 utilset-0.0.1/tests/test_string.py
-drwxr-xr-x   0 sai        (501) staff       (20)        0 2023-02-28 07:13:42.217894 utilset-0.0.1/utilset/
--rw-r--r--   0 sai        (501) staff       (20)     3285 2023-02-28 06:47:05.000000 utilset-0.0.1/utilset/Bitmap.py
--rw-r--r--   0 sai        (501) staff       (20)      109 2023-02-28 06:54:57.000000 utilset-0.0.1/utilset/dict.py
--rw-r--r--   0 sai        (501) staff       (20)      234 2023-02-24 01:54:56.000000 utilset-0.0.1/utilset/file.py
--rw-r--r--   0 sai        (501) staff       (20)      143 2023-02-24 02:11:49.000000 utilset-0.0.1/utilset/list.py
--rw-r--r--   0 sai        (501) staff       (20)      104 2022-12-20 07:58:21.000000 utilset-0.0.1/utilset/string.py
-drwxr-xr-x   0 sai        (501) staff       (20)        0 2023-02-28 07:13:42.221912 utilset-0.0.1/utilset.egg-info/
--rw-r--r--   0 sai        (501) staff       (20)      597 2023-02-28 07:13:42.000000 utilset-0.0.1/utilset.egg-info/PKG-INFO
--rw-r--r--   0 sai        (501) staff       (20)      314 2023-02-28 07:13:42.000000 utilset-0.0.1/utilset.egg-info/SOURCES.txt
--rw-r--r--   0 sai        (501) staff       (20)        1 2023-02-28 07:13:42.000000 utilset-0.0.1/utilset.egg-info/dependency_links.txt
--rw-r--r--   0 sai        (501) staff       (20)        8 2023-02-28 07:13:42.000000 utilset-0.0.1/utilset.egg-info/top_level.txt
+drwxr-xr-x   0 sai        (501) staff       (20)        0 2023-07-13 07:26:57.311323 utilset-0.0.2/
+-rw-r--r--   0 sai        (501) staff       (20)     1060 2023-02-28 03:00:41.000000 utilset-0.0.2/LICENSE
+-rw-r--r--   0 sai        (501) staff       (20)      702 2023-07-13 07:26:57.310716 utilset-0.0.2/PKG-INFO
+-rw-r--r--   0 sai        (501) staff       (20)       63 2023-02-28 07:24:02.000000 utilset-0.0.2/README.md
+-rw-r--r--   0 sai        (501) staff       (20)       38 2023-07-13 07:26:57.312993 utilset-0.0.2/setup.cfg
+-rw-r--r--   0 sai        (501) staff       (20)      994 2023-07-13 07:26:44.000000 utilset-0.0.2/setup.py
+drwxr-xr-x   0 sai        (501) staff       (20)        0 2023-07-13 07:26:57.286821 utilset-0.0.2/tests/
+-rw-r--r--   0 sai        (501) staff       (20)      300 2023-02-28 07:12:58.000000 utilset-0.0.2/tests/test_bitmap.py
+-rw-r--r--   0 sai        (501) staff       (20)      291 2023-02-28 07:12:58.000000 utilset-0.0.2/tests/test_dict.py
+-rw-r--r--   0 sai        (501) staff       (20)      281 2023-02-28 07:12:58.000000 utilset-0.0.2/tests/test_file.py
+-rw-r--r--   0 sai        (501) staff       (20)      447 2023-07-13 07:13:51.000000 utilset-0.0.2/tests/test_list.py
+-rw-r--r--   0 sai        (501) staff       (20)      326 2023-07-13 07:17:02.000000 utilset-0.0.2/tests/test_string.py
+drwxr-xr-x   0 sai        (501) staff       (20)        0 2023-07-13 07:26:57.305127 utilset-0.0.2/utilset/
+-rw-r--r--   0 sai        (501) staff       (20)     3285 2023-02-28 06:47:05.000000 utilset-0.0.2/utilset/Bitmap.py
+-rw-r--r--   0 sai        (501) staff       (20)      109 2023-02-28 06:54:57.000000 utilset-0.0.2/utilset/dict.py
+-rw-r--r--   0 sai        (501) staff       (20)      234 2023-02-24 01:54:56.000000 utilset-0.0.2/utilset/file.py
+-rw-r--r--   0 sai        (501) staff       (20)      268 2023-07-13 07:19:22.000000 utilset-0.0.2/utilset/list.py
+-rw-r--r--   0 sai        (501) staff       (20)      190 2023-07-13 07:16:23.000000 utilset-0.0.2/utilset/string.py
+drwxr-xr-x   0 sai        (501) staff       (20)        0 2023-07-13 07:26:57.310094 utilset-0.0.2/utilset.egg-info/
+-rw-r--r--   0 sai        (501) staff       (20)      702 2023-07-13 07:26:57.000000 utilset-0.0.2/utilset.egg-info/PKG-INFO
+-rw-r--r--   0 sai        (501) staff       (20)      333 2023-07-13 07:26:57.000000 utilset-0.0.2/utilset.egg-info/SOURCES.txt
+-rw-r--r--   0 sai        (501) staff       (20)        1 2023-07-13 07:26:57.000000 utilset-0.0.2/utilset.egg-info/dependency_links.txt
+-rw-r--r--   0 sai        (501) staff       (20)        8 2023-07-13 07:26:57.000000 utilset-0.0.2/utilset.egg-info/top_level.txt
```

### Comparing `utilset-0.0.1/LICENSE` & `utilset-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utilset-0.0.1/utilset/Bitmap.py` & `utilset-0.0.2/utilset/Bitmap.py`

 * *Files identical despite different names*

