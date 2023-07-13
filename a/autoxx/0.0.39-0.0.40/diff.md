# Comparing `tmp/autoxx-0.0.39.tar.gz` & `tmp/autoxx-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.39.tar", max compression
+gzip compressed data, was "autoxx-0.0.40.tar", max compression
```

## Comparing `autoxx-0.0.39.tar` & `autoxx-0.0.40.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.39/README.md
--rw-r--r--   0        0        0     7808 2023-06-30 08:04:50.564037 autoxx-0.0.39/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.39/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.39/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.39/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.39/autoxx/setup.py
--rw-r--r--   0        0        0     8797 2023-07-13 11:23:21.080866 autoxx-0.0.39/autoxx/tools/knowledge_base/app.py
--rw-r--r--   0        0        0     9162 2023-07-13 04:58:33.666381 autoxx-0.0.39/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      255 2023-06-28 01:49:32.283422 autoxx-0.0.39/autoxx/tools/knowledge_base/prompts/__init__.py
--rw-r--r--   0        0        0      602 2023-06-27 12:55:09.037466 autoxx-0.0.39/autoxx/tools/knowledge_base/prompts/qa
--rw-r--r--   0        0        0      409 2023-06-30 08:58:04.196529 autoxx-0.0.39/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.39/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13277 2023-06-30 08:12:57.916963 autoxx-0.0.39/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.39/autoxx/utils/base.py
--rw-r--r--   0        0        0     3197 2023-06-30 08:58:09.827276 autoxx-0.0.39/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.39/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.39/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.39/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.39/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      683 2023-07-13 11:23:56.216923 autoxx-0.0.39/pyproject.toml
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 autoxx-0.0.39/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.40/README.md
+-rw-r--r--   0        0        0     7808 2023-06-30 08:04:50.564037 autoxx-0.0.40/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.40/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.40/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.40/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.40/autoxx/setup.py
+-rw-r--r--   0        0        0     8929 2023-07-13 12:31:55.585029 autoxx-0.0.40/autoxx/tools/knowledge_base/app.py
+-rw-r--r--   0        0        0     9162 2023-07-13 04:58:33.666381 autoxx-0.0.40/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      255 2023-06-28 01:49:32.283422 autoxx-0.0.40/autoxx/tools/knowledge_base/prompts/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-27 12:55:09.037466 autoxx-0.0.40/autoxx/tools/knowledge_base/prompts/qa
+-rw-r--r--   0        0        0      409 2023-06-30 08:58:04.196529 autoxx-0.0.40/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.40/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13277 2023-06-30 08:12:57.916963 autoxx-0.0.40/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.40/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3197 2023-06-30 08:58:09.827276 autoxx-0.0.40/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.40/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.40/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.40/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.40/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      683 2023-07-13 12:31:30.466944 autoxx-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 autoxx-0.0.40/PKG-INFO
```

### Comparing `autoxx-0.0.39/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.40/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.40/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/agent/react/agent.py` & `autoxx-0.0.40/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/config/config.py` & `autoxx-0.0.40/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/tools/knowledge_base/app.py` & `autoxx-0.0.40/autoxx/tools/knowledge_base/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
 
     def query(self, query:str, enable_hype:bool = True, chat_history: Optional[list[dict[str, str]]]=None):
         """
         chat_history: list of dict, each dict has two keys: "role" (ai, human, system) and "content"
         """
         docs = self.similarity_search(query, enable_hype)
+        if len(docs) == 0:
+            return {"answer": None, "reference": docs}
 
         system_prompt = load_prompt("qa")
         for index, doc in enumerate(docs):
             system_prompt += f"Document_{index}: {doc.text}\n\n"
 
         messages = [
             SystemMessage(content=system_prompt),
@@ -91,14 +93,15 @@
     def upsert_document(self, docs: List[Document]) -> List[str]:
         texts = []
         medadatas = []
         ids = []
         for doc in docs:
             doc.doc_id = doc.doc_id or str(uuid.uuid4())
             # chunks = [chunk for chunk, _ in (split_text(doc.text))]
+            doc.extra_info["doc_id"] = doc.doc_id
             texts.append(doc.text)
             medadatas.append(doc.extra_info)
             ids.append(doc.doc_id)
 
         return self.vectorstore.add_texts(texts, medadatas, ids=ids, namespace=self.namespace)
 
     def delete_document(self, document_ids: Optional[List[str]] = None) -> None:
```

### Comparing `autoxx-0.0.39/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.40/autoxx/tools/knowledge_base/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/tools/knowledge_base/prompts/qa` & `autoxx-0.0.40/autoxx/tools/knowledge_base/prompts/qa`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.40/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/tools/web_search/search.py` & `autoxx-0.0.40/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/utils/base.py` & `autoxx-0.0.40/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/utils/llm.py` & `autoxx-0.0.40/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/utils/openai_models.py` & `autoxx-0.0.40/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/utils/processing_html.py` & `autoxx-0.0.40/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/utils/processing_text.py` & `autoxx-0.0.40/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/autoxx/utils/token_counter.py` & `autoxx-0.0.40/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.39/pyproject.toml` & `autoxx-0.0.40/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.39"
+version = "0.0.40"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.39/PKG-INFO` & `autoxx-0.0.40/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.39
+Version: 0.0.40
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

