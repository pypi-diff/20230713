# Comparing `tmp/BERTSimilar-0.1.0.tar.gz` & `tmp/BERTSimilar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BERTSimilar-0.1.0.tar", last modified: Thu Jul 13 00:25:53 2023, max compression
+gzip compressed data, was "BERTSimilar-0.1.1.tar", last modified: Thu Jul 13 00:46:04 2023, max compression
```

## Comparing `BERTSimilar-0.1.0.tar` & `BERTSimilar-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:25:53.092534 BERTSimilar-0.1.0/
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:25:53.091153 BERTSimilar-0.1.0/BERTSimilar/
--rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.0/BERTSimilar/__init__.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:25:53.092090 BERTSimilar-0.1.0/BERTSimilar.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)    11579 2023-07-13 00:25:53.000000 BERTSimilar-0.1.0/BERTSimilar.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      228 2023-07-13 00:25:53.000000 BERTSimilar-0.1.0/BERTSimilar.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-13 00:25:53.000000 BERTSimilar-0.1.0/BERTSimilar.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      147 2023-07-13 00:25:53.000000 BERTSimilar-0.1.0/BERTSimilar.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-13 00:25:53.000000 BERTSimilar-0.1.0/BERTSimilar.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.0/LICENSE.txt
--rw-r--r--   0 rdp        (501) staff       (20)    11579 2023-07-13 00:25:53.092329 BERTSimilar-0.1.0/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)    11055 2023-01-07 23:48:06.000000 BERTSimilar-0.1.0/README.md
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-13 00:25:53.092588 BERTSimilar-0.1.0/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-13 00:22:24.000000 BERTSimilar-0.1.0/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:46:04.744695 BERTSimilar-0.1.1/
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:46:04.742816 BERTSimilar-0.1.1/BERTSimilar/
+-rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.1/BERTSimilar/__init__.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:46:04.743790 BERTSimilar-0.1.1/BERTSimilar.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      228 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      147 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.1/LICENSE.txt
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-13 00:46:04.744114 BERTSimilar-0.1.1/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.1/README.md
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-13 00:46:04.744755 BERTSimilar-0.1.1/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-13 00:45:38.000000 BERTSimilar-0.1.1/setup.py
```

### Comparing `BERTSimilar-0.1.0/BERTSimilar.egg-info/PKG-INFO` & `BERTSimilar-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,69 @@
-Metadata-Version: 2.1
-Name: BERTSimilar
-Version: 0.1.0
-Summary: Get Similar Words and Embeddings using BERT Models
-Home-page: https://github.com/rdpahalavan/BERTSimilarWords
-Author: Pahalavan R D
-Author-email: rdpahalavan24@gmail.com
-License: MIT
-Keywords: BERT NLP
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+# BERTSimilar
 
-# BERTSimilarWords
+## Get Similar Words and Embeddings using BERT Models
 
-## Find Similar Words using BERT
-
-BERTSimilarWords is a python library that is used to find similar words using BERT. It uses a pre-trained BERT base model (cased) and cosine similarity to find the closest neighbor to the given words. It is similar to the Gensim Word2Vec similar words, but with context.
+BERTSimilar is used to get similar words and embeddings using BERT models. It uses **bert-base-cased** model as default and cosine similarity to find the closest word to the given words.
 
 BERT generates contextual word embeddings, so the word embedding for the same word will differ based on its context. For example, the word **Apple** in *"Apple is a good fruit"* and *"Apple is a good phone"* have different word embeddings. Generating word embeddings for all vocabulary in the English language based on context is time-consuming and needs many resources. So, this library requires the vocabulary for generating word embeddings beforehand.
 
 Vocabularies used to generate word embeddings can be given in two ways:
 
 * [Using Wikipedia Pages](#using-wikipedia-pages)
 * [Using Text Files](#using-text-files)
 
 ## Install and Import
 
 Install the Python package using
 ```
-pip install BERTSimilarWords
+pip install BERTSimilar
 ```
 
 Import the module using
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
+>>> from BERTSimilar import SimilarWords
 ```
 
 ## Providing the Vocabulary
 
 Provide the text (in terms of paragraphs), so the BERT model can generate the word embeddings for all the words present in the text.
 
 ### Using Wikipedia Pages
 
 1) Using Wikipedia page names as a list (the content of the pages will be taken as input and processed)
 
 ```python
 >>> wikipedia_pages = ['Apple', 'Apple Inc.']
->>> similar = BERTSimilarWords().load_dataset(wikipedia_page_list=wikipedia_pages)
+>>> similar = SimilarWords().load_dataset(wikipedia_page_list=wikipedia_pages)
 
 # To get the Wikipedia pages used,
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.'}
 ```
 
 2) Using Wikipedia search query as string (the content of the pages related to the query will be taken as input and processed)
 
 ```python
 # Get 5 Wikipedia pages based on the query
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
 
 # To get the Wikipedia pages used (duplicate pages are ignored),
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.',
  'Apples to Apples': 'https://en.wikipedia.org/wiki/Apples_to_Apples',
  'MacOS': 'https://en.wikipedia.org/wiki/MacOS'}
 ```
 
 3) Using Wikipedia search queries as a list (the content of the pages related to each query will be taken as input and processed)
 
 ```python
 # Get 5 Wikipedia pages based on each query
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query=['Apple', 'Banana'], wikipedia_query_limit=5)
+>>> similar = SimilarWords().load_dataset(wikipedia_query=['Apple', 'Banana'], wikipedia_query_limit=5)
 
 # To get the Wikipedia pages used (duplicate pages are ignored),
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.',
  'Apples to Apples': 'https://en.wikipedia.org/wiki/Apples_to_Apples',
  'MacOS': 'https://en.wikipedia.org/wiki/MacOS',
