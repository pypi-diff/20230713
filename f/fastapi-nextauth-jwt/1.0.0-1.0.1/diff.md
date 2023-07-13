# Comparing `tmp/fastapi_nextauth_jwt-1.0.0.tar.gz` & `tmp/fastapi_nextauth_jwt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_nextauth_jwt-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_nextauth_jwt-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_nextauth_jwt-1.0.0.tar` & `fastapi_nextauth_jwt-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1002 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      741 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3089 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/.gitignore
--rw-r--r--   0        0        0     1069 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/LICENSE
--rw-r--r--   0        0        0      135 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/README.md
--rw-r--r--   0        0        0      563 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      222 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/__init__.py
--rw-r--r--   0        0        0      974 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/cookies.py
--rw-r--r--   0        0        0      938 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/csrf.py
--rw-r--r--   0        0        0      696 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/exceptions.py
--rw-r--r--   0        0        0     5422 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
--rw-r--r--   0        0        0      312 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/operations.py
--rw-r--r--   0        0        0      646 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/tests/fastapi/main.py
--rw-r--r--   0        0        0    17406 2023-07-13 19:24:34.767618 fastapi_nextauth_jwt-1.0.0/tests/fastapi/test_main.py
--rw-r--r--   0        0        0     1021 2023-07-13 19:24:34.767618 fastapi_nextauth_jwt-1.0.0/tests/unit/test_cookies.py
--rw-r--r--   0        0        0     1654 2023-07-13 19:24:34.767618 fastapi_nextauth_jwt-1.0.0/tests/unit/test_csrf.py
--rw-r--r--   0        0        0      503 2023-07-13 19:24:34.767618 fastapi_nextauth_jwt-1.0.0/tests/unit/test_operations.py
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      985 2023-07-13 19:58:45.841817 fastapi_nextauth_jwt-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      741 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3089 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1069 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1484 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/README.md
+-rw-r--r--   0        0        0      563 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/__init__.py
+-rw-r--r--   0        0        0      974 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/cookies.py
+-rw-r--r--   0        0        0      938 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/csrf.py
+-rw-r--r--   0        0        0      696 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/exceptions.py
+-rw-r--r--   0        0        0     5412 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
+-rw-r--r--   0        0        0      312 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/operations.py
+-rw-r--r--   0        0        0      646 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/fastapi/main.py
+-rw-r--r--   0        0        0    17406 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/fastapi/test_main.py
+-rw-r--r--   0        0        0     1021 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/unit/test_cookies.py
+-rw-r--r--   0        0        0     1654 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/unit/test_csrf.py
+-rw-r--r--   0        0        0      503 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/unit/test_operations.py
+-rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-1.0.1/PKG-INFO
```

### Comparing `fastapi_nextauth_jwt-1.0.0/.github/workflows/publish.yml` & `fastapi_nextauth_jwt-1.0.1/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 name: 'Run tests and publish fastapi-nextauth-jwt to pypi'
 
-on:
-  push:
-    branches:
-      - main
+on: workflow_dispatch
 
 jobs:
   test:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
```

### Comparing `fastapi_nextauth_jwt-1.0.0/.github/workflows/test.yml` & `fastapi_nextauth_jwt-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/.gitignore` & `fastapi_nextauth_jwt-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/LICENSE` & `fastapi_nextauth_jwt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/pyproject.toml` & `fastapi_nextauth_jwt-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/cookies.py` & `fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/csrf.py` & `fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/csrf.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/exceptions.py` & `fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py` & `fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                  hash_algorithm: Any = hashes.SHA256(),
                  csrf_prevention_enabled: bool = None,
                  csrf_methods: Set[str] = None):
         """
         Initializes a new instance of the NextAuthJWT class.
 
         Args:
-            secret (str, optional): The secret used for key derivation.
+            secret (str): The secret used for key derivation.
 
             cookie_name (str, optional): The name of the session cookie. Defaults to "__Secure-next-auth.session-token"
              if using secure cookies, otherwise "next-auth.session-token"
 
             secure_cookie (bool, optional): Indicates if the session cookie is a secure cookie. Defaults to True
              if NEXTAUTH_URL starts with https://. else False.
```

### Comparing `fastapi_nextauth_jwt-1.0.0/tests/fastapi/main.py` & `fastapi_nextauth_jwt-1.0.1/tests/fastapi/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/tests/fastapi/test_main.py` & `fastapi_nextauth_jwt-1.0.1/tests/fastapi/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/tests/unit/test_cookies.py` & `fastapi_nextauth_jwt-1.0.1/tests/unit/test_cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.0/tests/unit/test_csrf.py` & `fastapi_nextauth_jwt-1.0.1/tests/unit/test_csrf.py`

 * *Files identical despite different names*

