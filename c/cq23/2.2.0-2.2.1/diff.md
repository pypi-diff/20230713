# Comparing `tmp/cq23-2.2.0.tar.gz` & `tmp/cq23-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-2.2.0.tar", last modified: Sat Jun 24 02:24:47 2023, max compression
+gzip compressed data, was "cq23-2.2.1.tar", last modified: Thu Jul 13 09:47:12 2023, max compression
```

## Comparing `cq23-2.2.0.tar` & `cq23-2.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.414855 cq23-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-24 02:24:47.414855 cq23-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-24 02:24:39.000000 cq23-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 02:24:39.000000 cq23-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-24 02:24:47.414855 cq23-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.406854 cq23-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/build_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/build_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/build_image/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/build_image/docker_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/client_logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/client_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/client_logs/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/web_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/web_server/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/web_server/files/loading_screen.html
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.414855 cq23-2.2.0/src/cq23/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/zip/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-13 09:47:12.887735 cq23-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 09:47:03.000000 cq23-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 09:47:03.000000 cq23-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 09:47:12.887735 cq23-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.883735 cq23-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.883735 cq23-2.2.1/src/cq23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.883735 cq23-2.2.1/src/cq23/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.883735 cq23-2.2.1/src/cq23/build_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/build_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/build_image/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/build_image/docker_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.883735 cq23-2.2.1/src/cq23/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/client_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/client_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/client_logs/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/web_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/web_server/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/web_server/files/loading_screen.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.887735 cq23-2.2.1/src/cq23/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 09:47:03.000000 cq23-2.2.1/src/cq23/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:47:12.883735 cq23-2.2.1/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-13 09:47:12.000000 cq23-2.2.1/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 09:47:12.000000 cq23-2.2.1/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:47:12.000000 cq23-2.2.1/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 09:47:12.000000 cq23-2.2.1/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-13 09:47:12.000000 cq23-2.2.1/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 09:47:12.000000 cq23-2.2.1/src/cq23.egg-info/top_level.txt
```

### Comparing `cq23-2.2.0/PKG-INFO` & `cq23-2.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.2.0
+Version: 2.2.1
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.2.0/setup.cfg` & `cq23-2.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 2.2.0
+version = 2.2.1
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-2.2.0/src/cq23/admin/aws.py` & `cq23-2.2.1/src/cq23/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/admin/builder.py` & `cq23-2.2.1/src/cq23/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/admin/worker.py` & `cq23-2.2.1/src/cq23/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/build_image/command.py` & `cq23-2.2.1/src/cq23/build_image/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/build_image/docker_tools.py` & `cq23-2.2.1/src/cq23/build_image/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/check/command.py` & `cq23-2.2.1/src/cq23/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/cleanup/command.py` & `cq23-2.2.1/src/cq23/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/client_logs/command.py` & `cq23-2.2.1/src/cq23/client_logs/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/main/command.py` & `cq23-2.2.1/src/cq23/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/main/utils.py` & `cq23-2.2.1/src/cq23/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/new_client/command.py` & `cq23-2.2.1/src/cq23/new_client/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 import os
 import shutil
+import stat
 import subprocess
+import sys
+
+
+def shutil_onerror(func, path, exc_info):
+    # Is the error an access error on windows?
+    if sys.platform.startswith("win") and not os.access(path, os.W_OK):
+        os.chmod(path, stat.S_IWUSR)
+        func(path)
+    else:
+        raise
 
 
 def clone_repository(repo_url, repo_directory):
     subprocess_args = ["git", "clone", repo_url, repo_directory]
     try:
         subprocess.run(subprocess_args, check=True)
         print("\nTemplate cloned.")
```

### Comparing `cq23-2.2.0/src/cq23/replay/command.py` & `cq23-2.2.1/src/cq23/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/run_game/command.py` & `cq23-2.2.1/src/cq23/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/run_game/docker_tools.py` & `cq23-2.2.1/src/cq23/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/run_game/gcs.py` & `cq23-2.2.1/src/cq23/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/web_server/files/loading_screen.html` & `cq23-2.2.1/src/cq23/web_server/files/loading_screen.html`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/web_server/flask_api.py` & `cq23-2.2.1/src/cq23/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23/zip/command.py` & `cq23-2.2.1/src/cq23/zip/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.2.0/src/cq23.egg-info/PKG-INFO` & `cq23-2.2.1/src/cq23.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.2.0
+Version: 2.2.1
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.2.0/src/cq23.egg-info/SOURCES.txt` & `cq23-2.2.1/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

