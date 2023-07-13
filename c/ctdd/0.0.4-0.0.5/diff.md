# Comparing `tmp/ctdd-0.0.4.tar.gz` & `tmp/ctdd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdd-0.0.4.tar", max compression
+gzip compressed data, was "ctdd-0.0.5.tar", max compression
```

## Comparing `ctdd-0.0.4.tar` & `ctdd-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.4/LICENSE
--rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.4/README.md
--rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.4/ctdd/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.4/ctdd/__main__.py
--rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.4/ctdd/ffi_factory.py
--rw-r--r--   0        0        0     1661 2023-07-09 18:51:45.635857 ctdd-0.0.4/ctdd/mocker.py
--rw-r--r--   0        0        0     2592 2023-07-11 11:26:17.438280 ctdd-0.0.4/ctdd/tester.py
--rw-r--r--   0        0        0     2977 2023-07-11 11:28:00.016820 ctdd-0.0.4/ctdd/tester_state.py
--rw-r--r--   0        0        0      736 2023-07-11 16:41:26.864826 ctdd-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.5/README.md
+-rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.5/ctdd/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.5/ctdd/__main__.py
+-rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.5/ctdd/ffi_factory.py
+-rw-r--r--   0        0        0     1663 2023-07-13 11:47:07.434036 ctdd-0.0.5/ctdd/mocker.py
+-rw-r--r--   0        0        0     2592 2023-07-11 11:26:17.438280 ctdd-0.0.5/ctdd/tester.py
+-rw-r--r--   0        0        0     2979 2023-07-13 11:45:15.551318 ctdd-0.0.5/ctdd/tester_state.py
+-rw-r--r--   0        0        0      736 2023-07-13 11:48:01.933872 ctdd-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.5/PKG-INFO
```

### Comparing `ctdd-0.0.4/LICENSE` & `ctdd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.4/README.md` & `ctdd-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.4/ctdd/__main__.py` & `ctdd-0.0.5/ctdd/__main__.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.4/ctdd/ffi_factory.py` & `ctdd-0.0.5/ctdd/ffi_factory.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.4/ctdd/mocker.py` & `ctdd-0.0.5/ctdd/mocker.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.called = {}
 
     def print_all(self):
         for b in self.called:
             print(b, self.called[b])
 
     def get_number_of_calls(self, key):
-        print(f'called: {self.called}')
+        # print(f'called: {self.called}')
         if isinstance(key, int):
             if key >= len(self.called):
                 raise ValueError(f'invalid mock id {key}')
         else:
             key = key.__name__
 
             if not key in self.called:
```

### Comparing `ctdd-0.0.4/ctdd/tester.py` & `ctdd-0.0.5/ctdd/tester.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.4/ctdd/tester_state.py` & `ctdd-0.0.5/ctdd/tester_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
                 function_decl = paste.function_decl(
                     typedef_name, binding_point_name) + ';'
                 self.externs.append(function_decl)
 
                 func = partial(mock_binder, self, binding_point_name)
 
-                print(f'binding {typedef_name} to {binding_point_name}')
+                # print(f'binding {typedef_name} to {binding_point_name}')
 
                 setattr(self.factory, f'{typedef_name}', func)
 
     def create_tube(self, name=None):
         test_case_module = importlib.import_module(self._module_name)
         test_case_filename = test_case_module.__file__
         test_case_name = os.path.splitext(
```

### Comparing `ctdd-0.0.4/pyproject.toml` & `ctdd-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctdd"
-version = "0.0.4"
+version = "0.0.5"
 description = "C test-driven development framework implemented in Python"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ctdd-0.0.4/PKG-INFO` & `ctdd-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctdd
-Version: 0.0.4
+Version: 0.0.5
 Summary: C test-driven development framework implemented in Python
 Home-page: https://github.com/wideopensource/ctdd
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

