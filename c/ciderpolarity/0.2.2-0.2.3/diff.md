# Comparing `tmp/ciderpolarity-0.2.2.tar.gz` & `tmp/ciderpolarity-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciderpolarity-0.2.2.tar", max compression
+gzip compressed data, was "ciderpolarity-0.2.3.tar", max compression
```

## Comparing `ciderpolarity-0.2.2.tar` & `ciderpolarity-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.2/LICENSE
--rw-r--r--   0        0        0     4580 2023-07-11 15:29:00.896330 ciderpolarity-0.2.2/README.md
--rw-r--r--   0        0        0     8790 2023-07-10 14:03:02.477624 ciderpolarity-0.2.2/ciderpolarity/CIDER.py
--rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.2/ciderpolarity/__init__.py
--rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.2/ciderpolarity/create_embeddings.py
--rw-r--r--   0        0        0     2630 2023-07-11 09:15:25.743879 ciderpolarity-0.2.2/ciderpolarity/create_vader.py
--rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.2/ciderpolarity/load_polarities.py
--rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.2/ciderpolarity/run_bootstrapping.py
--rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.2/ciderpolarity/stopwords.py
--rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.2/ciderpolarity/suggest_seeds.py
--rw-r--r--   0        0        0     1138 2023-07-11 14:31:11.901762 ciderpolarity-0.2.2/ciderpolarity/utils_funcs.py
--rw-r--r--   0        0        0      518 2023-07-11 15:30:05.547752 ciderpolarity-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5468 1970-01-01 00:00:00.000000 ciderpolarity-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4354 2023-07-12 14:24:52.744113 ciderpolarity-0.2.3/README.md
+-rw-r--r--   0        0        0     9384 2023-07-12 14:00:08.052546 ciderpolarity-0.2.3/ciderpolarity/CIDER.py
+-rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.3/ciderpolarity/__init__.py
+-rw-r--r--   0        0        0     3214 2023-07-10 14:03:14.701505 ciderpolarity-0.2.3/ciderpolarity/create_embeddings.py
+-rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.3/ciderpolarity/create_vader.py
+-rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.3/ciderpolarity/load_polarities.py
+-rw-r--r--   0        0        0     5285 2023-07-10 13:13:25.613474 ciderpolarity-0.2.3/ciderpolarity/run_bootstrapping.py
+-rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.3/ciderpolarity/stopwords.py
+-rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.3/ciderpolarity/suggest_seeds.py
+-rw-r--r--   0        0        0     1138 2023-07-11 14:31:11.901762 ciderpolarity-0.2.3/ciderpolarity/utils_funcs.py
+-rw-r--r--   0        0        0      518 2023-07-12 14:09:31.471572 ciderpolarity-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 ciderpolarity-0.2.3/PKG-INFO
```

### Comparing `ciderpolarity-0.2.2/LICENSE` & `ciderpolarity-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.2/README.md` & `ciderpolarity-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,32 +28,25 @@
 ## Overview
 
 The easiest way to use the package is as follows:
 
 ```python
 from ciderpolarity import CIDER
 
-# For a running example, the ideal input will have many thousands of lines.
-texts = ['Really hate this heat. Just want AC',
-         'I love an icecream in this heat!',
-         'I’m melting - terrible weather!',
-         'Very dehydrated in this heat',
-                ...                    ,
-         'this sunny weather is great',
-         'Oh my icecream is melting',
-         'My AC is broken! 🥵']
-
+# download test data from: https://github.com/jcy204/ciderPolarity/tree/main/tests/test_data.csv
+# data input is either a one column csv file where each row is a text entry, or list of strings
 
+input_data = 'test_data.csv'
 output_folder = '/path/to/output/folder/'
 
-cdr = CIDER(input_file, output_folder)
+cdr = CIDER(input_data, output_folder)
 results = cdr.fit_transform()
 ```
 
