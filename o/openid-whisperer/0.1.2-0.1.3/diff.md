# Comparing `tmp/openid_whisperer-0.1.2.tar.gz` & `tmp/openid_whisperer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openid_whisperer-0.1.2.tar", max compression
+gzip compressed data, was "openid_whisperer-0.1.3.tar", max compression
```

## Comparing `openid_whisperer-0.1.2.tar` & `openid_whisperer-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.2/LICENSE
--rw-r--r--   0        0        0     7097 2023-07-12 16:26:48.893540 openid_whisperer-0.1.2/README.md
--rw-r--r--   0        0        0     2097 2023-07-12 20:18:28.421057 openid_whisperer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.2/src/openid_whisperer/__init__.py
--rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.2/src/openid_whisperer/__main__.py
--rw-r--r--   0        0        0     7799 2023-07-10 20:59:59.115502 openid_whisperer-0.1.2/src/openid_whisperer/config.py
--rw-r--r--   0        0        0     1112 2023-07-11 21:48:13.064616 openid_whisperer-0.1.2/src/openid_whisperer/main.py
--rw-r--r--   0        0        0    20852 2023-07-12 17:42:03.339267 openid_whisperer-0.1.2/src/openid_whisperer/openid_blueprint.py
--rw-r--r--   0        0        0    26013 2023-07-11 22:18:31.791763 openid_whisperer-0.1.2/src/openid_whisperer/openid_interface.py
--rw-r--r--   0        0        0      922 2023-07-09 21:10:04.200881 openid_whisperer-0.1.2/src/openid_whisperer/openid_types.py
--rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.2/src/openid_whisperer/py.typed
--rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.2/src/openid_whisperer/static/style.css
--rw-r--r--   0        0        0    29080 2023-07-11 19:49:56.711266 openid_whisperer-0.1.2/src/openid_whisperer/templates/authenticate.html
--rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.2/src/openid_whisperer/utils/__init__.py
--rw-r--r--   0        0        0    13725 2023-07-05 20:49:35.637180 openid_whisperer-0.1.2/src/openid_whisperer/utils/cert_utils.py
--rw-r--r--   0        0        0     4074 2023-07-11 20:23:52.969778 openid_whisperer-0.1.2/src/openid_whisperer/utils/common.py
--rw-r--r--   0        0        0     4723 2023-07-10 20:57:32.222046 openid_whisperer-0.1.2/src/openid_whisperer/utils/config_utils.py
--rw-r--r--   0        0        0     3756 2023-07-11 22:11:18.564325 openid_whisperer-0.1.2/src/openid_whisperer/utils/credential_store.py
--rw-r--r--   0        0        0    11696 2023-07-11 22:15:16.409405 openid_whisperer-0.1.2/src/openid_whisperer/utils/token_store.py
--rw-r--r--   0        0        0     3150 2023-07-10 21:09:46.426743 openid_whisperer-0.1.2/src/openid_whisperer/utils/token_utils.py
--rw-r--r--   0        0        0     7094 2023-07-12 13:56:33.537165 openid_whisperer-0.1.2/src/openid_whisperer/utils/user_info_ext.py
--rw-r--r--   0        0        0     8132 1970-01-01 00:00:00.000000 openid_whisperer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7097 2023-07-12 16:26:48.893540 openid_whisperer-0.1.3/README.md
+-rw-r--r--   0        0        0     2143 2023-07-12 22:01:50.709606 openid_whisperer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.3/src/openid_whisperer/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.3/src/openid_whisperer/__main__.py
+-rw-r--r--   0        0        0     7799 2023-07-10 20:59:59.115502 openid_whisperer-0.1.3/src/openid_whisperer/config.py
+-rw-r--r--   0        0        0     1112 2023-07-11 21:48:13.064616 openid_whisperer-0.1.3/src/openid_whisperer/main.py
+-rw-r--r--   0        0        0    20852 2023-07-12 17:42:03.339267 openid_whisperer-0.1.3/src/openid_whisperer/openid_blueprint.py
+-rw-r--r--   0        0        0    26013 2023-07-11 22:18:31.791763 openid_whisperer-0.1.3/src/openid_whisperer/openid_interface.py
+-rw-r--r--   0        0        0      922 2023-07-09 21:10:04.200881 openid_whisperer-0.1.3/src/openid_whisperer/openid_types.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.3/src/openid_whisperer/py.typed
+-rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.3/src/openid_whisperer/static/style.css
+-rw-r--r--   0        0        0    29080 2023-07-11 19:49:56.711266 openid_whisperer-0.1.3/src/openid_whisperer/templates/authenticate.html
+-rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.3/src/openid_whisperer/utils/__init__.py
+-rw-r--r--   0        0        0    13725 2023-07-05 20:49:35.637180 openid_whisperer-0.1.3/src/openid_whisperer/utils/cert_utils.py
+-rw-r--r--   0        0        0     4074 2023-07-11 20:23:52.969778 openid_whisperer-0.1.3/src/openid_whisperer/utils/common.py
+-rw-r--r--   0        0        0     4723 2023-07-10 20:57:32.222046 openid_whisperer-0.1.3/src/openid_whisperer/utils/config_utils.py
+-rw-r--r--   0        0        0     3756 2023-07-11 22:11:18.564325 openid_whisperer-0.1.3/src/openid_whisperer/utils/credential_store.py
+-rw-r--r--   0        0        0    11696 2023-07-11 22:15:16.409405 openid_whisperer-0.1.3/src/openid_whisperer/utils/token_store.py
+-rw-r--r--   0        0        0     3150 2023-07-10 21:09:46.426743 openid_whisperer-0.1.3/src/openid_whisperer/utils/token_utils.py
+-rw-r--r--   0        0        0     7094 2023-07-12 13:56:33.537165 openid_whisperer-0.1.3/src/openid_whisperer/utils/user_info_ext.py
+-rw-r--r--   0        0        0     8183 1970-01-01 00:00:00.000000 openid_whisperer-0.1.3/PKG-INFO
```

### Comparing `openid_whisperer-0.1.2/LICENSE` & `openid_whisperer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/README.md` & `openid_whisperer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/pyproject.toml` & `openid_whisperer-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "openid-whisperer"
-version = "0.1.2"
+version = "0.1.3"
 description = "OpenID 1.0 Mock Identity Service"
 license = "MIT"
 authors = ["Robert Betts <betts_robert@yahoo.com>"]
 maintainers = ["Robert Betts <betts_robert@yahoo.com>"]
 readme = "README.md"
 homepage = "https://github.com/robertbetts/openid-whisperer"
 repository = "https://github.com/robertbetts/openid-whisperer"
 keywords = ["python", "mock", "api", "oauth2", "openid"]
 classifiers = [
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.10',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
 ]
 packages = [
     {include = "openid_whisperer", from = "src" }
 ]
 
