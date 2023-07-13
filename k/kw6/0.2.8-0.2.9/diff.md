# Comparing `tmp/kw6-0.2.8.tar.gz` & `tmp/kw6-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kw6-0.2.8.tar", max compression
+gzip compressed data, was "kw6-0.2.9.tar", max compression
```

## Comparing `kw6-0.2.8.tar` & `kw6-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    90835 2021-10-01 21:40:20.700974 kw6-0.2.8/LICENSE
--rw-r--r--   0        0        0      189 2021-10-01 21:40:20.700974 kw6-0.2.8/kw6/__init__.py
--rw-r--r--   0        0        0     2302 2021-10-01 21:40:20.700974 kw6-0.2.8/kw6/camera.py
--rw-r--r--   0        0        0      595 2021-10-01 21:40:20.700974 kw6-0.2.8/kw6/header.py
--rw-r--r--   0        0        0     1603 2021-10-01 21:40:20.700974 kw6-0.2.8/kw6/position.py
--rw-r--r--   0        0        0    11471 2021-10-01 21:40:20.700974 kw6-0.2.8/kw6/reader.py
--rw-r--r--   0        0        0       59 2021-10-01 21:40:20.700974 kw6-0.2.8/kw6/settings.py
--rw-r--r--   0        0        0       39 2021-10-01 21:40:20.700974 kw6-0.2.8/kw6/types.py
--rw-r--r--   0        0        0      476 2021-10-01 21:40:49.705168 kw6-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      667 2021-10-01 21:40:50.192566 kw6-0.2.8/setup.py
--rw-r--r--   0        0        0      501 2021-10-01 21:40:50.192811 kw6-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    90835 2021-10-02 00:56:32.657958 kw6-0.2.9/LICENSE
+-rw-r--r--   0        0        0      189 2021-10-02 00:56:32.657958 kw6-0.2.9/kw6/__init__.py
+-rw-r--r--   0        0        0     2302 2021-10-02 00:56:32.657958 kw6-0.2.9/kw6/camera.py
+-rw-r--r--   0        0        0      595 2021-10-02 00:56:32.657958 kw6-0.2.9/kw6/header.py
+-rw-r--r--   0        0        0     1630 2021-10-02 00:56:32.661958 kw6-0.2.9/kw6/position.py
+-rw-r--r--   0        0        0    11471 2021-10-02 00:56:32.661958 kw6-0.2.9/kw6/reader.py
+-rw-r--r--   0        0        0       59 2021-10-02 00:56:32.661958 kw6-0.2.9/kw6/settings.py
+-rw-r--r--   0        0        0       39 2021-10-02 00:56:32.661958 kw6-0.2.9/kw6/types.py
+-rw-r--r--   0        0        0      476 2021-10-02 00:57:02.414204 kw6-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      667 2021-10-02 00:57:02.920928 kw6-0.2.9/setup.py
+-rw-r--r--   0        0        0      501 2021-10-02 00:57:02.921181 kw6-0.2.9/PKG-INFO
```

### Comparing `kw6-0.2.8/LICENSE` & `kw6-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kw6-0.2.8/kw6/camera.py` & `kw6-0.2.9/kw6/camera.py`

 * *Files identical despite different names*

### Comparing `kw6-0.2.8/kw6/header.py` & `kw6-0.2.9/kw6/header.py`

 * *Files identical despite different names*

### Comparing `kw6-0.2.8/kw6/position.py` & `kw6-0.2.9/kw6/position.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,27 @@
 
     class Config:
         allow_mutation = False
 
     @staticmethod
     def peek_from_stream(stream):
         byte_size = PositionHeader.byte_size()
-        return PositionHeader(**dict(zip(
-            PositionHeader.__fields__.keys(),
-            array.array("d", stream.peek(byte_size)[:byte_size]),
-        )))
+        return PositionHeader.from_bytes(stream.peek(byte_size)[:byte_size])
 
     @staticmethod
     def from_stream_(stream):
+        return PositionHeader.from_bytes(
+            stream.read(PositionHeader.byte_size())
+        )
+
+    @staticmethod
+    def from_bytes(bytes):
         return PositionHeader(**dict(zip(
             PositionHeader.__fields__.keys(),
-            array.array("d", stream.read(PositionHeader.byte_size()))
+            array.array("d", bytes)
         )))
 
     @staticmethod
     def byte_size():
         names = PositionHeader.__fields__.keys()
         return settings.N_BYTES_DOUBLE * len(names)
```

### Comparing `kw6-0.2.8/kw6/reader.py` & `kw6-0.2.9/kw6/reader.py`

 * *Files identical despite different names*

### Comparing `kw6-0.2.8/setup.py` & `kw6-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=8.3.1,<9.0.0', 'numpy>=1.21.2,<2.0.0', 'pydantic>=1.8.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'kw6',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Minimalistic library for reading files in the kw6 file format',
     'long_description': None,
     'author': 'Aiwizo AB',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

