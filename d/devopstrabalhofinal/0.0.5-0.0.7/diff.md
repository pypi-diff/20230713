# Comparing `tmp/devopstrabalhofinal-0.0.5.tar.gz` & `tmp/devopstrabalhofinal-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstrabalhofinal-0.0.5.tar", last modified: Thu Jul 13 01:16:45 2023, max compression
+gzip compressed data, was "devopstrabalhofinal-0.0.7.tar", last modified: Thu Jul 13 01:24:49 2023, max compression
```

## Comparing `devopstrabalhofinal-0.0.5.tar` & `devopstrabalhofinal-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.205706 devopstrabalhofinal-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/src/codigo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/src/codigo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/src/codigo/comando.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/test/test_saudacao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:24:49.097838 devopstrabalhofinal-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 01:24:37.000000 devopstrabalhofinal-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-13 01:24:49.097838 devopstrabalhofinal-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-13 01:24:37.000000 devopstrabalhofinal-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-13 01:24:37.000000 devopstrabalhofinal-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 01:24:37.000000 devopstrabalhofinal-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 01:24:49.097838 devopstrabalhofinal-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:24:49.097838 devopstrabalhofinal-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:24:49.097838 devopstrabalhofinal-0.0.7/src/codigo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 01:24:37.000000 devopstrabalhofinal-0.0.7/src/codigo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 01:24:37.000000 devopstrabalhofinal-0.0.7/src/codigo/comando.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:24:49.097838 devopstrabalhofinal-0.0.7/src/devopstrabalhofinal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-13 01:24:49.000000 devopstrabalhofinal-0.0.7/src/devopstrabalhofinal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-13 01:24:49.000000 devopstrabalhofinal-0.0.7/src/devopstrabalhofinal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 01:24:49.000000 devopstrabalhofinal-0.0.7/src/devopstrabalhofinal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 01:24:49.000000 devopstrabalhofinal-0.0.7/src/devopstrabalhofinal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 01:24:49.000000 devopstrabalhofinal-0.0.7/src/devopstrabalhofinal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:24:49.097838 devopstrabalhofinal-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 01:24:37.000000 devopstrabalhofinal-0.0.7/test/test_saudacao.py
```

### Comparing `devopstrabalhofinal-0.0.5/LICENSE` & `devopstrabalhofinal-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `devopstrabalhofinal-0.0.5/PKG-INFO` & `devopstrabalhofinal-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: devopstrabalhofinal
-Version: 0.0.5
+Version: 0.0.7
 Summary: Código de Comando: Saudação
-Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimentagit <1286408@sga.pucminas.br>
+Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimenta <1286408@sga.pucminas.br>
 Project-URL: Homepage, https://github.com/jvmg96/devops_trabalho
 Project-URL: Bug Tracker, https://github.com/jvmg96/devops_trabalho/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -19,8 +19,8 @@
 ## Grupo:
 João Victor Milagres Guimarães
 
 Allan da Silveira e Silva
 
 Felipe Ferreira Alexandre
 
-Gabriel Murta Pimentagit
+Gabriel Murta Pimenta
```

### Comparing `devopstrabalhofinal-0.0.5/pyproject.toml` & `devopstrabalhofinal-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "devopstrabalhofinal"
-version = "0.0.5"
+version = "0.0.7"
 authors = [
   { name="João Victor Milagres Guimarães", email="1398500@sga.pucminas.br" },
   { name="Allan da Silveira e Silva", email="1405224@sga.pucminas.br" },
   { name="Felipe Ferreira Alexandre", email="1386198@sga.pucminas.br" },
-  { name="Gabriel Murta Pimentagit", email="1286408@sga.pucminas.br" },
+  { name="Gabriel Murta Pimenta", email="1286408@sga.pucminas.br" },
 ]
 description = "Código de Comando: Saudação"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/PKG-INFO` & `devopstrabalhofinal-0.0.7/src/devopstrabalhofinal.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: devopstrabalhofinal
-Version: 0.0.5
+Version: 0.0.7
 Summary: Código de Comando: Saudação
-Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimentagit <1286408@sga.pucminas.br>
+Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimenta <1286408@sga.pucminas.br>
 Project-URL: Homepage, https://github.com/jvmg96/devops_trabalho
 Project-URL: Bug Tracker, https://github.com/jvmg96/devops_trabalho/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -19,8 +19,8 @@
 ## Grupo:
 João Victor Milagres Guimarães
 
 Allan da Silveira e Silva
 
 Felipe Ferreira Alexandre
 
-Gabriel Murta Pimentagit
+Gabriel Murta Pimenta
```