@@ -93,21 +76,21 @@
 ### Using Text Files
 
 File extensions supported are .docx and .txt (For other file types, please convert them to the supporting format)
 
 1) Using single text file (the content of the file will be taken as input and processed)
 
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path='Book_1.docx')
+>>> similar = SimilarWords().load_dataset(dataset_path='Book_1.docx')
 ```
 
 2) Using multiple text files (the contents of each file will be taken as input and processed)
 
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path=['Book_1.docx','Book_1.txt'])
+>>> similar = SimilarWords().load_dataset(dataset_path=['Book_1.docx','Book_1.txt'])
 ```
 
 ## Find Similar Words
 
 Similar words can be generated using the `find_similar_words` method. This method calculates the cosine similarity between the average of the input words based on the given context and all the words present in the given vocabulary. The parameters for this method are
 
 - **input_words** - the input words (list of strings)
@@ -135,16 +118,16 @@
   - if True, *"Apple phones"* given as input will be converted to *"apple phone"* and processed
 
 ## Full Examples
 
 ### Example 1
 
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
+>>> from BERTSimilar import SimilarWords
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
 
 >>> similar.find_similar_words(input_context='company',input_words=['Apple'])
 {'iPhone': 0.7655301993367924,
  'Microsoft': 0.7644559773925612,
  'Samsung': 0.7483747939272186,
  'Nokia': 0.7418908483628721,
  'Macintosh': 0.7415292245659537,
@@ -166,16 +149,16 @@
  'juice': 0.7247635163014543,
  'nuts': 0.724424004884171}
 ```
 
 ### Example 2
 
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Tesla', wikipedia_query_limit=10)
+>>> from BERTSimilar import SimilarWords
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Tesla', wikipedia_query_limit=10)
 
 >>> similar.find_similar_words(input_context='Tesla Motors', input_words=['CEO'], output_words_ngram=5, max_output_words=5)
 {'Chief Executive Elon Musk handing': 0.7596588355056113,
  '2018 CEO Elon Musk briefly': 0.751011374230985,
  'August 2018 CEO Elon Musk': 0.7492089016517951,
  '2021 CEO Elon Musk revealed': 0.7470401856896459,
  'SEC questioned Tesla CFO Zach': 0.738144930474394}
@@ -188,15 +171,15 @@
  'Nikola Tesla Technical Museum': 0.8759513407776292}
 ```
 
 ## Useful Attributes
 
 These attributes can be used to get values or modify default values, and can be used after the `load_dataset` method. For example, to get the maximum n-gram supported
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path='Book_1.docx')
+>>> similar = SimilarWords().load_dataset(dataset_path='Book_1.docx')
 
 # This will give the maximum n-gram supported (default: 10)
 >>> similar.max_ngram
 10
 
 # To change this to only support up to 5-gram words
 >>> similar.max_ngram = 5
