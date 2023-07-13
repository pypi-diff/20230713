# Comparing `tmp/nvidia-smi2-0.0.1.tar.gz` & `tmp/nvidia-smi2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-smi2-0.0.1.tar", last modified: Thu Jul 13 05:26:35 2023, max compression
+gzip compressed data, was "nvidia-smi2-0.0.2.tar", last modified: Thu Jul 13 05:38:27 2023, max compression
```

## Comparing `nvidia-smi2-0.0.1.tar` & `nvidia-smi2-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:26:35.537221 nvidia-smi2-0.0.1/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:26:35.537221 nvidia-smi2-0.0.1/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8144 2023-07-12 04:42:41.000000 nvidia-smi2-0.0.1/README.md
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      155 2023-07-13 05:26:35.537221 nvidia-smi2-0.0.1/setup.cfg
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      180 2023-07-13 05:02:01.000000 nvidia-smi2-0.0.1/setup.py
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:26:35.537221 nvidia-smi2-0.0.1/src/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     2931 2023-07-13 04:44:42.000000 nvidia-smi2-0.0.1/src/nvidia-smi2
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:26:35.537221 nvidia-smi2-0.0.1/src/nvidia_smi2.egg-info/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:26:35.000000 nvidia-smi2-0.0.1/src/nvidia_smi2.egg-info/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      238 2023-07-13 05:26:35.000000 nvidia-smi2-0.0.1/src/nvidia_smi2.egg-info/SOURCES.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:26:35.000000 nvidia-smi2-0.0.1/src/nvidia_smi2.egg-info/dependency_links.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-13 05:26:35.000000 nvidia-smi2-0.0.1/src/nvidia_smi2.egg-info/requires.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:26:35.000000 nvidia-smi2-0.0.1/src/nvidia_smi2.egg-info/top_level.txt
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8144 2023-07-12 04:42:41.000000 nvidia-smi2-0.0.2/README.md
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/bin/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     2930 2023-07-13 05:34:40.000000 nvidia-smi2-0.0.2/bin/nvidia-smi2
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       55 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      218 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/requires.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 05:38:27.000000 nvidia-smi2-0.0.2/nvidia_smi2.egg-info/top_level.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      155 2023-07-13 05:38:27.354116 nvidia-smi2-0.0.2/setup.cfg
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      329 2023-07-13 05:36:28.000000 nvidia-smi2-0.0.2/setup.py
```

### Comparing `nvidia-smi2-0.0.1/README.md` & `nvidia-smi2-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nvidia-smi2-0.0.1/src/nvidia-smi2` & `nvidia-smi2-0.0.2/bin/nvidia-smi2`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
     print(sum_format % (
         user,
         str(user_detail[user]["total_gpu_mem"]) + "MiB",
         str(round(user_detail[user]["total_cpu"], 1)),
         str(round(user_detail[user]["total_mem"], 1))
     ))
 
-print("+" + ("-" * (len(line) - 2)) + "+")
+print("+" + ("-" * (len(line) - 2)) + "+")
```

