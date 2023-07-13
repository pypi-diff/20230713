# Comparing `tmp/skillbridge-1.4.0.tar.gz` & `tmp/skillbridge-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillbridge-1.4.0.tar", last modified: Fri Dec 16 14:14:24 2022, max compression
+gzip compressed data, was "skillbridge-1.5.0.tar", last modified: Thu Jul 13 08:44:06 2023, max compression
```

## Comparing `skillbridge-1.4.0.tar` & `skillbridge-1.5.0.tar`

### file list

```diff
@@ -1,39 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:24.823418 skillbridge-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2022-12-16 14:14:09.000000 skillbridge-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-16 14:14:09.000000 skillbridge-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2022-12-16 14:14:24.823418 skillbridge-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2022-12-16 14:14:09.000000 skillbridge-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-16 14:14:09.000000 skillbridge-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2022-12-16 14:14:24.823418 skillbridge-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:24.819419 skillbridge-1.4.0/skillbridge/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:24.823418 skillbridge-1.4.0/skillbridge/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/hints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/var.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:24.823418 skillbridge-1.4.0/skillbridge/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/server/python_server.il
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/server/python_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:24.823418 skillbridge-1.4.0/skillbridge/test/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/test/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/test/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2022-12-16 14:14:09.000000 skillbridge-1.4.0/skillbridge/test/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-16 14:14:17.000000 skillbridge-1.4.0/skillbridge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:14:24.819419 skillbridge-1.4.0/skillbridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2022-12-16 14:14:24.000000 skillbridge-1.4.0/skillbridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-16 14:14:24.000000 skillbridge-1.4.0/skillbridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 14:14:24.000000 skillbridge-1.4.0/skillbridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-16 14:14:24.000000 skillbridge-1.4.0/skillbridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-16 14:14:24.000000 skillbridge-1.4.0/skillbridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-16 14:14:24.000000 skillbridge-1.4.0/skillbridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:06.292534 skillbridge-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-13 08:43:48.000000 skillbridge-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-13 08:43:48.000000 skillbridge-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-13 08:44:06.292534 skillbridge-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-13 08:43:48.000000 skillbridge-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-13 08:43:48.000000 skillbridge-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-13 08:44:06.296534 skillbridge-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:06.288534 skillbridge-1.5.0/skillbridge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:06.292534 skillbridge-1.5.0/skillbridge/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/var.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:06.292534 skillbridge-1.5.0/skillbridge/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/server/python_server.il
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/server/python_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:06.292534 skillbridge-1.5.0/skillbridge/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/test/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/test/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-13 08:43:48.000000 skillbridge-1.5.0/skillbridge/test/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 08:43:58.000000 skillbridge-1.5.0/skillbridge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:06.292534 skillbridge-1.5.0/skillbridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-13 08:44:06.000000 skillbridge-1.5.0/skillbridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 08:44:06.000000 skillbridge-1.5.0/skillbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:44:06.000000 skillbridge-1.5.0/skillbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 08:44:06.000000 skillbridge-1.5.0/skillbridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-13 08:44:06.000000 skillbridge-1.5.0/skillbridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 08:44:06.000000 skillbridge-1.5.0/skillbridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:06.292534 skillbridge-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-07-13 08:43:48.000000 skillbridge-1.5.0/tests/test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-13 08:43:48.000000 skillbridge-1.5.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-13 08:43:48.000000 skillbridge-1.5.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-13 08:43:48.000000 skillbridge-1.5.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-13 08:43:48.000000 skillbridge-1.5.0/tests/test_test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-13 08:43:48.000000 skillbridge-1.5.0/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 08:43:48.000000 skillbridge-1.5.0/tests/test_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-13 08:43:48.000000 skillbridge-1.5.0/tests/test_workspace.py
```

### Comparing `skillbridge-1.4.0/LICENSE` & `skillbridge-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/PKG-INFO` & `skillbridge-1.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: skillbridge
-Version: 1.4.0
+Version: 1.5.0
 Summary: A seamless Python remote bridge to Cadence's Skill in Virtuoso
 Home-page: https://github.com/unihd-cag/skillbridge
 Author: Niels Buwen
 Author-email: dev@niels-buwen.de
 Maintainer: Tobias Markus
 Maintainer-email: tobias_markus@gmx.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -23,15 +27,15 @@
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # Python-Skill Bridge
 
 [![PyPI version](https://badge.fury.io/py/skillbridge.svg)](https://badge.fury.io/py/skillbridge)
-![build](https://github.com/unihd-cag/simple-geometry/workflows/Python%20package/badge.svg)
+![build](https://github.com/unihd-cag/skillbridge/workflows/Python%20package/badge.svg)
 
 ### Prerequisites
 
 - Python 3.6 or higher
 - pip
 - IC 6.1.7 or ICADV/M or higher
```

### Comparing `skillbridge-1.4.0/README.md` & `skillbridge-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Python-Skill Bridge
 
 [![PyPI version](https://badge.fury.io/py/skillbridge.svg)](https://badge.fury.io/py/skillbridge)
-![build](https://github.com/unihd-cag/simple-geometry/workflows/Python%20package/badge.svg)
+![build](https://github.com/unihd-cag/skillbridge/workflows/Python%20package/badge.svg)
 
 ### Prerequisites
 
 - Python 3.6 or higher
 - pip
 - IC 6.1.7 or ICADV/M or higher
```

### Comparing `skillbridge-1.4.0/setup.cfg` & `skillbridge-1.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [metadata]
 name = skillbridge
-version = 1.4.0
+version = attr: skillbridge.version.__version__
 author = Niels Buwen
 author_email = dev@niels-buwen.de
 maintainer = Tobias Markus
 maintainer_email = tobias_markus@gmx.net
 description = A seamless Python remote bridge to Cadence's Skill in Virtuoso
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/unihd-cag/skillbridge
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Intended Audience :: Information Technology
 	Operating System :: POSIX :: Linux
 	Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 	Topic :: Software Development
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skillbridge-1.4.0/skillbridge/__init__.py` & `skillbridge-1.5.0/skillbridge/__init__.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/__main__.py` & `skillbridge-1.5.0/skillbridge/__main__.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/client/channel.py` & `skillbridge-1.5.0/skillbridge/client/channel.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/client/functions.py` & `skillbridge-1.5.0/skillbridge/client/functions.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/client/globals.py` & `skillbridge-1.5.0/skillbridge/client/globals.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/client/hints.py` & `skillbridge-1.5.0/skillbridge/client/hints.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/client/objects.py` & `skillbridge-1.5.0/skillbridge/client/objects.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/client/remote.py` & `skillbridge-1.5.0/skillbridge/client/remote.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/client/translator.py` & `skillbridge-1.5.0/skillbridge/client/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         kw_keys = map(snake_to_camel, kwargs)
         kw_values = map(python_value_to_skill, kwargs.values())
         kwargs_code = ' '.join(f'?{key} {value}' for key, value in zip(kw_keys, kw_values))
         return SkillCode(f'{func_name}({args_code} {kwargs_code})')
 
     @staticmethod
     def encode_dir(obj: SkillCode) -> SkillCode:
-
         parts = ' '.join(
             (
                 f'{obj}->?',
                 f"if( type({obj}) == 'rodObj then {obj}->systemHandleNames)",
                 f'if( type({obj}) == \'rodObj then {obj}->userHandleNames)',
             )
         )
```

### Comparing `skillbridge-1.4.0/skillbridge/client/var.py` & `skillbridge-1.5.0/skillbridge/client/var.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/client/workspace.py` & `skillbridge-1.5.0/skillbridge/client/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,14 @@
         if direct and not sys.stdin.isatty():
             stdout = sys.stdout
             sys.stdout = sys.stderr
 
             return Workspace(DirectChannel(stdout), workspace_id)
 
         if workspace_id not in _open_workspaces:
-
             try:
                 channel_class = create_channel_class()
                 channel = channel_class(workspace_id)
             except FileNotFoundError:
                 raise RuntimeError("No server found. Is it running?") from None
 
             _open_workspaces[workspace_id] = Workspace(channel, workspace_id)
```

### Comparing `skillbridge-1.4.0/skillbridge/server/python_server.il` & `skillbridge-1.5.0/skillbridge/server/python_server.il`

 * *Files 3% similar despite different names*

```diff
@@ -214,18 +214,20 @@
             )
         )
     )
 
     pyStartServer.logName = lsprintf("%s/skillbridge_skill.log" _logDirectory)
 
     putd('pyRunScript nil)
-    defun(pyRunScript (script @key (python "python") (args nil) "ttl")
-        let((command)
+    defun(pyRunScript (script @key (python "python") (args nil) (block nil) "ttlg")
+        let((command process)
             command = lsprintf("%s %s %s" python script buildString(args))
-            ipcBeginProcess(command "" '__pyOnData '__pyOnError '__pyOnFinishScript pyRunScript.logName)
+            process = ipcBeginProcess(command "" '__pyOnData '__pyOnError '__pyOnFinishScript pyRunScript.logName)
+
+            if(block then ipcWait(process) else process)
         )
     )
 
     pyRunScript.logName = lsprintf("%s/skillbridge_script.log" _logDirectory)
 
     pyStartServer.ipc = nil
     pyStartServer.exe = _executable
```

### Comparing `skillbridge-1.4.0/skillbridge/server/python_server.py` & `skillbridge-1.5.0/skillbridge/server/python_server.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/test/channel.py` & `skillbridge-1.5.0/skillbridge/test/channel.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/test/translator.py` & `skillbridge-1.5.0/skillbridge/test/translator.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge/test/workspace.py` & `skillbridge-1.5.0/skillbridge/test/workspace.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.4.0/skillbridge.egg-info/PKG-INFO` & `skillbridge-1.5.0/skillbridge.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: skillbridge
-Version: 1.4.0
+Version: 1.5.0
 Summary: A seamless Python remote bridge to Cadence's Skill in Virtuoso
 Home-page: https://github.com/unihd-cag/skillbridge
 Author: Niels Buwen
 Author-email: dev@niels-buwen.de
 Maintainer: Tobias Markus
 Maintainer-email: tobias_markus@gmx.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -23,15 +27,15 @@
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # Python-Skill Bridge
 
 [![PyPI version](https://badge.fury.io/py/skillbridge.svg)](https://badge.fury.io/py/skillbridge)
-![build](https://github.com/unihd-cag/simple-geometry/workflows/Python%20package/badge.svg)
+![build](https://github.com/unihd-cag/skillbridge/workflows/Python%20package/badge.svg)
 
 ### Prerequisites
 
 - Python 3.6 or higher
 - pip
 - IC 6.1.7 or ICADV/M or higher
```

