# Comparing `tmp/py-machineid-0.4.1.tar.gz` & `tmp/py-machineid-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-machineid-0.4.1.tar", last modified: Mon Jul  3 16:11:41 2023, max compression
+gzip compressed data, was "py-machineid-0.4.2.tar", last modified: Thu Jul 13 15:01:44 2023, max compression
```

## Comparing `py-machineid-0.4.1.tar` & `py-machineid-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-03 16:11:41.744592 py-machineid-0.4.1/
--rw-r--r--   0 zeke      (1000) zeke      (1000)     1826 2023-07-03 16:11:41.744592 py-machineid-0.4.1/PKG-INFO
--rw-r--r--   0 zeke      (1000) zeke      (1000)      993 2023-07-03 15:27:13.000000 py-machineid-0.4.1/README.md
-drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-03 16:11:41.744592 py-machineid-0.4.1/machineid/
--rw-r--r--   0 zeke      (1000) zeke      (1000)     3364 2023-07-03 16:11:00.000000 py-machineid-0.4.1/machineid/__init__.py
-drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-03 16:11:41.744592 py-machineid-0.4.1/py_machineid.egg-info/
--rw-r--r--   0 zeke      (1000) zeke      (1000)     1826 2023-07-03 16:11:41.000000 py-machineid-0.4.1/py_machineid.egg-info/PKG-INFO
--rw-r--r--   0 zeke      (1000) zeke      (1000)      219 2023-07-03 16:11:41.000000 py-machineid-0.4.1/py_machineid.egg-info/SOURCES.txt
--rw-r--r--   0 zeke      (1000) zeke      (1000)        1 2023-07-03 16:11:41.000000 py-machineid-0.4.1/py_machineid.egg-info/dependency_links.txt
--rw-r--r--   0 zeke      (1000) zeke      (1000)       12 2023-07-03 16:11:41.000000 py-machineid-0.4.1/py_machineid.egg-info/requires.txt
--rw-r--r--   0 zeke      (1000) zeke      (1000)       10 2023-07-03 16:11:41.000000 py-machineid-0.4.1/py_machineid.egg-info/top_level.txt
--rw-r--r--   0 zeke      (1000) zeke      (1000)       38 2023-07-03 16:11:41.744592 py-machineid-0.4.1/setup.cfg
--rw-r--r--   0 zeke      (1000) zeke      (1000)      637 2023-07-03 16:11:02.000000 py-machineid-0.4.1/setup.py
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:01:44.169391 py-machineid-0.4.2/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     1067 2023-07-03 14:39:52.000000 py-machineid-0.4.2/LICENSE
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     2090 2023-07-13 15:01:44.169391 py-machineid-0.4.2/PKG-INFO
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     1233 2023-07-03 19:38:03.000000 py-machineid-0.4.2/README.md
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:01:44.169391 py-machineid-0.4.2/machineid/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     3367 2023-07-13 14:51:19.000000 py-machineid-0.4.2/machineid/__init__.py
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-13 15:01:44.169391 py-machineid-0.4.2/py_machineid.egg-info/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     2090 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/PKG-INFO
+-rw-r--r--   0 zeke      (1000) zeke      (1000)      227 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/SOURCES.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)        1 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/dependency_links.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       40 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/requires.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       10 2023-07-13 15:01:44.000000 py-machineid-0.4.2/py_machineid.egg-info/top_level.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       38 2023-07-13 15:01:44.169391 py-machineid-0.4.2/setup.cfg
+-rw-r--r--   0 zeke      (1000) zeke      (1000)      706 2023-07-13 14:56:32.000000 py-machineid-0.4.2/setup.py
```

### Comparing `py-machineid-0.4.1/PKG-INFO` & `py-machineid-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: py-machineid
-Version: 0.4.1
+Version: 0.4.2
 Summary: Get the unique machine ID of any host (without admin privileges)
 Home-page: https://github.com/keygen-sh/py-machineid
 Author: Zeke Gabrielse
 Author-email: oss@keygen.sh
 License: MIT
 Description: # py-machineid
         
