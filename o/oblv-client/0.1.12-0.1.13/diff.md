# Comparing `tmp/oblv_client-0.1.12-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/oblv_client-0.1.13-cp311-cp311-macosx_10_7_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6130110 bytes, number of entries: 5
--rw-r--r--  4.6 unx     2079 b- defN 23-Jul-11 12:11 oblv_client-0.1.12.dist-info/METADATA
--rw-r--r--  4.6 unx      136 b- defN 23-Jul-11 12:11 oblv_client-0.1.12.dist-info/WHEEL
--rw-r--r--  4.6 unx    13552 b- defN 23-Jul-11 12:11 oblv_client/__init__.py
--rwxr-xr-x  4.6 unx 18280200 b- defN 23-Jul-11 12:11 oblv_client/oblv_client.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      419 b- defN 23-Jul-11 12:11 oblv_client-0.1.12.dist-info/RECORD
-5 files, 18296386 bytes uncompressed, 6129340 bytes compressed:  66.5%
+Zip file size: 4340599 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     2079 b- defN 23-Jul-13 17:01 oblv_client-0.1.13.dist-info/METADATA
+-rw-r--r--  4.6 unx      107 b- defN 23-Jul-13 17:01 oblv_client-0.1.13.dist-info/WHEEL
+-rw-r--r--  4.6 unx    13552 b- defN 23-Jul-13 17:01 oblv_client/__init__.py
+-rwxr-xr-x  4.6 unx 11335520 b- defN 23-Jul-13 17:01 oblv_client/oblv_client.cpython-311-darwin.so
+-rw-r--r--  4.6 unx      409 b- defN 23-Jul-13 17:01 oblv_client-0.1.13.dist-info/RECORD
+5 files, 11351667 bytes uncompressed, 4339849 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: oblv_client-0.1.12.dist-info/METADATA
+Filename: oblv_client-0.1.13.dist-info/METADATA
 Comment: 
 
-Filename: oblv_client-0.1.12.dist-info/WHEEL
+Filename: oblv_client-0.1.13.dist-info/WHEEL
 Comment: 
 
 Filename: oblv_client/__init__.py
 Comment: 
 
-Filename: oblv_client/oblv_client.pypy39-pp73-x86_64-linux-gnu.so
+Filename: oblv_client/oblv_client.cpython-311-darwin.so
 Comment: 
 
-Filename: oblv_client-0.1.12.dist-info/RECORD
+Filename: oblv_client-0.1.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `oblv_client-0.1.12.dist-info/METADATA` & `oblv_client-0.1.13.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oblv-client
-Version: 0.1.12
+Version: 0.1.13
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: urllib3
 Summary: python bindings for using enclaves with oblivious tooling
 Home-Page: https://oblivious.ai
 Author: OBLV Devs <hello@oblivious.ai>
```

