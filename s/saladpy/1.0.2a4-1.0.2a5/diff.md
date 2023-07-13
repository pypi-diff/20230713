# Comparing `tmp/saladpy-1.0.2a4.tar.gz` & `tmp/saladpy-1.0.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saladpy-1.0.2a4.tar", last modified: Sun Jul  9 14:38:28 2023, max compression
+gzip compressed data, was "saladpy-1.0.2a5.tar", last modified: Thu Jul 13 09:45:32 2023, max compression
```

## Comparing `saladpy-1.0.2a4.tar` & `saladpy-1.0.2a5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/saladpy/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/saladpy/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/User.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/saladpy/methods/types/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/types/BaseClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/types/UserTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/saladpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:45:32.442062 saladpy-1.0.2a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-13 09:45:32.442062 saladpy-1.0.2a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:45:32.438062 saladpy-1.0.2a5/saladpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/saladpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/saladpy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/saladpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:45:32.438062 saladpy-1.0.2a5/saladpy/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/saladpy/methods/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/saladpy/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:45:32.438062 saladpy-1.0.2a5/saladpy/methods/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/saladpy/methods/types/BaseClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/saladpy/methods/types/UserTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/saladpy/methods/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:45:32.438062 saladpy-1.0.2a5/saladpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-13 09:45:32.000000 saladpy-1.0.2a5/saladpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-13 09:45:32.000000 saladpy-1.0.2a5/saladpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:45:32.000000 saladpy-1.0.2a5/saladpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 09:45:32.000000 saladpy-1.0.2a5/saladpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 09:45:32.000000 saladpy-1.0.2a5/saladpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:45:32.442062 saladpy-1.0.2a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 09:45:22.000000 saladpy-1.0.2a5/setup.py
```

### Comparing `saladpy-1.0.2a4/LICENSE` & `saladpy-1.0.2a5/LICENSE`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a4/PKG-INFO` & `saladpy-1.0.2a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saladpy
-Version: 1.0.2a4
+Version: 1.0.2a5
 Summary: A Python wrapper for the Salad Web API
 Home-page: https://github.com/Coddo-Python/SaladPy
 Author: Coddo-Python
 Author-email: Coddo <coddobusiness@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015-present Coddo-Python
```

### Comparing `saladpy-1.0.2a4/README.md` & `saladpy-1.0.2a5/README.md`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a4/pyproject.toml` & `saladpy-1.0.2a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saladpy"
-version = "1.0.2-a.4"
+version = "1.0.2-a.5"
 description = "A Python wrapper for the Salad Web API"
 readme = "README.md"
 authors = [{ name = "Coddo", email = "coddobusiness@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `saladpy-1.0.2a4/saladpy/client.py` & `saladpy-1.0.2a5/saladpy/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,17 @@
                     if self.cachePath.stat().st_size > 0:  # File is not empty
                         self.http.cookie_jar.load(self.cachePath)
                         self.cached = True
                     
     @property
     def cookies(self):
         return {cookie.key: cookie.value for cookie in list(self.http.cookie_jar) }
+    
+    async def clear_cookies(self):
+        self.http.cookie_jar.clear()
                             
     async def close(self):
         """
         Closes aiohttp `ClientSession` safely
         Using any methods after calling `close` will not work
         """
         await self.http.close()
@@ -131,33 +134,31 @@
             try:
                 assert r.status == 200
             except AssertionError:
                 if (
                     "try refresh token" in text
                 ):  # DO NOT convert to JSON as it's not always guaranteed to be JSON
                     # Refresh token
-                    print("Token expired, refreshing...")
-                    await self.refresh_token()
+                    await self.refresh_token(**kwargs)
+                    return await self._req(api_url, method, endpoint, params, token, *args, **kwargs)
                 else:
                     return r.status
             else:
                 return text
 
-    async def refresh_token(self):
-        #TODO: Test refresh token
-        self.temp_cookie_backup = self.cookies
-        cookies = {"sRefreshToken": self.cookies["sRefreshToken"], "sIdRefreshToken": self.cookies["sIdRefreshToken"]}
-        self.http.cookie_jar.clear()
-        async with self.http.post(f"{self.AUTH_API_URL}session/refresh", cookies=cookies) as r:
-            print(r.status)
+    async def refresh_token(self, **kwargs):
+        headers = {
+            'rid': 'session'
+        }
+        async with self.http.post(f"{self.AUTH_API_URL}session/refresh", headers=headers, **kwargs) as r:
             text = await r.text()
-            print(text)
             if r.status == 200:
                 self.http.cookie_jar.update_cookies(r.cookies)
-                self.http.cookie_jar.save(self.cachePath)
+                if self.cachePath is not None:
+                    self.http.cookie_jar.save(self.cachePath)
 
     async def _get(self, api_url: str, endpoint: str, params: Optional[dict] = None, **kwargs):
         resp = await self._req(api_url, "GET", endpoint, params, **kwargs)
         if resp == 404:
             return resp
         return json.loads(resp)
```

### Comparing `saladpy-1.0.2a4/saladpy/methods/User.py` & `saladpy-1.0.2a5/saladpy/methods/User.py`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a4/saladpy/methods/types/BaseClient.py` & `saladpy-1.0.2a5/saladpy/methods/types/BaseClient.py`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a4/saladpy/methods/types/UserTypes.py` & `saladpy-1.0.2a5/saladpy/methods/types/UserTypes.py`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a4/saladpy.egg-info/PKG-INFO` & `saladpy-1.0.2a5/saladpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saladpy
-Version: 1.0.2a4
+Version: 1.0.2a5
 Summary: A Python wrapper for the Salad Web API
 Home-page: https://github.com/Coddo-Python/SaladPy
 Author: Coddo-Python
 Author-email: Coddo <coddobusiness@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015-present Coddo-Python
```

### Comparing `saladpy-1.0.2a4/setup.py` & `saladpy-1.0.2a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     author='Coddo-Python',
     url='https://github.com/Coddo-Python/SaladPy',
     project_urls={
         'Github': 'https://github.com/Coddo-Python/SaladPy',
         'Issue tracker': 'https://github.com/Coddo-Python/SaladPy/issues',
         'Docs': 'https://saladpy.gitbook.io/saladpy-docs/'
     },
-    version="1.0.2-a.4",
+    version="1.0.2-a.5",
     license='MIT',
     description='A Python wrapper for the Salad Web API',
     long_description=readme,
     packages=["saladpy", "saladpy.methods", "saladpy.methods.types"],
     install_requires=requirements,
     python_requires='>=3.8.0',
     classifiers=[
```

