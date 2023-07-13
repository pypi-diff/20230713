# Comparing `tmp/predictionguard-1.2.1.tar.gz` & `tmp/predictionguard-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictionguard-1.2.1.tar", last modified: Thu Jul 13 00:14:33 2023, max compression
+gzip compressed data, was "predictionguard-1.2.2.tar", last modified: Thu Jul 13 00:27:51 2023, max compression
```

## Comparing `predictionguard-1.2.1.tar` & `predictionguard-1.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-1.2.1/LICENSE
--rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-1.2.1/README.md
--rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-1.2.1/examples/sentiment.ipynb
--rw-r--r--   0        0        0      133 2023-07-13 00:14:30.870617 predictionguard-1.2.1/predictionguard/__init__.py
--rw-r--r--   0        0        0    16108 2023-07-13 00:10:29.468065 predictionguard-1.2.1/predictionguard/client.py
--rw-r--r--   0        0        0      483 2023-05-11 18:10:58.709630 predictionguard-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-1.2.2/README.md
+-rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-1.2.2/examples/sentiment.ipynb
+-rw-r--r--   0        0        0      133 2023-07-13 00:27:44.334445 predictionguard-1.2.2/predictionguard/__init__.py
+-rw-r--r--   0        0        0    16190 2023-07-13 00:27:40.826501 predictionguard-1.2.2/predictionguard/client.py
+-rw-r--r--   0        0        0      483 2023-05-11 18:10:58.709630 predictionguard-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.2.2/PKG-INFO
```

### Comparing `predictionguard-1.2.1/LICENSE` & `predictionguard-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.1/README.md` & `predictionguard-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.1/examples/sentiment.ipynb` & `predictionguard-1.2.2/examples/sentiment.ipynb`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.1/predictionguard/client.py` & `predictionguard-1.2.2/predictionguard/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,17 @@
     def _generate_completion(self, model, prompt, output, max_tokens, temperature, top_p, top_k):
         """
         Function to generate a single completion. 
         """
 
         # Make a prediction using the proxy.
         headers = {"Authorization": "Bearer " + self.token}
-        if "openai" in model.lower():
+        if isinstance(model, list):
+            model_join = ",".join(model)
+        if "openai" in model_join.lower():
             if os.environ.get("OPENAI_API_KEY") != "":
                 headers["OpenAI-ApiKey"] = os.environ.get("OPENAI_API_KEY")
             else:
                 raise ValueError("OpenAI API key not set. Please set the environment variable OPENAI_API_KEY.")
         payload_dict = {
             "model": model,
             "prompt": prompt,
```

### Comparing `predictionguard-1.2.1/PKG-INFO` & `predictionguard-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictionguard
-Version: 1.2.1
+Version: 1.2.2
 Summary: Create controlled and compliant AI systems with PredictionGuard.
 Author-email: Daniel Whitenack <dan@predictionguard.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: tabulate >=0.8.10
 Requires-Dist: requests >=2.27.1
 Project-URL: Home, https://predictionguard.com
```

