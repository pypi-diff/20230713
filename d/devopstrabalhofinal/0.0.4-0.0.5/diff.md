# Comparing `tmp/devopstrabalhofinal-0.0.4.tar.gz` & `tmp/devopstrabalhofinal-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstrabalhofinal-0.0.4.tar", last modified: Thu Jul 13 00:49:37 2023, max compression
+gzip compressed data, was "devopstrabalhofinal-0.0.5.tar", last modified: Thu Jul 13 01:16:45 2023, max compression
```

## Comparing `devopstrabalhofinal-0.0.4.tar` & `devopstrabalhofinal-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:49:37.912761 devopstrabalhofinal-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 00:49:27.000000 devopstrabalhofinal-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-13 00:49:37.912761 devopstrabalhofinal-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 00:49:27.000000 devopstrabalhofinal-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-13 00:49:27.000000 devopstrabalhofinal-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 00:49:27.000000 devopstrabalhofinal-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:49:37.912761 devopstrabalhofinal-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:49:37.912761 devopstrabalhofinal-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:49:37.912761 devopstrabalhofinal-0.0.4/src/codigo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 00:49:27.000000 devopstrabalhofinal-0.0.4/src/codigo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 00:49:27.000000 devopstrabalhofinal-0.0.4/src/codigo/comando.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:49:37.912761 devopstrabalhofinal-0.0.4/src/devopstrabalhofinal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-13 00:49:37.000000 devopstrabalhofinal-0.0.4/src/devopstrabalhofinal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-13 00:49:37.000000 devopstrabalhofinal-0.0.4/src/devopstrabalhofinal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:49:37.000000 devopstrabalhofinal-0.0.4/src/devopstrabalhofinal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 00:49:37.000000 devopstrabalhofinal-0.0.4/src/devopstrabalhofinal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 00:49:37.000000 devopstrabalhofinal-0.0.4/src/devopstrabalhofinal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:49:37.912761 devopstrabalhofinal-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 00:49:27.000000 devopstrabalhofinal-0.0.4/test/test_saudacao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.205706 devopstrabalhofinal-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/src/codigo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/src/codigo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/src/codigo/comando.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 01:16:45.000000 devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 01:16:45.209706 devopstrabalhofinal-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 01:16:33.000000 devopstrabalhofinal-0.0.5/test/test_saudacao.py
```

### Comparing `devopstrabalhofinal-0.0.4/LICENSE` & `devopstrabalhofinal-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `devopstrabalhofinal-0.0.4/PKG-INFO` & `devopstrabalhofinal-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstrabalhofinal
-Version: 0.0.4
+Version: 0.0.5
 Summary: Código de Comando: Saudação
 Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimentagit <1286408@sga.pucminas.br>
 Project-URL: Homepage, https://github.com/jvmg96/devops_trabalho
 Project-URL: Bug Tracker, https://github.com/jvmg96/devops_trabalho/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,14 @@
 License-File: LICENSE
 
 # Trabalho Final - DevOps
 
 Código Comando: Saudação
 
 ## Grupo:
-João Victor Milgres Guimarães
+João Victor Milagres Guimarães
 
 Allan da Silveira e Silva
 
 Felipe Ferreira Alexandre
 
 Gabriel Murta Pimentagit
```

### Comparing `devopstrabalhofinal-0.0.4/pyproject.toml` & `devopstrabalhofinal-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "devopstrabalhofinal"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="João Victor Milagres Guimarães", email="1398500@sga.pucminas.br" },
   { name="Allan da Silveira e Silva", email="1405224@sga.pucminas.br" },
   { name="Felipe Ferreira Alexandre", email="1386198@sga.pucminas.br" },
   { name="Gabriel Murta Pimentagit", email="1286408@sga.pucminas.br" },
 ]
 description = "Código de Comando: Saudação"
```

### Comparing `devopstrabalhofinal-0.0.4/src/devopstrabalhofinal.egg-info/PKG-INFO` & `devopstrabalhofinal-0.0.5/src/devopstrabalhofinal.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstrabalhofinal
-Version: 0.0.4
+Version: 0.0.5
 Summary: Código de Comando: Saudação
 Author-email: João Victor Milagres Guimarães <1398500@sga.pucminas.br>, Allan da Silveira e Silva <1405224@sga.pucminas.br>, Felipe Ferreira Alexandre <1386198@sga.pucminas.br>, Gabriel Murta Pimentagit <1286408@sga.pucminas.br>
 Project-URL: Homepage, https://github.com/jvmg96/devops_trabalho
 Project-URL: Bug Tracker, https://github.com/jvmg96/devops_trabalho/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,14 @@
 License-File: LICENSE
 
 # Trabalho Final - DevOps
 
 Código Comando: Saudação
 
 ## Grupo:
-João Victor Milgres Guimarães
+João Victor Milagres Guimarães
 
 Allan da Silveira e Silva
 
 Felipe Ferreira Alexandre
 
 Gabriel Murta Pimentagit
```

