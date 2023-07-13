# Comparing `tmp/tarn-0.9.2.tar.gz` & `tmp/tarn-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.9.2.tar", last modified: Tue Jul 11 08:56:38 2023, max compression
+gzip compressed data, was "tarn-0.9.3.tar", last modified: Thu Jul 13 16:25:40 2023, max compression
```

## Comparing `tarn-0.9.2.tar` & `tarn-0.9.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-11 08:56:33.000000 tarn-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 08:56:33.000000 tarn-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 08:56:38.443924 tarn-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 08:56:33.000000 tarn-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-11 08:56:33.000000 tarn-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 08:56:33.000000 tarn-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:56:38.443924 tarn-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-11 08:56:33.000000 tarn-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.439924 tarn-0.9.2/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.439924 tarn-0.9.2/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.439924 tarn-0.9.2/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-13 16:25:36.000000 tarn-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 16:25:36.000000 tarn-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 16:25:40.056749 tarn-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-13 16:25:36.000000 tarn-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-13 16:25:36.000000 tarn-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-13 16:25:36.000000 tarn-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:25:40.056749 tarn-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-13 16:25:36.000000 tarn-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.052749 tarn-0.9.3/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.052749 tarn-0.9.3/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 16:25:39.000000 tarn-0.9.3/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-13 16:25:40.000000 tarn-0.9.3/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:25:39.000000 tarn-0.9.3/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-13 16:25:39.000000 tarn-0.9.3/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 16:25:40.000000 tarn-0.9.3/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.9.2/LICENSE` & `tarn-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/PKG-INFO` & `tarn-0.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.9.2
+Version: 0.9.3
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.2.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.3.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.9.2/README.md` & `tarn-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/pyproject.toml` & `tarn-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/setup.py` & `tarn-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/cache/storage.py` & `tarn-0.9.3/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/compat.py` & `tarn-0.9.3/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/config.py` & `tarn-0.9.3/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/digest.py` & `tarn-0.9.3/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/interface.py` & `tarn-0.9.3/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/local/storage.py` & `tarn-0.9.3/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/location/disk_dict.py` & `tarn-0.9.3/tarn/location/disk_dict.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/location/fanout.py` & `tarn-0.9.3/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/location/interface.py` & `tarn-0.9.3/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/location/levels.py` & `tarn-0.9.3/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/location/nginx.py` & `tarn-0.9.3/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/location/redis.py` & `tarn-0.9.3/tarn/location/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,22 @@
                 with value_to_buffer(self.redis.get(content_key)) as buffer:
                     yield buffer, labels
                     return
             with value_to_buffer(self.redis.get(content_key)) as buffer:
                 yield buffer
         except StorageCorruption:
             self.delete(key)
-    
-    def read_batch(self, keys: Keys) -> Iterable[Optional[Tuple[Key, Tuple[Value, MaybeLabels]]]]:
+
+    def read_batch(
+        self, keys: Keys
+    ) -> Iterable[Optional[Tuple[Key, Tuple[Value, MaybeLabels]]]]:
         for key in keys:
             with self.read(key, True) as value:
                 yield key, value
-                
+
     @contextmanager
     def write(self, key: Key, value: Value, labels: MaybeLabels) -> ContextManager:
         try:
             content_key = self.prefix + key
             with value_to_buffer(value) as value:
                 content = self.redis.get(content_key)
                 if content is None:
@@ -60,15 +62,17 @@
                     self.update_labels(key, labels)
                     self.update_usage_date(key)
                     with value_to_buffer(self.redis.get(content_key)) as buffer:
                         yield buffer
                         return
                 old_content = self.redis.get(content_key)
                 if old_content != value.read():
-                    raise CollisionError(f"Written value and the new one doesn't match: {key}")
+                    raise CollisionError(
+                        f'Written value and the new one does not match: {key}'
+                    )
                 self.update_labels(key, labels)
                 self.update_usage_date(key)
                 with value_to_buffer(self.redis.get(content_key)) as buffer:
                     yield buffer
         except StorageCorruption:
             self.delete(key)
```

### Comparing `tarn-0.9.2/tarn/location/s3.py` & `tarn-0.9.3/tarn/location/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from contextlib import contextmanager
 from datetime import datetime
 from io import SEEK_CUR, SEEK_END, SEEK_SET
 from typing import Any, BinaryIO, ContextManager, Iterable, Mapping, Optional, Tuple, Union
 
