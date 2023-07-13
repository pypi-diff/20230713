# Comparing `tmp/nvidia-smi2-0.0.2.tar.gz` & `tmp/nvidia-smi2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-smi2-0.0.2.tar", last modified: Thu Jul 13 05:38:27 2023, max compression
+gzip compressed data, was "nvidia-smi2-0.0.3.tar", last modified: Thu Jul 13 05:51:44 2023, max compression
```

## Comparing `nvidia-smi2-0.0.2.tar` & `nvidia-smi2-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8144 2023-07-12 04:42:41.000000 nvidia-smi2-0.0.2/README.md
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/bin/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     2930 2023-07-13 05:34:40.000000 nvidia-smi2-0.0.2/bin/nvidia-smi2
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      218 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/SOURCES.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/dependency_links.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/requires.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/top_level.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      155 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/setup.cfg
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      329 2023-07-13 05:36:28.000000 nvidia-smi2-0.0.2/setup.py
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8144 2023-07-12 04:42:41.000000 nvidia-smi2-0.0.3/README.md
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/bin/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     2930 2023-07-13 05:34:40.000000 nvidia-smi2-0.0.3/bin/nvidia-smi2
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/nvidia-smi2/
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:51:44.399761 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      278 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/requires.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:51:44.000000 nvidia-smi2-0.0.3/nvidia-smi2/nvidia_smi2.egg-info/top_level.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      247 2023-07-13 05:51:44.403761 nvidia-smi2-0.0.3/setup.cfg
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      368 2023-07-13 05:51:36.000000 nvidia-smi2-0.0.3/setup.py
```

### Comparing `nvidia-smi2-0.0.2/README.md` & `nvidia-smi2-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nvidia-smi2-0.0.2/bin/nvidia-smi2` & `nvidia-smi2-0.0.3/bin/nvidia-smi2`

 * *Files identical despite different names*

