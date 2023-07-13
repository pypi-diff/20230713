# Comparing `tmp/ForestPy-0.0.3.tar.gz` & `tmp/ForestPy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForestPy-0.0.3.tar", last modified: Wed Jul 12 23:29:40 2023, max compression
+gzip compressed data, was "ForestPy-0.0.4.tar", last modified: Thu Jul 13 03:28:22 2023, max compression
```

## Comparing `ForestPy-0.0.3.tar` & `ForestPy-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 23:29:40.473949 ForestPy-0.0.3/
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 23:29:40.307949 ForestPy-0.0.3/ForestPy/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-12 23:29:14.000000 ForestPy-0.0.3/ForestPy/__init__.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1903 2023-07-12 23:29:14.000000 ForestPy-0.0.3/ForestPy/_modidx.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14960 2023-07-12 23:29:14.000000 ForestPy-0.0.3/ForestPy/core.py
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 23:29:40.447949 ForestPy-0.0.3/ForestPy.egg-info/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1400 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      334 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/SOURCES.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/dependency_links.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/entry_points.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:32:00.000000 ForestPy-0.0.3/ForestPy.egg-info/not-zip-safe
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/requires.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        9 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/top_level.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11558 2023-07-09 02:16:06.000000 ForestPy-0.0.3/LICENSE
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestPy-0.0.3/MANIFEST.in
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1400 2023-07-12 23:29:40.470949 ForestPy-0.0.3/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      643 2023-07-11 23:40:52.000000 ForestPy-0.0.3/README.md
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      853 2023-07-12 22:02:17.000000 ForestPy-0.0.3/settings.ini
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-12 23:29:40.474949 ForestPy-0.0.3/setup.cfg
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestPy-0.0.3/setup.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 03:28:22.487657 ForestPy-0.0.4/
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 03:28:22.322655 ForestPy-0.0.4/ForestPy/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-13 03:28:10.000000 ForestPy-0.0.4/ForestPy/__init__.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2184 2023-07-13 03:28:10.000000 ForestPy-0.0.4/ForestPy/_modidx.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14960 2023-07-13 03:28:10.000000 ForestPy-0.0.4/ForestPy/inventario.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 03:28:22.461655 ForestPy-0.0.4/ForestPy.egg-info/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1400 2023-07-13 03:28:22.000000 ForestPy-0.0.4/ForestPy.egg-info/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      340 2023-07-13 03:28:22.000000 ForestPy-0.0.4/ForestPy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 03:28:22.000000 ForestPy-0.0.4/ForestPy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-13 03:28:22.000000 ForestPy-0.0.4/ForestPy.egg-info/entry_points.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:32:00.000000 ForestPy-0.0.4/ForestPy.egg-info/not-zip-safe
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-13 03:28:22.000000 ForestPy-0.0.4/ForestPy.egg-info/requires.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        9 2023-07-13 03:28:22.000000 ForestPy-0.0.4/ForestPy.egg-info/top_level.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11558 2023-07-09 02:16:06.000000 ForestPy-0.0.4/LICENSE
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestPy-0.0.4/MANIFEST.in
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1400 2023-07-13 03:28:22.484656 ForestPy-0.0.4/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      620 2023-07-13 03:27:04.000000 ForestPy-0.0.4/README.md
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      853 2023-07-13 03:28:10.000000 ForestPy-0.0.4/settings.ini
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-13 03:28:22.488657 ForestPy-0.0.4/setup.cfg
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestPy-0.0.4/setup.py
```

### Comparing `ForestPy-0.0.3/ForestPy/_modidx.py` & `ForestPy-0.0.4/ForestPy/_modidx.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/ForestPy',
                 'doc_host': 'https://gabrielfbueno.github.io',
                 'git_url': 'https://github.com/gabrielfbueno/ForestPy',
                 'lib_path': 'ForestPy'},
