# Comparing `tmp/fief-client-0.8.0.tar.gz` & `tmp/fief-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fief-client-0.8.0.tar", last modified: Wed Apr 13 12:40:42 2022, max compression
+gzip compressed data, was "fief-client-0.9.0.tar", last modified: Thu May 12 14:34:45 2022, max compression
```

## Comparing `fief-client-0.8.0.tar` & `fief-client-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      229 2022-04-13 12:40:17.348378 fief-client-0.8.0/.editorconfig
--rw-r--r--   0        0        0      604 2022-04-13 12:40:17.348378 fief-client-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      224 2022-04-13 12:40:17.348378 fief-client-0.8.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      143 2022-04-13 12:40:17.348378 fief-client-0.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1465 2022-04-13 12:40:17.348378 fief-client-0.8.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2334 2022-04-13 12:40:17.348378 fief-client-0.8.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1295 2022-04-13 12:40:17.348378 fief-client-0.8.0/.gitignore
--rw-r--r--   0        0        0     1072 2022-04-13 12:40:17.348378 fief-client-0.8.0/LICENSE
--rw-r--r--   0        0        0     1087 2022-04-13 12:40:17.348378 fief-client-0.8.0/README.md
--rw-r--r--   0        0        0      519 2022-04-13 12:40:17.348378 fief-client-0.8.0/fief_client/__init__.py
--rw-r--r--   0        0        0    15988 2022-04-13 12:40:17.352378 fief-client-0.8.0/fief_client/client.py
--rw-r--r--   0        0        0      529 2022-04-13 12:40:17.352378 fief-client-0.8.0/fief_client/crypto.py
--rw-r--r--   0        0        0        0 2022-04-13 12:40:17.352378 fief-client-0.8.0/fief_client/integrations/__init__.py
--rw-r--r--   0        0        0     3164 2022-04-13 12:40:17.352378 fief-client-0.8.0/fief_client/integrations/fastapi.py
--rw-r--r--   0        0        0     2192 2022-04-13 12:40:17.352378 fief-client-0.8.0/fief_client/integrations/flask.py
--rw-r--r--   0        0        0        0 2022-04-13 12:40:17.352378 fief-client-0.8.0/fief_client/py.typed
--rw-r--r--   0        0        0      329 2022-04-13 12:40:17.352378 fief-client-0.8.0/justfile
--rw-r--r--   0        0        0     1429 2022-04-13 12:40:17.352378 fief-client-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      190 2022-04-13 12:40:17.352378 fief-client-0.8.0/setup.cfg
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 fief-client-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      229 2022-05-12 14:34:14.615247 fief-client-0.9.0/.editorconfig
+-rw-r--r--   0        0        0      604 2022-05-12 14:34:14.615247 fief-client-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      224 2022-05-12 14:34:14.615247 fief-client-0.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      143 2022-05-12 14:34:14.615247 fief-client-0.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1465 2022-05-12 14:34:14.615247 fief-client-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2334 2022-05-12 14:34:14.615247 fief-client-0.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1295 2022-05-12 14:34:14.615247 fief-client-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1072 2022-05-12 14:34:14.615247 fief-client-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1087 2022-05-12 14:34:14.615247 fief-client-0.9.0/README.md
+-rw-r--r--   0        0        0      519 2022-05-12 14:34:14.615247 fief-client-0.9.0/fief_client/__init__.py
+-rw-r--r--   0        0        0    16785 2022-05-12 14:34:14.615247 fief-client-0.9.0/fief_client/client.py
+-rw-r--r--   0        0        0      529 2022-05-12 14:34:14.615247 fief-client-0.9.0/fief_client/crypto.py
+-rw-r--r--   0        0        0        0 2022-05-12 14:34:14.615247 fief-client-0.9.0/fief_client/integrations/__init__.py
+-rw-r--r--   0        0        0     3164 2022-05-12 14:34:14.615247 fief-client-0.9.0/fief_client/integrations/fastapi.py
+-rw-r--r--   0        0        0     2192 2022-05-12 14:34:14.615247 fief-client-0.9.0/fief_client/integrations/flask.py
+-rw-r--r--   0        0        0        0 2022-05-12 14:34:14.615247 fief-client-0.9.0/fief_client/py.typed
+-rw-r--r--   0        0        0      329 2022-05-12 14:34:14.615247 fief-client-0.9.0/justfile
+-rw-r--r--   0        0        0     1429 2022-05-12 14:34:14.615247 fief-client-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      190 2022-05-12 14:34:14.615247 fief-client-0.9.0/setup.cfg
+-rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 fief-client-0.9.0/PKG-INFO
```

### Comparing `fief-client-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `fief-client-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/.github/workflows/build.yml` & `fief-client-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/.github/workflows/codeql-analysis.yml` & `fief-client-0.9.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/.gitignore` & `fief-client-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/LICENSE` & `fief-client-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/README.md` & `fief-client-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/fief_client/__init__.py` & `fief-client-0.9.0/fief_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     FiefAccessTokenMissingScope,
     FiefAsync,
     FiefError,
     FiefIdTokenInvalid,
     FiefTokenResponse,
 )
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 __all__ = [
     "Fief",
     "FiefAsync",
     "FiefTokenResponse",
     "FiefAccessTokenInfo",
     "FiefError",
```

