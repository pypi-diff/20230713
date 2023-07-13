# Comparing `tmp/adafri-0.0.14.tar.gz` & `tmp/adafri-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.14.tar", last modified: Thu Jul 13 02:57:43 2023, max compression
+gzip compressed data, was "adafri-0.0.15.tar", last modified: Thu Jul 13 16:14:04 2023, max compression
```

## Comparing `adafri-0.0.14.tar` & `adafri-0.0.15.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.257335 adafri-0.0.14/
--rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 02:57:43.256825 adafri-0.0.14/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.228038 adafri-0.0.14/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.14/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.232207 adafri-0.0.14/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.14/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.14/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.14/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.233157 adafri-0.0.14/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.14/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.234143 adafri-0.0.14/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.14/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.236846 adafri-0.0.14/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.14/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.14/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.14/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.237722 adafri-0.0.14/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.14/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.239456 adafri-0.0.14/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.14/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.14/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.240647 adafri-0.0.14/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.14/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.241000 adafri-0.0.14/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.14/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.248209 adafri-0.0.14/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.14/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6342 2023-07-13 02:56:27.000000 adafri-0.0.14/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4344 2023-07-12 22:07:29.000000 adafri-0.0.14/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9417 2023-07-13 02:07:53.000000 adafri-0.0.14/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.14/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9007 2023-07-13 02:08:22.000000 adafri-0.0.14/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.14/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.250391 adafri-0.0.14/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.14/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 01:22:01.000000 adafri-0.0.14/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.251860 adafri-0.0.14/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.14/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.255352 adafri-0.0.14/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.14/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9358 2023-07-13 02:08:54.000000 adafri-0.0.14/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.14/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:57:43.230195 adafri-0.0.14/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 02:57:43.000000 adafri-0.0.14/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-13 02:57:43.000000 adafri-0.0.14/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-13 02:57:43.000000 adafri-0.0.14/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-13 02:57:43.000000 adafri-0.0.14/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-13 02:57:43.257526 adafri-0.0.14/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)     1007 2023-07-13 02:57:16.000000 adafri-0.0.14/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.294408 adafri-0.0.15/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 16:14:04.293776 adafri-0.0.15/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.266305 adafri-0.0.15/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.15/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.270856 adafri-0.0.15/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.15/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.15/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.15/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.271695 adafri-0.0.15/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.15/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.272534 adafri-0.0.15/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.15/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.275122 adafri-0.0.15/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.15/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.15/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.15/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.275990 adafri-0.0.15/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.15/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.277930 adafri-0.0.15/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.15/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.15/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.279094 adafri-0.0.15/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.15/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.279814 adafri-0.0.15/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.15/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.285831 adafri-0.0.15/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6357 2023-07-13 16:12:37.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9417 2023-07-13 16:07:22.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9007 2023-07-13 02:08:22.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.287845 adafri-0.0.15/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.15/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.15/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.288644 adafri-0.0.15/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.15/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.292094 adafri-0.0.15/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.15/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.15/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.15/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.268517 adafri-0.0.15/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 16:14:04.000000 adafri-0.0.15/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-13 16:14:04.000000 adafri-0.0.15/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-13 16:14:04.000000 adafri-0.0.15/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-13 16:14:04.000000 adafri-0.0.15/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-13 16:14:04.294698 adafri-0.0.15/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1007 2023-07-13 16:13:54.000000 adafri-0.0.15/setup.py
```

### Comparing `adafri-0.0.14/adafri/utils/response.py` & `adafri-0.0.15/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/utils/utils.py` & `adafri-0.0.15/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/account/models/account.py` & `adafri-0.0.15/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/account/models/account_fields.py` & `adafri-0.0.15/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.15/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.15/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.15/adafri/v1/auth/oauth/models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     client_secret: str
     uri: str
     grant_types: list[str]
     response_types: list[str]
     token_endpoint_auth_method: str
     redirect_uris: list[str]
     scopes: list[str]
+    scope: str
     client_id_issued_at: int
     createdAt: any
     allowed_redirect_uris: list[str]
     default_redirect_uri: str
     
     def __init__(self, client=None, default_redirect_uri=None, **kwargs):
         (cls_object, keys, data_args) = init_class_kwargs(self, client, STANDARD_FIELDS, ClientFieldProps, CLIENT_COLLECTION, ['id'], **kwargs)
```

### Comparing `adafri-0.0.14/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.15/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     redirect_uris = "redirect_uris"
     allowed_redirect_uris = "allowed_redirect_uris"
     uri = "uri"
     grant_types = "grant_types" 
     response_types = "response_types"
     token_endpoint_auth_method  = "token_endpoint_auth_method"
     scopes = "scopes"
+    scope = "scope"
     client_id_issued_at = "client_id_issued_at"
+    default_redirect_uri = "default_redirect_uri"
     created_at = "createdAt"
 
     @staticmethod
     def keys():
         return DictUtils.get_keys(ClientFieldProps);
 
     @staticmethod
@@ -80,14 +82,32 @@
         "type": str,
         "required": True,
         "mutable": True,
         "editable": True,
         "interactive": True,
         "default_value": "",
         "pickable": True
+    },
+    ClientFields.default_redirect_uri: {
+        "type": str,
+        "required": True,
+        "mutable": True,
+        "editable": True,
+        "interactive": True,
+        "default_value": "",
+        "pickable": True
+    },
+    ClientFields.scope: {
+        "type": str,
+        "required": True,
+        "mutable": True,
+        "editable": True,
+        "interactive": True,
+        "default_value": "",
+        "pickable": True
     },
     ClientFields.token_endpoint_auth_method: {
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
```

### Comparing `adafri-0.0.14/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.15/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.15/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.15/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.15/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/base/firebase_collection.py` & `adafri-0.0.15/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri/v1/user/models/user.py` & `adafri-0.0.15/adafri/v1/user/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,14 @@
     @staticmethod
     def from_dict(user: Any, db=None, collection_name=USERS_COLLECTION) -> 'User':
         cls_object, keys = get_object_model_class(user, User, UserFieldProps);
         _user = User(cls_object, db=db, collection_name=collection_name)
         return _user
     
     def get(self):
-        print('self', self.id)
         doc = self.document_reference().get();
         if doc.exists is False:
             return None;
         return User.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
 
     def query(self, query_params: list, first=False, limit=None):
         query_result = [];
```

### Comparing `adafri-0.0.14/adafri/v1/user/models/user_fields.py` & `adafri-0.0.15/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/adafri.egg-info/SOURCES.txt` & `adafri-0.0.15/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.14/setup.py` & `adafri-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.14' 
+VERSION = '0.0.15' 
 DESCRIPTION = 'Adafri python module'
 LONG_DESCRIPTION = 'Adafri python module helper'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri",
```

