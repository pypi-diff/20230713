# Comparing `tmp/IngeoDash-0.0.19.tar.gz` & `tmp/IngeoDash-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IngeoDash-0.0.19.tar", last modified: Wed Jul 12 21:08:06 2023, max compression
+gzip compressed data, was "IngeoDash-0.0.20.tar", last modified: Thu Jul 13 16:46:58 2023, max compression
```

## Comparing `IngeoDash-0.0.19.tar` & `IngeoDash-0.0.20.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:08:06.790624 IngeoDash-0.0.19/IngeoDash/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/IngeoDash/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/IngeoDash/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/IngeoDash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 21:08:06.000000 IngeoDash-0.0.19/IngeoDash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:08:06.794624 IngeoDash-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 21:06:06.000000 IngeoDash-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/IngeoDash/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/IngeoDash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/IngeoDash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/setup.py
```

### Comparing `IngeoDash-0.0.19/IngeoDash/__init__.py` & `IngeoDash-0.0.20/IngeoDash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import label_column, flip_label, store, similarity
 
-__version__ = '0.0.19'
+__version__ = '0.0.20'
```

### Comparing `IngeoDash-0.0.19/IngeoDash/annotate.py` & `IngeoDash-0.0.20/IngeoDash/annotate.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,43 +14,49 @@
 from EvoMSA import BoW, DenseBoW
 from typing import Union
 from IngeoDash.config import Config
 from IngeoDash.config import CONFIG
 import numpy as np
 
 
-def label_column_predict(mem: Config):
-    db = CONFIG.db[mem[mem.username]]
-    data = db[mem.data]
-    if len(data) == 0:
-        return   
+def model(mem: Config, data: dict):
     lang = mem[mem.lang]
