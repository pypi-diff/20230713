# Comparing `tmp/mysql-mimic-2.2.5.tar.gz` & `tmp/mysql-mimic-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.2.5.tar", last modified: Tue Jun 27 18:47:36 2023, max compression
+gzip compressed data, was "mysql-mimic-2.2.6.tar", last modified: Wed Jul 12 22:47:51 2023, max compression
```

## Comparing `mysql-mimic-2.2.5.tar` & `mysql-mimic-2.2.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:47:36.082422 mysql-mimic-2.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-27 18:47:36.078422 mysql-mimic-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:47:36.078422 mysql-mimic-2.2.5/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:47:36.078422 mysql-mimic-2.2.5/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:47:36.082422 mysql-mimic-2.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:47:36.078422 mysql-mimic-2.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28686 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:47:51.084466 mysql-mimic-2.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-12 22:47:51.084466 mysql-mimic-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:47:51.080466 mysql-mimic-2.2.6/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:47:51.080466 mysql-mimic-2.2.6/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:47:51.084466 mysql-mimic-2.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:47:51.084466 mysql-mimic-2.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28686 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_version.py
```

### Comparing `mysql-mimic-2.2.5/LICENSE` & `mysql-mimic-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/PKG-INFO` & `mysql-mimic-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.5
+Version: 2.2.6
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.5/README.md` & `mysql-mimic-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/auth.py` & `mysql-mimic-2.2.6/mysql_mimic/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 
     def __init__(self, service: str, realm: str) -> None:
         self.service = service
         self.realm = realm
 
     async def auth(self, auth_info: Optional[AuthInfo] = None) -> AuthState:
         import gssapi
+        from gssapi.exceptions import GSSError
 
         # Fast authentication not supported
         if not auth_info:
             yield b""
 
         auth_info = (
             yield len(self.service).to_bytes(2, "little")
@@ -203,27 +204,23 @@
         )
 
         server_creds = gssapi.Credentials(
             usage="accept", name=gssapi.Name(f"{self.service}@{self.realm}")
         )
         server_ctx = gssapi.SecurityContext(usage="accept", creds=server_creds)
 
-        client_name = gssapi.Name(f"{auth_info.username}@{self.realm}").canonicalize(
-            gssapi.MechType.kerberos
-        )
-        client_token = auth_info.data
-
-        server_token = server_ctx.step(client_token)
-
-        if server_ctx.initiator_name == client_name:
-            if gssapi.RequirementFlag.mutual_authentication in server_ctx.actual_flags:
-                auth_info = yield server_token
-            yield Success(auth_info.username)
-        else:
-            yield Forbidden()
+        try:
+            server_ctx.step(auth_info.data)
+        except GSSError as e:
+            yield Forbidden(str(e))
+
+        username = str(server_ctx.initiator_name).split("@", 1)[0]
+        if auth_info.username and auth_info.username != username:
+            yield Forbidden("Given username different than kerberos client")
+        yield Success(username)
 
 
 class NoLoginAuthPlugin(AuthPlugin):
     """
     Standard plugin that prevents all clients from direct login.
 
     This is useful for user accounts that can only be accessed by proxy authentication.
```

### Comparing `mysql-mimic-2.2.5/mysql_mimic/charset.py` & `mysql-mimic-2.2.6/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/connection.py` & `mysql-mimic-2.2.6/mysql_mimic/connection.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/constants.py` & `mysql-mimic-2.2.6/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/errors.py` & `mysql-mimic-2.2.6/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/intercept.py` & `mysql-mimic-2.2.6/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/packets.py` & `mysql-mimic-2.2.6/mysql_mimic/packets.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/results.py` & `mysql-mimic-2.2.6/mysql_mimic/results.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/schema.py` & `mysql-mimic-2.2.6/mysql_mimic/schema.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/server.py` & `mysql-mimic-2.2.6/mysql_mimic/server.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/session.py` & `mysql-mimic-2.2.6/mysql_mimic/session.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/stream.py` & `mysql-mimic-2.2.6/mysql_mimic/stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/types.py` & `mysql-mimic-2.2.6/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/utils.py` & `mysql-mimic-2.2.6/mysql_mimic/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic/variables.py` & `mysql-mimic-2.2.6/mysql_mimic/variables.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.2.6/mysql_mimic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.5
+Version: 2.2.6
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.5/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.2.6/mysql_mimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/setup.py` & `mysql-mimic-2.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/tests/test_auth.py` & `mysql-mimic-2.2.6/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/tests/test_query.py` & `mysql-mimic-2.2.6/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/tests/test_ssl.py` & `mysql-mimic-2.2.6/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/tests/test_stream.py` & `mysql-mimic-2.2.6/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/tests/test_types.py` & `mysql-mimic-2.2.6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.5/tests/test_variables.py` & `mysql-mimic-2.2.6/tests/test_variables.py`

 * *Files identical despite different names*

