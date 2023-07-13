# Comparing `tmp/adafri-0.0.12.tar.gz` & `tmp/adafri-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.12.tar", last modified: Tue Jul 11 22:42:58 2023, max compression
+gzip compressed data, was "adafri-0.0.13.tar", last modified: Thu Jul 13 02:34:27 2023, max compression
```

## Comparing `adafri-0.0.12.tar` & `adafri-0.0.13.tar`

### file list

```diff
@@ -1,30 +1,49 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.510805 adafri-0.0.12/
--rw-r--r--   0 ibrahima   (502) staff       (20)      552 2023-07-11 22:42:58.510368 adafri-0.0.12/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.499457 adafri-0.0.12/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       50 2023-07-11 19:48:50.000000 adafri-0.0.12/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.504249 adafri-0.0.12/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       79 2023-07-11 21:48:50.000000 adafri-0.0.12/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1040 2023-07-11 22:40:50.000000 adafri-0.0.12/adafri/utils/firebase_collection.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.12/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    12814 2023-07-11 19:22:02.000000 adafri-0.0.12/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.504847 adafri-0.0.12/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       40 2023-07-11 21:48:14.000000 adafri-0.0.12/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.505443 adafri-0.0.12/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       42 2023-07-11 19:50:47.000000 adafri-0.0.12/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.507214 adafri-0.0.12/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:36:21.000000 adafri-0.0.12/adafri/v1/auth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5254 2023-07-11 19:45:53.000000 adafri-0.0.12/adafri/v1/auth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4321 2023-07-11 19:45:25.000000 adafri-0.0.12/adafri/v1/auth/models/client_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.507825 adafri-0.0.12/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)       21 2023-07-11 21:22:03.000000 adafri-0.0.12/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.509562 adafri-0.0.12/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-11 21:47:06.000000 adafri-0.0.12/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     8801 2023-07-11 21:51:21.000000 adafri-0.0.12/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4519 2023-07-11 19:25:49.000000 adafri-0.0.12/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.501975 adafri-0.0.12/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      552 2023-07-11 22:42:58.000000 adafri-0.0.12/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)      537 2023-07-11 22:42:58.000000 adafri-0.0.12/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-11 22:42:58.000000 adafri-0.0.12/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-11 22:42:58.000000 adafri-0.0.12/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-11 22:42:58.511001 adafri-0.0.12/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)     1000 2023-07-11 22:42:53.000000 adafri-0.0.12/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.070731 adafri-0.0.13/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 02:34:27.070206 adafri-0.0.13/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.032678 adafri-0.0.13/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.13/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.042209 adafri-0.0.13/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.13/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.13/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.13/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.043398 adafri-0.0.13/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.13/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.045145 adafri-0.0.13/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.13/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.048230 adafri-0.0.13/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.13/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.13/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.13/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.049644 adafri-0.0.13/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.13/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.051562 adafri-0.0.13/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.13/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.13/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.052731 adafri-0.0.13/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.13/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.053144 adafri-0.0.13/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.13/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.061659 adafri-0.0.13/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.13/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6129 2023-07-13 02:07:02.000000 adafri-0.0.13/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4344 2023-07-12 22:07:29.000000 adafri-0.0.13/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9417 2023-07-13 02:07:53.000000 adafri-0.0.13/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.13/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9007 2023-07-13 02:08:22.000000 adafri-0.0.13/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.13/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.063785 adafri-0.0.13/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.13/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 01:22:01.000000 adafri-0.0.13/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.064851 adafri-0.0.13/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.13/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.068745 adafri-0.0.13/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.13/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9358 2023-07-13 02:08:54.000000 adafri-0.0.13/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.13/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 02:34:27.037805 adafri-0.0.13/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 02:34:26.000000 adafri-0.0.13/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-13 02:34:27.000000 adafri-0.0.13/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-13 02:34:26.000000 adafri-0.0.13/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-13 02:34:26.000000 adafri-0.0.13/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-13 02:34:27.070894 adafri-0.0.13/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1007 2023-07-13 02:32:33.000000 adafri-0.0.13/setup.py
```

### Comparing `adafri-0.0.12/adafri/utils/response.py` & `adafri-0.0.13/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.12/adafri/utils/utils.py` & `adafri-0.0.13/adafri/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,39 +49,92 @@
     
     response = [];
     for f in request_fields:
         response.append(str(f).strip())
     
     return response;
 
