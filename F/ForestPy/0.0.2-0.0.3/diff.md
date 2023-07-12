# Comparing `tmp/ForestPy-0.0.2.tar.gz` & `tmp/ForestPy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForestPy-0.0.2.tar", last modified: Wed Jul 12 21:52:57 2023, max compression
+gzip compressed data, was "ForestPy-0.0.3.tar", last modified: Wed Jul 12 23:29:40 2023, max compression
```

## Comparing `ForestPy-0.0.2.tar` & `ForestPy-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:52:57.306477 ForestPy-0.0.2/
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:52:57.152475 ForestPy-0.0.2/ForestPy/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-12 21:51:22.000000 ForestPy-0.0.2/ForestPy/__init__.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1903 2023-07-12 21:51:22.000000 ForestPy-0.0.2/ForestPy/_modidx.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14960 2023-07-12 21:51:22.000000 ForestPy-0.0.2/ForestPy/core.py
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:52:57.282477 ForestPy-0.0.2/ForestPy.egg-info/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1420 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      334 2023-07-12 21:52:57.000000 ForestPy-0.0.2/ForestPy.egg-info/SOURCES.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/dependency_links.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       59 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/entry_points.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:32:00.000000 ForestPy-0.0.2/ForestPy.egg-info/not-zip-safe
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/requires.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        9 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/top_level.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11558 2023-07-09 02:16:06.000000 ForestPy-0.0.2/LICENSE
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestPy-0.0.2/MANIFEST.in
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1420 2023-07-12 21:52:57.303476 ForestPy-0.0.2/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      643 2023-07-11 23:40:52.000000 ForestPy-0.0.2/README.md
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      853 2023-07-12 21:51:22.000000 ForestPy-0.0.2/settings.ini
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-12 21:52:57.307475 ForestPy-0.0.2/setup.cfg
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestPy-0.0.2/setup.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 23:29:40.473949 ForestPy-0.0.3/
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 23:29:40.307949 ForestPy-0.0.3/ForestPy/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-12 23:29:14.000000 ForestPy-0.0.3/ForestPy/__init__.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1903 2023-07-12 23:29:14.000000 ForestPy-0.0.3/ForestPy/_modidx.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14960 2023-07-12 23:29:14.000000 ForestPy-0.0.3/ForestPy/core.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 23:29:40.447949 ForestPy-0.0.3/ForestPy.egg-info/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1400 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      334 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/entry_points.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:32:00.000000 ForestPy-0.0.3/ForestPy.egg-info/not-zip-safe
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/requires.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        9 2023-07-12 23:29:40.000000 ForestPy-0.0.3/ForestPy.egg-info/top_level.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11558 2023-07-09 02:16:06.000000 ForestPy-0.0.3/LICENSE
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestPy-0.0.3/MANIFEST.in
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1400 2023-07-12 23:29:40.470949 ForestPy-0.0.3/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      643 2023-07-11 23:40:52.000000 ForestPy-0.0.3/README.md
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      853 2023-07-12 22:02:17.000000 ForestPy-0.0.3/settings.ini
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-12 23:29:40.474949 ForestPy-0.0.3/setup.cfg
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestPy-0.0.3/setup.py
```

### Comparing `ForestPy-0.0.2/ForestPy/_modidx.py` & `ForestPy-0.0.3/ForestPy/_modidx.py`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.2/ForestPy/core.py` & `ForestPy-0.0.3/ForestPy/core.py`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.2/ForestPy.egg-info/PKG-INFO` & `ForestPy-0.0.3/ForestPy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ForestPy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestPy
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev python florestal inventario
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Portuguese
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,9 +39,7 @@
 e exemplos de uso da biblioteca. Se tiver alguma dúvida ou sugestão, não
 hesite em entrar em contato conosco por meio do LinkedIn ou e-mail.
 
 ## Autor
 
 Gabriel Fernandes Bueno. <br> Linkedin: linkedin.com/in/gabrielfbueno/
 <br> E-mail: gabrielfbueno@outlook.com
-
-
```

### Comparing `ForestPy-0.0.2/LICENSE` & `ForestPy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.2/PKG-INFO` & `ForestPy-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ForestPy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestPy
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev python florestal inventario
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Portuguese
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,9 +39,7 @@
 e exemplos de uso da biblioteca. Se tiver alguma dúvida ou sugestão, não
 hesite em entrar em contato conosco por meio do LinkedIn ou e-mail.
 
 ## Autor
 
 Gabriel Fernandes Bueno. <br> Linkedin: linkedin.com/in/gabrielfbueno/
 <br> E-mail: gabrielfbueno@outlook.com
-
-
```

### Comparing `ForestPy-0.0.2/README.md` & `ForestPy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.2/settings.ini` & `ForestPy-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ForestPy
 lib_name = ForestPy
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ForestPy
 nbs_path = nbs
 recursive = True
```

### Comparing `ForestPy-0.0.2/setup.py` & `ForestPy-0.0.3/setup.py`

 * *Files identical despite different names*

