# Comparing `tmp/ciderpolarity-0.2.3.tar.gz` & `tmp/ciderpolarity-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciderpolarity-0.2.3.tar", max compression
+gzip compressed data, was "ciderpolarity-0.2.4.tar", max compression
```

## Comparing `ciderpolarity-0.2.3.tar` & `ciderpolarity-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.3/LICENSE
--rw-r--r--   0        0        0     4354 2023-07-12 14:24:52.744113 ciderpolarity-0.2.3/README.md
--rw-r--r--   0        0        0     9384 2023-07-12 14:00:08.052546 ciderpolarity-0.2.3/ciderpolarity/CIDER.py
--rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.3/ciderpolarity/__init__.py
--rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.3/ciderpolarity/create_embeddings.py
--rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.3/ciderpolarity/create_vader.py
--rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.3/ciderpolarity/load_polarities.py
--rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.3/ciderpolarity/run_bootstrapping.py
--rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.3/ciderpolarity/stopwords.py
--rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.3/ciderpolarity/suggest_seeds.py
--rw-r--r--   0        0        0     1138 2023-07-11 14:31:11.901762 ciderpolarity-0.2.3/ciderpolarity/utils_funcs.py
--rw-r--r--   0        0        0      518 2023-07-12 14:09:31.471572 ciderpolarity-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 ciderpolarity-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5139 2023-07-13 10:21:11.115976 ciderpolarity-0.2.4/README.md
+-rw-r--r--   0        0        0     9384 2023-07-12 14:00:08.052546 ciderpolarity-0.2.4/ciderpolarity/CIDER.py
+-rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.4/ciderpolarity/__init__.py
+-rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.4/ciderpolarity/create_embeddings.py
+-rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.4/ciderpolarity/create_vader.py
+-rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.4/ciderpolarity/load_polarities.py
+-rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.4/ciderpolarity/run_bootstrapping.py
+-rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.4/ciderpolarity/stopwords.py
+-rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.4/ciderpolarity/suggest_seeds.py
+-rw-r--r--   0        0        0     1138 2023-07-11 14:31:11.901762 ciderpolarity-0.2.4/ciderpolarity/utils_funcs.py
+-rw-r--r--   0        0        0      518 2023-07-13 10:21:17.355916 ciderpolarity-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6027 1970-01-01 00:00:00.000000 ciderpolarity-0.2.4/PKG-INFO
```

### Comparing `ciderpolarity-0.2.3/LICENSE` & `ciderpolarity-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/README.md` & `ciderpolarity-0.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 The approach taken to generate polarities is taken from [SocialSent](https://github.com/williamleif/socialsent).
 
 ## Contents
 
 - [Installation](#installation)
 - [Overview](#overview)
 - [Examples](#examples)
-
+- [Alternative Scales](#alternativescales)
 
 ## Installation
 
 Before you begin, ensure you have met the following requirements:
 
 * You have installed Python 3.7 or later.
 * You have a Windows/Linux/Mac machine.
@@ -86,15 +86,15 @@
 
 ```python
 cdr_example.fit()
 ```
 
 And the resulting polarities (before filtering and scaling) can be viewed:
 
-<img src="https://github.com/jcy204/ciderPolarity/blob/main/cdr_out_example.png?raw=true" alt="drawing" width="500"/>
+<img src="https://github.com/jcy204/ciderPolarity/blob/main/figs/cdr_out_example.png?raw=true" alt="drawing" width="500"/>
 
 ___
 
 ### Generating Seedwords
 
 Whilst CIDER has built in seed words (found [here](ciderpolarity/suggest_seeds.py)), custom seed words can be generated and suggested. The following shows how this is carried out:
 
@@ -103,7 +103,24 @@
 ```
 Which looks at strongly polarised words which occur both often, are close to one seed set, and distant from the opposing seed set.
 
 The following returns all words in the data, alongside their seed word suitability.
 ```python
 df = cdr_example.generate_seeds(['good','brilliant','love'],['bad','terrible','hate'], return_all = True, sentiment = True)
 ```
+
+## Alternative Scales
+
+CIDER is not limited to sentiment. By initiating the model with alternative sets of seed words, non-intuitive linguistic scales can be produced. For instance:
+```python
+from ciderpolarity import CIDER
+
+input_data = 'test_data.csv'
+output_folder = '/path/to/output/folder/'
+
+cdr = CIDER(input_data, output_folder, predefined_seeds = 'gender')
+cdr.fit()
+```
+The above creates a linguistic scale based off of proximity to gendered seed words (i.e. 'he', 'him', 'brother' and 'she', 'her', 'sister').
+Below shows a sample output for this scale when applied to all of the tweets from the UK in 2020.
+<img src="https://github.com/jcy204/ciderPolarity/blob/main/figs/genderpols.png?raw=true" alt="drawing" width="850"/>
+
```

### Comparing `ciderpolarity-0.2.3/ciderpolarity/CIDER.py` & `ciderpolarity-0.2.4/ciderpolarity/CIDER.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/ciderpolarity/create_embeddings.py` & `ciderpolarity-0.2.4/ciderpolarity/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/ciderpolarity/create_vader.py` & `ciderpolarity-0.2.4/ciderpolarity/create_vader.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/ciderpolarity/load_polarities.py` & `ciderpolarity-0.2.4/ciderpolarity/load_polarities.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/ciderpolarity/run_bootstrapping.py` & `ciderpolarity-0.2.4/ciderpolarity/run_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/ciderpolarity/stopwords.py` & `ciderpolarity-0.2.4/ciderpolarity/stopwords.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/ciderpolarity/suggest_seeds.py` & `ciderpolarity-0.2.4/ciderpolarity/suggest_seeds.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/ciderpolarity/utils_funcs.py` & `ciderpolarity-0.2.4/ciderpolarity/utils_funcs.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.3/pyproject.toml` & `ciderpolarity-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ciderpolarity"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["jcy204 <jcy204@exeter.ac.uk>"]
 readme = "README.md"
 homepage = "https://github.com/jcy204/ciderPolarity"
 repository = "https://github.com/jcy204/ciderPolarity"
 
 [tool.poetry.dependencies]
```

### Comparing `ciderpolarity-0.2.3/PKG-INFO` & `ciderpolarity-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciderpolarity
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Home-page: https://github.com/jcy204/ciderPolarity
 Author: jcy204
 Author-email: jcy204@exeter.ac.uk
 Requires-Python: >=3.7,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,15 +30,15 @@
 The approach taken to generate polarities is taken from [SocialSent](https://github.com/williamleif/socialsent).
 
 ## Contents
 
 - [Installation](#installation)
 - [Overview](#overview)
 - [Examples](#examples)
-
+- [Alternative Scales](#alternativescales)
 
 ## Installation
 
 Before you begin, ensure you have met the following requirements:
 
 * You have installed Python 3.7 or later.
 * You have a Windows/Linux/Mac machine.
@@ -110,15 +110,15 @@
 
 ```python
 cdr_example.fit()
 ```
 
 And the resulting polarities (before filtering and scaling) can be viewed:
 
-<img src="https://github.com/jcy204/ciderPolarity/blob/main/cdr_out_example.png?raw=true" alt="drawing" width="500"/>
+<img src="https://github.com/jcy204/ciderPolarity/blob/main/figs/cdr_out_example.png?raw=true" alt="drawing" width="500"/>
 
 ___
 
 ### Generating Seedwords
 
 Whilst CIDER has built in seed words (found [here](ciderpolarity/suggest_seeds.py)), custom seed words can be generated and suggested. The following shows how this is carried out:
 
@@ -128,7 +128,24 @@
 Which looks at strongly polarised words which occur both often, are close to one seed set, and distant from the opposing seed set.
 
 The following returns all words in the data, alongside their seed word suitability.
 ```python
 df = cdr_example.generate_seeds(['good','brilliant','love'],['bad','terrible','hate'], return_all = True, sentiment = True)
 ```
 
+## Alternative Scales
+
+CIDER is not limited to sentiment. By initiating the model with alternative sets of seed words, non-intuitive linguistic scales can be produced. For instance:
+```python
+from ciderpolarity import CIDER
+
+input_data = 'test_data.csv'
+output_folder = '/path/to/output/folder/'
+
+cdr = CIDER(input_data, output_folder, predefined_seeds = 'gender')
+cdr.fit()
+```
+The above creates a linguistic scale based off of proximity to gendered seed words (i.e. 'he', 'him', 'brother' and 'she', 'her', 'sister').
+Below shows a sample output for this scale when applied to all of the tweets from the UK in 2020.
+<img src="https://github.com/jcy204/ciderPolarity/blob/main/figs/genderpols.png?raw=true" alt="drawing" width="850"/>
+
+
```

