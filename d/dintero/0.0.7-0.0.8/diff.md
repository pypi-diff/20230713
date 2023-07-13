# Comparing `tmp/dintero-0.0.7.tar.gz` & `tmp/dintero-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dintero-0.0.7.tar", last modified: Thu Jul 13 19:32:29 2023, max compression
+gzip compressed data, was "dintero-0.0.8.tar", last modified: Thu Jul 13 19:42:31 2023, max compression
```

## Comparing `dintero-0.0.7.tar` & `dintero-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-13 19:32:27.000000 dintero-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 19:32:27.000000 dintero-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-13 19:32:29.304495 dintero-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-13 19:32:27.000000 dintero-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/dintero/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/dintero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-13 19:32:27.000000 dintero-0.0.7/examples/create_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 19:32:27.000000 dintero-0.0.7/examples/manage_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 19:32:27.000000 dintero-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 19:32:29.304495 dintero-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-13 19:32:27.000000 dintero-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:27.000000 dintero-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 19:32:27.000000 dintero-0.0.7/tests/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-13 19:32:27.000000 dintero-0.0.7/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 19:32:27.000000 dintero-0.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:42:31.325761 dintero-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-13 19:42:29.000000 dintero-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 19:42:29.000000 dintero-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-13 19:42:31.325761 dintero-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 19:42:29.000000 dintero-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:42:31.325761 dintero-0.0.8/dintero/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 19:42:29.000000 dintero-0.0.8/dintero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-13 19:42:29.000000 dintero-0.0.8/dintero/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 19:42:29.000000 dintero-0.0.8/dintero/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-13 19:42:29.000000 dintero-0.0.8/dintero/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-13 19:42:29.000000 dintero-0.0.8/dintero/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 19:42:29.000000 dintero-0.0.8/dintero/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:42:31.325761 dintero-0.0.8/dintero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-13 19:42:31.000000 dintero-0.0.8/dintero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-13 19:42:31.000000 dintero-0.0.8/dintero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:42:31.000000 dintero-0.0.8/dintero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:42:31.000000 dintero-0.0.8/dintero.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 19:42:31.000000 dintero-0.0.8/dintero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 19:42:31.000000 dintero-0.0.8/dintero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:42:31.325761 dintero-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-13 19:42:29.000000 dintero-0.0.8/examples/create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 19:42:29.000000 dintero-0.0.8/examples/manage_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 19:42:29.000000 dintero-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 19:42:31.329761 dintero-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-13 19:42:29.000000 dintero-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:42:31.325761 dintero-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:42:29.000000 dintero-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 19:42:29.000000 dintero-0.0.8/tests/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-13 19:42:29.000000 dintero-0.0.8/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 19:42:29.000000 dintero-0.0.8/tox.ini
```

### Comparing `dintero-0.0.7/LICENSE` & `dintero-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dintero-0.0.7/PKG-INFO` & `dintero-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dintero
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python bindings for the Dintero API
 Home-page: https://github.com/dintero/Dintero.Python.SDK
 Author: Dintero
 Author-email: integration@dintero.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dintero/Dintero.Python.SDK/issues
 Project-URL: Documentation, https://docs.dintero.com
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -46,15 +47,15 @@
 
 * Python 3.6+
 
 ## Using the SDK
 
 Create an account through https://onboarding.dintero.com.
 
-Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout-client/).
+Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout/checkout-client).
 
 Create a payment profile by going to [Dintero Backoffice](https://backoffice.dintero.com) --> Settings --> Payment
 Profiles
 
 Use your newly created credentials to create a session:
 
 ```python
```

### Comparing `dintero-0.0.7/README.md` & `dintero-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 * Python 3.6+
 
 ## Using the SDK
 
 Create an account through https://onboarding.dintero.com.
 
-Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout-client/).
+Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout/checkout-client).
 
 Create a payment profile by going to [Dintero Backoffice](https://backoffice.dintero.com) --> Settings --> Payment
 Profiles
 
 Use your newly created credentials to create a session:
 
 ```python
```

### Comparing `dintero-0.0.7/dintero/__init__.py` & `dintero-0.0.8/dintero/__init__.py`

 * *Files identical despite different names*

### Comparing `dintero-0.0.7/dintero/checkout.py` & `dintero-0.0.8/dintero/checkout.py`

 * *Files identical despite different names*

### Comparing `dintero-0.0.7/dintero/error.py` & `dintero-0.0.8/dintero/error.py`

 * *Files identical despite different names*

### Comparing `dintero-0.0.7/dintero.egg-info/PKG-INFO` & `dintero-0.0.8/dintero.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dintero
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python bindings for the Dintero API
 Home-page: https://github.com/dintero/Dintero.Python.SDK
 Author: Dintero
 Author-email: integration@dintero.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dintero/Dintero.Python.SDK/issues
 Project-URL: Documentation, https://docs.dintero.com
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -46,15 +47,15 @@
 
 * Python 3.6+
 
 ## Using the SDK
 
 Create an account through https://onboarding.dintero.com.
 
-Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout-client/).
+Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout/checkout-client).
 
 Create a payment profile by going to [Dintero Backoffice](https://backoffice.dintero.com) --> Settings --> Payment
 Profiles
 
 Use your newly created credentials to create a session:
 
 ```python
```

### Comparing `dintero-0.0.7/examples/create_session.py` & `dintero-0.0.8/examples/create_session.py`

 * *Files identical despite different names*

### Comparing `dintero-0.0.7/setup.py` & `dintero-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,11 +47,12 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `dintero-0.0.7/tests/test_checkout.py` & `dintero-0.0.8/tests/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dintero-0.0.7/tox.ini` & `dintero-0.0.8/tox.ini`

 * *Files identical despite different names*