@@ -60,15 +61,15 @@
     "src/mocking_examples"
 ]
 
 [tool.pylint]
 ignore-paths = "tests"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 pyjwt = "^2.6.0"
 requests = {extras = ["security"], version = "^2.31.0"}
 types-requests = "^2.31.0.1"
 cryptography = "^41.0.1"
 pyyaml = "^6.0"
 flask = {extras = ["async"], version = "^2.2.3"}
 python-dotenv = "^1.0.0"
```

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/config.py` & `openid_whisperer-0.1.3/src/openid_whisperer/config.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/main.py` & `openid_whisperer-0.1.3/src/openid_whisperer/main.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/openid_blueprint.py` & `openid_whisperer-0.1.3/src/openid_whisperer/openid_blueprint.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/openid_interface.py` & `openid_whisperer-0.1.3/src/openid_whisperer/openid_interface.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/openid_types.py` & `openid_whisperer-0.1.3/src/openid_whisperer/openid_types.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/static/style.css` & `openid_whisperer-0.1.3/src/openid_whisperer/static/style.css`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/templates/authenticate.html` & `openid_whisperer-0.1.3/src/openid_whisperer/templates/authenticate.html`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/utils/cert_utils.py` & `openid_whisperer-0.1.3/src/openid_whisperer/utils/cert_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/utils/common.py` & `openid_whisperer-0.1.3/src/openid_whisperer/utils/common.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/utils/config_utils.py` & `openid_whisperer-0.1.3/src/openid_whisperer/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/utils/credential_store.py` & `openid_whisperer-0.1.3/src/openid_whisperer/utils/credential_store.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/utils/token_store.py` & `openid_whisperer-0.1.3/src/openid_whisperer/utils/token_store.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/utils/token_utils.py` & `openid_whisperer-0.1.3/src/openid_whisperer/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/src/openid_whisperer/utils/user_info_ext.py` & `openid_whisperer-0.1.3/src/openid_whisperer/utils/user_info_ext.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.2/PKG-INFO` & `openid_whisperer-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: openid-whisperer
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenID 1.0 Mock Identity Service
 Home-page: https://github.com/robertbetts/openid-whisperer
 License: MIT
 Keywords: python,mock,api,oauth2,openid
 Author: Robert Betts
 Author-email: betts_robert@yahoo.com
 Maintainer: Robert Betts
 Maintainer-email: betts_robert@yahoo.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Faker (>=18.13.0,<19.0.0)
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: flask[async] (>=2.2.3,<3.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
```

