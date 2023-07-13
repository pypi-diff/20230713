# Comparing `tmp/autoxx-0.0.38.tar.gz` & `tmp/autoxx-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.38.tar", max compression
+gzip compressed data, was "autoxx-0.0.39.tar", max compression
```

## Comparing `autoxx-0.0.38.tar` & `autoxx-0.0.39.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.38/README.md
--rw-r--r--   0        0        0     7808 2023-06-30 08:04:50.564037 autoxx-0.0.38/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.38/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.38/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.38/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.38/autoxx/setup.py
--rw-r--r--   0        0        0     9300 2023-06-28 01:49:25.155903 autoxx-0.0.38/autoxx/tools/knowledge_base/app.py
--rw-r--r--   0        0        0     9024 2023-06-30 09:09:02.593689 autoxx-0.0.38/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      255 2023-06-28 01:49:32.283422 autoxx-0.0.38/autoxx/tools/knowledge_base/prompts/__init__.py
--rw-r--r--   0        0        0      602 2023-06-27 12:55:09.037466 autoxx-0.0.38/autoxx/tools/knowledge_base/prompts/qa
--rw-r--r--   0        0        0      409 2023-06-30 08:58:04.196529 autoxx-0.0.38/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.38/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13277 2023-06-30 08:12:57.916963 autoxx-0.0.38/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.38/autoxx/utils/base.py
--rw-r--r--   0        0        0     3197 2023-06-30 08:58:09.827276 autoxx-0.0.38/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.38/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.38/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.38/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.38/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      683 2023-06-30 09:12:03.071406 autoxx-0.0.38/pyproject.toml
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 autoxx-0.0.38/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.39/README.md
+-rw-r--r--   0        0        0     7808 2023-06-30 08:04:50.564037 autoxx-0.0.39/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.39/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.39/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.39/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.39/autoxx/setup.py
+-rw-r--r--   0        0        0     8797 2023-07-13 11:23:21.080866 autoxx-0.0.39/autoxx/tools/knowledge_base/app.py
+-rw-r--r--   0        0        0     9162 2023-07-13 04:58:33.666381 autoxx-0.0.39/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      255 2023-06-28 01:49:32.283422 autoxx-0.0.39/autoxx/tools/knowledge_base/prompts/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-27 12:55:09.037466 autoxx-0.0.39/autoxx/tools/knowledge_base/prompts/qa
+-rw-r--r--   0        0        0      409 2023-06-30 08:58:04.196529 autoxx-0.0.39/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.39/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13277 2023-06-30 08:12:57.916963 autoxx-0.0.39/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.39/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3197 2023-06-30 08:58:09.827276 autoxx-0.0.39/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.39/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.39/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.39/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.39/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      683 2023-07-13 11:23:56.216923 autoxx-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 autoxx-0.0.39/PKG-INFO
```

### Comparing `autoxx-0.0.38/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.39/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.39/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/agent/react/agent.py` & `autoxx-0.0.39/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/config/config.py` & `autoxx-0.0.39/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/tools/knowledge_base/app.py` & `autoxx-0.0.39/autoxx/tools/knowledge_base/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,27 @@
 from autoxx.utils.processing_text import split_text
 from langchain.chains import HypotheticalDocumentEmbedder
 from autoxx.tools.knowledge_base.prompts import load_prompt
 from langchain.schema import HumanMessage, SystemMessage, AIMessage, BaseMessage
 logger = logging.getLogger(__name__)
 
 class Document(Serializable):
-    id: str = None
-    page_content: str
-    metadata: dict = Field(default_factory=dict)
+    text: str
+    doc_id: str = None
+    extra_info: dict = Field(default_factory=dict)
     score: float = None
 
 class knowleage_application:
     def __init__(self, corpus:str, namespace:Optional[str] = None, model:str = "gpt-3.5-turbo-16k", embedding_model: str="text-embedding-ada-002"):
         if not is_valid_corpus_name(corpus):
             raise ValueError(f"Invalid corpus name: {corpus}. coprus name must consist of lower case alphanumeric characters or '-', and must start and end with an alphanumeric character")
         
         self.corpus = corpus
         self.namespace=namespace
         self._text_key = "text"
-        self._kb_id_key = "_internal_kb_id"
 
         pinecone_api_key = os.getenv("PINECONE_API_KEY")
         assert pinecone_api_key is not None, "Please set PINECONE_API_KEY environment variable"
         pinecone_environment =  os.getenv("PINECONE_ENVIRONMENT") or "us-central1-gcp"
 
         pinecone.init(api_key=pinecone_api_key, environment=pinecone_environment)
         index_list = pinecone.list_indexes()
@@ -54,15 +53,15 @@
         """
         chat_history: list of dict, each dict has two keys: "role" (ai, human, system) and "content"
         """
         docs = self.similarity_search(query, enable_hype)
 
         system_prompt = load_prompt("qa")
         for index, doc in enumerate(docs):
-            system_prompt += f"Document_{index}: {doc.page_content}\n\n"
+            system_prompt += f"Document_{index}: {doc.text}\n\n"
 
         messages = [
             SystemMessage(content=system_prompt),
         ]
 
         if chat_history is not None and len(chat_history) > 0:
             messages.extend(messages_from_dict(chat_history))