-This trains the model, creating a customised VADER classifier, before classifying the provided input using the model. An example output is as follows:
+This trains the model, creating a customised VADER classifier, before classifying the provided input using the model. A ficticious example output is as follows:
 
 ```python
 results = [
     ['Really hate this heat. Just want AC', {"neg":0.6, "neu":0.4, "pos":0.0, "compound":-0.6}],
     ['I love an icecream in this heat!', {"neg":0.0, "neu":0.5, "pos":0.5, "compound":0.6}],
     ['I’m melting - terrible weather!', {"neg":0.7, "neu":0.3, "pos":0.0, "compound":-0.7}],
     ['Very dehydrated in this heat', {"neg":0.5, "neu":0.4, "pos":0.0, "compound":-0.5}],
@@ -64,24 +57,24 @@
 ]
 
 ```
 
 ## Examples
 **Some alternative ways to use the library are as follows:**
 
-Applying CIDER to a saved dataset, adding custom seed words, custom stopwords, and tuning various parameters:
+Applying CIDER to a list of strings, adding custom seed words, custom stopwords, and tuning various parameters:
 
 ```python
 POS_seeds = {'lovely':1, 'excellent':2, 'fortunate':4, 'excited':1, 'loves':2, '♥':1, '🙂':2}
 NEG_seeds = {'bad':1, 'horrible':2, 'hate':4, 'crappy':1, 'sad':2, 'bitch':1, 'hates':2}
 
-input_file = '/path/to/input/file.csv'
+input_data = ['list of strings']
 output = '/path/to/output/test_outputs/'
 
-cdr_example = CIDER(input_file,                   # input path (one column csv file where each row is a text entry)
+cdr_example = CIDER(input_data,                   # input data 
                     output,                       # output path
                     iterations=100,               # number of iterations for bootstrapped label propagation
                     stopwords=['i', 'it', 'the'], # custom stopwords, alternativly set as 'default' for the nltk set
                     keep=['code', 'python'],      # words to force into the final lexicon
                     no_below=5,                   # exclude words that occur fewer times than this
                     max_polarities_returned=3000, # maximum number of words returned
                     pos_seeds=POS_seeds,          # positive seeds with custom weighting
@@ -99,15 +92,15 @@
 
 <img src="https://github.com/jcy204/ciderPolarity/blob/main/cdr_out_example.png?raw=true" alt="drawing" width="500"/>
 
 ___
 
 ### Generating Seedwords
 
-Whilst CIDER has built in seed words (found [here](CIDER/suggest_seeds.py)), custom seed words can be generated and suggested. The following shows how this is carried out:
+Whilst CIDER has built in seed words (found [here](ciderpolarity/suggest_seeds.py)), custom seed words can be generated and suggested. The following shows how this is carried out:
 
 ```python
 Pos, Neg = cdr_example.generate_seeds(['good','brilliant','love'],['bad','terrible','hate'], n=20, sentiment = True)
 ```
 Which looks at strongly polarised words which occur both often, are close to one seed set, and distant from the opposing seed set.
 
 The following returns all words in the data, alongside their seed word suitability.
```

### Comparing `ciderpolarity-0.2.2/ciderpolarity/CIDER.py` & `ciderpolarity-0.2.3/ciderpolarity/CIDER.py`

 * *Files 10% similar despite different names*