### Comparing `fief-client-0.8.0/fief_client/client.py` & `fief-client-0.9.0/fief_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,27 @@
     def __init__(
         self,
         base_url: str,
         client_id: str,
         client_secret: str,
         *,
         encryption_key: Optional[str] = None,
+        host: Optional[str] = None,
     ) -> None:
         self.base_url = base_url
         self.client_id = client_id
         self.client_secret = client_secret
         if encryption_key is not None:
             self.encryption_key = jwk.JWK.from_json(encryption_key)
+        self.host = host
+
+    def _get_endpoint_url(
+        self, openid_configuration: Dict[str, Any], field: str
+    ) -> str:
+        return openid_configuration[field]
 
     def _auth_url(
         self,
         openid_configuration: Dict[str, Any],
         redirect_uri: str,
         *,
         state: str = None,
@@ -102,15 +109,17 @@
         if code_challenge is not None and code_challenge_method is not None:
             params["code_challenge"] = code_challenge
             params["code_challenge_method"] = code_challenge_method
 
         if extras_params is not None:
             params = {**params, **extras_params}
 
-        authorization_endpoint = openid_configuration["authorization_endpoint"]
+        authorization_endpoint = self._get_endpoint_url(
+            openid_configuration, "authorization_endpoint"
+        )
         return f"{authorization_endpoint}?{urlencode(params)}"
 
     def _validate_access_token(
         self,
         access_token: str,
         jwks: jwk.JWKSet,
         *,
@@ -266,15 +275,17 @@
             access_token=token_response.get("access_token"),
         )
         return token_response, userinfo
 
     def auth_refresh_token(
         self, refresh_token: str, *, scope: Optional[List[str]] = None
     ) -> Tuple[FiefTokenResponse, Dict[str, Any]]:
-        token_endpoint = self._get_openid_configuration()["token_endpoint"]
+        token_endpoint = self._get_endpoint_url(
+            self._get_openid_configuration(), "token_endpoint"
+        )
         with self._get_httpx_client() as client:
             request = self._get_auth_refresh_token_request(
                 client,
                 endpoint=token_endpoint,
                 refresh_token=refresh_token,
                 scope=scope,
             )
@@ -296,15 +307,17 @@
     ) -> FiefAccessTokenInfo:
         jwks = self._get_jwks()
         return self._validate_access_token(
             access_token, jwks, required_scope=required_scope
         )
 
     def userinfo(self, access_token: str) -> Dict[str, Any]:
-        userinfo_endpoint = self._get_openid_configuration()["userinfo_endpoint"]
+        userinfo_endpoint = self._get_endpoint_url(
+            self._get_openid_configuration(), "userinfo_endpoint"
+        )
         with self._get_httpx_client() as client:
             request = self._get_userinfo_request(
                 client, endpoint=userinfo_endpoint, access_token=access_token
             )
             response = client.send(request)
 
             response.raise_for_status()
@@ -313,15 +326,19 @@
 
     def logout_url(self, redirect_uri: str) -> str:
         params = {"redirect_uri": redirect_uri}
         return f"{self.base_url}/logout?{urlencode(params)}"
 
     @contextlib.contextmanager
     def _get_httpx_client(self):
-        with httpx.Client(base_url=self.base_url) as client:
+        headers = {}
+        if self.host is not None:
+            headers["Host"] = self.host
+
+        with httpx.Client(base_url=self.base_url, headers=headers) as client:
             yield client
 
     def _get_openid_configuration(self) -> Dict[str, Any]:
         if self._openid_configuration is not None:
             return self._openid_configuration
 
         with self._get_httpx_client() as client:
@@ -331,24 +348,26 @@
             self._openid_configuration = json
             return json
 
     def _get_jwks(self) -> jwk.JWKSet:
         if self._jwks is not None:
             return self._jwks
 
-        jwks_uri = self._get_openid_configuration()["jwks_uri"]
+        jwks_uri = self._get_endpoint_url(self._get_openid_configuration(), "jwks_uri")
         with self._get_httpx_client() as client:
             response = client.get(jwks_uri)
             self._jwks = jwk.JWKSet.from_json(response.text)
             return self._jwks
 
     def _auth_exchange_token(
         self, code: str, redirect_uri: str, *, code_verifier: Optional[str] = None
     ) -> FiefTokenResponse:
