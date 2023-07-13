# Comparing `tmp/yori-1.7.7-py3-none-any.whl.zip` & `tmp/yori-1.7.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 24052 bytes, number of entries: 17
+Zip file size: 24148 bytes, number of entries: 17
 -rwxr-xr-x  2.0 unx     6464 b- defN 20-Feb-02 00:00 yori/IOtools.py
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 yori/__init__.py
 -rw-r--r--  2.0 unx    14015 b- defN 20-Feb-02 00:00 yori/aggrtools.py
 -rw-r--r--  2.0 unx     4670 b- defN 20-Feb-02 00:00 yori/config_reader.py
 -rw-r--r--  2.0 unx    20221 b- defN 20-Feb-02 00:00 yori/gridtools.py
 -rwxr-xr-x  2.0 unx    10158 b- defN 20-Feb-02 00:00 yori/run_yori.py
 -rw-r--r--  2.0 unx    11502 b- defN 20-Feb-02 00:00 yori/yori_aggregate.py
 -rw-r--r--  2.0 unx     5807 b- defN 20-Feb-02 00:00 yori/yori_merge.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 yori/tools/__init__.py
--rw-r--r--  2.0 unx     3424 b- defN 20-Feb-02 00:00 yori/tools/aggr.py
--rw-r--r--  2.0 unx     1196 b- defN 20-Feb-02 00:00 yori/tools/grid.py
+-rw-r--r--  2.0 unx     3540 b- defN 20-Feb-02 00:00 yori/tools/aggr.py
+-rw-r--r--  2.0 unx     1305 b- defN 20-Feb-02 00:00 yori/tools/grid.py
 -rw-r--r--  2.0 unx     2268 b- defN 20-Feb-02 00:00 yori/tools/merge.py
-?rw-r--r--  2.0 unx     1129 b- defN 20-Feb-02 00:00 yori-1.7.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 yori-1.7.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx      119 b- defN 20-Feb-02 00:00 yori-1.7.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 yori-1.7.7.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1286 b- defN 20-Feb-02 00:00 yori-1.7.7.dist-info/RECORD
-17 files, 83437 bytes uncompressed, 21988 bytes compressed:  73.6%
+?rw-r--r--  2.0 unx     1179 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx      119 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1286 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/RECORD
+17 files, 83712 bytes uncompressed, 22084 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: yori/tools/grid.py
 Comment: 
 
 Filename: yori/tools/merge.py
 Comment: 
 
-Filename: yori-1.7.7.dist-info/METADATA
+Filename: yori-1.7.8.dist-info/METADATA
 Comment: 
 
-Filename: yori-1.7.7.dist-info/WHEEL
+Filename: yori-1.7.8.dist-info/WHEEL
 Comment: 
 
-Filename: yori-1.7.7.dist-info/entry_points.txt
+Filename: yori-1.7.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: yori-1.7.7.dist-info/licenses/LICENSE
+Filename: yori-1.7.8.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: yori-1.7.7.dist-info/RECORD
+Filename: yori-1.7.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yori/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.7.7"
+__version__ = "1.7.8"
```

## yori/tools/aggr.py

```diff
@@ -1,11 +1,15 @@
 import sys
 import os.path
 
-from ..yori_aggregate import aggregate
+try:
+    from yori.yori_aggregate import aggregate
+except ImportError:
+    from ..yori_aggregate import aggregate
+
 from pkg_resources import get_distribution
 
 VERSION = get_distribution('yori').version
 
 
 def main():
     import argparse
@@ -62,7 +66,11 @@
               daily=args.daily,
               satellite=args.method,
               force=args.force,
               compression=args.compression,
               use_min_pixel_counts=args.min_pixel_counts,
               use_min_valid_days=args.min_valid_days,
               batch_size=args.batch_size)
+
+
+if __name__ == "__main__":
+    main()
```

## yori/tools/grid.py

```diff
@@ -1,8 +1,12 @@
-from ..run_yori import callYori
+try:
+    from yori.run_yori import callYori
+except ImportError:
+    from ..run_yori import callYori
+
 from pkg_resources import get_distribution
 # from setuptools_scm import get_version
 
 VERSION = get_distribution('yori').version
 
 
 def main():
@@ -22,7 +26,11 @@
 
     args = parser.parse_args()
 
     callYori(args.cfgfile,
              args.input,
              args.output,
              compression=args.compression)
