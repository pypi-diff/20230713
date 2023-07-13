# Comparing `tmp/qna-builder-0.1.2.tar.gz` & `tmp/qna-builder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qna-builder-0.1.2.tar", last modified: Tue Jun  6 18:27:44 2023, max compression
+gzip compressed data, was "qna-builder-0.1.3.tar", last modified: Thu Jul 13 02:03:09 2023, max compression
```

## Comparing `qna-builder-0.1.2.tar` & `qna-builder-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:27:44.698556 qna-builder-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-06 18:27:44.698556 qna-builder-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-06 18:27:33.000000 qna-builder-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:27:44.698556 qna-builder-0.1.2/qna_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:27:44.698556 qna-builder-0.1.2/qnabuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 18:27:33.000000 qna-builder-0.1.2/qnabuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 18:27:33.000000 qna-builder-0.1.2/qnabuilder/_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-06 18:27:33.000000 qna-builder-0.1.2/qnabuilder/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-06 18:27:33.000000 qna-builder-0.1.2/qnabuilder/qna_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 18:27:44.698556 qna-builder-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-06 18:27:33.000000 qna-builder-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:03:09.885734 qna-builder-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-13 02:03:09.885734 qna-builder-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-13 02:02:57.000000 qna-builder-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:03:09.885734 qna-builder-0.1.3/qna_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-13 02:03:09.000000 qna-builder-0.1.3/qna_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 02:03:09.000000 qna-builder-0.1.3/qna_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 02:03:09.000000 qna-builder-0.1.3/qna_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 02:03:09.000000 qna-builder-0.1.3/qna_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 02:03:09.000000 qna-builder-0.1.3/qna_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:03:09.885734 qna-builder-0.1.3/qnabuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-13 02:02:57.000000 qna-builder-0.1.3/qnabuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-13 02:02:57.000000 qna-builder-0.1.3/qnabuilder/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-13 02:02:57.000000 qna-builder-0.1.3/qnabuilder/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-13 02:02:57.000000 qna-builder-0.1.3/qnabuilder/qna_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 02:03:09.885734 qna-builder-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-13 02:02:57.000000 qna-builder-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:03:09.885734 qna-builder-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-13 02:02:57.000000 qna-builder-0.1.3/tests/test_qna_bot.py
```

### Comparing `qna-builder-0.1.2/PKG-INFO` & `qna-builder-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 Metadata-Version: 2.1
 Name: qna-builder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Similarity-based conversational dialog engine for Python.
 Home-page: https://github.com/msamsami/qna-builder
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,qna,qnabuilder,chat,chatbot,conversation,dialog
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Communications :: Chat
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: kb_editor
+Provides-Extra: dev
+Provides-Extra: editor
 
 # QnA Builder
 