-        token_endpoint = self._get_openid_configuration()["token_endpoint"]
+        token_endpoint = self._get_endpoint_url(
+            self._get_openid_configuration(), "token_endpoint"
+        )
         with self._get_httpx_client() as client:
             request = self._get_auth_exchange_token_request(
                 client,
                 endpoint=token_endpoint,
                 code=code,
                 redirect_uri=redirect_uri,
                 code_verifier=code_verifier,
@@ -396,15 +415,17 @@
             access_token=token_response.get("access_token"),
         )
         return token_response, userinfo
 
     async def auth_refresh_token(
         self, refresh_token: str, *, scope: Optional[List[str]] = None
     ) -> Tuple[FiefTokenResponse, Dict[str, Any]]:
-        token_endpoint = (await self._get_openid_configuration())["token_endpoint"]
+        token_endpoint = self._get_endpoint_url(
+            await self._get_openid_configuration(), "token_endpoint"
+        )
         async with self._get_httpx_client() as client:
             request = self._get_auth_refresh_token_request(
                 client,
                 endpoint=token_endpoint,
                 refresh_token=refresh_token,
                 scope=scope,
             )
@@ -427,17 +448,17 @@
     ) -> FiefAccessTokenInfo:
         jwks = await self._get_jwks()
         return self._validate_access_token(
             access_token, jwks, required_scope=required_scope
         )
 
     async def userinfo(self, access_token: str) -> Dict[str, Any]:
-        userinfo_endpoint = (await self._get_openid_configuration())[
-            "userinfo_endpoint"
-        ]
+        userinfo_endpoint = self._get_endpoint_url(
+            await self._get_openid_configuration(), "userinfo_endpoint"
+        )
         async with self._get_httpx_client() as client:
             request = self._get_userinfo_request(
                 client, endpoint=userinfo_endpoint, access_token=access_token
             )
             response = await client.send(request)
 
             response.raise_for_status()
@@ -446,15 +467,19 @@
 
     async def logout_url(self, redirect_uri: str) -> str:
         params = {"redirect_uri": redirect_uri}
         return f"{self.base_url}/logout?{urlencode(params)}"
 
     @contextlib.asynccontextmanager
     async def _get_httpx_client(self):
-        async with httpx.AsyncClient(base_url=self.base_url) as client:
+        headers = {}
+        if self.host is not None:
+            headers["Host"] = self.host
+
+        async with httpx.AsyncClient(base_url=self.base_url, headers=headers) as client:
             yield client
 
     async def _get_openid_configuration(self) -> Dict[str, Any]:
         if self._openid_configuration is not None:
             return self._openid_configuration
 
         async with self._get_httpx_client() as client:
@@ -464,24 +489,28 @@
             self._openid_configuration = json
             return json
 
     async def _get_jwks(self) -> jwk.JWKSet:
         if self._jwks is not None:
             return self._jwks
 
-        jwks_uri = (await self._get_openid_configuration())["jwks_uri"]
+        jwks_uri = self._get_endpoint_url(
+            await self._get_openid_configuration(), "jwks_uri"
+        )
         async with self._get_httpx_client() as client:
             response = await client.get(jwks_uri)
             self._jwks = jwk.JWKSet.from_json(response.text)
             return self._jwks
 
     async def _auth_exchange_token(
         self, code: str, redirect_uri: str, *, code_verifier: Optional[str] = None
     ) -> FiefTokenResponse:
-        token_endpoint = (await self._get_openid_configuration())["token_endpoint"]
+        token_endpoint = self._get_endpoint_url(
+            await self._get_openid_configuration(), "token_endpoint"
+        )
         async with self._get_httpx_client() as client:
             request = self._get_auth_exchange_token_request(
                 client,
                 endpoint=token_endpoint,
                 code=code,
                 redirect_uri=redirect_uri,
                 code_verifier=code_verifier,
```

### Comparing `fief-client-0.8.0/fief_client/crypto.py` & `fief-client-0.9.0/fief_client/crypto.py`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/fief_client/integrations/fastapi.py` & `fief-client-0.9.0/fief_client/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/fief_client/integrations/flask.py` & `fief-client-0.9.0/fief_client/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `fief-client-0.8.0/pyproject.toml` & `fief-client-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
     "httpx >=0.21.3,<0.23.0",
-    "jwcrypto ==1.0",
+    "jwcrypto ==1.2",
     "typing-extensions >=4.0.1; python_version < '3.8'",
 ]
 
 [project.optional-dependencies]
 dev = [
   "black",
   "bumpversion",
```

### Comparing `fief-client-0.8.0/PKG-INFO` & `fief-client-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fief-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Fief Client for Python
 Author-email: François Voron <contact@fief.dev>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: httpx >=0.21.3,<0.23.0
-Requires-Dist: jwcrypto ==1.0
+Requires-Dist: jwcrypto ==1.2
 Requires-Dist: typing-extensions >=4.0.1; python_version < '3.8'
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: coverage[toml] ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: greenlet ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
```