+import inspect
+def get_class_properties(cls, property='__match_args__'):
+        inspected = inspect.getmembers(cls, lambda a:not(inspect.isroutine(a)))
+        # attr = [a for a in inspected if not(a[0].startswith('__') and a[0].endswith('__'))]
+        attr = [a[1] for a in inspected if a[0]=='__match_args__']
+        if(len(attr)>0):
+            if type(attr[0]) is tuple:
+                return list(attr[0])
+        return list(attr)
 
+def get_object_model_class(object_model, cls, fields=None, property='__match_args__'):
+        obj = object_model
+        attributes = get_class_properties(cls, property);
+        if bool(obj) is False:
+            obj = {}
+            for key in attributes:
+                obj[key] = getattr(cls, key, None)
+
+        data_object = DictUtils.pick_object_values(obj, attributes);
+        keys = DictUtils.get_keys(data_object);
+        if fields is not None:
+            for key in attributes:
+                if key in fields:
+                    if key not in data_object or data_object[key] is None or data_object[key] == 'None':
+                        if 'default_value' in fields[key]:
+                            data_object[key] = fields[key]['default_value']
+        return data_object, attributes
+
+def init_class_kwargs(cls, obj, class_fields, class_fields_props, class_collection_name, ids_key: list[str], **kwargs):
+        cls_object, keys = get_object_model_class(obj, cls, class_fields_props);
+        kwargs['fields'] = class_fields
+        kwargs['fields_props'] = class_fields_props
+
+        for key in ids_key:
+            documentId = None;
+            if key in cls_object:
+                documentId = cls_object[key]
+            if documentId is not None and bool(documentId):
+                # print('docId', documentId)
+                kwargs['id'] = documentId;
+                break;
+        
+        collection_name = getattr(kwargs, 'collection_name', None)
+        if collection_name is None or bool(collection_name) is False:
+            kwargs['collection_name'] = class_collection_name;
+        return cls_object, keys, kwargs;
 
 class JsonEncoder(json.JSONEncoder):
     def default(self, obj):
         # try:
         #     iterable = iter(obj)
         # except TypeError:
         #     pass
         # else:
         #     return list(iterable)
         # Let the base class default method raise the TypeError
         #return json.JSONEncoder.default(self, obj)
  
- 
-       return obj.__dict__ 
+       attr = getattr(obj, '__dict__', None)
+       if attr is not None:
+            return obj.__dict__ 
+       return {}
 
 class DateUtils:
     def from_iso(date_str):
         try:
             return date.fromisoformat(date_str);
         except Exception as e:
             return None;
 class DictUtils:
 
     @staticmethod
+    def pick_object_values(obj, keys: list[str]):
+        cls_object = {};
+        for attr in keys:
+            cls_object[attr] = pydash.get(obj, attr, None)
+        return cls_object
+    @staticmethod
     def every_match(element, exceptions=[]):
         if element is None:
             return False;
     
         data = pydash.omit(element, exceptions);
         keys = pydash.keys(data);
         if bool(keys) == False:
```

### Comparing `adafri-0.0.12/adafri/v1/auth/models/client.py` & `adafri-0.0.13/adafri/v1/auth/oauth/models/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from utils.utils import ArrayUtils, JsonEncoder, DictUtils, Crypto
-from .client_fields import ClientFields, ClientFieldProps
-from utils.response import ApiResponse, Error, ResponseStatus, StatusCode
+from ....base.firebase_collection import FirebaseCollectionBase
+from .....utils import ArrayUtils, DictUtils, Crypto, get_object_model_class, init_class_kwargs
+from .client_fields import ClientFields, ClientFieldProps, STANDARD_FIELDS, CLIENT_COLLECTION
+from .....utils.response import ApiResponse, Error, ResponseStatus, StatusCode
 from werkzeug.security import gen_salt
 import time