```diff
@@ -136,21 +136,23 @@
         return_all - BOOL - set as True to return full filtered dataframe
         sentiment - BOOL - set as False if the generating non-sentiment seeds 
         '''
         return custom_seeds(self, pos_initial, neg_initial, n, return_all,sentiment)
     
 
 
-    def fit(self, full_run=True):
+    def fit(self, full_run=True, remove_neutral=True):
         '''
         Train CIDER and fit a VADER model on the outputs
 
         Parameters
         ----------
         full_run - BOOL - set as False to just return previously executed results
+        remove_neutral - BOOL - set as True to remove words from VADER that CIDER 
+                                classifies as neutral
         '''
         if full_run:
             ## Generating embeddings
             for ind, _ in enumerate(utils_funcs.text_iterate(self)):
                 continue
             self.LINES = ind + 1
             if (self.LINES < 30000) & (self.NO_BELOW > 30):
@@ -161,15 +163,15 @@
             create_embeddings.embed_text(self)
 
             ## Running Bootstrapping
             run_bootstrapping.propogate_labels(self)
         
         ## Loading Polarities
         self.create_df()
-        self.train_VADER()
+        self.train_VADER(remove_neutral)
 
 
 
     def transform(self, save_outputs=False, return_outputs = True):
         '''
         Apply fitted VADER model on the inputs.
 
@@ -178,39 +180,46 @@
         save_outputs - BOOL - save the outputs into .json file
         return_outputs - BOOL - return the outputs as a list
         '''
         return create_vader.apply_vader(self, save_outputs, return_outputs)
     
 
 
-    def fit_transform(self, save_outputs=False, return_outputs = True, full_run = True):
+    def fit_transform(self, save_outputs=False, return_outputs = True, full_run = True, remove_neutral=True):
         '''
         Train CIDER and fit a VADER model on the outputs. Apply fitted VADER model on the inputs
         
         Parameters
         ----------
         save_outputs - BOOL - save the outputs into .json file
         return_outputs - BOOL - return the outputs as a list
         full_run - BOOL - set as False to just return previously executed results
-
+        remove_neutral - BOOL - set as True to remove words from VADER that CIDER 
+                                classifies as neutral
         '''
-        self.fit(full_run)
+        self.fit(full_run, remove_neutral)
         return self.transform(save_outputs, return_outputs)
     
 
 
     def create_df(self):
         'returns polarities only'
         self.polarities = load_polarities.make_df(self)
 
 
 
-    def train_VADER(self):
-        'trains VADER only'
-        self.classify = create_vader.modify_vader(self)
+    def train_VADER(self,remove_neutral=True):
+        '''
+        trains VADER only        
+        Parameters
+        ----------
+        remove_neutral - BOOL - set as True to remove words from VADER that CIDER 
+                                classifies as neutral
+        '''
+        self.classify = create_vader.modify_vader(self,remove_neutral)
         
 
     def clean_text(self,text):
         '''
         cleans and tokenises the text
         '''
         if self.PREPROCESSING == 'default':
```

### Comparing `ciderpolarity-0.2.2/ciderpolarity/create_embeddings.py` & `ciderpolarity-0.2.3/ciderpolarity/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.2/ciderpolarity/create_vader.py` & `ciderpolarity-0.2.3/ciderpolarity/create_vader.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,30 @@
 from .utils_funcs import text_iterate
 
 
 SIA = SentimentIntensityAnalyzer()
 r_arg = {'pct':True,'method':'dense'}
 
 ################################ CHECK THESE THRESHOLDS ####################################
-def modify_vader(SS):
+def modify_vader(SS,remove_neutral=True):
+    '''
+    remove_neutral - BOOL - set as True to remove words from VADER that CIDER 
+                            classifies as neutral   
+    '''
+
     try: 
         df = SS.polarities
     except:
         SS.create_df()
         df = SS.polarities
     
     ## Filter DF
     df_pos, df_neg, remove = filter_df(df, SS.NEU_THRESH, SS.VAR_UPPER, SS.VAR_LOWER)
+    if remove_neutral == False:
+        remove = []
     return make_VADER_custom(df_pos, df_neg, remove)
 
     
 def make_VADER_custom(positive, negative, remove):
     SIA_Custom = SentimentIntensityAnalyzer()
     
     for i in remove:
```

### Comparing `ciderpolarity-0.2.2/ciderpolarity/load_polarities.py` & `ciderpolarity-0.2.3/ciderpolarity/load_polarities.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.2/ciderpolarity/run_bootstrapping.py` & `ciderpolarity-0.2.3/ciderpolarity/run_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.2/ciderpolarity/stopwords.py` & `ciderpolarity-0.2.3/ciderpolarity/stopwords.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.2/ciderpolarity/suggest_seeds.py` & `ciderpolarity-0.2.3/ciderpolarity/suggest_seeds.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.2/ciderpolarity/utils_funcs.py` & `ciderpolarity-0.2.3/ciderpolarity/utils_funcs.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.2/pyproject.toml` & `ciderpolarity-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ciderpolarity"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["jcy204 <jcy204@exeter.ac.uk>"]
 readme = "README.md"
 homepage = "https://github.com/jcy204/ciderPolarity"
 repository = "https://github.com/jcy204/ciderPolarity"
 
 [tool.poetry.dependencies]
