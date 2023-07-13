# Comparing `tmp/geohashr-0.1.0.tar.gz` & `tmp/geohashr-1.0.0.tar.gz`

## Comparing `geohashr-0.1.0.tar` & `geohashr-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 geohashr-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     1486 2023-07-12 08:30:38.000000 geohashr-0.1.0/LICENSE
--rw-r--r--   0     1001      123      289 2023-07-12 08:30:38.000000 geohashr-0.1.0/README.md
--rw-r--r--   0     1001      123       54 2023-07-12 08:30:38.000000 geohashr-0.1.0/build.rs
--rw-r--r--   0     1001      123       52 2023-07-12 08:30:38.000000 geohashr-0.1.0/geohashr/__init__.py
--rw-r--r--   0     1001      123       22 2023-07-12 08:30:38.000000 geohashr-0.1.0/geohashr/__version__.py
--rw-r--r--   0     1001      123      208 2023-07-12 08:30:38.000000 geohashr-0.1.0/geohashr/_geohashr.pyi
--rw-r--r--   0     1001      123        0 2023-07-12 08:30:38.000000 geohashr-0.1.0/geohashr/py.typed
--rw-r--r--   0     1001      123     1360 2023-07-12 08:30:38.000000 geohashr-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     1654 2023-07-12 08:30:38.000000 geohashr-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123      246 2023-07-12 08:30:38.000000 geohashr-0.1.0/tests/test_decode.py
--rw-r--r--   0     1001      123      197 2023-07-12 08:30:38.000000 geohashr-0.1.0/tests/test_encode.py
--rw-r--r--   0     1001      123    10005 2023-07-12 08:30:38.000000 geohashr-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 geohashr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 geohashr-1.0.0/Cargo.toml
+-rw-r--r--   0     1001      123     1500 2023-07-13 09:55:02.000000 geohashr-1.0.0/LICENSE
+-rw-r--r--   0     1001      123      778 2023-07-13 09:55:02.000000 geohashr-1.0.0/README.md
+-rw-r--r--   0     1001      123       54 2023-07-13 09:55:02.000000 geohashr-1.0.0/build.rs
+-rw-r--r--   0     1001      123      157 2023-07-13 09:55:02.000000 geohashr-1.0.0/geohashr/__init__.py
+-rw-r--r--   0     1001      123       22 2023-07-13 09:55:02.000000 geohashr-1.0.0/geohashr/__version__.py
+-rw-r--r--   0     1001      123      654 2023-07-13 09:55:02.000000 geohashr-1.0.0/geohashr/_geohashr.pyi
+-rw-r--r--   0     1001      123        0 2023-07-13 09:55:02.000000 geohashr-1.0.0/geohashr/py.typed
+-rw-r--r--   0     1001      123     1420 2023-07-13 09:55:02.000000 geohashr-1.0.0/pyproject.toml
+-rw-r--r--   0     1001      123     4751 2023-07-13 09:55:02.000000 geohashr-1.0.0/src/lib.rs
+-rw-r--r--   0     1001      123      786 2023-07-13 09:55:02.000000 geohashr-1.0.0/tests/test_bbox.py
+-rw-r--r--   0     1001      123     1463 2023-07-13 09:55:02.000000 geohashr-1.0.0/tests/test_decode.py
+-rw-r--r--   0     1001      123      203 2023-07-13 09:55:02.000000 geohashr-1.0.0/tests/test_encode.py
+-rw-r--r--   0     1001      123     1338 2023-07-13 09:55:02.000000 geohashr-1.0.0/tests/test_neighbors.py
+-rw-r--r--   0     1001      123    10216 2023-07-13 09:55:02.000000 geohashr-1.0.0/Cargo.lock
+-rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 geohashr-1.0.0/PKG-INFO
```

### Comparing `geohashr-0.1.0/Cargo.toml` & `geohashr-1.0.0/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [package]
 name = "geohashr"
-version = "0.1.0"
+version = "1.0.0"
 description = "Just another geohashing library"