@@ -221,9 +204,8 @@
 - **pos_tags_info()** - to get the POS tags and information to be used in the `find_similar_words` method
 
 ## References
 
 1) Wolf, T., Debut, L., Sanh, V., Chaumond, J., Delangue, C., Moi, A., Cistac, P., Ma, C., Jernite, Y., Plu, J., Xu, C., Le Scao, T., Gugger, S., Drame, M., Lhoest, Q., & Rush, A. M. (2020). Transformers: State-of-the-Art Natural Language Processing [Conference paper]. 38–45. https://www.aclweb.org/anthology/2020.emnlp-demos.6
 2) Paszke, A., Gross, S., Massa, F., Lerer, A., Bradbury, J., Chanan, G., Killeen, T., Lin, Z., Gimelshein, N., Antiga, L., Desmaison, A., Kopf, A., Yang, E., DeVito, Z., Raison, M., Tejani, A., Chilamkurthy, S., Steiner, B., Fang, L., Bai, J., & Chintala, S. (2019). PyTorch: An Imperative Style, High-Performance Deep Learning Library [Conference paper]. Advances in Neural Information Processing Systems 32, 8024–8035. http://papers.neurips.cc/paper/9015-pytorch-an-imperative-style-high-performance-deep-learning-library.pdf
 3) Pedregosa, F. and Varoquaux, G. and Gramfort, A. and Michel, V. and Thirion, B. and Grisel, O. and Blondel, M. and Prettenhofer, P. and Weiss, R. and Dubourg, V. and Vanderplas, J. and Passos, A. and Cournapeau, D. and Brucher, M. and Perrot, M. and Duchesnay, E. (2011). Scikit-learn: Machine Learning in Python. Journal of Machine Learning Research 12, 2825-2830. https://jmlr.csail.mit.edu/papers/v12/pedregosa11a.html
-4) Bird, S., Klein, E., & Loper, E. (2009). Natural Language Processing with Python: Analyzing Text with the Natural Language Toolkit. O'Reilly Media, Inc.
-
+4) Bird, S., Klein, E., & Loper, E. (2009). Natural Language Processing with Python: Analyzing Text with the Natural Language Toolkit. O'Reilly Media, Inc.
```

### Comparing `BERTSimilar-0.1.0/LICENSE.txt` & `BERTSimilar-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.0/PKG-INFO` & `BERTSimilar-0.1.1/BERTSimilar.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.0
+Version: 0.1.1
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# BERTSimilarWords
+# BERTSimilar
 
-## Find Similar Words using BERT
+## Get Similar Words and Embeddings using BERT Models
 
-BERTSimilarWords is a python library that is used to find similar words using BERT. It uses a pre-trained BERT base model (cased) and cosine similarity to find the closest neighbor to the given words. It is similar to the Gensim Word2Vec similar words, but with context.
+BERTSimilar is used to get similar words and embeddings using BERT models. It uses **bert-base-cased** model as default and cosine similarity to find the closest word to the given words.
 
 BERT generates contextual word embeddings, so the word embedding for the same word will differ based on its context. For example, the word **Apple** in *"Apple is a good fruit"* and *"Apple is a good phone"* have different word embeddings. Generating word embeddings for all vocabulary in the English language based on context is time-consuming and needs many resources. So, this library requires the vocabulary for generating word embeddings beforehand.
 
 Vocabularies used to generate word embeddings can be given in two ways:
 
 * [Using Wikipedia Pages](#using-wikipedia-pages)
 * [Using Text Files](#using-text-files)
 
 ## Install and Import
 
 Install the Python package using
 ```
-pip install BERTSimilarWords
+pip install BERTSimilar
 ```
 
 Import the module using
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
+>>> from BERTSimilar import SimilarWords
 ```
 
 ## Providing the Vocabulary
 
 Provide the text (in terms of paragraphs), so the BERT model can generate the word embeddings for all the words present in the text.
 
 ### Using Wikipedia Pages
 
 1) Using Wikipedia page names as a list (the content of the pages will be taken as input and processed)
 
 ```python
 >>> wikipedia_pages = ['Apple', 'Apple Inc.']
->>> similar = BERTSimilarWords().load_dataset(wikipedia_page_list=wikipedia_pages)
+>>> similar = SimilarWords().load_dataset(wikipedia_page_list=wikipedia_pages)
 
 # To get the Wikipedia pages used,
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.'}
 ```
 
 2) Using Wikipedia search query as string (the content of the pages related to the query will be taken as input and processed)
 
 ```python
 # Get 5 Wikipedia pages based on the query
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
 
 # To get the Wikipedia pages used (duplicate pages are ignored),
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.',
  'Apples to Apples': 'https://en.wikipedia.org/wiki/Apples_to_Apples',
  'MacOS': 'https://en.wikipedia.org/wiki/MacOS'}
 ```
 
 3) Using Wikipedia search queries as a list (the content of the pages related to each query will be taken as input and processed)
 
 ```python
 # Get 5 Wikipedia pages based on each query
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query=['Apple', 'Banana'], wikipedia_query_limit=5)
+>>> similar = SimilarWords().load_dataset(wikipedia_query=['Apple', 'Banana'], wikipedia_query_limit=5)
 
 # To get the Wikipedia pages used (duplicate pages are ignored),
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.',
  'Apples to Apples': 'https://en.wikipedia.org/wiki/Apples_to_Apples',
  'MacOS': 'https://en.wikipedia.org/wiki/MacOS',