-from botocore.exceptions import ClientError
-
-from tarn.exceptions import CollisionError
+from botocore.exceptions import ClientError, ConnectionError
 
 from ..compat import S3Client
 from ..digest import key_to_relative, value_to_buffer
 from ..exceptions import CollisionError, StorageCorruption
 from ..interface import Key, Keys, MaybeLabels, Meta, Value
 from ..utils import match_buffers
 from .interface import Writable
@@ -29,89 +27,116 @@
             if 'Contents' in response:
                 for obj in response['Contents']:
                     path = obj['Key']
                     key = self._path_to_key(path)
                     yield key, self, S3Meta(path=path, location=self)
 
     @contextmanager
-    def read(self, key: Key, return_labels: bool) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
+    def read(
+        self, key: Key, return_labels: bool
+    ) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
         try:
             path = self._key_to_path(key)
             try:
                 if return_labels:
                     self.update_usage_date(path)
                     yield self._get_buffer(path), self.get_labels(path)
                 else:
                     self.update_usage_date(path)
                     yield self._get_buffer(path)
 
             except ClientError as e:
-                if e.response['Error']['Code'] == "404" or e.response['Error']['Code'] == "NoSuchKey":  # file doesn't exist
+                if (
+                    e.response['Error']['Code'] == '404'
+                    or e.response['Error']['Code'] == 'NoSuchKey'
+                ):  # file doesn't exist
                     yield
                 else:
                     raise
+            except ConnectionError:
+                yield
         except StorageCorruption:
             self.delete(key)
 
     def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, Union[Value, MaybeLabels]]]:
         for key in keys:
             with self.read(key, True) as value:
                 yield key, value
 
     @contextmanager
     def write(self, key: Key, value: Value, labels: MaybeLabels) -> ContextManager:
         try:
             path = self._key_to_path(key)
             with value_to_buffer(value) as value:
                 try:
-                    self.s3.get_object(Bucket=self.bucket, Key=path)
-                    obj_body = self.s3.get_object(Bucket=self.bucket, Key=path).get('Body')
+                    obj_body_buffer = self._get_buffer(path)
                     try:
-                        match_buffers(value, obj_body, context=key.hex())
+                        match_buffers(value, obj_body_buffer, context=key.hex())
                     except ValueError as e:
-                        raise CollisionError(f"Written value and the new one doesn't match: {key}") from e
+                        raise CollisionError(
+                            f'Written value and the new one does not match: {key}'
+                        ) from e
                     self.update_labels(path, labels)
                     self.update_usage_date(path)
                     yield self._get_buffer(path)
                     return
                 except ClientError as e:
-                    if e.response['Error']['Code'] == "404" or e.response['Error']['Code'] == "NoSuchKey":
-                        self.s3.upload_fileobj(Bucket=self.bucket, Key=path, Fileobj=value)
+                    if (
+                        e.response['Error']['Code'] == '404'
+                        or e.response['Error']['Code'] == 'NoSuchKey'
+                    ):
+                        self.s3.upload_fileobj(
+                            Bucket=self.bucket, Key=path, Fileobj=value
+                        )
                         self.update_labels(path, labels)
                         self.update_usage_date(path)
                         yield self._get_buffer(path)
                         return
                     else:
                         raise
+                except ConnectionError:
+                    yield
         except StorageCorruption:
             self.delete(key)
 
     def delete(self, key: Key):
         path = self._key_to_path(key)
         self.s3.delete_object(Bucket=self.bucket, Key=path)
 
     def update_labels(self, path: str, labels: MaybeLabels):
         if labels is not None:
