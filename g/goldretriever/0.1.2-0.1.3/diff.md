# Comparing `tmp/goldretriever-0.1.2.tar.gz` & `tmp/goldretriever-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goldretriever-0.1.2.tar", max compression
+gzip compressed data, was "goldretriever-0.1.3.tar", max compression
```

## Comparing `goldretriever-0.1.2.tar` & `goldretriever-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1063 2023-05-21 20:28:15.508056 goldretriever-0.1.2/LICENSE
--rw-r--r--   0        0        0     4417 2023-05-21 20:28:15.508056 goldretriever-0.1.2/README.md
--rw-r--r--   0        0        0      758 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/.well-known/ai-plugin.json
--rw-r--r--   0        0        0      760 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/.well-known/default-ai-plugin.json
--rw-r--r--   0        0        0      836 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/.well-known/logo.png
--rw-r--r--   0        0        0     4737 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/.well-known/openapi.yaml
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/__init__.py
--rw-r--r--   0        0        0       98 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/config.yml
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/datastore/__init__.py
--rw-r--r--   0        0        0     3046 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/datastore/datastore.py
--rw-r--r--   0        0        0      143 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/datastore/executor/Dockerfile
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/datastore/executor/__init__.py
--rw-r--r--   0        0        0      161 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/datastore/executor/config.yml
--rw-r--r--   0        0        0     3193 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/datastore/executor/docarray_v1.py
--rw-r--r--   0        0        0     1220 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/datastore/factory.py
--rw-r--r--   0        0        0      777 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/flow.yml
--rw-r--r--   0        0        0    11289 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/gateway.py
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/models/__init__.py
--rw-r--r--   0        0        0      634 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/models/api.py
--rw-r--r--   0        0        0     1460 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/models/models.py
--rw-r--r--   0        0        0    10199 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/retriever.py
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/__init__.py
--rw-r--r--   0        0        0     3016 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_json/README.md
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_json/__init__.py
--rw-r--r--   0        0        0      630 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_json/example.json
--rw-r--r--   0        0        0     5356 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_json/process_json.py
--rw-r--r--   0        0        0     3091 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_jsonl/README.md
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_jsonl/__init__.py
--rw-r--r--   0        0        0      879 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_jsonl/example.jsonl
--rw-r--r--   0        0        0     5253 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_jsonl/process_jsonl.py
--rw-r--r--   0        0        0     2699 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_zip/README.md
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_zip/__init__.py
--rw-r--r--   0        0        0    53296 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_zip/example.zip
--rw-r--r--   0        0        0     5668 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/scripts/process_zip/process_zip.py
--rw-r--r--   0        0        0        0 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/services/__init__.py
--rw-r--r--   0        0        0     7609 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/services/chunks.py
--rw-r--r--   0        0        0      793 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/services/date.py
--rw-r--r--   0        0        0     1201 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/services/extract_metadata.py
--rw-r--r--   0        0        0     3674 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/services/file.py
--rw-r--r--   0        0        0     1879 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/services/openai.py
--rw-r--r--   0        0        0     1350 2023-05-21 20:28:15.508056 goldretriever-0.1.2/goldretriever/services/pii_detection.py
--rw-r--r--   0        0        0      998 2023-05-21 20:28:15.512056 goldretriever-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5766 1970-01-01 00:00:00.000000 goldretriever-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-13 10:07:22.962369 goldretriever-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4730 2023-07-13 10:07:22.962369 goldretriever-0.1.3/README.md
+-rw-r--r--   0        0        0      758 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/.well-known/ai-plugin.json
+-rw-r--r--   0        0        0      760 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/.well-known/default-ai-plugin.json
+-rw-r--r--   0        0        0      836 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/.well-known/logo.png
+-rw-r--r--   0        0        0     4737 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/.well-known/openapi.yaml
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/__init__.py
+-rw-r--r--   0        0        0       98 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/config.yml
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/__init__.py
+-rw-r--r--   0        0        0     3046 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/datastore.py
+-rw-r--r--   0        0        0      143 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/executor/Dockerfile
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/executor/__init__.py
+-rw-r--r--   0        0        0      161 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/executor/config.yml
+-rw-r--r--   0        0        0     3193 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/executor/docarray_v1.py
+-rw-r--r--   0        0        0     1220 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/factory.py
+-rw-r--r--   0        0        0      796 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/flow.yml
+-rw-r--r--   0        0        0    11289 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/gateway.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/models/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/models/api.py
+-rw-r--r--   0        0        0     1460 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/models/models.py
+-rw-r--r--   0        0        0    10199 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/retriever.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/__init__.py
+-rw-r--r--   0        0        0     3016 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_json/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_json/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_json/example.json
+-rw-r--r--   0        0        0     5356 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_json/process_json.py
+-rw-r--r--   0        0        0     3091 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_jsonl/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_jsonl/__init__.py
+-rw-r--r--   0        0        0      879 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_jsonl/example.jsonl
+-rw-r--r--   0        0        0     5253 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_jsonl/process_jsonl.py
+-rw-r--r--   0        0        0     2699 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_zip/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_zip/__init__.py
+-rw-r--r--   0        0        0    53296 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_zip/example.zip
+-rw-r--r--   0        0        0     5668 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_zip/process_zip.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/__init__.py
+-rw-r--r--   0        0        0     7609 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/chunks.py
+-rw-r--r--   0        0        0      793 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/date.py
+-rw-r--r--   0        0        0     1201 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/extract_metadata.py
+-rw-r--r--   0        0        0     3674 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/file.py
+-rw-r--r--   0        0        0     1879 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/openai.py
+-rw-r--r--   0        0        0     1350 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/pii_detection.py
+-rw-r--r--   0        0        0      956 2023-07-13 10:07:22.970368 goldretriever-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6076 1970-01-01 00:00:00.000000 goldretriever-0.1.3/PKG-INFO
```

### Comparing `goldretriever-0.1.2/LICENSE` & `goldretriever-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/README.md` & `goldretriever-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # 🐕 Gold Retriever
+>Powered by [Jina](https://github.com/jina-ai/jina) and [DocArray](https://github.com/docarray/docarray)
+
 Easily empower ChatGPT to store and analyze your data using `goldretriever`, a powerful command-line tool for creating and hosting retrieval plugins in just a few simple steps.
 
-![Blog images](https://github.com/jina-ai/GoldRetriever/assets/45267439/7f35d0ed-9ec7-489d-8ab7-ac8ea84d207a)
+![Blog images](https://github.com/jina-ai/GoldRetriever/assets/45267439/e722a8a8-3308-45a4-a7f6-34c71f5a2215)
+
+### 🎬 Showcase: Real-world Plugin Creations
 
+- Personal Study Assistant - [Blog](https://jina.ai/news/gold-retriever-let-chatgpt-talk-to-your-data/) | [Video](https://www.youtube.com/watch?v=gQz-vuo8w5I)
 
 ## ⚡ Quick Start
 
 ### 📦 Installation
 
 1. Ensure you have Python 3.8 or later.
 2. Install the tool via pip:
```

### Comparing `goldretriever-0.1.2/goldretriever/.well-known/ai-plugin.json` & `goldretriever-0.1.3/goldretriever/.well-known/ai-plugin.json`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/.well-known/default-ai-plugin.json` & `goldretriever-0.1.3/goldretriever/.well-known/default-ai-plugin.json`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/.well-known/logo.png` & `goldretriever-0.1.3/goldretriever/.well-known/logo.png`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/.well-known/openapi.yaml` & `goldretriever-0.1.3/goldretriever/.well-known/openapi.yaml`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/datastore/datastore.py` & `goldretriever-0.1.3/goldretriever/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/datastore/executor/docarray_v1.py` & `goldretriever-0.1.3/goldretriever/datastore/executor/docarray_v1.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/datastore/factory.py` & `goldretriever-0.1.3/goldretriever/datastore/factory.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/flow.yml` & `goldretriever-0.1.3/goldretriever/flow.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 jtype: Flow
 version: '1'
 jcloud:
+  docarray: 0.21.0
   name: retrieval-plugin
 gateway:
   protocol: [http]
   uses: jinaai+docker://auth0-unified-b06aa99c0fdac54c/GptRetrievalGateway:latest
   port:
     - 12345
   port_monitoring: 51036
```

### Comparing `goldretriever-0.1.2/goldretriever/gateway.py` & `goldretriever-0.1.3/goldretriever/gateway.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/models/api.py` & `goldretriever-0.1.3/goldretriever/models/api.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/models/models.py` & `goldretriever-0.1.3/goldretriever/models/models.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/retriever.py` & `goldretriever-0.1.3/goldretriever/retriever.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_json/README.md` & `goldretriever-0.1.3/goldretriever/scripts/process_json/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_json/example.json` & `goldretriever-0.1.3/goldretriever/scripts/process_json/example.json`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_json/process_json.py` & `goldretriever-0.1.3/goldretriever/scripts/process_json/process_json.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_jsonl/README.md` & `goldretriever-0.1.3/goldretriever/scripts/process_jsonl/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_jsonl/example.jsonl` & `goldretriever-0.1.3/goldretriever/scripts/process_jsonl/example.jsonl`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_jsonl/process_jsonl.py` & `goldretriever-0.1.3/goldretriever/scripts/process_jsonl/process_jsonl.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_zip/README.md` & `goldretriever-0.1.3/goldretriever/scripts/process_zip/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_zip/example.zip` & `goldretriever-0.1.3/goldretriever/scripts/process_zip/example.zip`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/scripts/process_zip/process_zip.py` & `goldretriever-0.1.3/goldretriever/scripts/process_zip/process_zip.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/services/chunks.py` & `goldretriever-0.1.3/goldretriever/services/chunks.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/services/date.py` & `goldretriever-0.1.3/goldretriever/services/date.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/services/extract_metadata.py` & `goldretriever-0.1.3/goldretriever/services/extract_metadata.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/services/file.py` & `goldretriever-0.1.3/goldretriever/services/file.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/services/openai.py` & `goldretriever-0.1.3/goldretriever/services/openai.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/goldretriever/services/pii_detection.py` & `goldretriever-0.1.3/goldretriever/services/pii_detection.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.2/pyproject.toml` & `goldretriever-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "goldretriever"
-version = "0.1.2"
+version = "0.1.3"
 description = "Create and host retrieval plugins for ChatGPT in one click"
-authors = ["saba <saba.sturua@jina.ai>", "johannes <johannes.messner@jina.ai>"]
+authors = ["Jina AI <hello@jina.ai>"]
 readme = "README.md"
 include = ["goldretriever/**/*"]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = "^0.92.0"
```

### Comparing `goldretriever-0.1.2/PKG-INFO` & `goldretriever-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: goldretriever
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create and host retrieval plugins for ChatGPT in one click
-Author: saba
-Author-email: saba.sturua@jina.ai
+Author: Jina AI
+Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyPDF2 (>=3.0.1,<4.0.0)
@@ -30,18 +30,23 @@
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Requires-Dist: wheel (>=0.37.0,<0.38.0)
 Description-Content-Type: text/markdown
 
 # 🐕 Gold Retriever
+>Powered by [Jina](https://github.com/jina-ai/jina) and [DocArray](https://github.com/docarray/docarray)
+
 Easily empower ChatGPT to store and analyze your data using `goldretriever`, a powerful command-line tool for creating and hosting retrieval plugins in just a few simple steps.
 
-![Blog images](https://github.com/jina-ai/GoldRetriever/assets/45267439/7f35d0ed-9ec7-489d-8ab7-ac8ea84d207a)
+![Blog images](https://github.com/jina-ai/GoldRetriever/assets/45267439/e722a8a8-3308-45a4-a7f6-34c71f5a2215)
+
+### 🎬 Showcase: Real-world Plugin Creations
 
+- Personal Study Assistant - [Blog](https://jina.ai/news/gold-retriever-let-chatgpt-talk-to-your-data/) | [Video](https://www.youtube.com/watch?v=gQz-vuo8w5I)
 
 ## ⚡ Quick Start
 
 ### 📦 Installation
 
 1. Ensure you have Python 3.8 or later.
 2. Install the tool via pip:
```