@@ -93,21 +93,21 @@
 ### Using Text Files
 
 File extensions supported are .docx and .txt (For other file types, please convert them to the supporting format)
 
 1) Using single text file (the content of the file will be taken as input and processed)
 
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path='Book_1.docx')
+>>> similar = SimilarWords().load_dataset(dataset_path='Book_1.docx')
 ```
 
 2) Using multiple text files (the contents of each file will be taken as input and processed)
 
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path=['Book_1.docx','Book_1.txt'])
+>>> similar = SimilarWords().load_dataset(dataset_path=['Book_1.docx','Book_1.txt'])
 ```
 
 ## Find Similar Words
 
 Similar words can be generated using the `find_similar_words` method. This method calculates the cosine similarity between the average of the input words based on the given context and all the words present in the given vocabulary. The parameters for this method are
 
 - **input_words** - the input words (list of strings)
@@ -135,16 +135,16 @@
   - if True, *"Apple phones"* given as input will be converted to *"apple phone"* and processed
 
 ## Full Examples
 
 ### Example 1
 
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
+>>> from BERTSimilar import SimilarWords
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
 
 >>> similar.find_similar_words(input_context='company',input_words=['Apple'])
 {'iPhone': 0.7655301993367924,
  'Microsoft': 0.7644559773925612,
  'Samsung': 0.7483747939272186,
  'Nokia': 0.7418908483628721,
  'Macintosh': 0.7415292245659537,
@@ -166,16 +166,16 @@
  'juice': 0.7247635163014543,
  'nuts': 0.724424004884171}
 ```
 
 ### Example 2
 
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Tesla', wikipedia_query_limit=10)
+>>> from BERTSimilar import SimilarWords
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Tesla', wikipedia_query_limit=10)
 
 >>> similar.find_similar_words(input_context='Tesla Motors', input_words=['CEO'], output_words_ngram=5, max_output_words=5)
 {'Chief Executive Elon Musk handing': 0.7596588355056113,
  '2018 CEO Elon Musk briefly': 0.751011374230985,
  'August 2018 CEO Elon Musk': 0.7492089016517951,
  '2021 CEO Elon Musk revealed': 0.7470401856896459,
  'SEC questioned Tesla CFO Zach': 0.738144930474394}
@@ -188,15 +188,15 @@
  'Nikola Tesla Technical Museum': 0.8759513407776292}
 ```
 
 ## Useful Attributes
 
 These attributes can be used to get values or modify default values, and can be used after the `load_dataset` method. For example, to get the maximum n-gram supported
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path='Book_1.docx')
+>>> similar = SimilarWords().load_dataset(dataset_path='Book_1.docx')
 
 # This will give the maximum n-gram supported (default: 10)
 >>> similar.max_ngram
 10
 
 # To change this to only support up to 5-gram words
 >>> similar.max_ngram = 5
```

### Comparing `BERTSimilar-0.1.0/README.md` & `BERTSimilar-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,86 @@
-# BERTSimilarWords
+Metadata-Version: 2.1
+Name: BERTSimilar
+Version: 0.1.1
+Summary: Get Similar Words and Embeddings using BERT Models
+Home-page: https://github.com/rdpahalavan/BERTSimilarWords
+Author: Pahalavan R D
+Author-email: rdpahalavan24@gmail.com
+License: MIT
+Keywords: BERT NLP
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-## Find Similar Words using BERT
+# BERTSimilar
 
