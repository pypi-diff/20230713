# Comparing `tmp/py-helper-mod-0.0.39.tar.gz` & `tmp/py-helper-mod-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.39.tar", last modified: Wed Jul 12 16:44:46 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.40.tar", last modified: Thu Jul 13 15:39:47 2023, max compression
```

## Comparing `py-helper-mod-0.0.39.tar` & `py-helper-mod-0.0.40.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-12 16:44:46.389260 py-helper-mod-0.0.39/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.39/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-12 16:44:46.389260 py-helper-mod-0.0.39/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.39/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89230 2023-07-12 16:40:01.000000 py-helper-mod-0.0.39/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-12 16:44:46.389260 py-helper-mod-0.0.39/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-12 16:44:46.000000 py-helper-mod-0.0.39/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-12 16:44:46.000000 py-helper-mod-0.0.39/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-12 16:44:46.000000 py-helper-mod-0.0.39/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-12 16:44:46.000000 py-helper-mod-0.0.39/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.39/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-12 16:44:46.393261 py-helper-mod-0.0.39/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.39/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-13 15:39:47.075878 py-helper-mod-0.0.40/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.40/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-13 15:39:47.075878 py-helper-mod-0.0.40/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.40/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    89466 2023-07-13 15:38:33.000000 py-helper-mod-0.0.40/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-13 15:39:47.075878 py-helper-mod-0.0.40/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-13 15:39:47.000000 py-helper-mod-0.0.40/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-13 15:39:47.000000 py-helper-mod-0.0.40/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-13 15:39:47.000000 py-helper-mod-0.0.40/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-13 15:39:47.000000 py-helper-mod-0.0.40/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.40/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-13 15:39:47.075878 py-helper-mod-0.0.40/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.40/setup.py
```

### Comparing `py-helper-mod-0.0.39/LICENSE` & `py-helper-mod-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.39/PKG-INFO` & `py-helper-mod-0.0.40/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.39
+Version: 0.0.40
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.39/py_helper.py` & `py-helper-mod-0.0.40/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1181,15 +1181,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,38)
+VERSION=(0,0,39)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1500,15 +1500,19 @@
 
 		if timestamp:
 			prefix = f"{prefix} {datetime.now()}"
 
 		if delta != None:
 			msg = f"{msg} - Delta from last call {delta}"
 
-		adjusted = f"{prefix} {caller_str} : {msg}" if caller_str != "" else f"{prefix} : {msg}"
+		# Just because I don't like putting null pointers into string functions... I know python None is not a null pointer, but it rubs
+		# me the wrong way allowing this anyway.
+		dbglbl = "None" if dbglabel is None else dbglabel
+
+		adjusted = f"{prefix} {caller_str}/{dbglbl} : {msg}" if caller_str != "" else f"{prefix} : {msg}"
 
 		Msg(adjusted,func,ignoreModuleMode=True,end=end,file=file,flush=flush)
 
 		if break_point:
 			breakpoint()
 
 # DbgAuto Messages
```

### Comparing `py-helper-mod-0.0.39/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.40/py_helper_mod.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.39
+Version: 0.0.40
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

