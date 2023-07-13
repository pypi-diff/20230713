# Comparing `tmp/giza_cli-0.0.1.tar.gz` & `tmp/giza_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_cli-0.0.1.tar", max compression
+gzip compressed data, was "giza_cli-0.0.2.tar", max compression
```

## Comparing `giza_cli-0.0.1.tar` & `giza_cli-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1074 2023-07-12 13:15:06.780504 giza_cli-0.0.1/LICENSE
--rw-r--r--   0        0        0     4276 2023-07-12 13:15:06.780504 giza_cli-0.0.1/README.md
--rw-r--r--   0        0        0       61 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/__init__.py
--rw-r--r--   0        0        0       77 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/__main__.py
--rw-r--r--   0        0        0     1048 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/callbacks.py
--rw-r--r--   0        0        0     1145 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/cli.py
--rw-r--r--   0        0        0     9651 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/client.py
--rw-r--r--   0        0        0        0 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/commands/__init__.py
--rw-r--r--   0        0        0     2126 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/commands/transpile.py
--rw-r--r--   0        0        0     5159 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/commands/users.py
--rw-r--r--   0        0        0      372 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/commands/version.py
--rw-r--r--   0        0        0      241 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/options.py
--rw-r--r--   0        0        0      107 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/schemas/token.py
--rw-r--r--   0        0        0      902 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/schemas/users.py
--rw-r--r--   0        0        0      771 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/utils/__init__.py
--rw-r--r--   0        0        0     1244 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/utils/decorators.py
--rw-r--r--   0        0        0     3568 2023-07-12 13:15:06.780504 giza_cli-0.0.1/giza/utils/echo.py
--rw-r--r--   0        0        0     1375 2023-07-12 13:15:06.784504 giza_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 giza_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-13 09:38:22.745132 giza_cli-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4276 2023-07-13 09:38:22.745132 giza_cli-0.0.2/README.md
+-rw-r--r--   0        0        0       61 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/__init__.py
+-rw-r--r--   0        0        0       77 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/__main__.py
+-rw-r--r--   0        0        0     1048 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/callbacks.py
+-rw-r--r--   0        0        0     1145 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/cli.py
+-rw-r--r--   0        0        0     9779 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/client.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/commands/__init__.py
+-rw-r--r--   0        0        0     2126 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/commands/transpile.py
+-rw-r--r--   0        0        0     5159 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/commands/users.py
+-rw-r--r--   0        0        0      372 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/commands/version.py
+-rw-r--r--   0        0        0      241 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/options.py
+-rw-r--r--   0        0        0      107 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/schemas/token.py
+-rw-r--r--   0        0        0      902 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/schemas/users.py
+-rw-r--r--   0        0        0      771 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/utils/__init__.py
+-rw-r--r--   0        0        0     1244 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/utils/decorators.py
+-rw-r--r--   0        0        0     3568 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/utils/echo.py
+-rw-r--r--   0        0        0     1375 2023-07-13 09:38:22.745132 giza_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 giza_cli-0.0.2/PKG-INFO
```

### Comparing `giza_cli-0.0.1/LICENSE` & `giza_cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/README.md` & `giza_cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/giza/callbacks.py` & `giza_cli-0.0.2/giza/callbacks.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/giza/cli.py` & `giza_cli-0.0.2/giza/cli.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/giza/client.py` & `giza_cli-0.0.2/giza/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,15 +231,19 @@
             user (users.UserCreate): information used to create a new user
 
         Returns:
             users.UserResponse: the created user information
         """
         response = self.session.post(
             f"{self.url}/{self.USERS_ENDPOINT}/",
-            json=user.dict(exclude_unset=True),
+            json={
+                "username": user.username,
+                "password": user.password.get_secret_value(),
+                "email": user.email,
+            },
         )
 
         response.raise_for_status()
         body = response.json()
         self._echo_debug(body, json=True)
         return users.UserResponse(**body)
```

### Comparing `giza_cli-0.0.1/giza/commands/transpile.py` & `giza_cli-0.0.2/giza/commands/transpile.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/giza/commands/users.py` & `giza_cli-0.0.2/giza/commands/users.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/giza/schemas/users.py` & `giza_cli-0.0.2/giza/schemas/users.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/giza/utils/__init__.py` & `giza_cli-0.0.2/giza/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/giza/utils/decorators.py` & `giza_cli-0.0.2/giza/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/giza/utils/echo.py` & `giza_cli-0.0.2/giza/utils/echo.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.1/pyproject.toml` & `giza_cli-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-cli"
-version = "0.0.1"
+version = "0.0.2"
 description = "CLI for interacting with Giza Platform"
 authors = ["Gonzalo Mellizo-Soto <gonzalo@gizatech.xyz>"]
 readme = "README.md"
 packages = [{include = "giza"}]
 
 [tool.poetry.scripts]
 giza = "giza.cli:entrypoint"
```

### Comparing `giza_cli-0.0.1/PKG-INFO` & `giza_cli-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI for interacting with Giza Platform
 Author: Gonzalo Mellizo-Soto
 Author-email: gonzalo@gizatech.xyz
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.0,<9.0.0)
```

