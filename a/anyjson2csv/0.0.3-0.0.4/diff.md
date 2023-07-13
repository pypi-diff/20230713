# Comparing `tmp/anyjson2csv-0.0.3.tar.gz` & `tmp/anyjson2csv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyjson2csv-0.0.3.tar", last modified: Wed Jul 12 12:05:06 2023, max compression
+gzip compressed data, was "anyjson2csv-0.0.4.tar", last modified: Thu Jul 13 07:02:20 2023, max compression
```

## Comparing `anyjson2csv-0.0.3.tar` & `anyjson2csv-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:05:06.571759 anyjson2csv-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-07-12 08:57:26.000000 anyjson2csv-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      526 2023-07-12 12:05:06.568757 anyjson2csv-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-12 08:55:33.000000 anyjson2csv-0.0.3/README.md
--rw-rw-rw-   0        0        0      626 2023-07-12 12:04:23.000000 anyjson2csv-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 12:05:06.571759 anyjson2csv-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 12:05:06.495755 anyjson2csv-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 12:05:06.520761 anyjson2csv-0.0.3/src/anyjson2csv/
--rw-rw-rw-   0        0        0        2 2023-07-12 11:27:26.000000 anyjson2csv-0.0.3/src/anyjson2csv/__init__.py
--rw-rw-rw-   0        0        0     3312 2023-07-12 12:03:37.000000 anyjson2csv-0.0.3/src/anyjson2csv/flatten_json.py
--rw-rw-rw-   0        0        0      462 2023-07-12 12:03:34.000000 anyjson2csv-0.0.3/src/anyjson2csv/json_to_csv.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:05:06.565757 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/
--rw-rw-rw-   0        0        0      526 2023-07-12 12:05:06.000000 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-12 12:05:06.000000 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:05:06.000000 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 12:05:06.000000 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 07:02:20.074658 anyjson2csv-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-07-12 08:57:26.000000 anyjson2csv-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      849 2023-07-13 07:02:20.073659 anyjson2csv-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-07-12 12:37:53.000000 anyjson2csv-0.0.4/README.md
+-rw-rw-rw-   0        0        0      112 2023-07-12 13:41:36.000000 anyjson2csv-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 07:02:20.075659 anyjson2csv-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1386 2023-07-13 07:01:21.000000 anyjson2csv-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:02:20.010658 anyjson2csv-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 07:02:20.035658 anyjson2csv-0.0.4/src/anyjson2csv/
+-rw-rw-rw-   0        0        0        2 2023-07-12 11:27:26.000000 anyjson2csv-0.0.4/src/anyjson2csv/__init__.py
+-rw-rw-rw-   0        0        0     3312 2023-07-12 12:03:37.000000 anyjson2csv-0.0.4/src/anyjson2csv/flatten_json.py
+-rw-rw-rw-   0        0        0      462 2023-07-12 12:03:34.000000 anyjson2csv-0.0.4/src/anyjson2csv/json_to_csv.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:02:20.070669 anyjson2csv-0.0.4/src/anyjson2csv.egg-info/
+-rw-rw-rw-   0        0        0      849 2023-07-13 07:02:19.000000 anyjson2csv-0.0.4/src/anyjson2csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-07-13 07:02:20.000000 anyjson2csv-0.0.4/src/anyjson2csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 07:02:19.000000 anyjson2csv-0.0.4/src/anyjson2csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-13 07:02:19.000000 anyjson2csv-0.0.4/src/anyjson2csv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-13 07:02:19.000000 anyjson2csv-0.0.4/src/anyjson2csv.egg-info/top_level.txt
```

### Comparing `anyjson2csv-0.0.3/LICENSE.txt` & `anyjson2csv-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anyjson2csv-0.0.3/src/anyjson2csv/flatten_json.py` & `anyjson2csv-0.0.4/src/anyjson2csv/flatten_json.py`

 * *Files identical despite different names*