+        [![CI](https://github.com/keygen-sh/py-machineid/actions/workflows/test.yml/badge.svg)](https://github.com/keygen-sh/py-machineid/actions)
+        [![PyPI version](https://badge.fury.io/py/py-machineid.svg)](https://badge.fury.io/py/py-machineid)
+        
         Get the unique machine ID of any host (without admin privileges).
         
         Sponsored by:
         
         <a href="https://keygen.sh?ref=typed_params">
           <div>
             <img src="https://keygen.sh/images/logo-pill.png" width="200" alt="Keygen">
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
-Metadata-Version: 2.1 Name: py-machineid Version: 0.4.1 Summary: Get the unique
+Metadata-Version: 2.1 Name: py-machineid Version: 0.4.2 Summary: Get the unique
 machine ID of any host (without admin privileges) Home-page: https://
 github.com/keygen-sh/py-machineid Author: Zeke Gabrielse Author-email:
-oss@keygen.sh License: MIT Description: # py-machineid Get the unique machine
-ID of any host (without admin privileges). Sponsored by:
+oss@keygen.sh License: MIT Description: # py-machineid [![CI](https://
+github.com/keygen-sh/py-machineid/actions/workflows/test.yml/badge.svg)](https:
+//github.com/keygen-sh/py-machineid/actions) [![PyPI version](https://
+badge.fury.io/py/py-machineid.svg)](https://badge.fury.io/py/py-machineid) Get
+the unique machine ID of any host (without admin privileges). Sponsored by:
 [Keygen]
  _An open, source-available software licensing and distribution API._ ##
 Install Install using [`pip`](https://docs.python.org/3/installing/index.html):
 ```bash python3 -m pip install py-machineid ``` ## Usage To obtain the raw GUID
 of the device, use `id() -> str`: ```python import machineid print(machineid.id
 ()) ``` To obtain an anonymized (hashed) version of the GUID, see below. The
 `hashed_id(str) -> str` function takes an optional application ID, which will
```

### Comparing `py-machineid-0.4.1/README.md` & `py-machineid-0.4.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # py-machineid
 
+[![CI](https://github.com/keygen-sh/py-machineid/actions/workflows/test.yml/badge.svg)](https://github.com/keygen-sh/py-machineid/actions)
+[![PyPI version](https://badge.fury.io/py/py-machineid.svg)](https://badge.fury.io/py/py-machineid)
+
 Get the unique machine ID of any host (without admin privileges).
 
 Sponsored by:
 
 <a href="https://keygen.sh?ref=typed_params">
   <div>
     <img src="https://keygen.sh/images/logo-pill.png" width="200" alt="Keygen">
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
-# py-machineid Get the unique machine ID of any host (without admin
-privileges). Sponsored by:
+# py-machineid [![CI](https://github.com/keygen-sh/py-machineid/actions/
+workflows/test.yml/badge.svg)](https://github.com/keygen-sh/py-machineid/
+actions) [![PyPI version](https://badge.fury.io/py/py-machineid.svg)](https://
+badge.fury.io/py/py-machineid) Get the unique machine ID of any host (without
+admin privileges). Sponsored by:
 [Keygen]
  _An open, source-available software licensing and distribution API._ ##
 Install Install using [`pip`](https://docs.python.org/3/installing/index.html):
 ```bash python3 -m pip install py-machineid ``` ## Usage To obtain the raw GUID
 of the device, use `id() -> str`: ```python import machineid print(machineid.id
 ()) ``` To obtain an anonymized (hashed) version of the GUID, see below. The
 `hashed_id(str) -> str` function takes an optional application ID, which will
```

### Comparing `py-machineid-0.4.1/machineid/__init__.py` & `py-machineid-0.4.2/machineid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ce2127ade536eaa9529f4a7b73141bbc2f094c46e32742c97679e186e7f13fde
 
 Special thanks to Denis Brodbeck for his Go package, machineid (https://github.com/denisbrodbeck/machineid).
 
 :license: MIT, see LICENSE for more details.
 """
 
-__version__ = '0.2.1'
+__version__ = '0.4.2'
 __author__  = 'Zeke Gabrielse'
 __credits__ = 'https://github.com/denisbrodbeck/machineid'
 
 from platform import uname
 from sys import platform
 import subprocess
 import hashlib
@@ -60,25 +60,23 @@
 
 def id(winregistry: bool = True) -> str:
   """
   id returns the platform specific device GUID of the current host OS.
   """
   if platform == 'darwin':
     id = __exec__("ioreg -d2 -c IOPlatformExpertDevice | awk -F\\\" '/IOPlatformUUID/{print $(NF-1)}'")
-
-  if platform == 'win32' or platform == 'cygwin' or platform == 'msys':
+  elif platform == 'win32' or platform == 'cygwin' or platform == 'msys':
     if winregistry:
       id = __reg__('HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Cryptography', 'MachineGuid')
     else:
       id = __exec__("powershell.exe -ExecutionPolicy bypass -command (Get-CimInstance -Class Win32_ComputerSystemProduct).UUID")
     if not id:
       id = __exec__('wmic csproduct get uuid').split('\n')[2] \
                                               .strip()
-
-  if platform.startswith('linux'):
+  elif platform.startswith('linux'):
     id = __read__('/var/lib/dbus/machine-id')
     if not id:
       id = __read__('/etc/machine-id')
     if not id:
       cgroup = __read__('/proc/self/cgroup')
       if cgroup:
         if 'docker' in cgroup:
@@ -87,16 +85,15 @@
       mountinfo = __read__('/proc/self/mountinfo')
       if mountinfo:
         if 'docker' in mountinfo:
           id = __exec__("grep 'systemd' /proc/self/mountinfo | cut -d/ -f3")
     if not id:
       if 'microsoft' in uname().release: # wsl
         id = __exec__("powershell.exe -ExecutionPolicy bypass -command '(Get-CimInstance -Class Win32_ComputerSystemProduct).UUID'")
-
-  if platform.startswith('openbsd') or platform.startswith('freebsd'):
+  elif platform.startswith('openbsd') or platform.startswith('freebsd'):
     id = __read__('/etc/hostid')
     if not id:
       id = __exec__('kenv -q smbios.system.uuid')
 
   if not id:
     raise Exception('failed to obtain id on platform {}'.format(platform))
```

### Comparing `py-machineid-0.4.1/py_machineid.egg-info/PKG-INFO` & `py-machineid-0.4.2/py_machineid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: py-machineid
-Version: 0.4.1
+Version: 0.4.2
 Summary: Get the unique machine ID of any host (without admin privileges)
 Home-page: https://github.com/keygen-sh/py-machineid
 Author: Zeke Gabrielse
 Author-email: oss@keygen.sh
 License: MIT
 Description: # py-machineid
         
+        [![CI](https://github.com/keygen-sh/py-machineid/actions/workflows/test.yml/badge.svg)](https://github.com/keygen-sh/py-machineid/actions)
+        [![PyPI version](https://badge.fury.io/py/py-machineid.svg)](https://badge.fury.io/py/py-machineid)
+        
         Get the unique machine ID of any host (without admin privileges).
         
         Sponsored by:
         
         <a href="https://keygen.sh?ref=typed_params">
           <div>
             <img src="https://keygen.sh/images/logo-pill.png" width="200" alt="Keygen">
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
-Metadata-Version: 2.1 Name: py-machineid Version: 0.4.1 Summary: Get the unique
+Metadata-Version: 2.1 Name: py-machineid Version: 0.4.2 Summary: Get the unique
 machine ID of any host (without admin privileges) Home-page: https://
 github.com/keygen-sh/py-machineid Author: Zeke Gabrielse Author-email:
-oss@keygen.sh License: MIT Description: # py-machineid Get the unique machine
-ID of any host (without admin privileges). Sponsored by:
+oss@keygen.sh License: MIT Description: # py-machineid [![CI](https://
+github.com/keygen-sh/py-machineid/actions/workflows/test.yml/badge.svg)](https:
+//github.com/keygen-sh/py-machineid/actions) [![PyPI version](https://
+badge.fury.io/py/py-machineid.svg)](https://badge.fury.io/py/py-machineid) Get
+the unique machine ID of any host (without admin privileges). Sponsored by:
 [Keygen]
  _An open, source-available software licensing and distribution API._ ##
 Install Install using [`pip`](https://docs.python.org/3/installing/index.html):
 ```bash python3 -m pip install py-machineid ``` ## Usage To obtain the raw GUID
 of the device, use `id() -> str`: ```python import machineid print(machineid.id
 ()) ``` To obtain an anonymized (hashed) version of the GUID, see below. The
 `hashed_id(str) -> str` function takes an optional application ID, which will
```

### Comparing `py-machineid-0.4.1/setup.py` & `py-machineid-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+from machineid import __version__, __author__
 from setuptools import setup
 
 with open("README.md", "r") as fh:
   readme = fh.read()
 
 setup(
   name='py-machineid',
-  version='0.4.1',
+  version=__version__,
   description='Get the unique machine ID of any host (without admin privileges)',
   long_description_content_type='text/markdown',
   long_description=readme,
   url='https://github.com/keygen-sh/py-machineid',
-  author='Zeke Gabrielse',
+  author=__author__,
   author_email='oss@keygen.sh',
   license='MIT',
-  install_requires=['winregistry'],
+  install_requires=['winregistry; sys_platform == "win32"'],
   packages=['machineid'],
   classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
   ],
 )
```