-authors = ["Giovanni Barillari <g@baro.dev>"]
+authors = [
+    "Giovanni Barillari <g@baro.dev>",
+    "Paolo Quadri <pquadri10@gmail.com>"
+]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["geohash"]
 
 readme = "README.md"
 homepage = "https://github.com/gi0baro/geohashr"
@@ -30,14 +33,15 @@
 name = "_geohashr"
 crate-type = ["cdylib"]
 
 [dependencies]
 mimalloc = { version = "0.1.37", default-features = false, features = ["local_dynamic_tls"] }
 geohash = { version = "=0.13" }
 pyo3 = { version = "=0.19", features = ["extension-module"] }
+lazy_static = "1.4.0"
 
 [build-dependencies]
 pyo3-build-config = { version = "=0.19", features = ["resolve-config"] }
 
 [profile.release]
 codegen-units = 1
 debug = false
```

### Comparing `geohashr-0.1.0/LICENSE` & `geohashr-1.0.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023 Giovanni Barillari
+Copyright 2023 Giovanni Barillari, Paolo Quadri
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 1.  Redistributions of source code must retain the above copyright
     notice, this list of conditions and the following disclaimer.
```

### Comparing `geohashr-0.1.0/pyproject.toml` & `geohashr-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "geohashr"
 authors = [
-    {name = "Giovanni Barillari", email = "g@baro.dev"}
+    {name = "Giovanni Barillari", email = "g@baro.dev"},
+    {name = "Paolo Quadri", email = "pquadri10@gmail.com"}
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `geohashr-0.1.0/Cargo.lock` & `geohashr-1.0.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -54,29 +54,36 @@
 dependencies = [
  "geo-types",
  "libm",
 ]
 
 [[package]]
 name = "geohashr"
-version = "0.1.0"
+version = "1.0.0"
 dependencies = [
  "geohash",
+ "lazy_static",
  "mimalloc",
  "pyo3",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "lazy_static"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+
+[[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libm"
```

### Comparing `geohashr-0.1.0/PKG-INFO` & `geohashr-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geohashr
-Version: 0.1.0
+Version: 1.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: pytest ~=7.1.2 ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Just another geohashing library
 Keywords: geohash
 Home-Page: https://github.com/gi0baro/geohashr
-Author: Giovanni Barillari <g@baro.dev>
-Author-email: Giovanni Barillari <g@baro.dev>
+Author: Giovanni Barillari <g@baro.dev>, Paolo Quadri <pquadri10@gmail.com>
+Author-email: Giovanni Barillari <g@baro.dev>, Paolo Quadri <pquadri10@gmail.com>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/gi0baro/geohashr
 Project-URL: Funding, https://github.com/sponsors/gi0baro
 Project-URL: Source, https://github.com/gi0baro/geohashr
 
@@ -42,13 +42,36 @@
 import geohashr
 
 geohashr.encode(45.464664, 9.188540)
 # 't18k68dr5kn8'
 
 geohashr.decode('t18k68dr5kn8')
 # (45.46466404572129, 9.188540065661073)
+
+geohashr.bbox('t18k68dr5kn8')
+# {
+#     'e': 45.464664213359356, 
+#     's': 9.188539981842041, 
+#     'w': 45.46466387808323, 
+#     'n': 9.188540149480104
+# }
+
+geohashr.neighbors('t18k68dr5kn8')
+# {
+#     'e': 't18k68dr5knb', 
+#     'n': 't18k68dr5kn9', 
+#     'ne': 't18k68dr5knc', 
+#     'nw': 't18k68dr5kn3', 
+#     's': 't18k68dr57yx', 
+#     'se': 't18k68dr57yz', 
+#     'sw': 't18k68dr57yr', 
+#     'w': 't18k68dr5kn2'
+# }
+
+geohashr.neighbor('t18k68dr5kn8', 'e')
+# 't18k68dr5knb'
 ```
 
 ## License
 
 Geohashr is released under the BSD License.
```

