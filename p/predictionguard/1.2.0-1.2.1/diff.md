# Comparing `tmp/predictionguard-1.2.0.tar.gz` & `tmp/predictionguard-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictionguard-1.2.0.tar", last modified: Mon Jun 19 00:41:57 2023, max compression
+gzip compressed data, was "predictionguard-1.2.1.tar", last modified: Thu Jul 13 00:14:33 2023, max compression
```

## Comparing `predictionguard-1.2.0.tar` & `predictionguard-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-1.2.0/LICENSE
--rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-1.2.0/README.md
--rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-1.2.0/examples/sentiment.ipynb
--rw-r--r--   0        0        0      133 2023-06-19 00:28:31.124496 predictionguard-1.2.0/predictionguard/__init__.py
--rw-r--r--   0        0        0    16462 2023-06-19 00:28:22.224570 predictionguard-1.2.0/predictionguard/client.py
--rw-r--r--   0        0        0      483 2023-05-11 18:10:58.709630 predictionguard-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-1.2.1/README.md
+-rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-1.2.1/examples/sentiment.ipynb
+-rw-r--r--   0        0        0      133 2023-07-13 00:14:30.870617 predictionguard-1.2.1/predictionguard/__init__.py
+-rw-r--r--   0        0        0    16108 2023-07-13 00:10:29.468065 predictionguard-1.2.1/predictionguard/client.py
+-rw-r--r--   0        0        0      483 2023-05-11 18:10:58.709630 predictionguard-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.2.1/PKG-INFO
```

### Comparing `predictionguard-1.2.0/LICENSE` & `predictionguard-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.0/README.md` & `predictionguard-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.0/examples/sentiment.ipynb` & `predictionguard-1.2.1/examples/sentiment.ipynb`

 * *Files identical despite different names*

### Comparing `predictionguard-1.2.0/predictionguard/client.py` & `predictionguard-1.2.1/predictionguard/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,29 +427,16 @@
                 err = response.json()["error"]
             except:
                 pass
             raise ValueError("Could not make prediction. " + err)
 
     @classmethod
     def list_models(self) -> List[str]:
-        return {
-            "Dolly-7B",
-            "Dolly-3B",
-            "h2oGPT-6_9B",
-            "RedPajama-INCITE-Instruct-7B",
-            "Camel-5B",
-            "Pythia-6_9-Deduped",
-            "MPT-7B-Instruct",
-            "Falcon-7B-Instruct",
-            "Falcon-40B-Instruct",
-            "OpenAI-text-davinci-003",
-            "OpenAI-text-davinci-002",
-            "OpenAI-text-curie-001",
-            "OpenAI-text-babbage-001",
-            "OpenAI-text-ada-001",
-            "OpenAI-davinci",
-            "OpenAI-curie",
-            "OpenAI-babbage",
-            "OpenAI-ada",
-            "WizardCoder",
-            "StarCoder"
-        }
+
+        # Make sure we can connect to prediction guard.
+        self._connect()
+
+        # Get the list of current models.
+        headers = {"Authorization": "Bearer " + self.token}
+        response = requests.request("GET", url + "/completions", headers=headers)
+
+        return list(response.json())
```

### Comparing `predictionguard-1.2.0/PKG-INFO` & `predictionguard-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictionguard
-Version: 1.2.0
+Version: 1.2.1
 Summary: Create controlled and compliant AI systems with PredictionGuard.
 Author-email: Daniel Whitenack <dan@predictionguard.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: tabulate >=0.8.10
 Requires-Dist: requests >=2.27.1
 Project-URL: Home, https://predictionguard.com
```

