# Comparing `tmp/py-machineid-0.4.2.tar.gz` & `tmp/py-machineid-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-machineid-0.4.2.tar", last modified: Thu Jul 13 15:01:44 2023, max compression
+gzip compressed data, was "py-machineid-0.4.3.tar", last modified: Thu Jul 13 15:20:08 2023, max compression
```

## Comparing `py-machineid-0.4.2.tar` & `py-machineid-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:01:44.169391 py-machineid-0.4.2/
--rw-r--r--   0 zeke      (1000) zeke      (1000)     1067 2023-07-03 14:39:52.000000 py-machineid-0.4.2/LICENSE
--rw-r--r--   0 zeke      (1000) zeke      (1000)     2090 2023-07-13 15:01:44.169391 py-machineid-0.4.2/PKG-INFO
--rw-r--r--   0 zeke      (1000) zeke      (1000)     1233 2023-07-03 19:38:03.000000 py-machineid-0.4.2/README.md
-drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:01:44.169391 py-machineid-0.4.2/machineid/
--rw-r--r--   0 zeke      (1000) zeke      (1000)     3367 2023-07-13 14:51:19.000000 py-machineid-0.4.2/machineid/__init__.py
-drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:01:44.169391 py-machineid-0.4.2/py_machineid.egg-info/
--rw-r--r--   0 zeke      (1000) zeke      (1000)     2090 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/PKG-INFO
--rw-r--r--   0 zeke      (1000) zeke      (1000)      227 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/SOURCES.txt
--rw-r--r--   0 zeke      (1000) zeke      (1000)        1 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/dependency_links.txt
--rw-r--r--   0 zeke      (1000) zeke      (1000)       40 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/requires.txt
--rw-r--r--   0 zeke      (1000) zeke      (1000)       10 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/top_level.txt
--rw-r--r--   0 zeke      (1000) zeke      (1000)       38 2023-07-13 15:01:44.169391 py-machineid-0.4.2/setup.cfg
--rw-r--r--   0 zeke      (1000) zeke      (1000)      706 2023-07-13 14:56:32.000000 py-machineid-0.4.2/setup.py
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:20:08.875068 py-machineid-0.4.3/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     1067 2023-07-03 14:39:52.000000 py-machineid-0.4.3/LICENSE
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     2090 2023-07-13 15:20:08.875068 py-machineid-0.4.3/PKG-INFO
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     1233 2023-07-03 19:38:03.000000 py-machineid-0.4.3/README.md
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:20:08.875068 py-machineid-0.4.3/machineid/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     3368 2023-07-13 15:15:24.000000 py-machineid-0.4.3/machineid/__init__.py
+-rw-r--r--   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:11:27.000000 py-machineid-0.4.3/machineid/py.typed
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:20:08.875068 py-machineid-0.4.3/py_machineid.egg-info/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     2090 2023-07-13 15:20:08.000000 py-machineid-0.4.3/py_machineid.egg-info/PKG-INFO
+-rw-r--r--   0 zeke      (1000) zeke      (1000)      246 2023-07-13 15:20:08.000000 py-machineid-0.4.3/py_machineid.egg-info/SOURCES.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)        1 2023-07-13 15:20:08.000000 py-machineid-0.4.3/py_machineid.egg-info/dependency_links.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       40 2023-07-13 15:20:08.000000 py-machineid-0.4.3/py_machineid.egg-info/requires.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       10 2023-07-13 15:20:08.000000 py-machineid-0.4.3/py_machineid.egg-info/top_level.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       38 2023-07-13 15:20:08.875068 py-machineid-0.4.3/setup.cfg
+-rw-r--r--   0 zeke      (1000) zeke      (1000)      759 2023-07-13 15:19:21.000000 py-machineid-0.4.3/setup.py
```

### Comparing `py-machineid-0.4.2/LICENSE` & `py-machineid-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-machineid-0.4.2/PKG-INFO` & `py-machineid-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-machineid
-Version: 0.4.2
+Version: 0.4.3
 Summary: Get the unique machine ID of any host (without admin privileges)
 Home-page: https://github.com/keygen-sh/py-machineid
 Author: Zeke Gabrielse
 Author-email: oss@keygen.sh
 License: MIT
 Description: # py-machineid
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-machineid Version: 0.4.2 Summary: Get the unique
+Metadata-Version: 2.1 Name: py-machineid Version: 0.4.3 Summary: Get the unique
 machine ID of any host (without admin privileges) Home-page: https://
 github.com/keygen-sh/py-machineid Author: Zeke Gabrielse Author-email:
 oss@keygen.sh License: MIT Description: # py-machineid [![CI](https://
 github.com/keygen-sh/py-machineid/actions/workflows/test.yml/badge.svg)](https:
 //github.com/keygen-sh/py-machineid/actions) [![PyPI version](https://
 badge.fury.io/py/py-machineid.svg)](https://badge.fury.io/py/py-machineid) Get
 the unique machine ID of any host (without admin privileges). Sponsored by:
```

### Comparing `py-machineid-0.4.2/README.md` & `py-machineid-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `py-machineid-0.4.2/machineid/__init__.py` & `py-machineid-0.4.3/machineid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ce2127ade536eaa9529f4a7b73141bbc2f094c46e32742c97679e186e7f13fde
 
 Special thanks to Denis Brodbeck for his Go package, machineid (https://github.com/denisbrodbeck/machineid).
 
 :license: MIT, see LICENSE for more details.
 """
 
-__version__ = '0.4.2'
+__version__ = '0.4.3'
 __author__  = 'Zeke Gabrielse'
 __credits__ = 'https://github.com/denisbrodbeck/machineid'
 
 from platform import uname
 from sys import platform
 import subprocess
 import hashlib
@@ -58,14 +58,15 @@
   except:
     return None
 
 def id(winregistry: bool = True) -> str:
   """
   id returns the platform specific device GUID of the current host OS.
   """
+
   if platform == 'darwin':
     id = __exec__("ioreg -d2 -c IOPlatformExpertDevice | awk -F\\\" '/IOPlatformUUID/{print $(NF-1)}'")
   elif platform == 'win32' or platform == 'cygwin' or platform == 'msys':
     if winregistry:
       id = __reg__('HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Cryptography', 'MachineGuid')
     else:
       id = __exec__("powershell.exe -ExecutionPolicy bypass -command (Get-CimInstance -Class Win32_ComputerSystemProduct).UUID")
```

### Comparing `py-machineid-0.4.2/py_machineid.egg-info/PKG-INFO` & `py-machineid-0.4.3/py_machineid.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-machineid
-Version: 0.4.2
+Version: 0.4.3
 Summary: Get the unique machine ID of any host (without admin privileges)
 Home-page: https://github.com/keygen-sh/py-machineid
 Author: Zeke Gabrielse
 Author-email: oss@keygen.sh
 License: MIT
 Description: # py-machineid
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-machineid Version: 0.4.2 Summary: Get the unique
+Metadata-Version: 2.1 Name: py-machineid Version: 0.4.3 Summary: Get the unique
 machine ID of any host (without admin privileges) Home-page: https://
 github.com/keygen-sh/py-machineid Author: Zeke Gabrielse Author-email:
 oss@keygen.sh License: MIT Description: # py-machineid [![CI](https://
 github.com/keygen-sh/py-machineid/actions/workflows/test.yml/badge.svg)](https:
 //github.com/keygen-sh/py-machineid/actions) [![PyPI version](https://
 badge.fury.io/py/py-machineid.svg)](https://badge.fury.io/py/py-machineid) Get
 the unique machine ID of any host (without admin privileges). Sponsored by:
```

### Comparing `py-machineid-0.4.2/setup.py` & `py-machineid-0.4.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,13 +12,16 @@
   long_description=readme,
   url='https://github.com/keygen-sh/py-machineid',
   author=__author__,
   author_email='oss@keygen.sh',
   license='MIT',
   install_requires=['winregistry; sys_platform == "win32"'],
   packages=['machineid'],
+  package_data={
+    'machineid': ['py.typed'],
+  },
   classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
   ],
 )
```

