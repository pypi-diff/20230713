# Comparing `tmp/nvidia-smi2-0.0.3.tar.gz` & `tmp/nvidia-smi2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-smi2-0.0.3.tar", last modified: Thu Jul 13 05:51:44 2023, max compression
+gzip compressed data, was "nvidia-smi2-0.0.4.tar", last modified: Thu Jul 13 07:05:13 2023, max compression
```

## Comparing `nvidia-smi2-0.0.3.tar` & `nvidia-smi2-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8144 2023-07-12 04:42:41.000000 nvidia-smi2-0.0.3/README.md
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/bin/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     2930 2023-07-13 05:34:40.000000 nvidia-smi2-0.0.3/bin/nvidia-smi2
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/nvidia-smi2/
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      278 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/SOURCES.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/dependency_links.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/requires.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/top_level.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      247 2023-07-13 05:51:44.403761 nvidia-smi2-0.0.3/setup.cfg
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      368 2023-07-13 05:51:36.000000 nvidia-smi2-0.0.3/setup.py
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 07:05:13.083518 nvidia-smi2-0.0.4/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 07:05:13.083518 nvidia-smi2-0.0.4/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8144 2023-07-12 04:42:41.000000 nvidia-smi2-0.0.4/README.md
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 07:05:13.083518 nvidia-smi2-0.0.4/bin/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     2934 2023-07-13 06:37:45.000000 nvidia-smi2-0.0.4/bin/nvidia-smi2
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       38 2023-07-13 07:05:13.083518 nvidia-smi2-0.0.4/setup.cfg
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      383 2023-07-13 07:05:05.000000 nvidia-smi2-0.0.4/setup.py
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 07:05:13.083518 nvidia-smi2-0.0.4/src/
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 07:05:13.083518 nvidia-smi2-0.0.4/src/nvidia-smi2/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:43:39.000000 nvidia-smi2-0.0.4/src/nvidia-smi2/__init__.py
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     5350 2023-07-13 05:43:36.000000 nvidia-smi2-0.0.4/src/nvidia-smi2/nvidia-smi2.py
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 07:05:13.083518 nvidia-smi2-0.0.4/src/nvidia_smi2.egg-info/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 07:05:13.000000 nvidia-smi2-0.0.4/src/nvidia_smi2.egg-info/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      287 2023-07-13 07:05:13.000000 nvidia-smi2-0.0.4/src/nvidia_smi2.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 07:05:13.000000 nvidia-smi2-0.0.4/src/nvidia_smi2.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-13 07:05:13.000000 nvidia-smi2-0.0.4/src/nvidia_smi2.egg-info/requires.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       12 2023-07-13 07:05:13.000000 nvidia-smi2-0.0.4/src/nvidia_smi2.egg-info/top_level.txt
```

### Comparing `nvidia-smi2-0.0.3/README.md` & `nvidia-smi2-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nvidia-smi2-0.0.3/bin/nvidia-smi2` & `nvidia-smi2-0.0.4/bin/nvidia-smi2`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 import importlib
 import argparse
 import sys
-nvidia_smi2 = importlib.import_module("nvidia-smi2")
+nvidia_smi2 = importlib.import_module("src/nvidia-smi2")
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-l', '--command-length', default=20, const=100, type=int, nargs='?')
 parser.add_argument('-c', '--color', action='store_true')
 parser.add_argument('-u', '--user', type = str, default = '', help = 'user to analyst instead of all user')
 
 args = parser.parse_args()
```

