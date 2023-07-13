# Comparing `tmp/starlette-authlib-0.1.8.tar.gz` & `tmp/starlette-authlib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette-authlib-0.1.8.tar", last modified: Tue May 18 12:27:18 2021, max compression
+gzip compressed data, was "starlette-authlib-0.1.9.tar", max compression
```

## Comparing `starlette-authlib-0.1.8.tar` & `starlette-authlib-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      638 2021-05-18 12:18:58.854925 starlette-authlib-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-21 16:07:43.710712 starlette-authlib-0.1.8/starlette_authlib/__init__.py
--rw-r--r--   0        0        0     4601 2021-05-18 12:18:58.854925 starlette-authlib-0.1.8/starlette_authlib/middleware.py
--rw-r--r--   0        0        0      750 2021-05-18 12:27:18.333575 starlette-authlib-0.1.8/setup.py
--rw-r--r--   0        0        0      566 2021-05-18 12:27:18.333849 starlette-authlib-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2069 2022-05-14 11:20:09.930977 starlette-authlib-0.1.9/README.md
+-rw-r--r--   0        0        0      661 2022-05-14 11:20:09.930977 starlette-authlib-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-05-14 11:20:09.934977 starlette-authlib-0.1.9/starlette_authlib/__init__.py
+-rw-r--r--   0        0        0     4618 2022-05-14 11:20:09.934977 starlette-authlib-0.1.9/starlette_authlib/middleware.py
+-rw-r--r--   0        0        0     2872 2022-05-14 11:20:41.803635 starlette-authlib-0.1.9/setup.py
+-rw-r--r--   0        0        0     2816 2022-05-14 11:20:41.803920 starlette-authlib-0.1.9/PKG-INFO
```

### Comparing `starlette-authlib-0.1.8/pyproject.toml` & `starlette-authlib-0.1.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "starlette-authlib"
-version = "0.1.8"
+version = "0.1.9"
 description = "A drop-in replacement for Starlette session middleware, using authlib's jwt"
 authors = ["Alessandro Ogier <alessandro.ogier@gmail.com>"]
+readme = "README.md"
+repository = "https://github.com/aogier/starlette-authlib"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-authlib = ">=0.14.1,<0.16.0"
-uvicorn = "^0.13.4"
-starlette = "^0.14.2"
+authlib = "<1"
+uvicorn = "<0.18"
+starlette = "<0.21"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
-mypy = "^0.790"
+mypy = "^0.950"
 requests = "^2.25.1"
-black = "^20.8b1"
+black = "^22"
 autoflake = "^1.4"
 pytest-cov = "^2.11.0"
-wheel = "^0.34.2"
-twine = "^3.3.0"
 poetry-version = "^0.1.5"
 changelog-cli = "^0.7.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `starlette-authlib-0.1.8/starlette_authlib/middleware.py` & `starlette-authlib-0.1.9/starlette_authlib/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author: Alessandro Ogier <alessandro.ogier@gmail.com>
 """
 import time
 import typing
 from collections import namedtuple
 
 from authlib.jose import jwt
-from authlib.jose.errors import BadSignatureError, ExpiredTokenError, DecodeError
+from authlib.jose.errors import BadSignatureError, DecodeError, ExpiredTokenError
 from starlette.config import Config
 from starlette.datastructures import MutableHeaders, Secret
 from starlette.requests import HTTPConnection
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
 
 config = Config(".env")
 
@@ -24,15 +24,15 @@
         self,
         app: ASGIApp,
         secret_key: typing.Union[str, Secret, SecretKey],
         session_cookie: str = "session",
         max_age: int = 14 * 24 * 60 * 60,  # 14 days, in seconds
         same_site: str = "lax",
         https_only: bool = False,
-        domain: str = config("DOMAIN", cast=str, default=None),
+        domain: typing.Optional[str] = config("DOMAIN", cast=str, default=None),
         jwt_alg: str = config("JWT_ALG", cast=str, default="HS256"),
     ) -> None:
         self.app = app
 
         self.jwt_header = {"alg": jwt_alg}
         if not isinstance(secret_key, SecretKey):
             self.jwt_secret = SecretKey(Secret(str(secret_key)), None)
```

