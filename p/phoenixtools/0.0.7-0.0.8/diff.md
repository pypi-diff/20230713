# Comparing `tmp/phoenixtools-0.0.7.tar.gz` & `tmp/phoenixtools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoenixtools-0.0.7.tar", last modified: Wed Jul 12 00:12:55 2023, max compression
+gzip compressed data, was "phoenixtools-0.0.8.tar", last modified: Thu Jul 13 04:45:39 2023, max compression
```

## Comparing `phoenixtools-0.0.7.tar` & `phoenixtools-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/
--rw-r--r--   0 runner    (1000) runner    (1000)      491 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/phoenixtools/
--rw-r--r--   0 runner    (1000) runner    (1000)     1172 2023-07-12 00:04:12.000000 phoenixtools-0.0.7/phoenixtools/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      203 2023-07-12 00:09:54.000000 phoenixtools-0.0.7/phoenixtools/colors.py
--rw-r--r--   0 runner    (1000) runner    (1000)      234 2023-06-28 23:08:01.000000 phoenixtools-0.0.7/phoenixtools/iptools.py
--rw-r--r--   0 runner    (1000) runner    (1000)      280 2023-07-12 00:11:34.000000 phoenixtools-0.0.7/phoenixtools/math.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/phoenixtools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      491 2023-07-12 00:12:55.000000 phoenixtools-0.0.7/phoenixtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      245 2023-07-12 00:12:55.000000 phoenixtools-0.0.7/phoenixtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 00:12:55.000000 phoenixtools-0.0.7/phoenixtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-12 00:12:55.000000 phoenixtools-0.0.7/phoenixtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1002 2023-07-12 00:12:31.000000 phoenixtools-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 04:45:39.829848 phoenixtools-0.0.8/
+-rw-rw-rw-   0        0        0      530 2023-07-13 04:45:39.828784 phoenixtools-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 04:45:39.813047 phoenixtools-0.0.8/phoenixtools/
+-rw-rw-rw-   0        0        0     1235 2023-07-13 03:52:49.000000 phoenixtools-0.0.8/phoenixtools/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-07-11 09:48:52.000000 phoenixtools-0.0.8/phoenixtools/colors.py
+-rw-rw-rw-   0        0        0      538 2023-07-13 03:52:49.000000 phoenixtools-0.0.8/phoenixtools/encryption.py
+-rw-rw-rw-   0        0        0      705 2023-07-13 04:38:37.000000 phoenixtools-0.0.8/phoenixtools/iptools.py
+-rw-rw-rw-   0        0        0      280 2023-07-11 09:48:52.000000 phoenixtools-0.0.8/phoenixtools/math.py
+-rw-rw-rw-   0        0        0     4216 2023-07-13 04:15:19.000000 phoenixtools-0.0.8/phoenixtools/steamkeygen.py
+drwxrwxrwx   0        0        0        0 2023-07-13 04:45:39.827594 phoenixtools-0.0.8/phoenixtools.egg-info/
+-rw-rw-rw-   0        0        0      530 2023-07-13 04:45:39.000000 phoenixtools-0.0.8/phoenixtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-07-13 04:45:39.000000 phoenixtools-0.0.8/phoenixtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 04:45:39.000000 phoenixtools-0.0.8/phoenixtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 04:45:39.000000 phoenixtools-0.0.8/phoenixtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 04:45:39.829848 phoenixtools-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-07-13 04:38:37.000000 phoenixtools-0.0.8/setup.py
```

### Comparing `phoenixtools-0.0.7/phoenixtools/__init__.py` & `phoenixtools-0.0.8/phoenixtools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .iptools import iptools
 from .colors import colors
+from .math import math
+from .encryption import encryptionTools
 def convertToLetters(number):
     if number==1:
       letter="A"
     elif number==2: 
       letter="B"
     elif number==3: 
       letter="C"
```

### Comparing `phoenixtools-0.0.7/setup.py` & `phoenixtools-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = 'Easy hacking tools'
-LONG_DESCRIPTION = 'Easy hacking tools used for educational purposes. Update notes: Added math and colors.'
+LONG_DESCRIPTION = 'Easy hacking tools used for educational purposes. Update notes: Added encryptiontools and new iptools function.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="phoenixtools", 
         version=VERSION,
         author="Jack B.",
```

