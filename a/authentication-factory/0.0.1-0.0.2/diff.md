# Comparing `tmp/authentication-factory-0.0.1.tar.gz` & `tmp/authentication-factory-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/authentication-factory-0.0.1.tar", last modified: Tue Jul 11 11:06:49 2023, max compression
+gzip compressed data, was "dist/authentication-factory-0.0.2.tar", last modified: Thu Jul 13 09:29:48 2023, max compression
```

## Comparing `authentication-factory-0.0.1.tar` & `authentication-factory-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-07-11 11:06:49.020786 authentication-factory-0.0.1/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3078 2023-07-11 10:56:28.000000 authentication-factory-0.0.1/.gitignore
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1117 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/LICENSE
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      134 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/MANIFEST.in
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3055 2023-07-11 11:06:49.020786 authentication-factory-0.0.1/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1387 2023-07-11 11:00:07.000000 authentication-factory-0.0.1/README.md
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-07-11 11:06:49.016786 authentication-factory-0.0.1/authentication_factory/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       45 2023-07-11 11:06:48.000000 authentication-factory-0.0.1/authentication_factory/.version
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/authentication_factory/__init__.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-07-11 11:06:49.020786 authentication-factory-0.0.1/authentication_factory/auth/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/authentication_factory/auth/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     8382 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/authentication_factory/auth/ms_oauth2.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      271 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/authentication_factory/auth_decorators.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     2269 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/authentication_factory/auth_factory.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-07-11 11:06:49.020786 authentication-factory-0.0.1/authentication_factory.egg-info/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     3055 2023-07-11 11:06:48.000000 authentication-factory-0.0.1/authentication_factory.egg-info/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      549 2023-07-11 11:06:48.000000 authentication-factory-0.0.1/authentication_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        1 2023-07-11 11:06:48.000000 authentication-factory-0.0.1/authentication_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      378 2023-07-11 11:06:48.000000 authentication-factory-0.0.1/authentication_factory.egg-info/requires.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       23 2023-07-11 11:06:48.000000 authentication-factory-0.0.1/authentication_factory.egg-info/top_level.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       67 2023-07-11 11:06:49.020786 authentication-factory-0.0.1/setup.cfg
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5567 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/setup.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     4258 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/streamlit-example.md
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       18 2023-07-11 10:57:32.000000 authentication-factory-0.0.1/version.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-07-13 09:29:48.501025 authentication-factory-0.0.2/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     1117 2023-07-11 11:14:32.000000 authentication-factory-0.0.2/LICENSE
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      134 2023-07-11 11:14:32.000000 authentication-factory-0.0.2/MANIFEST.in
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3055 2023-07-13 09:29:48.501025 authentication-factory-0.0.2/PKG-INFO
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     1387 2023-07-11 11:14:32.000000 authentication-factory-0.0.2/README.md
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-07-13 09:29:48.501025 authentication-factory-0.0.2/authentication_factory/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       45 2023-07-13 09:29:48.000000 authentication-factory-0.0.2/authentication_factory/.version
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2023-07-11 11:14:32.000000 authentication-factory-0.0.2/authentication_factory/__init__.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-07-13 09:29:48.501025 authentication-factory-0.0.2/authentication_factory/auth/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2023-07-11 11:14:32.000000 authentication-factory-0.0.2/authentication_factory/auth/__init__.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     8512 2023-07-13 09:29:25.000000 authentication-factory-0.0.2/authentication_factory/auth/ms_oauth2.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      271 2023-07-11 11:14:32.000000 authentication-factory-0.0.2/authentication_factory/auth_decorators.py
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3243 2023-07-13 09:29:25.000000 authentication-factory-0.0.2/authentication_factory/auth_factory.py
+drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-07-13 09:29:48.501025 authentication-factory-0.0.2/authentication_factory.egg-info/
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     3055 2023-07-13 09:29:48.000000 authentication-factory-0.0.2/authentication_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      506 2023-07-13 09:29:48.000000 authentication-factory-0.0.2/authentication_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)        1 2023-07-13 09:29:48.000000 authentication-factory-0.0.2/authentication_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)      182 2023-07-13 09:29:48.000000 authentication-factory-0.0.2/authentication_factory.egg-info/requires.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       23 2023-07-13 09:29:48.000000 authentication-factory-0.0.2/authentication_factory.egg-info/top_level.txt
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)       67 2023-07-13 09:29:48.501025 authentication-factory-0.0.2/setup.cfg
+-rw-rw-r--   0 ankit     (1001) ankit     (1001)     5440 2023-07-13 09:29:25.000000 authentication-factory-0.0.2/setup.py
```

### Comparing `authentication-factory-0.0.1/LICENSE` & `authentication-factory-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `authentication-factory-0.0.1/PKG-INFO` & `authentication-factory-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentication-factory
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implementation for Microsoft Oauth2 authentication
 Home-page: https://github.com/shrivastava-v-ankit/authentication-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/authentication-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/authentication-factory/issues
 Description: # authentication-factory
```

