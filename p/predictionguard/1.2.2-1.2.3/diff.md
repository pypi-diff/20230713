# Comparing `tmp/predictionguard-1.2.2.tar.gz` & `tmp/predictionguard-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictionguard-1.2.2.tar", last modified: Thu Jul 13 00:27:51 2023, max compression
+gzip compressed data, was "predictionguard-1.2.3.tar", last modified: Thu Jul 13 01:02:59 2023, max compression
```

## Comparing `predictionguard-1.2.2.tar` & `predictionguard-1.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-1.2.2/LICENSE
--rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-1.2.2/README.md
--rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-1.2.2/examples/sentiment.ipynb
--rw-r--r--   0        0        0      133 2023-07-13 00:27:44.334445 predictionguard-1.2.2/predictionguard/__init__.py
--rw-r--r--   0        0        0    16190 2023-07-13 00:27:40.826501 predictionguard-1.2.2/predictionguard/client.py
--rw-r--r--   0        0        0      483 2023-05-11 18:10:58.709630 predictionguard-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-1.2.3/README.md
+-rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-1.2.3/examples/sentiment.ipynb
+-rw-r--r--   0        0        0      133 2023-07-13 01:02:08.573964 predictionguard-1.2.3/predictionguard/__init__.py
+-rw-r--r--   0        0        0    16235 2023-07-13 01:02:01.574029 predictionguard-1.2.3/predictionguard/client.py
+-rw-r--r--   0        0        0      483 2023-05-11 18:10:58.709630 predictionguard-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.2.3/PKG-INFO
```

### Comparing `predictionguard-1.2.2/LICENSE` & `predictionguard-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.2/README.md` & `predictionguard-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.2/examples/sentiment.ipynb` & `predictionguard-1.2.3/examples/sentiment.ipynb`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.2/predictionguard/client.py` & `predictionguard-1.2.3/predictionguard/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,14 +393,16 @@
         Function to generate a single completion. 
         """
 
         # Make a prediction using the proxy.
         headers = {"Authorization": "Bearer " + self.token}
         if isinstance(model, list):
             model_join = ",".join(model)
+        else:
+            model_join = model
         if "openai" in model_join.lower():
             if os.environ.get("OPENAI_API_KEY") != "":
                 headers["OpenAI-ApiKey"] = os.environ.get("OPENAI_API_KEY")
             else:
                 raise ValueError("OpenAI API key not set. Please set the environment variable OPENAI_API_KEY.")
         payload_dict = {
             "model": model,
```

### Comparing `predictionguard-1.2.2/PKG-INFO` & `predictionguard-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictionguard
-Version: 1.2.2
+Version: 1.2.3
 Summary: Create controlled and compliant AI systems with PredictionGuard.
 Author-email: Daniel Whitenack <dan@predictionguard.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: tabulate >=0.8.10
 Requires-Dist: requests >=2.27.1
 Project-URL: Home, https://predictionguard.com
```