-BERTSimilarWords is a python library that is used to find similar words using BERT. It uses a pre-trained BERT base model (cased) and cosine similarity to find the closest neighbor to the given words. It is similar to the Gensim Word2Vec similar words, but with context.
+## Get Similar Words and Embeddings using BERT Models
+
+BERTSimilar is used to get similar words and embeddings using BERT models. It uses **bert-base-cased** model as default and cosine similarity to find the closest word to the given words.
 
 BERT generates contextual word embeddings, so the word embedding for the same word will differ based on its context. For example, the word **Apple** in *"Apple is a good fruit"* and *"Apple is a good phone"* have different word embeddings. Generating word embeddings for all vocabulary in the English language based on context is time-consuming and needs many resources. So, this library requires the vocabulary for generating word embeddings beforehand.
 
 Vocabularies used to generate word embeddings can be given in two ways:
 
 * [Using Wikipedia Pages](#using-wikipedia-pages)
 * [Using Text Files](#using-text-files)
 
 ## Install and Import
 
 Install the Python package using
 ```
-pip install BERTSimilarWords
+pip install BERTSimilar
 ```
 
 Import the module using
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
+>>> from BERTSimilar import SimilarWords
 ```
 
 ## Providing the Vocabulary
 
 Provide the text (in terms of paragraphs), so the BERT model can generate the word embeddings for all the words present in the text.
 
 ### Using Wikipedia Pages
 
 1) Using Wikipedia page names as a list (the content of the pages will be taken as input and processed)
 
 ```python
 >>> wikipedia_pages = ['Apple', 'Apple Inc.']
->>> similar = BERTSimilarWords().load_dataset(wikipedia_page_list=wikipedia_pages)
+>>> similar = SimilarWords().load_dataset(wikipedia_page_list=wikipedia_pages)
 
 # To get the Wikipedia pages used,
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.'}
 ```
 
 2) Using Wikipedia search query as string (the content of the pages related to the query will be taken as input and processed)
 
 ```python
 # Get 5 Wikipedia pages based on the query
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
 
 # To get the Wikipedia pages used (duplicate pages are ignored),
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.',
  'Apples to Apples': 'https://en.wikipedia.org/wiki/Apples_to_Apples',
  'MacOS': 'https://en.wikipedia.org/wiki/MacOS'}
 ```
 
 3) Using Wikipedia search queries as a list (the content of the pages related to each query will be taken as input and processed)
 
 ```python
 # Get 5 Wikipedia pages based on each query
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query=['Apple', 'Banana'], wikipedia_query_limit=5)
+>>> similar = SimilarWords().load_dataset(wikipedia_query=['Apple', 'Banana'], wikipedia_query_limit=5)
 
 # To get the Wikipedia pages used (duplicate pages are ignored),
 >>> similar.wikipedia_dataset_info
 {'Apple': 'https://en.wikipedia.org/wiki/Apple',
  'Apple Inc.': 'https://en.wikipedia.org/wiki/Apple_Inc.',
  'Apples to Apples': 'https://en.wikipedia.org/wiki/Apples_to_Apples',
  'MacOS': 'https://en.wikipedia.org/wiki/MacOS',
@@ -76,21 +93,21 @@
 ### Using Text Files
 
 File extensions supported are .docx and .txt (For other file types, please convert them to the supporting format)
 
 1) Using single text file (the content of the file will be taken as input and processed)
 
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path='Book_1.docx')
+>>> similar = SimilarWords().load_dataset(dataset_path='Book_1.docx')
 ```
 
 2) Using multiple text files (the contents of each file will be taken as input and processed)
 
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path=['Book_1.docx','Book_1.txt'])
+>>> similar = SimilarWords().load_dataset(dataset_path=['Book_1.docx','Book_1.txt'])
 ```
 
 ## Find Similar Words
 
 Similar words can be generated using the `find_similar_words` method. This method calculates the cosine similarity between the average of the input words based on the given context and all the words present in the given vocabulary. The parameters for this method are
 
 - **input_words** - the input words (list of strings)
