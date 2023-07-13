# Comparing `tmp/uagents_whatsapp_utility-1.0.0.tar.gz` & `tmp/uagents_whatsapp_utility-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_whatsapp_utility-1.0.0.tar", max compression
+gzip compressed data, was "uagents_whatsapp_utility-2.0.tar", max compression
```

## Comparing `uagents_whatsapp_utility-1.0.0.tar` & `uagents_whatsapp_utility-2.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-07-13 12:41:16.397759 uagents_whatsapp_utility-1.0.0/LICENSE
--rw-r--r--   0        0        0      645 2023-07-13 12:41:16.397759 uagents_whatsapp_utility-1.0.0/README.rst
--rw-r--r--   0        0        0      885 2023-07-13 12:41:41.041567 uagents_whatsapp_utility-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       28 2023-07-13 12:41:16.397759 uagents_whatsapp_utility-1.0.0/uagents_whatsapp_utility/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 12:41:16.397759 uagents_whatsapp_utility-1.0.0/uagents_whatsapp_utility/models.py
--rw-r--r--   0        0        0      107 2023-07-13 12:41:16.397759 uagents_whatsapp_utility-1.0.0/uagents_whatsapp_utility/protocols/Chat.py
--rw-r--r--   0        0        0     1921 2023-07-13 12:41:16.397759 uagents_whatsapp_utility-1.0.0/uagents_whatsapp_utility/wrappers/TwilioChatWrapper.py
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 uagents_whatsapp_utility-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-13 13:14:05.183425 uagents_whatsapp_utility-2.0/LICENSE
+-rw-r--r--   0        0        0      645 2023-07-13 13:14:05.183425 uagents_whatsapp_utility-2.0/README.rst
+-rw-r--r--   0        0        0      883 2023-07-13 13:14:27.147897 uagents_whatsapp_utility-2.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-07-13 13:14:05.183425 uagents_whatsapp_utility-2.0/uagents_whatsapp_utility/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:14:05.183425 uagents_whatsapp_utility-2.0/uagents_whatsapp_utility/models.py
+-rw-r--r--   0        0        0      107 2023-07-13 13:14:05.183425 uagents_whatsapp_utility-2.0/uagents_whatsapp_utility/protocols/Chat.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:14:05.183425 uagents_whatsapp_utility-2.0/uagents_whatsapp_utility/protocols/__init__.py
+-rw-r--r--   0        0        0     1921 2023-07-13 13:14:05.183425 uagents_whatsapp_utility-2.0/uagents_whatsapp_utility/wrappers/TwilioChatWrapper.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:14:05.183425 uagents_whatsapp_utility-2.0/uagents_whatsapp_utility/wrappers/__init__.py
+-rw-r--r--   0        0        0     1641 1970-01-01 00:00:00.000000 uagents_whatsapp_utility-2.0/PKG-INFO
```

### Comparing `uagents_whatsapp_utility-1.0.0/LICENSE` & `uagents_whatsapp_utility-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents_whatsapp_utility-1.0.0/README.rst` & `uagents_whatsapp_utility-2.0/README.rst`

 * *Files identical despite different names*

### Comparing `uagents_whatsapp_utility-1.0.0/pyproject.toml` & `uagents_whatsapp_utility-2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "uagents-whatsapp-utility"
 #
-version = "1.0.0"
+version = "2.0"
 #
 description = ""
 authors = ["User A <user-a@example.com>"]
 readme = "README.rst"
 repository = "https://github.com/Github User/uagents-whatsapp-utility"
 packages = [{include = "uagents_whatsapp_utility"}]
 classifiers=[
```

### Comparing `uagents_whatsapp_utility-1.0.0/uagents_whatsapp_utility/wrappers/TwilioChatWrapper.py` & `uagents_whatsapp_utility-2.0/uagents_whatsapp_utility/wrappers/TwilioChatWrapper.py`

 * *Files identical despite different names*

### Comparing `uagents_whatsapp_utility-1.0.0/PKG-INFO` & `uagents_whatsapp_utility-2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents-whatsapp-utility
-Version: 1.0.0
+Version: 2.0
 Summary: 
 Home-page: https://github.com/Github User/uagents-whatsapp-utility
 Author: User A
 Author-email: user-a@example.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

