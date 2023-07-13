# Comparing `tmp/moore-itertools-0.0.2.tar.gz` & `tmp/moore-itertools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moore-itertools-0.0.2.tar", last modified: Fri Jul  7 06:11:12 2023, max compression
+gzip compressed data, was "moore-itertools-0.0.3.tar", last modified: Thu Jul 13 02:26:41 2023, max compression
```

## Comparing `moore-itertools-0.0.2.tar` & `moore-itertools-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1475 2023-07-06 01:22:24.000000 moore-itertools-0.0.2/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       33 2023-07-06 01:40:22.000000 moore-itertools-0.0.2/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)      612 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      164 2023-07-07 06:10:06.000000 moore-itertools-0.0.2/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/moore_itertools/
--rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-07-07 06:09:43.000000 moore-itertools-0.0.2/moore_itertools/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2693 2023-07-07 06:07:15.000000 moore-itertools-0.0.2/moore_itertools/product.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-07-06 01:40:26.000000 moore-itertools-0.0.2/moore_itertools/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/moore_itertools.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)      612 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      322 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      100 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       16 2023-07-07 06:11:12.000000 moore-itertools-0.0.2/moore_itertools.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     1344 2023-07-06 01:25:18.000000 moore-itertools-0.0.2/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-07-07 06:11:12.864566 moore-itertools-0.0.2/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-13 02:26:41.380549 moore-itertools-0.0.3/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1475 2023-07-06 01:22:24.000000 moore-itertools-0.0.3/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       33 2023-07-06 01:40:22.000000 moore-itertools-0.0.3/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)      612 2023-07-13 02:26:41.380549 moore-itertools-0.0.3/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      164 2023-07-07 06:10:06.000000 moore-itertools-0.0.3/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-13 02:26:41.380549 moore-itertools-0.0.3/moore_itertools/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-07-13 02:25:09.000000 moore-itertools-0.0.3/moore_itertools/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3005 2023-07-13 02:20:23.000000 moore-itertools-0.0.3/moore_itertools/product.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-07-06 01:40:26.000000 moore-itertools-0.0.3/moore_itertools/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-13 02:26:41.380549 moore-itertools-0.0.3/moore_itertools.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      612 2023-07-13 02:26:41.000000 moore-itertools-0.0.3/moore_itertools.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      322 2023-07-13 02:26:41.000000 moore-itertools-0.0.3/moore_itertools.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-07-13 02:26:41.000000 moore-itertools-0.0.3/moore_itertools.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      100 2023-07-13 02:26:41.000000 moore-itertools-0.0.3/moore_itertools.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       16 2023-07-13 02:26:41.000000 moore-itertools-0.0.3/moore_itertools.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1344 2023-07-06 01:25:18.000000 moore-itertools-0.0.3/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-07-13 02:26:41.380549 moore-itertools-0.0.3/setup.cfg
```

### Comparing `moore-itertools-0.0.2/LICENSE.txt` & `moore-itertools-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moore-itertools-0.0.2/PKG-INFO` & `moore-itertools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moore-itertools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Moore Itertools
 Author-email: Nick Moore <nick@zoic.org>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `moore-itertools-0.0.2/moore_itertools/product.py` & `moore-itertools-0.0.3/moore_itertools/product.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,28 +55,38 @@
         # gen1 and gen2 are producing new values, taking
         # it in turns and filling in missing values.
         try:
             val1 = next(gen1)
             yield from ((val1, val2) for val2 in mem2)
             mem1.append(val1)
         except StopIteration:
+            # gen1 is exhausted, so from here on in we just
+            # take values from gen2 and yield them with the
+            # mem1 values we took from gen1 already.
+
             # mem2 is no longer necessary so throw it away
             # to reduce memory usage.
             del mem2
 
-            # gen1 is exhausted, so from here on in we just
-            # take values from gen2 and yield them with the
-            # mem1 values we took from gen1 already.
-            for val2 in gen2:
-                yield from ((val1, val2) for val1 in mem1)
-            return
+            try:
+                while True:
+                    val2 = next(gen2)
+                    yield from ((val1, val2) for val1 in mem1)
+            except StopIteration:
+                return
 
         # same thing, opposite roles.
         try:
             val2 = next(gen2)
             yield from ((val1, val2) for val1 in mem1)
             mem2.append(val2)
         except StopIteration:
+            # gen2 is exhausted, throw away mem1 and take new
+            # values from gen1, combining them with mem2.
             del mem1
-            for val1 in gen1:
-                yield from ((val1, val2) for val2 in mem2)
-            return
+
+            try:
+                while True:
+                    val1 = next(gen1)
+                    yield from ((val1, val2) for val2 in mem2)
+            except StopIteration:
+                return
```

### Comparing `moore-itertools-0.0.2/moore_itertools.egg-info/PKG-INFO` & `moore-itertools-0.0.3/moore_itertools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moore-itertools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Moore Itertools
 Author-email: Nick Moore <nick@zoic.org>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `moore-itertools-0.0.2/pyproject.toml` & `moore-itertools-0.0.3/pyproject.toml`

 * *Files identical despite different names*