-            tags_dict = self._tags_to_dict(self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet'])
+            tags_dict = self._tags_to_dict(
+                self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet']
+            )
             tags_dict.update({f'_{label}': f'_{label}' for label in labels})
             tags = self._dict_to_tags(tags_dict)
-            self.s3.put_object_tagging(Bucket=self.bucket, Key=path, Tagging={'TagSet': tags})
+            self.s3.put_object_tagging(
+                Bucket=self.bucket, Key=path, Tagging={'TagSet': tags}
+            )
 
     def get_labels(self, path: str) -> MaybeLabels:
-        tags_dict = self._tags_to_dict(self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet'])
-        return [dict_key[1:] for dict_key in tags_dict if dict_key[0] == '_']
+        tags_dict = self._tags_to_dict(
+            self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet']
+        )
+        return [dict_key[1:] for dict_key in tags_dict if dict_key.startswith('_')]
 
     def update_usage_date(self, path: str):
-        tags_dict = self._tags_to_dict(self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet'])
+        tags_dict = self._tags_to_dict(
+            self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet']
+        )
         tags_dict['usage_date'] = str(datetime.now().timestamp())
         tags = self._dict_to_tags(tags_dict)
-        self.s3.put_object_tagging(Bucket=self.bucket, Key=path, Tagging={'TagSet': tags})
+        self.s3.put_object_tagging(
+            Bucket=self.bucket, Key=path, Tagging={'TagSet': tags}
+        )
 
     def get_usage_date(self, path: str) -> Optional[datetime]:
-        tags_dict = self._tags_to_dict(self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet'])
+        tags_dict = self._tags_to_dict(
+            self.s3.get_object_tagging(Bucket=self.bucket, Key=path)['TagSet']
+        )
         if 'usage_date' in tags_dict:
             return datetime.fromtimestamp(float(tags_dict['usage_date']))
         return None
 
     def _get_buffer(self, path):
         return StreamingBodyBuffer(self.s3.get_object, Bucket=self.bucket, Key=path)
 
@@ -120,15 +145,15 @@
 
     def _path_to_key(self, path: str):
         return bytes.fromhex(path.replace('/', ''))
 
     @staticmethod
     def _tags_to_dict(tags: Iterable[Mapping[str, str]]) -> Mapping[str, str]:
         return {tag['Key']: tag['Value'] for tag in tags}
-    
+
     @staticmethod
     def _dict_to_tags(tag_dict: Mapping[str, str]) -> Iterable[Mapping[str, str]]:
         return [{'Key': key, 'Value': value} for key, value in tag_dict.items()]
 
 
 class StreamingBodyBuffer(BinaryIO):
     def __init__(self, getter, **kwargs):
@@ -153,15 +178,15 @@
                 self._streaming_body = self.getter(**self.kwargs).get('Body')
                 return
 
         if whence == SEEK_END:
             if offset == 0:
                 return
 
-        raise NotImplementedError("Can't seek anywhere but the begining of the stream")
+        raise NotImplementedError('Cannot seek anywhere but the begining of the stream')
 
     def __getattribute__(self, attr) -> Any:
         if attr in ('seek', 'getter', 'kwargs'):
             return super().__getattribute__(attr)
         streaming_body = super().__getattribute__('_streaming_body')
         return getattr(streaming_body, attr)
```

### Comparing `tarn-0.9.2/tarn/location/scp.py` & `tarn-0.9.3/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/pickler/compat.py` & `tarn-0.9.3/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/pickler/interface.py` & `tarn-0.9.3/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/pool/hash_key.py` & `tarn-0.9.3/tarn/pool/hash_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def fetch(self, keys: Keys) -> Iterable[Tuple[Key, bool]]:
         for key, value in self._full.read_batch(keys):
             yield key, value is not None
 
     def read(self, func_or_key, *args, fetch: Optional[bool] = None, error: Optional[bool] = None, **kwargs):
         if callable(func_or_key):
             return self._read_func(func_or_key, *args, error=error, fetch=fetch, **kwargs)
-        return self._read_context(func_or_key, *args, **kwargs)
+        return self._read_context(func_or_key, fetch, error, *args, **kwargs)
 
     @contextmanager
     def _read_context(self, key, fetch, error) -> ContextManager[MaybeValue]:
         fetch = self._resolve_value(fetch, self._fetch, 'fetch')
         error = self._resolve_value(error, self._error, 'error')
 
         if isinstance(key, str):
```

### Comparing `tarn-0.9.2/tarn/pool/pickle_key.py` & `tarn-0.9.3/tarn/pool/pickle_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/serializers.py` & `tarn-0.9.3/tarn/serializers.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/tools/labels.py` & `tarn-0.9.3/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/tools/locker.py` & `tarn-0.9.3/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/tools/size.py` & `tarn-0.9.3/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/tools/usage.py` & `tarn-0.9.3/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn/utils.py` & `tarn-0.9.3/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.2/tarn.egg-info/PKG-INFO` & `tarn-0.9.3/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.9.2
+Version: 0.9.3
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.2.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.3.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.9.2/tarn.egg-info/SOURCES.txt` & `tarn-0.9.3/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

