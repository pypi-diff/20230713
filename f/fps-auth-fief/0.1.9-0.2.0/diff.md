# Comparing `tmp/fps_auth_fief-0.1.9.tar.gz` & `tmp/fps_auth_fief-0.2.0.tar.gz`

## Comparing `fps_auth_fief-0.1.9.tar` & `fps_auth_fief-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/config.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/main.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/COPYING.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/COPYING.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fps_auth_fief-0.2.0/PKG-INFO
```

### Comparing `fps_auth_fief-0.1.9/fps_auth_fief/backend.py` & `fps_auth_fief-0.2.0/fps_auth_fief/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 from fief_client import FiefAccessTokenInfo, FiefAsync, FiefUserInfo
 from fief_client.integrations.fastapi import FiefAuth
 from jupyverse_api.auth import User
 
 from .config import _AuthFiefConfig
 
 
-class CustomFiefAuth(FiefAuth):
-    client: FiefAsync
-
-    async def get_unauthorized_response(self, request: Request, response: Response):
-        redirect_uri = str(request.url_for("auth_callback"))
-        auth_url = await self.client.auth_url(redirect_uri, scope=["openid"])
-        raise HTTPException(
-            status_code=status.HTTP_307_TEMPORARY_REDIRECT,
-            headers={"Location": auth_url},
-        )
-
-
 @dataclass
 class Res:
     fief: FiefAsync
     session_cookie_name: str
-    auth: CustomFiefAuth
+    auth: FiefAuth
     current_user: Any
     update_user: Any
     websocket_auth: Any
 
 
 def get_backend(auth_fief_config: _AuthFiefConfig) -> Res:
+    class CustomFiefAuth(FiefAuth):
+        client: FiefAsync
+
+        async def get_unauthorized_response(self, request: Request, response: Response):
+            if auth_fief_config.callback_url:
+                redirect_uri = auth_fief_config.callback_url
+            else:
+                redirect_uri = str(request.url_for("auth_callback"))
+            auth_url = await self.client.auth_url(redirect_uri, scope=["openid", "offline_access"])
+            raise HTTPException(
+                status_code=status.HTTP_307_TEMPORARY_REDIRECT,
+                headers={"Location": auth_url},
+            )
+
     fief = FiefAsync(
         auth_fief_config.base_url,
         auth_fief_config.client_id,
         auth_fief_config.client_secret,
     )
 
     session_cookie_name = "fps_auth_fief_user_session"
```

### Comparing `fps_auth_fief-0.1.9/fps_auth_fief/main.py` & `fps_auth_fief-0.2.0/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.9/.gitignore` & `fps_auth_fief-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.9/COPYING.md` & `fps_auth_fief-0.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.9/pyproject.toml` & `fps_auth_fief-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.9/PKG-INFO` & `fps_auth_fief-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_auth_fief
-Version: 0.1.9
+Version: 0.2.0
 Summary: An FPS plugin for the authentication API, using Fief
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

