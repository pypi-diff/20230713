# Comparing `tmp/d20-securityLayer-2.0.0a8.tar.gz` & `tmp/d20-securityLayer-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-evjxy3hg\d20-securityLayer-2.0.0a8.tar", last modified: Tue Jun 20 03:07:46 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-jnc2tblm\d20-securityLayer-2.0.0a9.tar", last modified: Tue Jun 20 03:19:04 2023, max compression
```

## Comparing `d20-securityLayer-2.0.0a8.tar` & `d20-securityLayer-2.0.0a9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 03:07:46.301811 d20-securityLayer-2.0.0a8/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a8/LICENSE
--rw-rw-rw-   0        0        0      677 2023-06-20 03:07:46.299270 d20-securityLayer-2.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a8/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 03:07:46.301811 d20-securityLayer-2.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-06-20 03:07:08.000000 d20-securityLayer-2.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 03:07:46.227762 d20-securityLayer-2.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 03:07:46.255530 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/
--rw-rw-rw-   0        0        0      677 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-20 03:07:46.000000 d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 03:07:46.298299 d20-securityLayer-2.0.0a8/src/securityLayer/
--rw-rw-rw-   0        0        0    10081 2023-06-20 03:06:54.000000 d20-securityLayer-2.0.0a8/src/securityLayer/AccessControl.py
--rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a8/src/securityLayer/AuthAnswer.py
--rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a8/src/securityLayer/Error.py
--rw-rw-rw-   0        0        0    16797 2023-06-07 23:54:37.000000 d20-securityLayer-2.0.0a8/src/securityLayer/SSO.py
--rw-rw-rw-   0        0        0    15275 2023-06-20 03:06:27.000000 d20-securityLayer-2.0.0a8/src/securityLayer/SecurityLayer.py
--rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a8/src/securityLayer/__init__.py
--rw-rw-rw-   0        0        0      156 2023-06-20 03:07:02.000000 d20-securityLayer-2.0.0a8/src/securityLayer/__version__.py
--rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a8/src/securityLayer/default.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:19:04.756684 d20-securityLayer-2.0.0a9/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-06-20 03:19:04.753687 d20-securityLayer-2.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a9/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 03:19:04.756684 d20-securityLayer-2.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-06-20 03:18:48.000000 d20-securityLayer-2.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:19:04.688850 d20-securityLayer-2.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 03:19:04.719016 d20-securityLayer-2.0.0a9/src/d20_securityLayer.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-06-20 03:19:04.000000 d20-securityLayer-2.0.0a9/src/d20_securityLayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-06-20 03:19:04.000000 d20-securityLayer-2.0.0a9/src/d20_securityLayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 03:19:04.000000 d20-securityLayer-2.0.0a9/src/d20_securityLayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-20 03:19:04.000000 d20-securityLayer-2.0.0a9/src/d20_securityLayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-20 03:19:04.000000 d20-securityLayer-2.0.0a9/src/d20_securityLayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 03:19:04.751717 d20-securityLayer-2.0.0a9/src/securityLayer/
+-rw-rw-rw-   0        0        0    10081 2023-06-20 03:06:54.000000 d20-securityLayer-2.0.0a9/src/securityLayer/AccessControl.py
+-rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a9/src/securityLayer/AuthAnswer.py
+-rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a9/src/securityLayer/Error.py
+-rw-rw-rw-   0        0        0    16797 2023-06-07 23:54:37.000000 d20-securityLayer-2.0.0a9/src/securityLayer/SSO.py
+-rw-rw-rw-   0        0        0    15344 2023-06-20 03:18:38.000000 d20-securityLayer-2.0.0a9/src/securityLayer/SecurityLayer.py
+-rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a9/src/securityLayer/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-06-20 03:18:43.000000 d20-securityLayer-2.0.0a9/src/securityLayer/__version__.py
+-rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a9/src/securityLayer/default.py
```

### Comparing `d20-securityLayer-2.0.0a8/LICENSE` & `d20-securityLayer-2.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a8/PKG-INFO` & `d20-securityLayer-2.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a8/setup.py` & `d20-securityLayer-2.0.0a9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-securityLayer",
-    version="2.0.0a8",
+    version="2.0.0a9",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A simple access manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/security_layer_python_arangodb",
     project_urls={
```

### Comparing `d20-securityLayer-2.0.0a8/src/d20_securityLayer.egg-info/PKG-INFO` & `d20-securityLayer-2.0.0a9/src/d20_securityLayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a8/src/securityLayer/AccessControl.py` & `d20-securityLayer-2.0.0a9/src/securityLayer/AccessControl.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a8/src/securityLayer/Error.py` & `d20-securityLayer-2.0.0a9/src/securityLayer/Error.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a8/src/securityLayer/SSO.py` & `d20-securityLayer-2.0.0a9/src/securityLayer/SSO.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a8/src/securityLayer/SecurityLayer.py` & `d20-securityLayer-2.0.0a9/src/securityLayer/SecurityLayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         def make(self):
             self.attributes = ['_key', 'password', 'username', 'created', 'updated', 'partners', 'actions', 'email', 'active', 'oauth_urls', 'oauth_scopes', 'allowed_types', 'deleted']
             for key in self.attributes:
                 setattr(self, key, None)
 
         def update_all_tokens(self):
             tokens_list = SecurityLayer.AccessToken()
-            query = [{"dim":"apiuser", 'op':'==', 'val': self.get('username')}]
+            query = [{"dim":"username", 'op':'==', 'val': self.get('username')}]
             tokens_list.search(query_list=query)
             for t in tokens_list.found:
                 t.build_from_access(self)
                 try:
                     t.update()
                 except:
                     pass
@@ -310,21 +310,23 @@
             self.partners.append(partner_code)
             self.update()
         
         def auth(self):
             return self.verify_password()
             
         def verify_password(self):
+            print(self.to_dict())
+            stored_password = self.get("password")
             try:
                 self.load(self.get('username'))
             except:
                 query = [{"dim":"username", 'op':'==', 'val': self.get('username')}]
                 self.search(query_list=query)
                 self.set(id=self.found[0].get('_key'),data=self.found[0])
-            stored_password = self.get("password")
+            print(self.to_dict())
             self.id = self.get("_key")
             salt = stored_password[:64]
             stored_password = stored_password[64:]
             pwdhash = hashlib.pbkdf2_hmac('sha512', 
                                         self.get('password').encode('utf-8'), 
                                         salt.encode('ascii'), 
                                         100000)
```