-from typing import List
 from typing import Any
 from dataclasses import dataclass
 import json
-import pydash
 from authlib.oauth2.rfc6749 import ClientMixin
 import secrets
+import pydash
 
-@dataclass
-class Client(ClientMixin):
+@dataclass(init=False)
+class OAuthClient(ClientMixin, FirebaseCollectionBase):
     id: str
     name: str
     uid: str
     description: str
     client_id: str
     client_secret: str
     uri: str
@@ -24,50 +24,65 @@
     response_types: list[str]
     token_endpoint_auth_method: str
     redirect_uris: list[str]
     scopes: list[str]
     client_id_issued_at: int
     createdAt: any
     allowed_redirect_uris: list[str]
-
-    @staticmethod
-    def from_dict(obj: Any) -> 'Client':
-        _id = str(DictUtils.pick(obj, ClientFields.id, str));
-        _name = str(DictUtils.pick(obj, ClientFields.name, str));
-        _uid = str(DictUtils.pick(obj, ClientFields.uid, str));
-        _description = str(DictUtils.pick(obj, ClientFields.description, str));
-        _client_id = str(DictUtils.pick(obj, ClientFields.client_id, str));
-        _client_secret = str(DictUtils.pick(obj, ClientFields.client_secret, str));
-        _uri = str(DictUtils.pick(obj, ClientFields.uri, str));
-        _grant_types = [y for y in DictUtils.pick(obj, ClientFields.grant_types, list)]
-        _response_types = [y for y in DictUtils.pick(obj, ClientFields.response_types, list)]
-        _token_endpoint_auth_method = str(DictUtils.pick(obj, ClientFields.token_endpoint_auth_method, str));
-        _redirect_uris = [y for y in DictUtils.pick(obj, ClientFields.redirect_uris, list)]
-        _scopes = [y for y in DictUtils.pick(obj, ClientFields.scopes, list)]
-        _client_id_issued_at = int(str(DictUtils.pick(obj, ClientFields.client_id_issued_at, int)));
-        _createdAt = str(DictUtils.pick(obj, ClientFields.created_at, str, ""));
-        _allowed_redirect_uris = [y for y in DictUtils.pick(obj, ClientFields.allowed_redirect_uris, list)]
-        if bool(_allowed_redirect_uris) is False:
-            _allowed_redirect_uris = _redirect_uris
-        return Client(_id, _name, _uid, _description, _client_id, _client_secret, _uri, _grant_types,  _response_types, _token_endpoint_auth_method, _redirect_uris, _scopes, _client_id_issued_at, _createdAt, _allowed_redirect_uris)
+    default_redirect_uri: str
+    
+    def __init__(self, client=None, default_redirect_uri=None, **kwargs):
+        (cls_object, keys, data_args) = init_class_kwargs(self, client, STANDARD_FIELDS, ClientFieldProps, CLIENT_COLLECTION, ['id'], **kwargs)
+        super().__init__(**data_args);
+        for key in keys:
+            setattr(self, key, cls_object[key]) 
+        self.default_redirect_uri = default_redirect_uri
 
 
     @staticmethod
-    def generate_model():
+    def generate_model(_key_="default_value"):
         user = {};
-        for k in DictUtils.get_keys(ClientFieldProps):
-            _key_ = 'default_value';
-            user[k] = ClientFieldProps[k][_key_];
+        props = ClientFieldProps
+        for k in DictUtils.get_keys(props):
+            user[k] = props[k][_key_];
         return user;
 
     @staticmethod
