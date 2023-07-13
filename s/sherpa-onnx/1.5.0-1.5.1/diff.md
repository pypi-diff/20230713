# Comparing `tmp/sherpa-onnx-1.5.0.tar.gz` & `tmp/sherpa-onnx-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.5.0.tar", last modified: Sun Jul  9 07:03:52 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.5.1.tar", last modified: Thu Jul 13 07:13:09 2023, max compression
```

## Comparing `sherpa-onnx-1.5.0.tar` & `sherpa-onnx-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.941250 sherpa-onnx-1.5.0/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.941250 sherpa-onnx-1.5.0/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.986547 sherpa-onnx-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:13:09.986547 sherpa-onnx-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.5.0/LICENSE` & `sherpa-onnx-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.0/PKG-INFO` & `sherpa-onnx-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.5.0
+Version: 1.5.1
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.5.0/setup.py` & `sherpa-onnx-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,12 +145,18 @@
 
     def is_ready(self, s: OnlineStream) -> bool:
         return self.recognizer.is_ready(s)
 
     def get_result(self, s: OnlineStream) -> str:
         return self.recognizer.get_result(s).text.strip()
 
+    def tokens(self, s: OnlineStream) -> List[str]:
+        return self.recognizer.get_result(s).tokens
+
+    def timestamps(self, s: OnlineStream) -> List[float]:
+        return self.recognizer.get_result(s).timestamps
+
     def is_endpoint(self, s: OnlineStream) -> bool:
         return self.recognizer.is_endpoint(s)
 
     def reset(self, s: OnlineStream) -> bool:
         return self.recognizer.reset(s)
```

### Comparing `sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,9 +66,9 @@
                 else:
                     for p in sp.encode_as_pieces(ch_or_w):
                         ids.append(
                             tokens_table[p]
                             if p in tokens_table
                             else tokens_table["<unk>"]
                         )
-        contexts_list.append(ids)
+            contexts_list.append(ids)
     return contexts_list
```

### Comparing `sherpa-onnx-1.5.0/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.5.1/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.5.0
+Version: 1.5.1
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

