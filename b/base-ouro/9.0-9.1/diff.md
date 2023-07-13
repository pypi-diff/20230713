# Comparing `tmp/base_ouro-9.0.tar.gz` & `tmp/base_ouro-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_ouro-9.0.tar", last modified: Fri Jan 27 13:25:52 2023, max compression
+gzip compressed data, was "base_ouro-9.1.tar", last modified: Fri Jan 27 13:53:01 2023, max compression
```

## Comparing `base_ouro-9.0.tar` & `base_ouro-9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 13:25:52.513366 base_ouro-9.0/
-drwxrwxrwx   0        0        0        0 2023-01-27 13:25:52.480399 base_ouro-9.0/Base Ouro/
--rw-rw-rw-   0        0        0       26 2023-01-27 13:15:10.000000 base_ouro-9.0/Base Ouro/__init__.py
--rw-rw-rw-   0        0        0    22106 2023-01-27 13:17:52.000000 base_ouro-9.0/Base Ouro/base_ouro.py
--rw-rw-rw-   0        0        0     1094 2023-01-27 13:16:28.000000 base_ouro-9.0/LICENSE.txt
--rw-rw-rw-   0        0        0      990 2023-01-27 13:25:52.513917 base_ouro-9.0/PKG-INFO
--rw-rw-rw-   0        0        0      675 2023-01-27 13:23:01.000000 base_ouro-9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-27 13:25:52.510302 base_ouro-9.0/base_ouro.egg-info/
--rw-rw-rw-   0        0        0      990 2023-01-27 13:25:52.000000 base_ouro-9.0/base_ouro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-01-27 13:25:52.000000 base_ouro-9.0/base_ouro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 13:25:52.000000 base_ouro-9.0/base_ouro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-01-27 13:25:52.000000 base_ouro-9.0/base_ouro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-01-27 13:25:52.520043 base_ouro-9.0/setup.cfg
--rw-rw-rw-   0        0        0      429 2023-01-27 13:25:26.000000 base_ouro-9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-27 13:53:01.789222 base_ouro-9.1/
+-rw-rw-rw-   0        0        0     1094 2023-01-27 13:16:28.000000 base_ouro-9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      990 2023-01-27 13:53:01.790219 base_ouro-9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-01-27 13:23:01.000000 base_ouro-9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-01-27 13:53:01.760557 base_ouro-9.1/base_ouro/
+-rw-rw-rw-   0        0        0       26 2023-01-27 13:15:10.000000 base_ouro-9.1/base_ouro/__init__.py
+-rw-rw-rw-   0        0        0    22106 2023-01-27 13:17:52.000000 base_ouro-9.1/base_ouro/base_ouro.py
+drwxrwxrwx   0        0        0        0 2023-01-27 13:53:01.787223 base_ouro-9.1/base_ouro.egg-info/
+-rw-rw-rw-   0        0        0      990 2023-01-27 13:53:01.000000 base_ouro-9.1/base_ouro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-01-27 13:53:01.000000 base_ouro-9.1/base_ouro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-27 13:53:01.000000 base_ouro-9.1/base_ouro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-01-27 13:53:01.000000 base_ouro-9.1/base_ouro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-01-27 13:53:01.797219 base_ouro-9.1/setup.cfg
+-rw-rw-rw-   0        0        0      429 2023-01-27 13:49:05.000000 base_ouro-9.1/setup.py
```

### Comparing `base_ouro-9.0/Base Ouro/base_ouro.py` & `base_ouro-9.1/base_ouro/base_ouro.py`

 * *Files identical despite different names*

### Comparing `base_ouro-9.0/LICENSE.txt` & `base_ouro-9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `base_ouro-9.0/PKG-INFO` & `base_ouro-9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base_ouro
-Version: 9.0
+Version: 9.1
 Summary: Conversor utilizado para a geração da Base Ouro
 Author: Gabriel Ernesto Barboza Pereira
 Author-email: ernesto.gabriel@pucpr.br
 License: MIT
 Keywords: conversor base_ouro
 License-File: LICENSE.txt
```

### Comparing `base_ouro-9.0/README.md` & `base_ouro-9.1/README.md`

 * *Files identical despite different names*

### Comparing `base_ouro-9.0/base_ouro.egg-info/PKG-INFO` & `base_ouro-9.1/base_ouro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-ouro
-Version: 9.0
+Version: 9.1
 Summary: Conversor utilizado para a geração da Base Ouro
 Author: Gabriel Ernesto Barboza Pereira
 Author-email: ernesto.gabriel@pucpr.br
 License: MIT
 Keywords: conversor base_ouro
 License-File: LICENSE.txt
```

