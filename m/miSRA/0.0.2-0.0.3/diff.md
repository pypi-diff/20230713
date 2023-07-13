# Comparing `tmp/misra-0.0.2.tar.gz` & `tmp/misra-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misra-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "misra-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `misra-0.0.2.tar` & `misra-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2826 2023-07-12 13:08:31.646185 misra-0.0.2/README.md
--rw-r--r--   0        0        0      831 2023-07-12 13:08:31.422197 misra-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      261 2023-07-12 13:08:32.670133 misra-0.0.2/src/miSRA/README.md
--rw-r--r--   0        0        0        0 2023-07-12 13:08:32.406146 misra-0.0.2/src/miSRA/__init__.py
--rw-r--r--   0        0        0      991 2023-07-12 13:08:33.282101 misra-0.0.2/src/miSRA/example_configs/annotated_miSRA_example_config.json
--rw-r--r--   0        0        0      161 2023-07-12 13:08:33.282101 misra-0.0.2/src/miSRA/example_configs/miSRA_example_config.json
--rw-r--r--   0        0        0    18524 2023-07-12 13:08:32.630135 misra-0.0.2/src/miSRA/miSRA.py
--rw-r--r--   0        0        0     3485 1970-01-01 00:00:00.000000 misra-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2826 2023-07-13 10:22:57.606971 misra-0.0.3/README.md
+-rw-r--r--   0        0        0      831 2023-07-13 10:22:57.370984 misra-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      261 2023-07-13 10:22:58.642918 misra-0.0.3/src/miSRA/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 10:22:58.402930 misra-0.0.3/src/miSRA/__init__.py
+-rw-r--r--   0        0        0      991 2023-07-13 10:22:59.334882 misra-0.0.3/src/miSRA/example_configs/annotated_miSRA_example_config.json
+-rw-r--r--   0        0        0      161 2023-07-13 10:22:59.330882 misra-0.0.3/src/miSRA/example_configs/miSRA_example_config.json
+-rw-r--r--   0        0        0    18937 2023-07-13 10:22:58.642918 misra-0.0.3/src/miSRA/miSRA.py
+-rw-r--r--   0        0        0     3485 1970-01-01 00:00:00.000000 misra-0.0.3/PKG-INFO
```

### Comparing `misra-0.0.2/README.md` & `misra-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `misra-0.0.2/pyproject.toml` & `misra-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "miSRA"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Michael Hackenberg", email="hackenberg@go.ugr.es" },
   { name="Ernesto Aparicio", email="eaparicioeaparicio@gmail.com" },
 ]
 description = "A command-line interface to the miSRA API. It allow to remotely query over 90,000 miRNA-seq samples from the Sequence Read Archive"
 readme = "README.md"
 requires-python = ">=3.7.0"
```

### Comparing `misra-0.0.2/src/miSRA/example_configs/annotated_miSRA_example_config.json` & `misra-0.0.3/src/miSRA/example_configs/annotated_miSRA_example_config.json`

 * *Files identical despite different names*

### Comparing `misra-0.0.2/src/miSRA/miSRA.py` & `misra-0.0.3/src/miSRA/miSRA.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,14 +388,21 @@
 
         if data['mode'] == "download":
             backdata["mode"] = "download"
             return (backdata, None)
         # check if mode is spike and the file is specified and does exist
         if (data["mode"] == "exact"):
             data["mode"] = "spike"
+            if (data.get("spikeFile") and os.path.isfile(data["spikeFile"])):
+                backdata["mode"] = "spike"
+                backdata["fn1"] = os.path.basename(data["spikeFile"])
+                return (backdata, {"spikeFile": data["spikeFile"]})
+            else:
+                print("The fasta file (spikeFile=) with localOut spike-in sequences could not be detected")
+                sys.exit(0)
         if (data["mode"] == "spike"):
             if (data.get("spikeFile") and os.path.isfile(data["spikeFile"])):
                 backdata["mode"] = "spike"
                 backdata["fn1"] = os.path.basename(data["spikeFile"])
                 return (backdata, {"spikeFile": data["spikeFile"]})
             else:
                 print("The fasta file (spikeFile=) with localOut spike-in sequences could not be detected")
```

### Comparing `misra-0.0.2/PKG-INFO` & `misra-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miSRA
-Version: 0.0.2
+Version: 0.0.3
 Summary: A command-line interface to the miSRA API. It allow to remotely query over 90,000 miRNA-seq samples from the Sequence Read Archive
 Author-email: Michael Hackenberg <hackenberg@go.ugr.es>, Ernesto Aparicio <eaparicioeaparicio@gmail.com>
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