@@ -78,74 +77,69 @@
         if enable_hype:
             docs = self.hyde_vectorstore.similarity_search_with_score(query, retrieve_top_k)
         else:
             docs = self.vectorstore.similarity_search_with_score(query, retrieve_top_k)
 
         for doc, score in docs:
             res.append(Document(
-                page_content=doc.page_content,
-                metadata=doc.metadata,
+                doc_id= doc.metadata["doc_id"] if "doc_id" in doc.metadata else None,
+                text=doc.page_content,
+                extra_info=doc.metadata,
                 score=score
             ))
         return res
 
     def upsert_document(self, docs: List[Document]) -> List[str]:
         texts = []
         medadatas = []
         ids = []
         for doc in docs:
-            doc.id = doc.id or str(uuid.uuid4())
-            doc.metadata[self._kb_id_key] = doc.id
-            chunks = [chunk for chunk, _ in (split_text(doc.page_content))]
-            if len(chunks) == 1:
-                texts.append(doc.page_content)
-                medadatas.append(doc.metadata)
-                ids.append(doc.id)
-                continue
-            for chunk_index, chunk in enumerate(chunks):
-                chunk_id = doc.id + f"-{chunk_index}"
-                texts.append(chunk)
-                chunk_metadata = {"chunk_id":chunk_id}
-                chunk_metadata.update(doc.metadata)
-                medadatas.append(chunk_metadata)
-                ids.append(chunk_id)
+            doc.doc_id = doc.doc_id or str(uuid.uuid4())
+            # chunks = [chunk for chunk, _ in (split_text(doc.text))]
+            texts.append(doc.text)
+            medadatas.append(doc.extra_info)
+            ids.append(doc.doc_id)
 
         return self.vectorstore.add_texts(texts, medadatas, ids=ids, namespace=self.namespace)
 
-    def delete_document(self, document_ids: Optional[List[str]] = None, internal_kb_ids: Optional[List[str]]=None) -> None:
+    def delete_document(self, document_ids: Optional[List[str]] = None) -> None:
         if document_ids is not None and len(document_ids) > 0:
             self.vectorstore.delete(
                 ids=document_ids,
             )
         
-        if internal_kb_ids is not None and len(internal_kb_ids) > 0:
+        """
+        if doc_ids is not None and len(doc_ids) > 0:
             self.pinecone_index.delete(
-                filter={self._kb_id_key: {"$in": internal_kb_ids}},
+                filter={"doc_id": {"$in": document_ids}},
                 namespace=self.namespace,
             )
+        """
 
-    def retrieve_document(self, document_ids: Optional[List[str]] = None, internal_kb_ids: Optional[List[str]]=None) ->  List[Document]:
+    def retrieve_document(self, document_ids: Optional[List[str]] = None) ->  List[Document]:
         docs = []
         # use fetch api to fecth specific documents
         if document_ids is not None and len(document_ids) > 0:
             response =  self.pinecone_index.fetch(ids=document_ids, namespace=self.namespace)
             for id, vector in response['vectors'].items():
                 metadata = vector['metadata']
                 if self._text_key in metadata:
                     text = metadata.pop(self._text_key)
-                    docs.append(Document(id=id, page_content=text, metadata=metadata))
+                    docs.append(Document(doc_id=id, text=text, extra_info=metadata))
                 else:
                     logger.warning(
                         f"Found document with no `{self._text_key}` key. Skipping."
                     )
             return docs
 
         filter = None
+        """
         if internal_kb_ids is not None and len(internal_kb_ids) > 0:
             filter={self._kb_id_key: {"$in": internal_kb_ids}}
+        """
 
         # try to load all documents in the index   
         index_description = self.pinecone_index.describe_index_stats()
         vector_count = index_description["total_vector_count"]
         if self.namespace in index_description["namespaces"]:
             vector_count = index_description["namespaces"][self.namespace]["vector_count"]
 
@@ -162,15 +156,15 @@
         )
 
         for res in response["matches"]:
             metadata = res["metadata"]
             id = res["id"]
             if self._text_key in metadata:
                 text = metadata.pop(self._text_key)
-                docs.append(Document(id=id, page_content=text, metadata=metadata))
+                docs.append(Document(doc_id=id, text=text, extra_info=metadata))
             else:
                 logger.warning(
                     f"Found document with no `{self._text_key}` key. Skipping."
                 )
         return docs
 
 def is_valid_corpus_name(corpus_name):
```

### Comparing `autoxx-0.0.38/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.39/autoxx/tools/knowledge_base/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,16 @@
 
         try:
             response = query_engine.query(query)
             logging.info(f"query: {query}, response: {response}, cost: {time.time() - start_time}")
             return response
         except Exception as e:
             print("Error:", e)
+            if "integer division or modulo by zero" in str(e):
+                raise Exception(f"failed to query: empty knowleadge base")
             raise Exception(f"failed to finish query: {str(e)}")
 
     def similarity_search(self, query:str, enable_hype:bool = True, retrieve_top_k:int = 3):
         start_time = time.time()
         query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k)
         if enable_hype:
             hyde = HyDEQueryTransform(include_original=True)
```

### Comparing `autoxx-0.0.38/autoxx/tools/knowledge_base/prompts/qa` & `autoxx-0.0.39/autoxx/tools/knowledge_base/prompts/qa`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.39/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/tools/web_search/search.py` & `autoxx-0.0.39/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/utils/base.py` & `autoxx-0.0.39/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/utils/llm.py` & `autoxx-0.0.39/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/utils/openai_models.py` & `autoxx-0.0.39/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/utils/processing_html.py` & `autoxx-0.0.39/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/utils/processing_text.py` & `autoxx-0.0.39/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/autoxx/utils/token_counter.py` & `autoxx-0.0.39/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.38/pyproject.toml` & `autoxx-0.0.39/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.38"
+version = "0.0.39"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.38/PKG-INFO` & `autoxx-0.0.39/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.38
+Version: 0.0.39
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

