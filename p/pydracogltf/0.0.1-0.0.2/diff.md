# Comparing `tmp/pydracogltf-0.0.1-py3-none-win_amd64.whl.zip` & `tmp/pydracogltf-0.0.2-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 468108 bytes, number of entries: 10
--rw-r--r--  2.0 unx      227 b- defN 23-Jul-13 05:03 pydracogltf/__init__.py
+Zip file size: 677325 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-13 08:09 pydracogltf/__init__.py
 -rw-r--r--  2.0 unx     5097 b- defN 23-Jul-13 05:42 pydracogltf/gltf_draco_decoder.py
 -rw-r--r--  2.0 unx     7852 b- defN 23-Jul-13 05:42 pydracogltf/gltf_draco_encoder.py
 -rw-rw-r--  2.0 unx   417848 b- defN 23-Jun-27 08:35 pydracogltf/libs/extern_draco.dll
+-rw-rw-r--  2.0 unx   788208 b- defN 23-Jul-13 08:01 pydracogltf/libs/libextern_draco.dylib
 -rwxrwxr-x  2.0 unx  1061712 b- defN 23-Jul-13 05:03 pydracogltf/libs/libextern_draco.so
--rw-rw-r--  2.0 unx     1062 b- defN 23-Jul-13 07:52 pydracogltf-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      602 b- defN 23-Jul-13 07:52 pydracogltf-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 23-Jul-13 07:52 pydracogltf-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-13 07:52 pydracogltf-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      851 b- defN 23-Jul-13 07:52 pydracogltf-0.0.1.dist-info/RECORD
-10 files, 1495361 bytes uncompressed, 466654 bytes compressed:  68.8%
+-rw-rw-r--  2.0 unx     1062 b- defN 23-Jul-13 08:10 pydracogltf-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      579 b- defN 23-Jul-13 08:10 pydracogltf-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-Jul-13 08:10 pydracogltf-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-13 08:10 pydracogltf-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      948 b- defN 23-Jul-13 08:10 pydracogltf-0.0.2.dist-info/RECORD
+11 files, 2283643 bytes uncompressed, 675719 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -6,26 +6,29 @@
 
 Filename: pydracogltf/gltf_draco_encoder.py
 Comment: 
 
 Filename: pydracogltf/libs/extern_draco.dll
 Comment: 
 
+Filename: pydracogltf/libs/libextern_draco.dylib
+Comment: 
+
 Filename: pydracogltf/libs/libextern_draco.so
 Comment: 
 
-Filename: pydracogltf-0.0.1.dist-info/LICENSE
+Filename: pydracogltf-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: pydracogltf-0.0.1.dist-info/METADATA
+Filename: pydracogltf-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pydracogltf-0.0.1.dist-info/WHEEL
+Filename: pydracogltf-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pydracogltf-0.0.1.dist-info/top_level.txt
+Filename: pydracogltf-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pydracogltf-0.0.1.dist-info/RECORD
+Filename: pydracogltf-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydracogltf/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 from .gltf_draco_encoder import encode_primitive_draco
 from .gltf_draco_decoder import decode_primitive_draco
 
 __all__ = [
     "__version__",
     "encode_primitive_draco",
```

## Comparing `pydracogltf-0.0.1.dist-info/LICENSE` & `pydracogltf-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pydracogltf-0.0.1.dist-info/METADATA` & `pydracogltf-0.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pydracogltf
-Version: 0.0.1
+Version: 0.0.2
 Summary: wrapper of blender draco gltf lib, used for trimesh gltf io
 Home-page: https://github.com/seed93/pydracogltf
 Author: Liang Ding
 Author-email: liangding1990@163.com
 License: MIT License
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: logging
 Requires-Dist: numpy
 
 # pydracogltf
 
 wrapper of blender draco gltf lib, used for trimesh gltf io
```

## Comparing `pydracogltf-0.0.1.dist-info/RECORD` & `pydracogltf-0.0.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-pydracogltf/__init__.py,sha256=yIe39oK2e6fCkuhXpR2LWOOTpOn9SomPWITADD-wIdk,227
+pydracogltf/__init__.py,sha256=A2H3qc71bvpnq03dyMLF0C-nvUQpRamMgdR7qaoXXVo,227
 pydracogltf/gltf_draco_decoder.py,sha256=BAO0hOl2RmAwCrgSEKiwlV4u0omZWz8LtMKaqtk3UJ8,5097
 pydracogltf/gltf_draco_encoder.py,sha256=JGml8P6erfrzHk6DclQIpoNvST6o4_Fg1w-wU-mYRO8,7852
 pydracogltf/libs/extern_draco.dll,sha256=T8QFS2zBQRDY0pB_Ub1UbqeeA_nBCNwYUfbTrjlluqI,417848
+pydracogltf/libs/libextern_draco.dylib,sha256=jkKpF0--83iueqZOmA3eLI0alVLSknLbQlT9XCl-Brg,788208
 pydracogltf/libs/libextern_draco.so,sha256=uQKeLt3RlaKhpu6COsv1ICUiZ0WrF0a3_E6gJMXIKOk,1061712
-pydracogltf-0.0.1.dist-info/LICENSE,sha256=DBZAK6xNPrXUVR-Ar-HaGfuxZKzKymlErwGExoFFPto,1062
-pydracogltf-0.0.1.dist-info/METADATA,sha256=Oc9K0n-lDwUa6KtsJf-kh8Ge0z3VPac9a5Mn7Tq9Axg,602
-pydracogltf-0.0.1.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
-pydracogltf-0.0.1.dist-info/top_level.txt,sha256=jFdia7i7hvxYqAYEJ3j4rwegASqmd2whlAj35PWBWvM,12
-pydracogltf-0.0.1.dist-info/RECORD,,
+pydracogltf-0.0.2.dist-info/LICENSE,sha256=DBZAK6xNPrXUVR-Ar-HaGfuxZKzKymlErwGExoFFPto,1062
+pydracogltf-0.0.2.dist-info/METADATA,sha256=BE1z0HfDvcwqdLOl2BEYnySPqyn8MoMkyVLhkawQNAg,579
+pydracogltf-0.0.2.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
+pydracogltf-0.0.2.dist-info/top_level.txt,sha256=jFdia7i7hvxYqAYEJ3j4rwegASqmd2whlAj35PWBWvM,12
+pydracogltf-0.0.2.dist-info/RECORD,,
```