+    def from_dict(client = None, db=None, collection_name=None, default_redirect_uri=None) -> 'OAuthClient':
+        cls_object, keys = get_object_model_class(client, OAuthClient, ClientFieldProps);
+        _client = OAuthClient(cls_object, db=db, collection_name=collection_name, default_redirect_uri=default_redirect_uri)
+        return _client
+
+    def query(self, query_params: list, first=False, limit=None):
+        query_result = [];
+        query_result = self.custom_query(query_params, first=first, limit=limit)
+        if bool(query_result):
+            if first:
+                return OAuthClient.from_dict(client=query_result, db=self.db, collection_name=self.collection_name, default_redirect_uri=self.default_redirect_uri)
+            else:
+                for doc in query_result:
+                    query_result.append(OAuthClient.from_dict(client=doc, db=self.db, collection_name=self.collection_name, default_redirect_uri=self.default_redirect_uri))
+                return query_result
+        if first:
+                return None
+        return [];
+
+    def get(self) -> 'OAuthClient':
+        if bool(self.id):
+            doc = self.document_reference().get();
+            if doc.exists is False:
+                return None;
+            return OAuthClient.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
+        if bool(self.client_id):
+            return self.query([{"key": "client_id", "comp": "==", "value": self.client_id}])
+
+    @staticmethod
     def generate(**kwargs) -> 'ApiResponse':
         data_dict = DictUtils.pick_fields(kwargs, ClientFields.filtered_keys('mutable', True));
-        print('data_dict:', data_dict)
-        client_model = Client.from_dict(DictUtils.merge_dict(data_dict, Client.generate_model()));
+        client_model = OAuthClient.from_dict(DictUtils.merge_dict(data_dict, OAuthClient.generate_model()));
         
         if bool(client_model.to_json()) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Empty request","INVALID_REQUEST", 1)).to_json()
         
         if bool(client_model.name) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("name required","INVALID_REQUEST", 1));
         
@@ -79,23 +94,32 @@
         client_model.client_id_issued_at = int(time.time())
         
         if client_model.token_endpoint_auth_method == 'none':
             client_model.client_secret = ''
         else:
             client_model.client_secret = gen_salt(48)
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, client_model.to_json(), None);
-
-    def to_json(self, fields=None):
-        if fields is None or type(fields) is not list:
-            return json.loads(JsonEncoder().encode(self));
-        return pydash.pick(json.loads(JsonEncoder().encode(self)), fields)
     
-    
-    # def get_default_redirect_uri(self):
-    #     return f"{baseUrl}/auth/challenge_success"
+    def update(self, data):
+        try:
+            last_value = self.to_json();
+            filtered_value = pydash.pick(data, ClientFields.filtered_keys('editable', True));
+            new_value = DictUtils.merge_dict(filtered_value, self.to_json());
+            changed_fields = DictUtils.get_changed_field(last_value, new_value);
+            data_update = DictUtils.dict_from_keys(filtered_value, changed_fields);
+            if bool(data_update) is False:
+                return None;
+            self.document_reference().set(data_update, merge=True)
+            return DictUtils.dict_from_keys(self.get().to_json(), changed_fields);
+        except Exception as e:
+            print(e)
+            return None;
+
+    def get_default_redirect_uri(self):
+        return self.default_redirect_uri
     
     def check_response_type(self, response_type):
         return response_type in self.response_types
     
     def check_client_secret(self, client_secret):
         return secrets.compare_digest(self.client_secret, client_secret)
```

### Comparing `adafri-0.0.12/adafri/v1/auth/models/client_fields.py` & `adafri-0.0.13/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from dataclasses import dataclass
-from typing import Any
-from utils.utils import DictUtils
+from .....utils.utils import DictUtils
 
+CLIENT_COLLECTION = "clients_collection"
 @dataclass
 class ClientFields:
     id = "id"
     name = "name"
     uid = "uid"
     description = "description"
     client_id = "client_id"
```

### Comparing `adafri-0.0.12/adafri/v1/user/models/user_fields.py` & `adafri-0.0.13/adafri/v1/user/models/user_fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from  utils.utils import DictUtils 
+from  ....utils.utils import DictUtils 
 
 USERS_COLLECTION = "users";
 
 @dataclass
 class UserFields:
     uid = "uid";
     email = 'email';
@@ -18,14 +18,15 @@
     address = 'addresse';
     photoURL = 'photoURL';
     profileCompleted = 'profileCompleted';
     telephone = 'telephone';
     postalCode = 'postal';
     token = 'token';
     deviceInfo = 'deviceInfo';
