# Comparing `tmp/ciderpolarity-0.2.4.tar.gz` & `tmp/ciderpolarity-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciderpolarity-0.2.4.tar", max compression
+gzip compressed data, was "ciderpolarity-0.2.5.tar", max compression
```

## Comparing `ciderpolarity-0.2.4.tar` & `ciderpolarity-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.4/LICENSE
--rw-r--r--   0        0        0     5139 2023-07-13 10:21:11.115976 ciderpolarity-0.2.4/README.md
--rw-r--r--   0        0        0     9384 2023-07-12 14:00:08.052546 ciderpolarity-0.2.4/ciderpolarity/CIDER.py
--rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.4/ciderpolarity/__init__.py
--rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.4/ciderpolarity/create_embeddings.py
--rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.4/ciderpolarity/create_vader.py
--rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.4/ciderpolarity/load_polarities.py
--rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.4/ciderpolarity/run_bootstrapping.py
--rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.4/ciderpolarity/stopwords.py
--rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.4/ciderpolarity/suggest_seeds.py
--rw-r--r--   0        0        0     1138 2023-07-11 14:31:11.901762 ciderpolarity-0.2.4/ciderpolarity/utils_funcs.py
--rw-r--r--   0        0        0      518 2023-07-13 10:21:17.355916 ciderpolarity-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6027 1970-01-01 00:00:00.000000 ciderpolarity-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5139 2023-07-13 10:21:11.115976 ciderpolarity-0.2.5/README.md
+-rw-r--r--   0        0        0     9384 2023-07-12 14:00:08.052546 ciderpolarity-0.2.5/ciderpolarity/CIDER.py
+-rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.5/ciderpolarity/__init__.py
+-rw-r--r--   0        0        0     3260 2023-07-13 12:14:50.023897 ciderpolarity-0.2.5/ciderpolarity/create_embeddings.py
+-rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.5/ciderpolarity/create_vader.py
+-rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.5/ciderpolarity/load_polarities.py
+-rw-r--r--   0        0        0     5331 2023-07-13 12:14:41.635977 ciderpolarity-0.2.5/ciderpolarity/run_bootstrapping.py
+-rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.5/ciderpolarity/stopwords.py
+-rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.5/ciderpolarity/suggest_seeds.py
+-rw-r--r--   0        0        0     1181 2023-07-13 12:14:28.216105 ciderpolarity-0.2.5/ciderpolarity/utils_funcs.py
+-rw-r--r--   0        0        0      518 2023-07-13 12:15:24.147572 ciderpolarity-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6027 1970-01-01 00:00:00.000000 ciderpolarity-0.2.5/PKG-INFO
```

### Comparing `ciderpolarity-0.2.4/LICENSE` & `ciderpolarity-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.4/README.md` & `ciderpolarity-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.4/ciderpolarity/CIDER.py` & `ciderpolarity-0.2.5/ciderpolarity/CIDER.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.4/ciderpolarity/create_embeddings.py` & `ciderpolarity-0.2.5/ciderpolarity/create_embeddings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import numpy as np
 from collections import Counter
 from sklearn.utils.extmath import randomized_svd
 from scipy.sparse.linalg import svds
 from scipy.sparse import diags, lil_matrix
 from gensim.matutils import corpus2csc
 from gensim.corpora import Dictionary
-from tqdm.auto import tqdm
+try:
+    from tqdm.auto import tqdm
+except:
+    from tqdm import tqdm
 from .utils_funcs import text_iterate
 
 
 
 
 def embed_text(SS):
```

### Comparing `ciderpolarity-0.2.4/ciderpolarity/create_vader.py` & `ciderpolarity-0.2.5/ciderpolarity/create_vader.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.4/ciderpolarity/load_polarities.py` & `ciderpolarity-0.2.5/ciderpolarity/load_polarities.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.4/ciderpolarity/run_bootstrapping.py` & `ciderpolarity-0.2.5/ciderpolarity/run_bootstrapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from sklearn import preprocessing
 from collections import Counter
 from scipy import sparse
 import numpy as np
-from tqdm.auto import tqdm
+try:
+    from tqdm.auto import tqdm
+except:
+    from tqdm import tqdm
 import json
 
 
 def propogate_labels(SS):
 
     ### Loading words to keep
     keep = list(SS.KEEP)
```

### Comparing `ciderpolarity-0.2.4/ciderpolarity/stopwords.py` & `ciderpolarity-0.2.5/ciderpolarity/stopwords.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.4/ciderpolarity/suggest_seeds.py` & `ciderpolarity-0.2.5/ciderpolarity/suggest_seeds.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.4/ciderpolarity/utils_funcs.py` & `ciderpolarity-0.2.5/ciderpolarity/utils_funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from tqdm.auto import tqdm
+try:
+    from tqdm.auto import tqdm
+except:
+    from tqdm import tqdm
 import csv
 
 from string import punctuation
 translator = str.maketrans('', '', punctuation)
 
 
 def default_clean_text(SS, doc):
```

### Comparing `ciderpolarity-0.2.4/pyproject.toml` & `ciderpolarity-0.2.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ciderpolarity"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["jcy204 <jcy204@exeter.ac.uk>"]
 readme = "README.md"
 homepage = "https://github.com/jcy204/ciderPolarity"
 repository = "https://github.com/jcy204/ciderPolarity"
 
 [tool.poetry.dependencies]
```

### Comparing `ciderpolarity-0.2.4/PKG-INFO` & `ciderpolarity-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciderpolarity
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Home-page: https://github.com/jcy204/ciderPolarity
 Author: jcy204
 Author-email: jcy204@exeter.ac.uk
 Requires-Python: >=3.7,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

