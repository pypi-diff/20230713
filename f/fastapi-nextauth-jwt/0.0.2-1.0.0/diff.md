# Comparing `tmp/fastapi_nextauth_jwt-0.0.2.tar.gz` & `tmp/fastapi_nextauth_jwt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_nextauth_jwt-0.0.2.tar", last modified: Fri May  5 14:11:28 2023, max compression
+gzip compressed data, was "fastapi_nextauth_jwt-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_nextauth_jwt-0.0.2.tar` & `fastapi_nextauth_jwt-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,18 @@
--rw-r--r--   0        0        0      535 2023-05-05 14:11:22.759380 fastapi_nextauth_jwt-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3077 2023-05-05 14:11:22.759380 fastapi_nextauth_jwt-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2023-05-05 14:11:22.759380 fastapi_nextauth_jwt-0.0.2/LICENSE
--rw-r--r--   0        0        0      135 2023-05-05 14:11:22.759380 fastapi_nextauth_jwt-0.0.2/README.md
--rw-r--r--   0        0        0     5637 2023-05-05 14:11:22.759380 fastapi_nextauth_jwt-0.0.2/fastapi_nextauth_jwt.py
--rw-r--r--   0        0        0      467 2023-05-05 14:11:22.759380 fastapi_nextauth_jwt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      741 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3089 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1069 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/LICENSE
+-rw-r--r--   0        0        0      135 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/README.md
+-rw-r--r--   0        0        0      563 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/__init__.py
+-rw-r--r--   0        0        0      974 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/cookies.py
+-rw-r--r--   0        0        0      938 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/csrf.py
+-rw-r--r--   0        0        0      696 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/exceptions.py
+-rw-r--r--   0        0        0     5422 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
+-rw-r--r--   0        0        0      312 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/src/fastapi_nextauth_jwt/operations.py
+-rw-r--r--   0        0        0      646 2023-07-13 19:24:34.763618 fastapi_nextauth_jwt-1.0.0/tests/fastapi/main.py
+-rw-r--r--   0        0        0    17406 2023-07-13 19:24:34.767618 fastapi_nextauth_jwt-1.0.0/tests/fastapi/test_main.py
+-rw-r--r--   0        0        0     1021 2023-07-13 19:24:34.767618 fastapi_nextauth_jwt-1.0.0/tests/unit/test_cookies.py
+-rw-r--r--   0        0        0     1654 2023-07-13 19:24:34.767618 fastapi_nextauth_jwt-1.0.0/tests/unit/test_csrf.py
+-rw-r--r--   0        0        0      503 2023-07-13 19:24:34.767618 fastapi_nextauth_jwt-1.0.0/tests/unit/test_operations.py
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-1.0.0/PKG-INFO
```

### Comparing `fastapi_nextauth_jwt-0.0.2/.gitignore` & `fastapi_nextauth_jwt-1.0.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
+/pytest.xml
```

### Comparing `fastapi_nextauth_jwt-0.0.2/LICENSE` & `fastapi_nextauth_jwt-1.0.0/LICENSE`

 * *Files identical despite different names*

