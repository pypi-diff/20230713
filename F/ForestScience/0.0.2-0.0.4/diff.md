# Comparing `tmp/ForestScience-0.0.2.tar.gz` & `tmp/ForestScience-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForestScience-0.0.2.tar", last modified: Thu Jul 13 04:02:24 2023, max compression
+gzip compressed data, was "ForestScience-0.0.4.tar", last modified: Thu Jul 13 04:16:03 2023, max compression
```

## Comparing `ForestScience-0.0.2.tar` & `ForestScience-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:02:24.877297 ForestScience-0.0.2/
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:02:24.723296 ForestScience-0.0.2/ForestScience/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-13 04:02:05.000000 ForestScience-0.0.2/ForestScience/__init__.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2374 2023-07-13 04:02:05.000000 ForestScience-0.0.2/ForestScience/_modidx.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14954 2023-07-13 04:02:05.000000 ForestScience-0.0.2/ForestScience/inventario.py
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:02:24.853296 ForestScience-0.0.2/ForestScience.egg-info/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1408 2023-07-13 04:02:24.000000 ForestScience-0.0.2/ForestScience.egg-info/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      390 2023-07-13 04:02:24.000000 ForestScience-0.0.2/ForestScience.egg-info/SOURCES.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 04:02:24.000000 ForestScience-0.0.2/ForestScience.egg-info/dependency_links.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       48 2023-07-13 04:02:24.000000 ForestScience-0.0.2/ForestScience.egg-info/entry_points.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 03:36:15.000000 ForestScience-0.0.2/ForestScience.egg-info/not-zip-safe
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-13 04:02:24.000000 ForestScience-0.0.2/ForestScience.egg-info/requires.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       14 2023-07-13 04:02:24.000000 ForestScience-0.0.2/ForestScience.egg-info/top_level.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11357 2023-07-13 03:11:19.000000 ForestScience-0.0.2/LICENSE
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestScience-0.0.2/MANIFEST.in
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1408 2023-07-13 04:02:24.874297 ForestScience-0.0.2/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      625 2023-07-13 03:51:19.000000 ForestScience-0.0.2/README.md
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      876 2023-07-13 04:02:05.000000 ForestScience-0.0.2/settings.ini
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-13 04:02:24.878296 ForestScience-0.0.2/setup.cfg
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestScience-0.0.2/setup.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:16:03.760211 ForestScience-0.0.4/
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:16:03.595210 ForestScience-0.0.4/ForestScience/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14954 2023-07-13 04:15:56.000000 ForestScience-0.0.4/ForestScience/InventarioFlorestal.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-13 04:15:56.000000 ForestScience-0.0.4/ForestScience/__init__.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2689 2023-07-13 04:15:56.000000 ForestScience-0.0.4/ForestScience/_modidx.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 04:16:03.736209 ForestScience-0.0.4/ForestScience.egg-info/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1418 2023-07-13 04:16:03.000000 ForestScience-0.0.4/ForestScience.egg-info/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      399 2023-07-13 04:16:03.000000 ForestScience-0.0.4/ForestScience.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 04:16:03.000000 ForestScience-0.0.4/ForestScience.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       48 2023-07-13 04:16:03.000000 ForestScience-0.0.4/ForestScience.egg-info/entry_points.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 03:36:15.000000 ForestScience-0.0.4/ForestScience.egg-info/not-zip-safe
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-13 04:16:03.000000 ForestScience-0.0.4/ForestScience.egg-info/requires.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       14 2023-07-13 04:16:03.000000 ForestScience-0.0.4/ForestScience.egg-info/top_level.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11357 2023-07-13 03:11:19.000000 ForestScience-0.0.4/LICENSE
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestScience-0.0.4/MANIFEST.in
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1418 2023-07-13 04:16:03.757212 ForestScience-0.0.4/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      635 2023-07-13 04:10:57.000000 ForestScience-0.0.4/README.md
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      876 2023-07-13 04:15:56.000000 ForestScience-0.0.4/settings.ini
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-13 04:16:03.761211 ForestScience-0.0.4/setup.cfg
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestScience-0.0.4/setup.py
```

### Comparing `ForestScience-0.0.2/ForestScience/_modidx.py` & `ForestScience-0.0.4/ForestScience/_modidx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/ForestScience',
                 'doc_host': 'https://gabrielfbueno.github.io',
                 'git_url': 'https://github.com/gabrielfbueno/ForestScience',
                 'lib_path': 'ForestScience'},
