# Comparing `tmp/benimang-0.3.8.tar.gz` & `tmp/benimang-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.3.8.tar", last modified: Sat Jul  8 04:04:06 2023, max compression
+gzip compressed data, was "benimang-0.3.9.tar", last modified: Sat Jul  8 06:59:50 2023, max compression
```

## Comparing `benimang-0.3.8.tar` & `benimang-0.3.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 04:04:06.036956 benimang-0.3.8/
--rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0      258 2023-07-08 04:04:06.036956 benimang-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 04:04:06.027954 benimang-0.3.8/beni/
--rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.8/beni/__init__.py
--rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-0.3.8/beni/bbyte.py
--rw-rw-rw-   0        0        0     5789 2023-07-05 03:38:40.000000 benimang-0.3.8/beni/bcache.py
--rw-rw-rw-   0        0        0    11460 2023-06-29 07:06:28.000000 benimang-0.3.8/beni/bcmd.py
--rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-0.3.8/beni/bcolor.py
--rw-rw-rw-   0        0        0      436 2023-06-29 07:09:07.000000 benimang-0.3.8/beni/bdefine.py
--rw-rw-rw-   0        0        0     2423 2023-07-08 04:02:39.000000 benimang-0.3.8/beni/bexecute.py
--rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-0.3.8/beni/bfile.py
--rw-rw-rw-   0        0        0     4562 2023-07-06 08:05:26.000000 benimang-0.3.8/beni/bfunc.py
--rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-0.3.8/beni/bhash.py
--rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-0.3.8/beni/bhttp.py
--rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-0.3.8/beni/binput.py
--rw-rw-rw-   0        0        0     5708 2023-06-30 02:08:08.000000 benimang-0.3.8/beni/block.py
--rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-0.3.8/beni/blog.py
--rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-0.3.8/beni/bpath.py
--rw-rw-rw-   0        0        0     2450 2023-07-08 04:02:42.000000 benimang-0.3.8/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-0.3.8/beni/bprogress.py
--rw-rw-rw-   0        0        0     3373 2023-07-06 08:05:08.000000 benimang-0.3.8/beni/bqiniu.py
--rw-rw-rw-   0        0        0     9866 2023-07-08 04:03:05.000000 benimang-0.3.8/beni/bsqlite.py
--rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-0.3.8/beni/bstorage.py
--rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-0.3.8/beni/btable.py
--rw-rw-rw-   0        0        0     4987 2023-07-05 06:44:09.000000 benimang-0.3.8/beni/btask.py
--rw-rw-rw-   0        0        0     1378 2023-06-29 07:10:32.000000 benimang-0.3.8/beni/btime.py
--rw-rw-rw-   0        0        0      324 2023-06-30 02:01:04.000000 benimang-0.3.8/beni/btype.py
--rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-0.3.8/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-08 04:04:06.034956 benimang-0.3.8/benimang.egg-info/
--rw-rw-rw-   0        0        0      258 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-07-08 04:03:36.000000 benimang-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 04:04:06.037957 benimang-0.3.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-08 04:04:06.035956 benimang-0.3.8/test/
--rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-0.3.8/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-08 06:59:50.549141 benimang-0.3.9/
+-rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      258 2023-07-08 06:59:50.549141 benimang-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 06:59:50.540558 benimang-0.3.9/beni/
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.9/beni/__init__.py
+-rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-0.3.9/beni/bbyte.py
+-rw-rw-rw-   0        0        0     5789 2023-07-05 03:38:40.000000 benimang-0.3.9/beni/bcache.py
+-rw-rw-rw-   0        0        0    11460 2023-06-29 07:06:28.000000 benimang-0.3.9/beni/bcmd.py
+-rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-0.3.9/beni/bcolor.py
+-rw-rw-rw-   0        0        0      436 2023-06-29 07:09:07.000000 benimang-0.3.9/beni/bdefine.py
+-rw-rw-rw-   0        0        0     2423 2023-07-08 04:02:39.000000 benimang-0.3.9/beni/bexecute.py
+-rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-0.3.9/beni/bfile.py
+-rw-rw-rw-   0        0        0     4562 2023-07-06 08:05:26.000000 benimang-0.3.9/beni/bfunc.py
+-rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-0.3.9/beni/bhash.py
+-rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-0.3.9/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-0.3.9/beni/binput.py
+-rw-rw-rw-   0        0        0     5708 2023-06-30 02:08:08.000000 benimang-0.3.9/beni/block.py
+-rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-0.3.9/beni/blog.py
+-rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-0.3.9/beni/bpath.py
+-rw-rw-rw-   0        0        0     2450 2023-07-08 04:02:42.000000 benimang-0.3.9/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-0.3.9/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3373 2023-07-06 08:05:08.000000 benimang-0.3.9/beni/bqiniu.py
+-rw-rw-rw-   0        0        0     9866 2023-07-08 04:03:05.000000 benimang-0.3.9/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-0.3.9/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-0.3.9/beni/btable.py
+-rw-rw-rw-   0        0        0     4987 2023-07-05 06:44:09.000000 benimang-0.3.9/beni/btask.py
+-rw-rw-rw-   0        0        0     1378 2023-06-29 07:10:32.000000 benimang-0.3.9/beni/btime.py
+-rw-rw-rw-   0        0        0      376 2023-07-08 06:57:34.000000 benimang-0.3.9/beni/btype.py
+-rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-0.3.9/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-08 06:59:50.546559 benimang-0.3.9/benimang.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-07-08 06:59:50.000000 benimang-0.3.9/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-07-08 06:59:50.000000 benimang-0.3.9/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 06:59:50.000000 benimang-0.3.9/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-08 06:59:50.000000 benimang-0.3.9/benimang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-07-08 06:59:50.000000 benimang-0.3.9/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-08 06:59:50.000000 benimang-0.3.9/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-07-08 06:58:21.000000 benimang-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 06:59:50.549141 benimang-0.3.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 06:59:50.547559 benimang-0.3.9/test/
+-rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-0.3.9/test/test_sample.py
```

### Comparing `benimang-0.3.8/beni/bbyte.py` & `benimang-0.3.9/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bcache.py` & `benimang-0.3.9/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bcmd.py` & `benimang-0.3.9/beni/bcmd.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bcolor.py` & `benimang-0.3.9/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bexecute.py` & `benimang-0.3.9/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bfile.py` & `benimang-0.3.9/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bfunc.py` & `benimang-0.3.9/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bhash.py` & `benimang-0.3.9/beni/bhash.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bhttp.py` & `benimang-0.3.9/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/binput.py` & `benimang-0.3.9/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/block.py` & `benimang-0.3.9/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/blog.py` & `benimang-0.3.9/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bpath.py` & `benimang-0.3.9/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bplaywright.py` & `benimang-0.3.9/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bprogress.py` & `benimang-0.3.9/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bqiniu.py` & `benimang-0.3.9/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bsqlite.py` & `benimang-0.3.9/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bstorage.py` & `benimang-0.3.9/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/btable.py` & `benimang-0.3.9/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/btask.py` & `benimang-0.3.9/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/btime.py` & `benimang-0.3.9/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/beni/bzip.py` & `benimang-0.3.9/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/benimang.egg-info/SOURCES.txt` & `benimang-0.3.9/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.3.8/pyproject.toml` & `benimang-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "benimang"
-version = "0.3.8"
+version = "0.3.9"
 description = "utils library for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"}
 ]
```

### Comparing `benimang-0.3.8/test/test_sample.py` & `benimang-0.3.9/test/test_sample.py`

 * *Files identical despite different names*