-![](https://img.shields.io/badge/version-v0.1.2-green)
+![](https://img.shields.io/badge/version-v0.1.3-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/qna-bot/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/qna-builder)](https://pypi.org/project/qna-builder/)
+![](https://img.shields.io/pypi/dm/qna-builder)
 
 <p>
-<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/logo.jpg" alt="QnA Builder logo" width="200"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/docs/logo.jpg" alt="QnA Builder logo" width="200"/>
 <br>
 </p>
 
 ## Introduction
-
-**QnA Builder** is a simple, no code way to build chatbots in Python. It provides a similarity-based conversational dialog
+**QnA Builder** is a simple, no-code way to build chatbots in Python. It provides a similarity-based conversational dialog
 engine, **QnA Bot**, which makes it easy to generate automated responses to input questions according to a set of known
 conversations, i.e., question-answer pairs, stored in a ***knowledge base***. QnA Bot relies on a collection of
-question-answer pairs to generate (predict) answers for new inputs.
+question-answer pairs to generate answers for new inputs.
 
 ## Install
-
 The easiest way to install the qna-builder is by using `pip`:
 ```shell
 pip install qna-builder
 ```
 This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements.
 
 ## Getting started
-
 A QnA Bot can be set up and used in four simple steps:
 
 1. Import `QnABot` class
 
 ```python
 from qnabuilder import QnABot
 ```
@@ -67,39 +66,47 @@
 4. Generate answers
 ```python
 bot.answer("Hey. What's up?")
 ```
 `"All good. What's up with you?"`
 
 ## Algorithms
-
 Currently, QnA Bot engine supports the following algorithms for similarity-based answer generation:
 - TF-IDF Vectorization (`'tfidf'`)
 - Murmurhash3 Vectorization (`'murmurhash'`)
 - Count Vectorization (`'count'`)
 
 Supported similarity metrics are as follows:
 - Cosine similarity (`'cosine'`)
 - Euclidean distance (`'euclidean'`)
 - Manhattan distance (`'manhattan'`)
-- Haversine distance (`'haversine'`)
 
 ## Knowledge base editor
-
 By calling `run_editor()` method of `QnAKnowledgeBase` class, the knowledge base editor window will open up in
 your web browser and allows you to edit your knowledge base by adding, removing, or modifying questions/answers.
 
 ```python
 from qnabuilder import QnAKnowledgeBase
 
 kb = QnAKnowledgeBase('my_knowledge_base.json')
 kb.run_editor()
 ```
 
 Here, you can see a screenshot of the knowledge base editor:
 
 <div style="text-align:center">
-<img src="docs/kb_editor.png" alt="QnA Bot Knowledge Base Editor" width="450"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/docs/kb_editor.png" alt="QnA Bot Knowledge Base Editor" width="450"/>
 </div>
 
 Note that you need to install the optional requirement [streamlit](https://streamlit.io/) to be able to use the
 knowledge base editor.
+
+## Tests
+To run the tests, install development requirements:
+```
+pip install -r requirements_dev.txt
+```
+
+Then, run pytest:
+```
+pytest
+```
```

### Comparing `qna-builder-0.1.2/README.md` & `qna-builder-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # QnA Builder
 
-![](https://img.shields.io/badge/version-v0.1.2-green)
+![](https://img.shields.io/badge/version-v0.1.3-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/qna-bot/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/qna-builder)](https://pypi.org/project/qna-builder/)
+![](https://img.shields.io/pypi/dm/qna-builder)
 
 <p>
-<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/logo.jpg" alt="QnA Builder logo" width="200"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/docs/logo.jpg" alt="QnA Builder logo" width="200"/>
 <br>
 </p>
 
 ## Introduction
-
-**QnA Builder** is a simple, no code way to build chatbots in Python. It provides a similarity-based conversational dialog
+**QnA Builder** is a simple, no-code way to build chatbots in Python. It provides a similarity-based conversational dialog
 engine, **QnA Bot**, which makes it easy to generate automated responses to input questions according to a set of known
 conversations, i.e., question-answer pairs, stored in a ***knowledge base***. QnA Bot relies on a collection of
-question-answer pairs to generate (predict) answers for new inputs.
+question-answer pairs to generate answers for new inputs.
 
 ## Install
-
 The easiest way to install the qna-builder is by using `pip`:
 ```shell
 pip install qna-builder
 ```
 This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements.
 
 ## Getting started
-
 A QnA Bot can be set up and used in four simple steps:
 
 1. Import `QnABot` class
 
 ```python
 from qnabuilder import QnABot
 ```
@@ -48,39 +46,47 @@
 4. Generate answers
 ```python
 bot.answer("Hey. What's up?")
 ```
 `"All good. What's up with you?"`
 
 ## Algorithms
-
 Currently, QnA Bot engine supports the following algorithms for similarity-based answer generation:
 - TF-IDF Vectorization (`'tfidf'`)
 - Murmurhash3 Vectorization (`'murmurhash'`)
 - Count Vectorization (`'count'`)
 
 Supported similarity metrics are as follows:
 - Cosine similarity (`'cosine'`)
 - Euclidean distance (`'euclidean'`)
 - Manhattan distance (`'manhattan'`)
-- Haversine distance (`'haversine'`)
 
 ## Knowledge base editor
-
 By calling `run_editor()` method of `QnAKnowledgeBase` class, the knowledge base editor window will open up in
 your web browser and allows you to edit your knowledge base by adding, removing, or modifying questions/answers.
 
 ```python
 from qnabuilder import QnAKnowledgeBase
 
 kb = QnAKnowledgeBase('my_knowledge_base.json')
 kb.run_editor()
 ```
 
 Here, you can see a screenshot of the knowledge base editor:
 
 <div style="text-align:center">
-<img src="docs/kb_editor.png" alt="QnA Bot Knowledge Base Editor" width="450"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/docs/kb_editor.png" alt="QnA Bot Knowledge Base Editor" width="450"/>
 </div>
 
 Note that you need to install the optional requirement [streamlit](https://streamlit.io/) to be able to use the
-knowledge base editor.
+knowledge base editor.
+
+## Tests
+To run the tests, install development requirements:
+```
+pip install -r requirements_dev.txt
+```
+
+Then, run pytest:
+```
+pytest
+```
```

### Comparing `qna-builder-0.1.2/qna_builder.egg-info/PKG-INFO` & `qna-builder-0.1.3/qna_builder.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 Metadata-Version: 2.1
 Name: qna-builder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Similarity-based conversational dialog engine for Python.
 Home-page: https://github.com/msamsami/qna-builder
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,qna,qnabuilder,chat,chatbot,conversation,dialog
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Communications :: Chat
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: kb_editor
+Provides-Extra: dev
+Provides-Extra: editor
 
 # QnA Builder
 
-![](https://img.shields.io/badge/version-v0.1.2-green)
+![](https://img.shields.io/badge/version-v0.1.3-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/qna-bot/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/qna-builder)](https://pypi.org/project/qna-builder/)
+![](https://img.shields.io/pypi/dm/qna-builder)
 
 <p>
-<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/logo.jpg" alt="QnA Builder logo" width="200"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/docs/logo.jpg" alt="QnA Builder logo" width="200"/>
 <br>
 </p>
 
 ## Introduction
-
-**QnA Builder** is a simple, no code way to build chatbots in Python. It provides a similarity-based conversational dialog
+**QnA Builder** is a simple, no-code way to build chatbots in Python. It provides a similarity-based conversational dialog
 engine, **QnA Bot**, which makes it easy to generate automated responses to input questions according to a set of known
 conversations, i.e., question-answer pairs, stored in a ***knowledge base***. QnA Bot relies on a collection of
-question-answer pairs to generate (predict) answers for new inputs.
+question-answer pairs to generate answers for new inputs.
 
 ## Install
-
 The easiest way to install the qna-builder is by using `pip`:
 ```shell
 pip install qna-builder
 ```
 This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements.
 
 ## Getting started
-
 A QnA Bot can be set up and used in four simple steps:
 
 1. Import `QnABot` class
 
 ```python
 from qnabuilder import QnABot
 ```
@@ -67,39 +66,47 @@
 4. Generate answers
 ```python
 bot.answer("Hey. What's up?")
 ```
 `"All good. What's up with you?"`
 
 ## Algorithms
-
 Currently, QnA Bot engine supports the following algorithms for similarity-based answer generation:
 - TF-IDF Vectorization (`'tfidf'`)
 - Murmurhash3 Vectorization (`'murmurhash'`)
 - Count Vectorization (`'count'`)
 
 Supported similarity metrics are as follows:
 - Cosine similarity (`'cosine'`)
 - Euclidean distance (`'euclidean'`)
 - Manhattan distance (`'manhattan'`)
-- Haversine distance (`'haversine'`)
 
 ## Knowledge base editor
-
 By calling `run_editor()` method of `QnAKnowledgeBase` class, the knowledge base editor window will open up in
 your web browser and allows you to edit your knowledge base by adding, removing, or modifying questions/answers.
 
 ```python
 from qnabuilder import QnAKnowledgeBase
 
 kb = QnAKnowledgeBase('my_knowledge_base.json')
 kb.run_editor()
 ```
 
 Here, you can see a screenshot of the knowledge base editor:
 
 <div style="text-align:center">
-<img src="docs/kb_editor.png" alt="QnA Bot Knowledge Base Editor" width="450"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/docs/kb_editor.png" alt="QnA Bot Knowledge Base Editor" width="450"/>
 </div>
 
 Note that you need to install the optional requirement [streamlit](https://streamlit.io/) to be able to use the
 knowledge base editor.
+
+## Tests
+To run the tests, install development requirements:
+```
+pip install -r requirements_dev.txt
+```
+
+Then, run pytest:
+```
+pytest
+```
```

### Comparing `qna-builder-0.1.2/qnabuilder/__init__.py` & `qna-builder-0.1.3/qnabuilder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-qna-bot is a similarity-based conversational dialog engine for Python that helps you quickly and easily create
+QnA Builder is a similarity-based conversational dialog engine for Python that helps you quickly and easily create
 smart chatbots using a knowledge base of pre-defined questions and answers.
 """
 
 __version__ = "0.1.2"
 __author__ = "Mehdi Samsami"
 
-__all__ = [
+__all__ = (
     "QnABot",
     "EmbeddingModel",
     "SimilarityMetric",
     "QnAKnowledgeBase",
-    "DEFAULT_KNOWLEDGE_BASE_FILE_PATH"
-]
+    "DEFAULT_KNOWLEDGE_BASE_FILE_PATH",
+)
 
 
 from .qna_bot import QnABot
-from ._enum import EmbeddingModel, SimilarityMetric
+from ._enums import EmbeddingModel, SimilarityMetric
 from .kb import QnAKnowledgeBase, DEFAULT_KNOWLEDGE_BASE_FILE_PATH
```

### Comparing `qna-builder-0.1.2/qnabuilder/_utils.py` & `qna-builder-0.1.3/qnabuilder/_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from typing import Any
 
 
 def parse_list_options(options: list) -> str:
     """Returns the parsed version of a list of options in string.
 
     Args:
-        options (list): a list of options, parameters, or items to be parsed.
+        options (list): A list of options, parameters, or items to be parsed.
 
     Returns:
-        str: comma-separated sequence of options with an 'or' after the last comma.
+        str: Comma-separated sequence of options with an 'or' after the last comma.
     """
-    check_type_error('options', options, list())
+    check_type_error("options", options, list())
 
-    options_str = ', '.join([str(option) for option in options])
-    last_comma_idx = options_str.rfind(',')
+    options_str = ", ".join([str(option) for option in options])
+    last_comma_idx = options_str.rfind(",")
 
     if len(options) == 2:
-        return options_str[:last_comma_idx] + ' or' + options_str[last_comma_idx + 1:]
+        return options_str[:last_comma_idx] + " or" + options_str[last_comma_idx + 1 :]
     else:
-        return options_str[:last_comma_idx + 2] + 'or' + options_str[last_comma_idx + 1:]
+        return (
+            options_str[: last_comma_idx + 2] + "or" + options_str[last_comma_idx + 1 :]
+        )
 
 
 def value_error_message(name: str, value: Any, options: list) -> str:
     if len(options) == 1:
         return f"{value} is not a valid {name}. Only {options[0]} is supported"
     else:
         return f"{value} is not a valid {name}. Must be either {parse_list_options(options)}"
```

### Comparing `qna-builder-0.1.2/qnabuilder/qna_bot.py` & `qna-builder-0.1.3/qnabuilder/qna_bot.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,52 +4,43 @@
 from scipy.sparse import csr_matrix
 
 from sklearn.exceptions import NotFittedError
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.feature_extraction.text import (
     TfidfVectorizer,
     HashingVectorizer,
-    CountVectorizer
+    CountVectorizer,
 )
 from sklearn.metrics.pairwise import (
     cosine_similarity,
     euclidean_distances,
     manhattan_distances,
-    haversine_distances
+    haversine_distances,
 )
 
 from .kb import QnAKnowledgeBase, FilePath, DEFAULT_KNOWLEDGE_BASE_FILE_PATH
-from ._enum import EmbeddingModel, SimilarityMetric
-
-
-similarity = {
-    'cosine': cosine_similarity,
-    'euclidean': euclidean_distances,
-    'manhattan': manhattan_distances,
-    'haversine': haversine_distances
-}
+from ._enums import EmbeddingModel, SimilarityMetric
+from ._utils import value_error_message
 
 
 class QnABot:
     _is_fitted: bool = False
     _model_kwargs: dict = {}
 
-    _params = {
-        "kb": None,
-        "model": None,
-        "ref_embeddings": None
-    }
-
-    def __init__(self,
-                 model_name: Union[str, EmbeddingModel] = "tfidf",
-                 similarity_metric: Union[str, SimilarityMetric] = "cosine",
-                 min_score: float = 0.25,
-                 cache: bool = False,
-                 **kwargs) -> None:
-        """Initializes an instance of the class.
+    _params = {"kb": None, "model": None, "ref_embeddings": None}
+
+    def __init__(
+        self,
+        model_name: Union[str, EmbeddingModel] = "tfidf",
+        similarity_metric: Union[str, SimilarityMetric] = "cosine",
+        min_score: float = 0.25,
+        cache: bool = False,
+        **kwargs
+    ) -> None:
+        """Initializes an instance of the QnABot class.
 
         Args:
             model_name (Union[str, EmbeddingModel]): Name of the model used for text embedding. Defaults to 'tfidf'.
             similarity_metric (Union[str, SimilarityMetric]): Similarity metric used to find the most similar question.
                                                               Defaults to 'cosine'.
             min_score (float): Minimum similarity score below which an "I don't know" answer will be returned.
                                Defaults to 0.25.
@@ -62,79 +53,116 @@
         self.min_score: float = min_score
         self.cache: bool = cache
 
         self._model_kwargs = kwargs
 
     @staticmethod
     def _initialize_model(model_name: str, **kwargs):
-        if model_name == 'tfidf':
+        if model_name == "tfidf":
             return TfidfVectorizer(**kwargs)
-        elif model_name == 'murmurhash':
+        elif model_name == "murmurhash":
             return HashingVectorizer(**kwargs)
-        elif model_name == 'count':
+        elif model_name == "count":
             return CountVectorizer(**kwargs)
         else:
-            return None
-
-    def fit(self, kb: Union[FilePath, QnAKnowledgeBase] = DEFAULT_KNOWLEDGE_BASE_FILE_PATH):
+            raise ValueError(
+                value_error_message(
+                    "model_name", model_name, [e.value for e in EmbeddingModel]
+                )
+            )
+
+    def fit(
+        self, kb: Union[FilePath, QnAKnowledgeBase] = DEFAULT_KNOWLEDGE_BASE_FILE_PATH
+    ):
         """Fits QnA Bot to a given knowledge base.
 
         Args:
             kb (Union[FilePath, QnAKnowledgeBase]): Path to the knowledge base JSON file or buffer, or a
                                                     QnAKnowledgeBase object. Defaults to the file path of the default
                                                     QnA Bot knowledge base.
 
         Returns:
             self: The instance itself.
         """
         self._is_fitted = False
-        self._params["kb"] = kb if isinstance(kb, QnAKnowledgeBase) else QnAKnowledgeBase(kb, self.cache)
-        self._params["model"] = self._initialize_model(model_name=self.model_name, **self._model_kwargs)
+        self._params["kb"] = (
+            kb if isinstance(kb, QnAKnowledgeBase) else QnAKnowledgeBase(kb, self.cache)
+        )
+        self._params["model"] = self._initialize_model(
+            model_name=self.model_name, **self._model_kwargs
+        )
         self._params["model"].fit(self.knowledge_base_.ref_questions)
-        self._params["ref_embeddings"] = self.model_.transform(self.knowledge_base_.ref_questions)
+        self._params["ref_embeddings"] = self.model_.transform(
+            self.knowledge_base_.ref_questions
+        )
 
         self._is_fitted = True
         return self
 
+    @property
+    def _similarity_function(self):
+        functions = {
+            "cosine": cosine_similarity,
+            "euclidean": euclidean_distances,
+            "manhattan": manhattan_distances,
+        }
+
+        if self.similarity_metric not in functions:
+            raise ValueError(
+                value_error_message(
+                    "similarity_metric",
+                    self.similarity_metric,
+                    [e.value for e in SimilarityMetric],
+                )
+            )
+        else:
+            return functions[self.similarity_metric]
+
     def find_similarity(self, input: str) -> Tuple[int, float]:
         """Returns the index and similarity score of the question in the knowledge base most similar to the input.
 
         Args:
             input (str): Input question.
 
         Returns:
             int: Index of the most similar question.
             float: Similarity score of the most similar question.
         """
         if not self._is_fitted:
-            raise NotFittedError('The model is not fitted. Use fit() method before calling answer()')
+            raise NotFittedError(
+                "The model is not fitted. Use fit() method before calling answer()"
+            )
 
         # Retrieve questions' indices from knowledge base
         q_idx = self.knowledge_base_.ref_questions_idx
 
         # Extract input statement embedding
         input_embeddings = self.model_.transform([input])
 
         # Calculate the similarities between the input embedding and the reference embeddings
-        similarities = similarity[self.similarity_metric](input_embeddings, self.ref_embeddings_).flatten()
+        similarities = self._similarity_function(
+            input_embeddings, self.ref_embeddings_
+        ).flatten()
 
-        if self.similarity_metric != 'cosine':
+        if self.similarity_metric != "cosine":
             similarities = MinMaxScaler().fit_transform(similarities.reshape(-1, 1))
             similarities = 1.0 - similarities.flatten()
 
         # Find the score of the answer with the highest score
         highest_id = int(np.argmax(similarities))
         score = float(similarities[highest_id])
 
         # Find the ID of the answer with the highest score
         highest_qna_id = q_idx[highest_id]
 
         return highest_qna_id, score
 
-    def answer(self, input: str, return_score: bool = False) -> Union[str, Tuple[str, float]]:
+    def answer(
+        self, input: str, return_score: bool = False
+    ) -> Union[str, Tuple[str, float]]:
         """Returns the index and similarity score of a question in the knowledge base that is most similar to the input.
 
         Args:
             input (str): Input question.
             return_score (bool): Whether to return the similarity score. Defaults to False.
 
         Returns:
@@ -148,15 +176,15 @@
         # If score was lower than the minimum accepted value
         if score < self.min_score:
             # Return a random "I don't know" answer
             answer_ = np.random.choice(self.knowledge_base_.idk_answers)
 
         else:
             # Pick a random answer among the answers of the most similar question
-            answer_ = np.random.choice(self.knowledge_base_.qna[highest_id]['a'])
+            answer_ = np.random.choice(self.knowledge_base_.qna[highest_id]["a"])
 
         if return_score:
             return answer_, score
         else:
             return answer_
 
     @property
@@ -177,9 +205,16 @@
     def ref_embeddings_(self) -> csr_matrix:
         """Returns the embedding matrix extracted from reference questions in the knowledge base.
 
         """
         return self._params["ref_embeddings"]
 
     def __repr__(self):
-        return "<QnABot(model_name='%s', similarity_metric='%s', min_score=%.2f, cache=%s)>" % \
-               (str(self.model_name), str(self.similarity_metric), self.min_score, self.cache)
+        return (
+            "<QnABot(model_name='%s', similarity_metric='%s', min_score=%.2f, cache=%s)>"
+            % (
+                str(self.model_name),
+                str(self.similarity_metric),
+                self.min_score,
+                self.cache,
+            )
+        )
```