### Comparing `authentication-factory-0.0.1/README.md` & `authentication-factory-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `authentication-factory-0.0.1/authentication_factory/auth/ms_oauth2.py` & `authentication-factory-0.0.2/authentication_factory/auth/ms_oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,12 +196,14 @@
 
                 if "error" not in result:
                     id_token = self.verify(token=result.get("access_token"),
                                            client_id=client_id,
                                            tenant_id=tenant_id)
 
                 kwargs["id_token"] = id_token
+                kwargs["access_token"] = result["access_token"]
+                kwargs["refresh_token"] = result["refresh_token"]
 
                 result = f(*args, **kwargs)
                 return result
             return wrapper
         return decorator
```

### Comparing `authentication-factory-0.0.1/authentication_factory.egg-info/PKG-INFO` & `authentication-factory-0.0.2/authentication_factory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentication-factory
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implementation for Microsoft Oauth2 authentication
 Home-page: https://github.com/shrivastava-v-ankit/authentication-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/authentication-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/authentication-factory/issues
 Description: # authentication-factory
```

### Comparing `authentication-factory-0.0.1/setup.py` & `authentication-factory-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,43 +34,32 @@
 
 ROOT = os.path.dirname(os.path.abspath(__file__))
 VERSION_FILE = os.path.join(ROOT, __NAME__.replace("-", "_"), ".version")
 VERSION_RE = re.compile(r'''__version__ = ['"]([0-9.]+)['"]''')
 
 base = [
     # Python HTTP for Humans.
-    "requests==2.28.2",
+    "requests==2.31.0",
     # The Microsoft Authentication Library (MSAL) for Python library by supporting authentication of users with Microsoft Azure Active Directory accounts (AAD) and Microsoft Accounts (MSA) using industry standard OAuth2 and OpenID Connect.
-    "msal==1.20.0",
+    "msal==1.22.0",
     # JSON Web Token implementation in Python
-    "pyjwt==2.6.0",
+    "PyJWT==2.6.0",
+    # Cryptography is a package which provides cryptographic recipes and primitives to Python developers.
+    "cryptography==36.0.2",
+    # Python wrapper module around the OpenSSL library
+    "pyopenssl==22.0.0"
 ]
 
 dependencies = [
-    "Flask==2.2.3",
-    "Jinja2==3.0.0",
-    "MarkupSafe==2.1.2",
-    "WTForms==3.0.1",
-    "Werkzeug==2.2.3",
-    "click==8.1.3",
-    "importlib-metadata==6.4.1",
-    "itsdangerous==2.1.2",
-    "zipp==3.15.0",
-    "pyasn1==0.4.8",
-    "ecdsa==0.18.0",
-    "rsa==4.9",
-    "six==1.16.0",
-    "certifi==2022.12.7",
-    "charset-normalizer==2.0.12",
+    "certifi==2023.5.7",
+    "charset-normalizer==3.2.0",
     "idna==3.4",
-    "urllib3==1.26.15",
+    "urllib3==1.26.16",
     "cffi==1.15.1",
-    "cryptography==36.0.2",
-    "pycparser==2.21",
-    "blinker==1.6.2"
+    "pycparser==2.21"
 ]
 
 setups = []
 
 ir = (base + dependencies)
 requires = ir
```