-    D = db[mem.permanent]
-    # bow = BoW(lang=lang, label_key=mem.label_header)
-    dense = DenseBoW(lang=lang, label_key=mem.label_header,
+    if lang not in CONFIG.denseBoW:
+        dense = DenseBoW(lang=lang, voc_size_exponent=15,
+                         n_jobs=mem.n_jobs, dataset=False)
+        CONFIG.denseBoW[lang] = dense.text_representations
+    dense = DenseBoW(lang=lang, key=mem.text,
+                     label_key=mem.label_header,
                      voc_size_exponent=15,
                      n_jobs=mem.n_jobs,
                      dataset=False, emoji=False, keyword=False)
     dense.text_representations_extend(CONFIG.denseBoW[lang])
-    dense.select(D=D).fit(D)
-    # cl = StackGeneralization(decision_function_models=[bow,
-    #                                                    dense]).fit(D)
+    return dense.select(D=data).fit(data)
+
+
+def label_column_predict(mem: Config, model=None):
+    db = CONFIG.db[mem[mem.username]]
+    data = db[mem.data]
+    if len(data) == 0:
+        return   
+    D = db[mem.permanent]
+    dense = model(mem, D)
     hys = dense.predict(data).tolist()
     for ele, hy in zip(data, hys):
         ele[mem.label_header] = ele.get(mem.label_header, hy)        
 
 
-def label_column(mem: Config):
+def label_column(mem: Config, model=model):
     db = CONFIG.db[mem[mem.username]]
     if mem.permanent in db:
         _ = np.unique([x[mem.label_header]
                        for x in db[mem.permanent]])
         if _.shape[0] > 1:
             mem[mem.labels] = tuple(_.tolist())
-            return label_column_predict(mem)
+            return label_column_predict(mem, model=model)
     label = mem.get(mem.labels, ('-', ))[0]
     data = db[mem.data]
     for ele in data:
         ele[mem.label_header] = ele.get(mem.label_header, label)
 
 
 def flip_label(mem: Config, k: int):
```

### Comparing `IngeoDash-0.0.19/IngeoDash/app.py` & `IngeoDash-0.0.20/IngeoDash/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,59 +8,74 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import flip_label, label_column, store
-from IngeoDash.config import CONFIG
+from IngeoDash.config import CONFIG, Config
+from dash import dcc, dash_table, html
 from dash.exceptions import PreventUpdate
-from EvoMSA import DenseBoW
-import base64
+import dash_bootstrap_components as dbc
+from dash import Patch
 import string
-import io
 import json
 import numpy as np
 
 
 def mock_data():
     from EvoMSA.tests.test_base import TWEETS
     from microtc.utils import tweet_iterator
     return [{'text': x['text']}
             for x in tweet_iterator(TWEETS) if x['klass'] in ['P', 'N']]
 
 
-def process_manager(mem,
-                    triggered_id=None,
-                    next=None,
-                    content=None,
-                    lang='es'):
-    if triggered_id == mem.upload:
-        upload(mem, content, lang=lang)
-        return json.dumps(mem.mem)
-    elif triggered_id == mem.next:
-        store(mem)
-        db = CONFIG.db[mem[mem.username]]
-        init = mem[mem.n]
-        data = db[mem.original]
-        if len(data):
-            rest = data[mem.n_value:]
-            data = data[:mem.n_value]
-            mem[mem.n] = init + mem.n_value
-        else:
-            data = []
-            rest = []
-        db[mem.data] = data
-        db[mem.original] = rest
-        label_column(mem)        
-        return json.dumps(mem.mem)
-    raise PreventUpdate
+def table_next(mem: Config):
+    store(mem)
+    db = CONFIG.db[mem[mem.username]]
+    init = mem[mem.n]
+    data = db[mem.original]
+    if len(data):
+        rest = data[mem.n_value:]
+        data = data[:mem.n_value]
+        mem[mem.n] = init + mem.n_value
+    else:
+        data = []
+        rest = []
+    db[mem.data] = data
+    db[mem.original] = rest
+    label_column(mem)        
+    return json.dumps(mem.mem)
+
+
+def table(mem: Config):
+    if mem.username in mem:
+        data = CONFIG.db[mem[mem.username]][mem.data]
+    else:
+        data = [{}]
+    return dash_table.DataTable(data if len(data) else [{}],
+                                style_data={'whiteSpace': 'normal',
+                                            'textAlign': 'left',
+                                            'height': 'auto'},
+                                style_header={'fontWeight': 'bold',
+                                              'textAlign': 'left'},
+                                id=CONFIG.data)
+
+
+def table_component():
+    return dbc.Stack([dbc.Progress(value=0, id=CONFIG.progress),
+                      html.Div(id=CONFIG.center,
+                               children=table(CONFIG)),
+                      dbc.Button('Next', 
+                                 color='primary', 
+                                 id=CONFIG.next,
+                                 n_clicks=0)])
 
 
-def user(mem):
+def user(mem: Config):
     try:
         username = mem[mem.username]
     except KeyError:
         for i in range(10):
             cdn = np.array([x for x in string.ascii_uppercase])
             _ = np.random.randint(cdn.shape[0], size=20)
             username = ''.join(cdn[_])
@@ -70,48 +85,43 @@
         db = CONFIG.db[username]
     except KeyError:
         db = dict()
         CONFIG.db[username] = db
     return username, db
            
 
-def upload(mem, content, lang='es'):
-    content_type, content_string = content.split(',')
-    decoded = base64.b64decode(content_string)
-    _ = io.StringIO(decoded.decode('utf-8'))
-    data = [json.loads(x) for x in _]
-    username, db = user(mem)
+def progress(mem: Config):
+    if mem.size not in mem:
+        return 0
+    tot = mem[mem.size]
+    if tot == 0:
+        return 100
+    n = mem[mem.n]
+    return np.ceil(100 * n / tot)
 
-    original = [x for x in data if mem.label_header not in x]
-    permanent = db.get(mem.permanent, list())
-    permanent.extend([x for x in data if mem.label_header in x])
-    db[mem.data] = original[:mem.n_value]
-    db[mem.permanent] = permanent
-    db[mem.original] = original[mem.n_value:]
-    mem.mem = {mem.n: mem.n_value,
-               mem.lang: lang,
-               mem.size: len(original), 
-               mem.username: username}
-    if lang not in mem.denseBoW:
-        dense = DenseBoW(lang=lang, voc_size_exponent=15,
-                         n_jobs=mem.n_jobs,
-                         dataset=False)
-        CONFIG.denseBoW[lang] = dense.text_representations
-    label_column(mem)
 
+def update_row(mem: Config, table: dict):
+    data = flip_label(mem, k=table['row'])
+    patch = Patch()
+    del patch[table['row']]
+    patch.insert(table['row'], data)
+    return patch
 
-def download(mem, filename):
+
+def download(mem: Config, filename: str):
     db = CONFIG.db[mem[mem.username]]
     permanent = db.get(mem.permanent, list())
     data = db.get(mem.data, list())
     _ = [json.dumps(x) for x in permanent + data]
     return dict(content='\n'.join(_), filename=filename)
 
 
-def progress(mem):
-    if mem.size not in mem:
-        return 0
-    tot = mem[mem.size]
-    if tot == 0:
-        return 100
-    n = mem[mem.n]
-    return np.ceil(100 * n / tot)    
+def download_component():
+    return dbc.InputGroup([dcc.Download(id=CONFIG.download),
+                           dbc.InputGroupText('Filename:'),
+                           dbc.Input(placeholder='output.json',
+                                     value='output.json',
+                                     type='text',
+                                     id=CONFIG.filename),
+                           dbc.Button('Download',
+                                      color='success',
+                                      id=CONFIG.save)])
```

### Comparing `IngeoDash-0.0.19/IngeoDash/config.py` & `IngeoDash-0.0.20/IngeoDash/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import Tuple
 from copy import deepcopy
 import json
 
 
 @dataclass
 class Config:
+    store: str = 'store'
     labels: str = 'labels'
     label_header: str = 'klass'
     data: str = 'corpus'
     permanent: str = 'permanent'
     original: str = 'original'
     next: str = 'next'
     next_label: str = 'Next'
@@ -36,28 +37,30 @@
     center: str = 'center'
     upload: str = 'upload'
     lang: str = 'lang'
     n_jobs: int = 1
     denseBoW: dict = field(default_factory=dict)
     db: dict = field(default_factory=dict)
     username: str = 'username'
-
-
+    text: str = 'text'
     mem: dict = field(default_factory=dict)
 
     def __getitem__(self, key):
         return self.mem[key]
     
     def __setitem__(self, key, value):
         self.mem[key] = value
 
     def __call__(self, value):
         cls = deepcopy(self)
         if value is not None:
             cls.mem = json.loads(value) if isinstance(value, str) else value
+        for key in ['label_header', 'text']:
+            if key in cls.mem:
+                setattr(cls, key, cls.mem[key])
         return cls
     
     def __contains__(self, key):
         return key in self.mem
     
     def pop(self, *args, **kwargs):
         return self.mem.pop(*args, **kwargs)
```

### Comparing `IngeoDash-0.0.19/IngeoDash/tests/test_annotate.py` & `IngeoDash-0.0.20/IngeoDash/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.19/IngeoDash/tests/test_config.py` & `IngeoDash-0.0.20/IngeoDash/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.config import Config
+from IngeoDash.config import CONFIG
 
 
 def test_Config():
     conf = Config()
-    default = dict(labels='labels',
+    default = dict(store='store',
+                   labels='labels',
                    label_header='klass',
                    data='corpus',
                    permanent='permanent',
                    original='original',
                    next='next',
                    next_label='Next',
                    n_value=10,
@@ -32,15 +34,17 @@
                    save='save',
                    center='center',
                    upload='upload',
                    lang='lang',
                    n_jobs=1,
                    denseBoW={},
                    db={},
-                   username='username')
+                   username='username',
+                   text='text',
+                   mem={})
     for k, v in default.items():
         assert v == getattr(conf, k)
 
 
 def test_Config_mem():
     config = Config()
 
@@ -56,10 +60,17 @@
     assert xxx['hola'] == 12
     config['adios'] = 2
     assert 'adios' not in xxx
     xxx['xxx'] = 3
     assert mem['xxx'] == 3
 
 
+def test_Config_call2():
+    mem = CONFIG(dict(label_header='label',
+                      text='texto'))
+    assert mem.label_header == 'label'
+    assert mem.text == 'texto'
+
+
 def test_CONFIG():
     from IngeoDash.config import CONFIG
     assert isinstance(CONFIG, Config)
```

### Comparing `IngeoDash-0.0.19/IngeoDash.egg-info/PKG-INFO` & `IngeoDash-0.0.20/IngeoDash.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.19
+Version: 0.0.20
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -15,11 +15,13 @@
 
 .. image:: https://coveralls.io/repos/github/INGEOTEC/IngeoDash/badge.svg?branch=develop
 		:target: https://coveralls.io/github/INGEOTEC/IngeoDash?branch=develop
 
 .. image:: https://badge.fury.io/py/IngeoDash.svg
 		:target: https://badge.fury.io/py/IngeoDash
 
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+		:target: https://colab.research.google.com/github/INGEOTEC/IngeoDash/blob/docs/docs/IngeoDash.ipynb 
 
 .. code-block:: bash
 
     python -m IngeoDash
```

### Comparing `IngeoDash-0.0.19/LICENSE` & `IngeoDash-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.19/PKG-INFO` & `IngeoDash-0.0.20/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.19
+Version: 0.0.20
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -15,11 +15,13 @@
 
 .. image:: https://coveralls.io/repos/github/INGEOTEC/IngeoDash/badge.svg?branch=develop
 		:target: https://coveralls.io/github/INGEOTEC/IngeoDash?branch=develop
 
 .. image:: https://badge.fury.io/py/IngeoDash.svg
 		:target: https://badge.fury.io/py/IngeoDash
 
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+		:target: https://colab.research.google.com/github/INGEOTEC/IngeoDash/blob/docs/docs/IngeoDash.ipynb 
 
 .. code-block:: bash
 
     python -m IngeoDash
```

### Comparing `IngeoDash-0.0.19/README.rst` & `IngeoDash-0.0.20/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -5,11 +5,13 @@
 
 .. image:: https://coveralls.io/repos/github/INGEOTEC/IngeoDash/badge.svg?branch=develop
 		:target: https://coveralls.io/github/INGEOTEC/IngeoDash?branch=develop
 
 .. image:: https://badge.fury.io/py/IngeoDash.svg
 		:target: https://badge.fury.io/py/IngeoDash
 
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+		:target: https://colab.research.google.com/github/INGEOTEC/IngeoDash/blob/docs/docs/IngeoDash.ipynb 
 
 .. code-block:: bash
 
     python -m IngeoDash
```

### Comparing `IngeoDash-0.0.19/setup.py` & `IngeoDash-0.0.20/setup.py`

 * *Files identical despite different names*

