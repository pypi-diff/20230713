# Comparing `tmp/pandasai-0.6.8.tar.gz` & `tmp/pandasai-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.6.8.tar", max compression
+gzip compressed data, was "pandasai-0.6.9.tar", max compression
```

## Comparing `pandasai-0.6.8.tar` & `pandasai-0.6.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1055 2023-07-10 23:04:58.032892 pandasai-0.6.8/LICENSE
--rw-r--r--   0        0        0     7705 2023-07-10 23:04:58.032892 pandasai-0.6.8/README.md
--rw-r--r--   0        0        0    25302 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/__init__.py
--rw-r--r--   0        0        0     1235 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3116 2023-07-10 23:04:58.036892 pandasai-0.6.8/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     3507 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4335 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11442 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3176 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1270 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1076 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1081 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1072 2023-07-10 23:04:58.040892 pandasai-0.6.8/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1900 2023-07-10 23:04:58.040892 pandasai-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-12 00:57:07.624913 pandasai-0.6.9/LICENSE
+-rw-r--r--   0        0        0     7705 2023-07-12 00:57:07.624913 pandasai-0.6.9/README.md
+-rw-r--r--   0        0        0    25302 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3116 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     3507 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4335 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11442 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      585 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3176 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1270 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1076 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1081 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1072 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1900 2023-07-12 00:57:07.632917 pandasai-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.6.9/PKG-INFO
```

### Comparing `pandasai-0.6.8/LICENSE` & `pandasai-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/README.md` & `pandasai-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/__init__.py` & `pandasai-0.6.9/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/constants.py` & `pandasai-0.6.9/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/exceptions.py` & `pandasai-0.6.9/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/helpers/_optional.py` & `pandasai-0.6.9/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/helpers/anonymizer.py` & `pandasai-0.6.9/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/helpers/cache.py` & `pandasai-0.6.9/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/helpers/from_excel.py` & `pandasai-0.6.9/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/helpers/notebook.py` & `pandasai-0.6.9/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/helpers/openai_info.py` & `pandasai-0.6.9/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/helpers/save_chart.py` & `pandasai-0.6.9/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/helpers/shortcuts.py` & `pandasai-0.6.9/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/llm/azure_openai.py` & `pandasai-0.6.9/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/llm/base.py` & `pandasai-0.6.9/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/llm/fake.py` & `pandasai-0.6.9/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/llm/falcon.py` & `pandasai-0.6.9/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/llm/google_palm.py` & `pandasai-0.6.9/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/llm/langchain.py` & `pandasai-0.6.9/pandasai/llm/langchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     _langchain_llm = None
 
     def __init__(self, langchain_llm):
         self._langchain_llm = langchain_llm
 
     def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
         prompt = str(instruction) + value + suffix
-        return self._langchain_llm(prompt)
+        return self._langchain_llm.predict(prompt)
 
     @property
     def type(self) -> str:
         return "langchain_" + self._langchain_llm._llm_type
```

### Comparing `pandasai-0.6.8/pandasai/llm/open_assistant.py` & `pandasai-0.6.9/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/llm/openai.py` & `pandasai-0.6.9/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/llm/starcoder.py` & `pandasai-0.6.9/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/middlewares/base.py` & `pandasai-0.6.9/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/middlewares/charts.py` & `pandasai-0.6.9/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/middlewares/streamlit.py` & `pandasai-0.6.9/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/prompts/base.py` & `pandasai-0.6.9/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.6.9/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.6.9/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/prompts/generate_python_code.py` & `pandasai-0.6.9/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.6.9/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.8/pyproject.toml` & `pandasai-0.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.6.8"
+version = "0.6.9"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.6.8/PKG-INFO` & `pandasai-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.6.8
+Version: 0.6.9
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

