# Comparing `tmp/uta-gms-engine-0.0.1.tar.gz` & `tmp/uta-gms-engine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "N:\PracaInzynierska\uta-gms-engine\dist\.tmp-98afd0gj\uta-gms-engine-0.0.1.tar", last modified: Thu Jul 13 20:44:54 2023, max compression
+gzip compressed data, was "uta-gms-engine-0.0.2.tar", last modified: Thu Jul 13 21:09:14 2023, max compression
```

## Comparing `uta-gms-engine-0.0.1.tar` & `uta-gms-engine-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 20:44:54.574860 uta-gms-engine-0.0.1/
--rw-rw-rw-   0        0        0      619 2023-07-13 20:44:54.575892 uta-gms-engine-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      100 2023-07-13 20:44:41.000000 uta-gms-engine-0.0.1/README.md
--rw-rw-rw-   0        0        0      112 2023-07-13 20:09:35.000000 uta-gms-engine-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      679 2023-07-13 20:44:54.580891 uta-gms-engine-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-13 20:44:54.560878 uta-gms-engine-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 20:44:54.572862 uta-gms-engine-0.0.1/src/uta_gms_engine.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-13 20:44:54.000000 uta-gms-engine-0.0.1/src/uta_gms_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-13 20:44:54.000000 uta-gms-engine-0.0.1/src/uta_gms_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 20:44:54.000000 uta-gms-engine-0.0.1/src/uta_gms_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-13 20:44:54.000000 uta-gms-engine-0.0.1/src/uta_gms_engine.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 20:44:54.574860 uta-gms-engine-0.0.1/src/utagms/
--rw-rw-rw-   0        0        0       74 2023-07-13 18:45:47.000000 uta-gms-engine-0.0.1/src/utagms/Solver.py
--rw-rw-rw-   0        0        0        0 2023-07-13 18:44:56.000000 uta-gms-engine-0.0.1/src/utagms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-13 21:09:05.000000 uta-gms-engine-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 21:09:05.000000 uta-gms-engine-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 21:09:14.143255 uta-gms-engine-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 21:09:14.000000 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 21:09:14.000000 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:09:14.000000 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 21:09:14.000000 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/src/utagms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:05.000000 uta-gms-engine-0.0.2/src/utagms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 21:09:05.000000 uta-gms-engine-0.0.2/src/utagms/solver.py
```

### Comparing `uta-gms-engine-0.0.1/PKG-INFO` & `uta-gms-engine-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: uta-gms-engine
-Version: 0.0.1
-Summary: Engine for UTA GMS method
-Home-page: https://github.com/UTA-WESOME/uta-gms-engine
-Author: Filip Marciniak
-Author-email: filip.marciniak15@gmail.com
-Project-URL: Bug Tracker, https://github.com/UTA-WESOME/uta-gms-engine/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# UTA GMS ENGINE
-
-## Deploy to PyPI
-
-```commandline
-py -m build
-py -m twine upload dist/*
-```
+Metadata-Version: 2.1
+Name: uta-gms-engine
+Version: 0.0.2
+Summary: Engine for UTA GMS method
+Home-page: https://github.com/UTA-WESOME/uta-gms-engine
+Author: Filip Marciniak
+Author-email: filip.marciniak15@gmail.com
+Project-URL: Bug Tracker, https://github.com/UTA-WESOME/uta-gms-engine/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# UTA GMS ENGINE
+
+## Deploy to PyPI
+
+```commandline
+py -m build
+py -m twine upload dist/*
+```
```

### Comparing `uta-gms-engine-0.0.1/setup.cfg` & `uta-gms-engine-0.0.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2075 7461 2d67 6d73 2d65 6e67 696e   = uta-gms-engin
-00000020: 650d 0a76 6572 7369 6f6e 203d 2030 2e30  e..version = 0.0
-00000030: 2e31 0d0a 6175 7468 6f72 203d 2046 696c  .1..author = Fil
-00000040: 6970 204d 6172 6369 6e69 616b 0d0a 6175  ip Marciniak..au
-00000050: 7468 6f72 5f65 6d61 696c 203d 2066 696c  thor_email = fil
-00000060: 6970 2e6d 6172 6369 6e69 616b 3135 4067  ip.marciniak15@g
-00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
-00000080: 7074 696f 6e20 3d20 456e 6769 6e65 2066  ption = Engine f
-00000090: 6f72 2055 5441 2047 4d53 206d 6574 686f  or UTA GMS metho
-000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000b0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000c0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-000000d0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-000000e0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
-000000f0: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
-00000100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f55  s://github.com/U
-00000110: 5441 2d57 4553 4f4d 452f 7574 612d 676d  TA-WESOME/uta-gm
-00000120: 732d 656e 6769 6e65 0d0a 7072 6f6a 6563  s-engine..projec
-00000130: 745f 7572 6c73 203d 200d 0a09 4275 6720  t_urls = ...Bug 
-00000140: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
-00000150: 2f2f 6769 7468 7562 2e63 6f6d 2f55 5441  //github.com/UTA
-00000160: 2d57 4553 4f4d 452f 7574 612d 676d 732d  -WESOME/uta-gms-
-00000170: 656e 6769 6e65 2f69 7373 7565 730d 0a63  engine/issues..c
-00000180: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-00000190: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001b0: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
-000001c0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000001d0: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-000001e0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000001f0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000200: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000210: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000220: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
-00000230: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-00000240: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000250: 380d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  8....[options.pa
-00000260: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000270: 6572 6520 3d20 7372 630d 0a0d 0a5b 6567  ere = src....[eg
-00000280: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000290: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000002a0: 3d20 300d 0a0d 0a                        = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7574 612d 676d 732d 656e 6769 6e65  = uta-gms-engine
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
+00000030: 0a61 7574 686f 7220 3d20 4669 6c69 7020  .author = Filip 
+00000040: 4d61 7263 696e 6961 6b0a 6175 7468 6f72  Marciniak.author
+00000050: 5f65 6d61 696c 203d 2066 696c 6970 2e6d  _email = filip.m
+00000060: 6172 6369 6e69 616b 3135 4067 6d61 696c  arciniak15@gmail
+00000070: 2e63 6f6d 0a64 6573 6372 6970 7469 6f6e  .com.description
+00000080: 203d 2045 6e67 696e 6520 666f 7220 5554   = Engine for UT
+00000090: 4120 474d 5320 6d65 7468 6f64 0a6c 6f6e  A GMS method.lon
+000000a0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+000000b0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640a  file: README.md.
+000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000d0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000e0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 7572  text/markdown.ur
+000000f0: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+00000100: 7562 2e63 6f6d 2f55 5441 2d57 4553 4f4d  ub.com/UTA-WESOM
+00000110: 452f 7574 612d 676d 732d 656e 6769 6e65  E/uta-gms-engine
+00000120: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
+00000130: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
+00000140: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000150: 6f6d 2f55 5441 2d57 4553 4f4d 452f 7574  om/UTA-WESOME/ut
+00000160: 612d 676d 732d 656e 6769 6e65 2f69 7373  a-gms-engine/iss
+00000170: 7565 730a 636c 6173 7369 6669 6572 7320  ues.classifiers 
+00000180: 3d20 0a09 5072 6f67 7261 6d6d 696e 6720  = ..Programming 
+00000190: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001a0: 6f6e 203a 3a20 330a 094c 6963 656e 7365  on :: 3..License
+000001b0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001c0: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
+000001d0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000001e0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000001f0: 656e 740a 0a5b 6f70 7469 6f6e 735d 0a70  ent..[options].p
+00000200: 6163 6b61 6765 5f64 6972 203d 200a 093d  ackage_dir = ..=
+00000210: 2073 7263 0a70 6163 6b61 6765 7320 3d20   src.packages = 
+00000220: 6669 6e64 3a0a 7079 7468 6f6e 5f72 6571  find:.python_req
+00000230: 7569 7265 7320 3d20 3e3d 332e 380a 0a5b  uires = >=3.8..[
+00000240: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000250: 2e66 696e 645d 0a77 6865 7265 203d 2073  .find].where = s
+00000260: 7263 0a0a 5b65 6767 5f69 6e66 6f5d 0a74  rc..[egg_info].t
+00000270: 6167 5f62 7569 6c64 203d 200a 7461 675f  ag_build = .tag_
+00000280: 6461 7465 203d 2030 0a0a                 date = 0..
```

### Comparing `uta-gms-engine-0.0.1/src/uta_gms_engine.egg-info/PKG-INFO` & `uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: uta-gms-engine
-Version: 0.0.1
-Summary: Engine for UTA GMS method
-Home-page: https://github.com/UTA-WESOME/uta-gms-engine
-Author: Filip Marciniak
-Author-email: filip.marciniak15@gmail.com
-Project-URL: Bug Tracker, https://github.com/UTA-WESOME/uta-gms-engine/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# UTA GMS ENGINE
-
-## Deploy to PyPI
-
-```commandline
-py -m build
-py -m twine upload dist/*
-```
+Metadata-Version: 2.1
+Name: uta-gms-engine
+Version: 0.0.2
+Summary: Engine for UTA GMS method
+Home-page: https://github.com/UTA-WESOME/uta-gms-engine
+Author: Filip Marciniak
+Author-email: filip.marciniak15@gmail.com
+Project-URL: Bug Tracker, https://github.com/UTA-WESOME/uta-gms-engine/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# UTA GMS ENGINE
+
+## Deploy to PyPI
+
+```commandline
+py -m build
+py -m twine upload dist/*
+```
```