-  'syms': { 'ForestScience.inventario': { 'ForestScience.inventario.InventarioFlorestal': ( 'inventario.html#inventarioflorestal',
-                                                                                            'ForestScience/inventario.py'),
-                                          'ForestScience.inventario.InventarioFlorestal.__estatisticas': ( 'inventario.html#inventarioflorestal.__estatisticas',
-                                                                                                           'ForestScience/inventario.py'),
-                                          'ForestScience.inventario.InventarioFlorestal.__grafico': ( 'inventario.html#inventarioflorestal.__grafico',
-                                                                                                      'ForestScience/inventario.py'),
-                                          'ForestScience.inventario.InventarioFlorestal.__init__': ( 'inventario.html#inventarioflorestal.__init__',
-                                                                                                     'ForestScience/inventario.py'),
-                                          'ForestScience.inventario.InventarioFlorestal.__tratativa_tabelas': ( 'inventario.html#inventarioflorestal.__tratativa_tabelas',
-                                                                                                                'ForestScience/inventario.py'),
-                                          'ForestScience.inventario.InventarioFlorestal.distribuicao_diametrica': ( 'inventario.html#inventarioflorestal.distribuicao_diametrica',
-                                                                                                                    'ForestScience/inventario.py'),
-                                          'ForestScience.inventario.InventarioFlorestal.salvar_resultados': ( 'inventario.html#inventarioflorestal.salvar_resultados',
-                                                                                                              'ForestScience/inventario.py')}}}
+  'syms': { 'ForestScience.InventarioFlorestal': { 'ForestScience.InventarioFlorestal.InventarioFlorestal': ( 'inventario.html#inventarioflorestal',
+                                                                                                              'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__estatisticas': ( 'inventario.html#inventarioflorestal.__estatisticas',
+                                                                                                                             'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__grafico': ( 'inventario.html#inventarioflorestal.__grafico',
+                                                                                                                        'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__init__': ( 'inventario.html#inventarioflorestal.__init__',
+                                                                                                                       'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__tratativa_tabelas': ( 'inventario.html#inventarioflorestal.__tratativa_tabelas',
+                                                                                                                                  'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.distribuicao_diametrica': ( 'inventario.html#inventarioflorestal.distribuicao_diametrica',
+                                                                                                                                      'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.salvar_resultados': ( 'inventario.html#inventarioflorestal.salvar_resultados',
+                                                                                                                                'ForestScience/InventarioFlorestal.py')}}}
```

### Comparing `ForestScience-0.0.2/ForestScience/inventario.py` & `ForestScience-0.0.4/ForestScience/InventarioFlorestal.py`

 * *Files identical despite different names*

### Comparing `ForestScience-0.0.2/ForestScience.egg-info/PKG-INFO` & `ForestScience-0.0.4/ForestScience.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestScience
-Version: 0.0.2
+Version: 0.0.4
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestScience
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# ForestPy
+# ForestScience
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-A biblioteca “ForestPy” foi desenvolvida visando simplificar e agilizar
-o cálculo das estatísticas em inventários florestais.
+A biblioteca “ForestScience” foi desenvolvida visando simplificar e
+agilizar o cálculo das estatísticas em inventários florestais.
 
 ## Como instalar
 
 ``` sh
 pip install ForestScience
 ```
```

### Comparing `ForestScience-0.0.2/LICENSE` & `ForestScience-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ForestScience-0.0.2/PKG-INFO` & `ForestScience-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestScience
-Version: 0.0.2
+Version: 0.0.4
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestScience
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# ForestPy
+# ForestScience
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-A biblioteca “ForestPy” foi desenvolvida visando simplificar e agilizar
-o cálculo das estatísticas em inventários florestais.
+A biblioteca “ForestScience” foi desenvolvida visando simplificar e
+agilizar o cálculo das estatísticas em inventários florestais.
 
 ## Como instalar
 
 ``` sh
 pip install ForestScience
 ```
```

### Comparing `ForestScience-0.0.2/README.md` & `ForestScience-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# ForestPy
+# ForestScience
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-A biblioteca “ForestPy” foi desenvolvida visando simplificar e agilizar
-o cálculo das estatísticas em inventários florestais.
+A biblioteca “ForestScience” foi desenvolvida visando simplificar e
+agilizar o cálculo das estatísticas em inventários florestais.
 
 ## Como instalar
 
 ``` sh
 pip install ForestScience
 ```
```

### Comparing `ForestScience-0.0.2/settings.ini` & `ForestScience-0.0.4/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ForestScience
 lib_name = ForestScience
-version = 0.0.2
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ForestScience
 nbs_path = nbs
 recursive = True
```

### Comparing `ForestScience-0.0.2/setup.py` & `ForestScience-0.0.4/setup.py`

 * *Files identical despite different names*