```

### Comparing `ciderpolarity-0.2.2/PKG-INFO` & `ciderpolarity-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciderpolarity
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Home-page: https://github.com/jcy204/ciderPolarity
 Author: jcy204
 Author-email: jcy204@exeter.ac.uk
 Requires-Python: >=3.7,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -52,32 +52,25 @@
 ## Overview
 
 The easiest way to use the package is as follows:
 
 ```python
 from ciderpolarity import CIDER
 
-# For a running example, the ideal input will have many thousands of lines.
-texts = ['Really hate this heat. Just want AC',
-         'I love an icecream in this heat!',
-         'I’m melting - terrible weather!',
-         'Very dehydrated in this heat',
-                ...                    ,
-         'this sunny weather is great',
-         'Oh my icecream is melting',
-         'My AC is broken! 🥵']
-
+# download test data from: https://github.com/jcy204/ciderPolarity/tree/main/tests/test_data.csv
+# data input is either a one column csv file where each row is a text entry, or list of strings
 
+input_data = 'test_data.csv'
 output_folder = '/path/to/output/folder/'
 
-cdr = CIDER(input_file, output_folder)
+cdr = CIDER(input_data, output_folder)
 results = cdr.fit_transform()
 ```
 
-This trains the model, creating a customised VADER classifier, before classifying the provided input using the model. An example output is as follows:
+This trains the model, creating a customised VADER classifier, before classifying the provided input using the model. A ficticious example output is as follows:
 
 ```python
 results = [
     ['Really hate this heat. Just want AC', {"neg":0.6, "neu":0.4, "pos":0.0, "compound":-0.6}],
     ['I love an icecream in this heat!', {"neg":0.0, "neu":0.5, "pos":0.5, "compound":0.6}],
     ['I’m melting - terrible weather!', {"neg":0.7, "neu":0.3, "pos":0.0, "compound":-0.7}],
     ['Very dehydrated in this heat', {"neg":0.5, "neu":0.4, "pos":0.0, "compound":-0.5}],
@@ -88,24 +81,24 @@
 ]
 
 ```
 
 ## Examples
 **Some alternative ways to use the library are as follows:**
 
-Applying CIDER to a saved dataset, adding custom seed words, custom stopwords, and tuning various parameters:
+Applying CIDER to a list of strings, adding custom seed words, custom stopwords, and tuning various parameters:
 
 ```python
 POS_seeds = {'lovely':1, 'excellent':2, 'fortunate':4, 'excited':1, 'loves':2, '♥':1, '🙂':2}
 NEG_seeds = {'bad':1, 'horrible':2, 'hate':4, 'crappy':1, 'sad':2, 'bitch':1, 'hates':2}
 
-input_file = '/path/to/input/file.csv'
+input_data = ['list of strings']
 output = '/path/to/output/test_outputs/'
 
-cdr_example = CIDER(input_file,                   # input path (one column csv file where each row is a text entry)
+cdr_example = CIDER(input_data,                   # input data 
                     output,                       # output path
                     iterations=100,               # number of iterations for bootstrapped label propagation
                     stopwords=['i', 'it', 'the'], # custom stopwords, alternativly set as 'default' for the nltk set
                     keep=['code', 'python'],      # words to force into the final lexicon
                     no_below=5,                   # exclude words that occur fewer times than this
                     max_polarities_returned=3000, # maximum number of words returned
                     pos_seeds=POS_seeds,          # positive seeds with custom weighting
@@ -123,15 +116,15 @@
 
 <img src="https://github.com/jcy204/ciderPolarity/blob/main/cdr_out_example.png?raw=true" alt="drawing" width="500"/>
 
 ___
 
 ### Generating Seedwords
 
-Whilst CIDER has built in seed words (found [here](CIDER/suggest_seeds.py)), custom seed words can be generated and suggested. The following shows how this is carried out:
+Whilst CIDER has built in seed words (found [here](ciderpolarity/suggest_seeds.py)), custom seed words can be generated and suggested. The following shows how this is carried out:
 
 ```python
 Pos, Neg = cdr_example.generate_seeds(['good','brilliant','love'],['bad','terrible','hate'], n=20, sentiment = True)
 ```
 Which looks at strongly polarised words which occur both often, are close to one seed set, and distant from the opposing seed set.
 
 The following returns all words in the data, alongside their seed word suitability.
```

