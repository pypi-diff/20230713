# Comparing `tmp/adafri-0.0.15.tar.gz` & `tmp/adafri-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.15.tar", last modified: Thu Jul 13 16:14:04 2023, max compression
+gzip compressed data, was "adafri-0.0.16.tar", last modified: Thu Jul 13 21:16:15 2023, max compression
```

## Comparing `adafri-0.0.15.tar` & `adafri-0.0.16.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.294408 adafri-0.0.15/
--rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 16:14:04.293776 adafri-0.0.15/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.266305 adafri-0.0.15/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.15/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.270856 adafri-0.0.15/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.15/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.15/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.15/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.271695 adafri-0.0.15/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.15/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.272534 adafri-0.0.15/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.15/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.275122 adafri-0.0.15/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.15/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.15/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.15/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.275990 adafri-0.0.15/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.15/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.277930 adafri-0.0.15/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.15/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.15/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.279094 adafri-0.0.15/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.15/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.279814 adafri-0.0.15/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.15/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.285831 adafri-0.0.15/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6357 2023-07-13 16:12:37.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9417 2023-07-13 16:07:22.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9007 2023-07-13 02:08:22.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.15/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.287845 adafri-0.0.15/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.15/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.15/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.288644 adafri-0.0.15/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.15/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.292094 adafri-0.0.15/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.15/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.15/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.15/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 16:14:04.268517 adafri-0.0.15/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 16:14:04.000000 adafri-0.0.15/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-13 16:14:04.000000 adafri-0.0.15/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-13 16:14:04.000000 adafri-0.0.15/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-13 16:14:04.000000 adafri-0.0.15/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-13 16:14:04.294698 adafri-0.0.15/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)     1007 2023-07-13 16:13:54.000000 adafri-0.0.15/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.287071 adafri-0.0.16/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 21:16:15.286740 adafri-0.0.16/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.262452 adafri-0.0.16/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.16/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.266685 adafri-0.0.16/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.16/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.16/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.16/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.267367 adafri-0.0.16/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.16/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.268080 adafri-0.0.16/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.16/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.270660 adafri-0.0.16/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.16/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.16/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.16/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.271596 adafri-0.0.16/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.16/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.273081 adafri-0.0.16/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.16/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.16/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.274268 adafri-0.0.16/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.16/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.274650 adafri-0.0.16/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.16/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.279852 adafri-0.0.16/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.16/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6354 2023-07-13 21:14:52.000000 adafri-0.0.16/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.16/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9421 2023-07-13 21:15:14.000000 adafri-0.0.16/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.16/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9007 2023-07-13 02:08:22.000000 adafri-0.0.16/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.16/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.281497 adafri-0.0.16/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.16/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.16/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.281918 adafri-0.0.16/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.16/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.285664 adafri-0.0.16/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.16/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.16/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.16/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 21:16:15.264587 adafri-0.0.16/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 21:16:15.000000 adafri-0.0.16/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-13 21:16:15.000000 adafri-0.0.16/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-13 21:16:15.000000 adafri-0.0.16/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-13 21:16:15.000000 adafri-0.0.16/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-13 21:16:15.287217 adafri-0.0.16/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1007 2023-07-13 21:15:41.000000 adafri-0.0.16/setup.py
```

### Comparing `adafri-0.0.15/adafri/utils/response.py` & `adafri-0.0.16/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/utils/utils.py` & `adafri-0.0.16/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/account/models/account.py` & `adafri-0.0.16/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/account/models/account_fields.py` & `adafri-0.0.16/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.16/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.16/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.16/adafri/v1/auth/oauth/models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     default_redirect_uri: str
     
     def __init__(self, client=None, default_redirect_uri=None, **kwargs):
         (cls_object, keys, data_args) = init_class_kwargs(self, client, STANDARD_FIELDS, ClientFieldProps, CLIENT_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]) 
-        self.default_redirect_uri = default_redirect_uri
+        #self.default_redirect_uri = default_redirect_uri
 
 
     @staticmethod
     def generate_model(_key_="default_value"):
         user = {};
         props = ClientFieldProps
         for k in DictUtils.get_keys(props):
@@ -118,15 +118,15 @@
             self.document_reference().set(data_update, merge=True)
             return DictUtils.dict_from_keys(self.get().to_json(), changed_fields);
         except Exception as e:
             print(e)
             return None;
 
     def get_default_redirect_uri(self):
-        return self.default_redirect_uri
+        return self.redirect_uris[0]
     
     def check_response_type(self, response_type):
         return response_type in self.response_types
     
     def check_client_secret(self, client_secret):
         return secrets.compare_digest(self.client_secret, client_secret)
```

### Comparing `adafri-0.0.15/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.16/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.16/adafri/v1/auth/oauth/models/grant.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             if self.id is None:
                 return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Cannot identify Authorization code with id {self.id} to delete","INVALID_REQUEST", 1));
             deleted = self.document_reference().delete();
             return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": f"Authorization code {self.id} deleted"}, None);
         except:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated while removing authorization code with id {self.id}","INVALID_REQUEST", 1));
 
-
+    
 
 class AuthorizationCodeGrant(grants.AuthorizationCodeGrant):
     RESPONSE_TYPES = set({"code", "token"})
     TOKEN_ENDPOINT_AUTH_METHODS = [
         'client_secret_basic',
         'client_secret_post'
     ]
```

### Comparing `adafri-0.0.15/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.16/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.16/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.16/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/base/firebase_collection.py` & `adafri-0.0.16/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/user/models/user.py` & `adafri-0.0.16/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri/v1/user/models/user_fields.py` & `adafri-0.0.16/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/adafri.egg-info/SOURCES.txt` & `adafri-0.0.16/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.15/setup.py` & `adafri-0.0.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.15' 
+VERSION = '0.0.16' 
 DESCRIPTION = 'Adafri python module'
 LONG_DESCRIPTION = 'Adafri python module helper'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri",
```

