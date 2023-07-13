# Comparing `tmp/edx-braze-client-0.1.6.tar.gz` & `tmp/edx-braze-client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-braze-client-0.1.6.tar", last modified: Wed Mar  1 14:04:16 2023, max compression
+gzip compressed data, was "edx-braze-client-0.1.7.tar", last modified: Thu Jul 13 00:52:35 2023, max compression
```

## Comparing `edx-braze-client-0.1.6.tar` & `edx-braze-client-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:04:16.370499 edx-braze-client-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35139 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-03-01 14:04:16.370499 edx-braze-client-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:04:16.370499 edx-braze-client-0.1.6/braze/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/braze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/braze/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/braze/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/braze/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:04:16.370499 edx-braze-client-0.1.6/edx_braze_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-03-01 14:04:16.000000 edx-braze-client-0.1.6/edx_braze_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-01 14:04:16.000000 edx-braze-client-0.1.6/edx_braze_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:04:16.000000 edx-braze-client-0.1.6/edx_braze_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:04:16.000000 edx-braze-client-0.1.6/edx_braze_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 14:04:16.000000 edx-braze-client-0.1.6/edx_braze_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:04:16.370499 edx-braze-client-0.1.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-01 14:04:16.370499 edx-braze-client-0.1.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5176 2023-03-01 14:03:54.000000 edx-braze-client-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:52:35.407261 edx-braze-client-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    35139 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-13 00:52:35.407261 edx-braze-client-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:52:35.407261 edx-braze-client-0.1.7/braze/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/braze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/braze/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/braze/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/braze/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:52:35.407261 edx-braze-client-0.1.7/edx_braze_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-13 00:52:35.000000 edx-braze-client-0.1.7/edx_braze_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-13 00:52:35.000000 edx-braze-client-0.1.7/edx_braze_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:52:35.000000 edx-braze-client-0.1.7/edx_braze_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:52:35.000000 edx-braze-client-0.1.7/edx_braze_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 00:52:35.000000 edx-braze-client-0.1.7/edx_braze_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:52:35.407261 edx-braze-client-0.1.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-13 00:52:35.407261 edx-braze-client-0.1.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5176 2023-07-13 00:52:07.000000 edx-braze-client-0.1.7/setup.py
```

### Comparing `edx-braze-client-0.1.6/CHANGELOG.rst` & `edx-braze-client-0.1.7/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.1.7]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: add retrieve_unsubscribed_emails method
+
 [0.1.6]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: add unsubscribe_user_email method
 
 [0.1.5]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: add send_canvas_message method
```

### Comparing `edx-braze-client-0.1.6/LICENSE` & `edx-braze-client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.1.6/LICENSE.txt` & `edx-braze-client-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.1.6/PKG-INFO` & `edx-braze-client-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-braze-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client for interacting with Braze APIs
 Home-page: https://github.com/edx/braze-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Platform: UNKNOWN
@@ -157,14 +157,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.1.7]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: add retrieve_unsubscribed_emails method
+
 [0.1.6]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: add unsubscribe_user_email method
 
 [0.1.5]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: add send_canvas_message method
```

### Comparing `edx-braze-client-0.1.6/README.rst` & `edx-braze-client-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.1.6/braze/constants.py` & `edx-braze-client-0.1.7/braze/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,13 +12,18 @@
     SEND_CANVAS = '/canvas/trigger/send'
     EXPORT_IDS = '/users/export/ids'
     SEND_MESSAGE = '/messages/send'
     NEW_ALIAS = '/users/alias/new'
     TRACK_USER = '/users/track'
     IDENTIFY_USERS = '/users/identify'
     UNSUBSCRIBE_USER_EMAIL = '/email/status'
+    UNSUBSCRIBED_EMAILS = '/email/unsubscribes'
 
 
 # Braze enforced request size limits
+REQUEST_TYPE_GET = 'get'
+REQUEST_TYPE_POST = 'post'
 TRACK_USER_COMPONENT_CHUNK_SIZE = 75
 USER_ALIAS_CHUNK_SIZE = 50
 UNSUBSCRIBED_STATE = 'unsubscribed'
+UNSUBSCRIBED_EMAILS_API_LIMIT = 500
+UNSUBSCRIBED_EMAILS_API_SORT_DIRECTION = 'desc'
```

### Comparing `edx-braze-client-0.1.6/braze/exceptions.py` & `edx-braze-client-0.1.7/braze/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.1.6/edx_braze_client.egg-info/PKG-INFO` & `edx-braze-client-0.1.7/edx_braze_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-braze-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client for interacting with Braze APIs
 Home-page: https://github.com/edx/braze-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Platform: UNKNOWN
@@ -157,14 +157,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.1.7]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: add retrieve_unsubscribed_emails method
+
 [0.1.6]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: add unsubscribe_user_email method
 
 [0.1.5]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: add send_canvas_message method
```

### Comparing `edx-braze-client-0.1.6/requirements/constraints.txt` & `edx-braze-client-0.1.7/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.1.6/setup.py` & `edx-braze-client-0.1.7/setup.py`

 * *Files identical despite different names*