@@ -118,16 +135,16 @@
   - if True, *"Apple phones"* given as input will be converted to *"apple phone"* and processed
 
 ## Full Examples
 
 ### Example 1
 
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
+>>> from BERTSimilar import SimilarWords
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Apple', wikipedia_query_limit=5)
 
 >>> similar.find_similar_words(input_context='company',input_words=['Apple'])
 {'iPhone': 0.7655301993367924,
  'Microsoft': 0.7644559773925612,
  'Samsung': 0.7483747939272186,
  'Nokia': 0.7418908483628721,
  'Macintosh': 0.7415292245659537,
@@ -149,16 +166,16 @@
  'juice': 0.7247635163014543,
  'nuts': 0.724424004884171}
 ```
 
 ### Example 2
 
 ```python
->>> from BERTSimilarWords import BERTSimilarWords
->>> similar = BERTSimilarWords().load_dataset(wikipedia_query='Tesla', wikipedia_query_limit=10)
+>>> from BERTSimilar import SimilarWords
+>>> similar = SimilarWords().load_dataset(wikipedia_query='Tesla', wikipedia_query_limit=10)
 
 >>> similar.find_similar_words(input_context='Tesla Motors', input_words=['CEO'], output_words_ngram=5, max_output_words=5)
 {'Chief Executive Elon Musk handing': 0.7596588355056113,
  '2018 CEO Elon Musk briefly': 0.751011374230985,
  'August 2018 CEO Elon Musk': 0.7492089016517951,
  '2021 CEO Elon Musk revealed': 0.7470401856896459,
  'SEC questioned Tesla CFO Zach': 0.738144930474394}
@@ -171,15 +188,15 @@
  'Nikola Tesla Technical Museum': 0.8759513407776292}
 ```
 
 ## Useful Attributes
 
 These attributes can be used to get values or modify default values, and can be used after the `load_dataset` method. For example, to get the maximum n-gram supported
 ```python
->>> similar = BERTSimilarWords().load_dataset(dataset_path='Book_1.docx')
+>>> similar = SimilarWords().load_dataset(dataset_path='Book_1.docx')
 
 # This will give the maximum n-gram supported (default: 10)
 >>> similar.max_ngram
 10
 
 # To change this to only support up to 5-gram words
 >>> similar.max_ngram = 5
@@ -204,8 +221,9 @@
 - **pos_tags_info()** - to get the POS tags and information to be used in the `find_similar_words` method
 
 ## References
 
 1) Wolf, T., Debut, L., Sanh, V., Chaumond, J., Delangue, C., Moi, A., Cistac, P., Ma, C., Jernite, Y., Plu, J., Xu, C., Le Scao, T., Gugger, S., Drame, M., Lhoest, Q., & Rush, A. M. (2020). Transformers: State-of-the-Art Natural Language Processing [Conference paper]. 38–45. https://www.aclweb.org/anthology/2020.emnlp-demos.6
 2) Paszke, A., Gross, S., Massa, F., Lerer, A., Bradbury, J., Chanan, G., Killeen, T., Lin, Z., Gimelshein, N., Antiga, L., Desmaison, A., Kopf, A., Yang, E., DeVito, Z., Raison, M., Tejani, A., Chilamkurthy, S., Steiner, B., Fang, L., Bai, J., & Chintala, S. (2019). PyTorch: An Imperative Style, High-Performance Deep Learning Library [Conference paper]. Advances in Neural Information Processing Systems 32, 8024–8035. http://papers.neurips.cc/paper/9015-pytorch-an-imperative-style-high-performance-deep-learning-library.pdf
 3) Pedregosa, F. and Varoquaux, G. and Gramfort, A. and Michel, V. and Thirion, B. and Grisel, O. and Blondel, M. and Prettenhofer, P. and Weiss, R. and Dubourg, V. and Vanderplas, J. and Passos, A. and Cournapeau, D. and Brucher, M. and Perrot, M. and Duchesnay, E. (2011). Scikit-learn: Machine Learning in Python. Journal of Machine Learning Research 12, 2825-2830. https://jmlr.csail.mit.edu/papers/v12/pedregosa11a.html
-4) Bird, S., Klein, E., & Loper, E. (2009). Natural Language Processing with Python: Analyzing Text with the Natural Language Toolkit. O'Reilly Media, Inc.
+4) Bird, S., Klein, E., & Loper, E. (2009). Natural Language Processing with Python: Analyzing Text with the Natural Language Toolkit. O'Reilly Media, Inc.
+
```

### Comparing `BERTSimilar-0.1.0/setup.py` & `BERTSimilar-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='BERTSimilar',
-    version='0.1.0',
+    version='0.1.1',
     description="Get Similar Words and Embeddings using BERT Models",
     keywords="BERT NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