+
+
+if __name__ == "__main__":
+    main()
```

## Comparing `yori-1.7.7.dist-info/METADATA` & `yori-1.7.8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: yori
-Version: 1.7.7
+Version: 1.7.8
 Summary: User-customizable set of tools to easily grid satellite data
 Project-URL: Homepage, https://gitlab.ssec.wisc.edu/pveglio/yori
 Project-URL: Documentation, https://sips.ssec.wisc.edu/docs/yori.html
 Project-URL: Changelog, https://gitlab.ssec.wisc.edu/pveglio/yori/-/blob/master/CHANGELOG.md
 Author-email: Paolo Veglio <paolo.veglio@ssec.wisc.edu>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: <3.12,>=3.8
 Requires-Dist: netcdf4
 Requires-Dist: numpy
```

## Comparing `yori-1.7.7.dist-info/licenses/LICENSE` & `yori-1.7.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `yori-1.7.7.dist-info/RECORD` & `yori-1.7.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 yori/IOtools.py,sha256=cgGHKfdloIM4O5RyvHntE8KYXzPWolqgIXlKCuN4eEI,6464
-yori/__init__.py,sha256=oz6WbPALTOKo9TBYJc2b4fL0yS8Ve8U31MYh0i3t420,22
+yori/__init__.py,sha256=3Cq_Tw1FdZarh3Ntzs6fWGvwyLilf-7jlfBYIVOyiyo,22
 yori/aggrtools.py,sha256=D1i60oCzO1umTAC-IZmDU4S-CSxiWQNPDmEaOUa9cq4,14015
 yori/config_reader.py,sha256=KM3OPxAbvsjxUNsbl_tDMW-Surp2bKt_J-wR3Ge8Vug,4670
 yori/gridtools.py,sha256=dBKJaCfHI5KlD_5rZrhJ9o8c3PivkPuo-EzBKOOmiYU,20221
 yori/run_yori.py,sha256=8QY5XzVmqKy0WQA2BfCgE15ynM4r1kiuvrDfSR38iv8,10158
 yori/yori_aggregate.py,sha256=Kkgi02-DMX0G_GfLbyazOw9VXDx6r40PHOIqD1RD52A,11502
 yori/yori_merge.py,sha256=QLe2V4N6vULqSEyW0R0XDDLQxf02nTBrNsMicJQBqrY,5807
 yori/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-yori/tools/aggr.py,sha256=onL3VpQlv_m8Lhr21M2ShnvsRzJ7c2gXy4Bs4E_3zeA,3424
-yori/tools/grid.py,sha256=1DJGluHNU0oeRy2mYxpBfYCGXZhiT-tf7OgBKdhaKJ0,1196
+yori/tools/aggr.py,sha256=d58Gd-qbTLyYrJgRjbOY8gcaGy6O0JhGw2jO7sZLuAw,3540
+yori/tools/grid.py,sha256=VbY_NSQnToIctDAB4ZxtDejbYgy7gx3NPW_uaQnNAsI,1305
 yori/tools/merge.py,sha256=CDSGN67OdrY3xAvyPyH6p2fMkmS7ssElv0eSA5sks00,2268
-yori-1.7.7.dist-info/METADATA,sha256=oaPuAn4gqjK8Mmu44P3IGFc5YlOqrbHyyJDHufaGbSU,1129
-yori-1.7.7.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-yori-1.7.7.dist-info/entry_points.txt,sha256=5hPsdZbRl0tMHWbUJV-FUkEVMr4C79BZUHDl6jqqtAQ,119
-yori-1.7.7.dist-info/licenses/LICENSE,sha256=ushvHBhEa4gm0SQ2DUAtI0N_ajIlmVfZHEl-VphTk5Y,1069
-yori-1.7.7.dist-info/RECORD,,
+yori-1.7.8.dist-info/METADATA,sha256=uQ7lFeoRJlVjaR5adYyt2iGrhcz-EdSfSRMAWcZYJhE,1179
+yori-1.7.8.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+yori-1.7.8.dist-info/entry_points.txt,sha256=5hPsdZbRl0tMHWbUJV-FUkEVMr4C79BZUHDl6jqqtAQ,119
+yori-1.7.8.dist-info/licenses/LICENSE,sha256=ushvHBhEa4gm0SQ2DUAtI0N_ajIlmVfZHEl-VphTk5Y,1069
+yori-1.7.8.dist-info/RECORD,,
```