+    phoneInfo = 'phoneInfo';
     country = 'country';
     showPushToken = 'showPushToken'
     authorizedPush = 'authorizedPush';
     hasApprouvedPolicy = 'hasApprouvedPolicy';
 
     @staticmethod
     def keys():
@@ -41,140 +42,167 @@
 UserFieldProps = {
     UserFields.uid: {
         "type": str,
         "required": True,
         "mutable": False,
         "editable": False,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.email: {
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
+        "pickable": True,
+        "default_value": ""
+    },
+    UserFields.address: {
+        "type": str,
+        "required": True,
+        "mutable": True,
+        "editable": False,
+        "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.password: {
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": False,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.firstName: {
         "type": str,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.lastName: {
         "type": str,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.displayName: {
         "type": str,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.address: {
         "type": str,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.postalCode: {
         "type": str,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.telephone: {
         "type": str,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.authorizedPush: {
         "type": bool,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": False
     },
     UserFields.hasApprouvedPolicy: {
         "type": bool,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": False
     },
     UserFields.profileCompleted: {
         "type": bool,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": False
     },
     UserFields.entrepriseUrl: {
         "type": str,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.photoURL:{
         "type": str,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": True,
+        "pickable": True,
         "default_value": ""
     },
     UserFields.provider:{
         "type": str,
         "required": False,
         "mutable": True,
         "editable": False,
         "interactive": False,
+        "pickable": True,
         "default_value": "https://app.adafri.com"
     },
     UserFields.isConnectWithMailAndPassword:{
         "type": bool,
         "required": False,
         "mutable": False,
         "editable": False,
         "interactive": False,
+        "pickable": True,
         "default_value": False
     },
     UserFields.token:{
         "type": list[str],
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": False,
+        "pickable": True,
         "default_value": []
-    }       
+    } 
+
 }
 
-STANDARD_FIELDS = UserFields.filtered_keys('mutable', True)
+STANDARD_FIELDS = UserFields.filtered_keys('pickable', True)
```

### Comparing `adafri-0.0.12/adafri.egg-info/SOURCES.txt` & `adafri-0.0.13/adafri.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 setup.py
 adafri/__init__.py
 adafri.egg-info/PKG-INFO
 adafri.egg-info/SOURCES.txt
 adafri.egg-info/dependency_links.txt
 adafri.egg-info/top_level.txt
 adafri/utils/__init__.py
-adafri/utils/firebase_collection.py
 adafri/utils/response.py
 adafri/utils/utils.py
 adafri/v1/__init__.py
+adafri/v1/account/__init__.py
+adafri/v1/account/models/__init__.py
+adafri/v1/account/models/account.py
+adafri/v1/account/models/account_fields.py
 adafri/v1/auth/__init__.py
+adafri/v1/auth/firebase_auth/__init__.py
+adafri/v1/auth/firebase_auth/firebase_auth.py
 adafri/v1/auth/models/__init__.py
-adafri/v1/auth/models/client.py
-adafri/v1/auth/models/client_fields.py
+adafri/v1/auth/oauth/__init__.py
+adafri/v1/auth/oauth/models/__init__.py
+adafri/v1/auth/oauth/models/client.py
+adafri/v1/auth/oauth/models/client_fields.py
+adafri/v1/auth/oauth/models/grant.py
+adafri/v1/auth/oauth/models/grant_fields.py
+adafri/v1/auth/oauth/models/token.py
+adafri/v1/auth/oauth/models/token_fields.py
+adafri/v1/base/__init__.py
+adafri/v1/base/firebase_collection.py
 adafri/v1/user/__init__.py
 adafri/v1/user/models/__init__.py
 adafri/v1/user/models/user.py
 adafri/v1/user/models/user_fields.py
```

### Comparing `adafri-0.0.12/setup.py` & `adafri-0.0.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.12' 
+VERSION = '0.0.13' 
 DESCRIPTION = 'Adafri python module'
-LONG_DESCRIPTION = 'Adafri python module'
+LONG_DESCRIPTION = 'Adafri python module helper'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri", 
         version=VERSION,
         author="Ibrahima Touré",
```

