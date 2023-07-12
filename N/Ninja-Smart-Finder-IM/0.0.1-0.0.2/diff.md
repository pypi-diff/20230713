# Comparing `tmp/Ninja_Smart_Finder_IM-0.0.1.tar.gz` & `tmp/Ninja_Smart_Finder_IM-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ninja_Smart_Finder_IM-0.0.1.tar", last modified: Wed Jul 12 21:43:28 2023, max compression
+gzip compressed data, was "Ninja_Smart_Finder_IM-0.0.2.tar", last modified: Wed Jul 12 22:04:59 2023, max compression
```

## Comparing `Ninja_Smart_Finder_IM-0.0.1.tar` & `Ninja_Smart_Finder_IM-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 21:43:28.621479 Ninja_Smart_Finder_IM-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-07-12 21:33:11.000000 Ninja_Smart_Finder_IM-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      647 2023-07-12 21:43:28.621770 Ninja_Smart_Finder_IM-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-12 21:34:25.000000 Ninja_Smart_Finder_IM-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      788 2023-07-12 21:43:28.623957 Ninja_Smart_Finder_IM-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 21:43:28.580620 Ninja_Smart_Finder_IM-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 21:43:28.610766 Ninja_Smart_Finder_IM-0.0.1/src/Ninja_Smart_Finder_IM.egg-info/
--rw-rw-rw-   0        0        0      647 2023-07-12 21:43:28.000000 Ninja_Smart_Finder_IM-0.0.1/src/Ninja_Smart_Finder_IM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-12 21:43:28.000000 Ninja_Smart_Finder_IM-0.0.1/src/Ninja_Smart_Finder_IM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 21:43:28.000000 Ninja_Smart_Finder_IM-0.0.1/src/Ninja_Smart_Finder_IM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 21:43:28.000000 Ninja_Smart_Finder_IM-0.0.1/src/Ninja_Smart_Finder_IM.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 21:43:28.618441 Ninja_Smart_Finder_IM-0.0.1/src/mypackage/
--rw-rw-rw-   0        0        0        0 2023-07-12 21:33:11.000000 Ninja_Smart_Finder_IM-0.0.1/src/mypackage/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-12 21:33:12.000000 Ninja_Smart_Finder_IM-0.0.1/src/mypackage/main.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:04:59.816323 Ninja_Smart_Finder_IM-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-07-12 21:33:11.000000 Ninja_Smart_Finder_IM-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      647 2023-07-12 22:04:59.816323 Ninja_Smart_Finder_IM-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-12 21:34:25.000000 Ninja_Smart_Finder_IM-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      788 2023-07-12 22:04:59.819896 Ninja_Smart_Finder_IM-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 22:04:59.776106 Ninja_Smart_Finder_IM-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 22:04:59.809177 Ninja_Smart_Finder_IM-0.0.2/src/Ninja_Smart_Finder_IM.egg-info/
+-rw-rw-rw-   0        0        0      647 2023-07-12 22:04:59.000000 Ninja_Smart_Finder_IM-0.0.2/src/Ninja_Smart_Finder_IM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-12 22:04:59.000000 Ninja_Smart_Finder_IM-0.0.2/src/Ninja_Smart_Finder_IM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 22:04:59.000000 Ninja_Smart_Finder_IM-0.0.2/src/Ninja_Smart_Finder_IM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 22:04:59.000000 Ninja_Smart_Finder_IM-0.0.2/src/Ninja_Smart_Finder_IM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 22:04:59.813333 Ninja_Smart_Finder_IM-0.0.2/src/mypackage/
+-rw-rw-rw-   0        0        0        0 2023-07-12 21:33:11.000000 Ninja_Smart_Finder_IM-0.0.2/src/mypackage/__init__.py
+-rw-rw-rw-   0        0        0      117 2023-07-12 22:01:45.000000 Ninja_Smart_Finder_IM-0.0.2/src/mypackage/main.py
```

### Comparing `Ninja_Smart_Finder_IM-0.0.1/PKG-INFO` & `Ninja_Smart_Finder_IM-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ninja_Smart_Finder_IM
-Version: 0.0.1
+Version: 0.0.2
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/Ninja_Smart_Finder_IM
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/Ninja_Smart_Finder_IM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ninja_Smart_Finder_IM-0.0.1/setup.cfg` & `Ninja_Smart_Finder_IM-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696e 6a61 5f53 6d61 7274 5f46   = Ninja_Smart_F
 00000020: 696e 6465 725f 494d 0d0a 7665 7273 696f  inder_IM..versio
-00000030: 6e20 3d20 302e 302e 310d 0a61 7574 686f  n = 0.0.1..autho
+00000030: 6e20 3d20 302e 302e 320d 0a61 7574 686f  n = 0.0.2..autho
 00000040: 7220 3d20 4d6f 6861 6d65 6420 456c 6861  r = Mohamed Elha
 00000050: 6a61 6264 6f75 0d0a 6175 7468 6f72 5f65  jabdou..author_e
 00000060: 6d61 696c 203d 206d 6f68 616d 6564 656c  mail = mohamedel
 00000070: 7361 7965 646d 6f68 616d 6d65 642e 3230  sayedmohammed.20
 00000080: 3230 4067 6d61 696c 2e63 6f6d 0d0a 6465  20@gmail.com..de
 00000090: 7363 7269 7074 696f 6e20 3d20 7468 6973  scription = this
 000000a0: 2076 6572 7369 6f6e 2069 7320 666f 7220   version is for
```

### Comparing `Ninja_Smart_Finder_IM-0.0.1/src/Ninja_Smart_Finder_IM.egg-info/PKG-INFO` & `Ninja_Smart_Finder_IM-0.0.2/src/Ninja_Smart_Finder_IM.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ninja-Smart-Finder-IM
-Version: 0.0.1
+Version: 0.0.2
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/Ninja_Smart_Finder_IM
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/Ninja_Smart_Finder_IM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