-  'syms': { 'ForestPy.core': { 'ForestPy.core.InventarioFlorestal': ('inventario.html#inventarioflorestal', 'ForestPy/core.py'),
-                               'ForestPy.core.InventarioFlorestal.__estatisticas': ( 'inventario.html#inventarioflorestal.__estatisticas',
-                                                                                     'ForestPy/core.py'),
-                               'ForestPy.core.InventarioFlorestal.__grafico': ( 'inventario.html#inventarioflorestal.__grafico',
-                                                                                'ForestPy/core.py'),
-                               'ForestPy.core.InventarioFlorestal.__init__': ( 'inventario.html#inventarioflorestal.__init__',
-                                                                               'ForestPy/core.py'),
-                               'ForestPy.core.InventarioFlorestal.__tratativa_tabelas': ( 'inventario.html#inventarioflorestal.__tratativa_tabelas',
-                                                                                          'ForestPy/core.py'),
-                               'ForestPy.core.InventarioFlorestal.distribuicao_diametrica': ( 'inventario.html#inventarioflorestal.distribuicao_diametrica',
-                                                                                              'ForestPy/core.py'),
-                               'ForestPy.core.InventarioFlorestal.salvar_resultados': ( 'inventario.html#inventarioflorestal.salvar_resultados',
-                                                                                        'ForestPy/core.py')}}}
+  'syms': { 'ForestPy.inventario': { 'ForestPy.inventario.InventarioFlorestal': ( 'inventario.html#inventarioflorestal',
+                                                                                  'ForestPy/inventario.py'),
+                                     'ForestPy.inventario.InventarioFlorestal.__estatisticas': ( 'inventario.html#inventarioflorestal.__estatisticas',
+                                                                                                 'ForestPy/inventario.py'),
+                                     'ForestPy.inventario.InventarioFlorestal.__grafico': ( 'inventario.html#inventarioflorestal.__grafico',
+                                                                                            'ForestPy/inventario.py'),
+                                     'ForestPy.inventario.InventarioFlorestal.__init__': ( 'inventario.html#inventarioflorestal.__init__',
+                                                                                           'ForestPy/inventario.py'),
+                                     'ForestPy.inventario.InventarioFlorestal.__tratativa_tabelas': ( 'inventario.html#inventarioflorestal.__tratativa_tabelas',
+                                                                                                      'ForestPy/inventario.py'),
+                                     'ForestPy.inventario.InventarioFlorestal.distribuicao_diametrica': ( 'inventario.html#inventarioflorestal.distribuicao_diametrica',
+                                                                                                          'ForestPy/inventario.py'),
+                                     'ForestPy.inventario.InventarioFlorestal.salvar_resultados': ( 'inventario.html#inventarioflorestal.salvar_resultados',
+                                                                                                    'ForestPy/inventario.py')}}}
```

### Comparing `ForestPy-0.0.3/ForestPy/core.py` & `ForestPy-0.0.4/ForestPy/inventario.py`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.3/ForestPy.egg-info/PKG-INFO` & `ForestPy-0.0.4/ForestPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestPy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestPy
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev python florestal inventario
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ForestPy-0.0.3/LICENSE` & `ForestPy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.3/PKG-INFO` & `ForestPy-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestPy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestPy
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev python florestal inventario
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ForestPy-0.0.3/README.md` & `ForestPy-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ForestPy
-
-<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-
-A biblioteca “ForestPy” foi desenvolvida visando simplificar e agilizar
-o cálculo das estatísticas em inventários florestais.
-
-## Como instalar
-
-``` sh
-pip install ForestPy
-```
-
-## Como usar?
-
-No tópico “InventarioFlorestal”, você encontrará a documentação completa
-e exemplos de uso da biblioteca. Se tiver alguma dúvida ou sugestão, não
-hesite em entrar em contato conosco por meio do LinkedIn ou e-mail.
-
-## Autor
-
-Gabriel Fernandes Bueno. <br> Linkedin: linkedin.com/in/gabrielfbueno/
-<br> E-mail: gabrielfbueno@outlook.com
+# ForestPy
+
+<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+A biblioteca “ForestPy” foi desenvolvida visando simplificar e agilizar
+o cálculo das estatísticas em inventários florestais.
+
+## Como instalar
+
+``` sh
+pip install ForestPy
+```
+
+## Como usar?
+
+No tópico “InventarioFlorestal”, você encontrará a documentação completa
+e exemplos de uso da biblioteca. Se tiver alguma dúvida ou sugestão, não
+hesite em entrar em contato conosco por meio do LinkedIn ou e-mail.
+
+## Autor
+
+Gabriel Fernandes Bueno. <br> Linkedin: linkedin.com/in/gabrielfbueno/
+<br> E-mail: gabrielfbueno@outlook.com
```

### Comparing `ForestPy-0.0.3/settings.ini` & `ForestPy-0.0.4/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ForestPy
 lib_name = ForestPy
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ForestPy
 nbs_path = nbs
 recursive = True
```

### Comparing `ForestPy-0.0.3/setup.py` & `ForestPy-0.0.4/setup.py`

 * *Files identical despite different names*

