# Comparing `tmp/py_go_goose-1.2.tar.gz` & `tmp/py_go_goose-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_go_goose-1.2.tar", last modified: Thu Jul 13 14:44:04 2023, max compression
+gzip compressed data, was "py_go_goose-1.3.tar", last modified: Thu Jul 13 16:27:10 2023, max compression
```

## Comparing `py_go_goose-1.2.tar` & `py_go_goose-1.3.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 14:44:04.460054 py_go_goose-1.2/
--rw-r--r--   0 dongmengnan   (501) staff       (20)    11325 2023-07-12 13:06:02.000000 py_go_goose-1.2/LICENSE
--rw-r--r--   0 dongmengnan   (501) staff       (20)       25 2023-07-13 14:43:26.000000 py_go_goose-1.2/MANIFEST.in
--rw-r--r--   0 dongmengnan   (501) staff       (20)       96 2023-07-13 14:44:04.459916 py_go_goose-1.2/PKG-INFO
--rw-r--r--   0 dongmengnan   (501) staff       (20)     2663 2023-07-12 13:06:02.000000 py_go_goose-1.2/README.md
-drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 14:44:04.457709 py_go_goose-1.2/go_goose/
--rw-r--r--   0 dongmengnan   (501) staff       (20)      337 2023-07-13 12:04:14.000000 py_go_goose-1.2/go_goose/go_goose.go
-drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 14:44:04.459062 py_go_goose-1.2/py_go_goose/
--rw-r--r--   0 dongmengnan   (501) staff       (20)        0 2023-07-13 14:43:43.000000 py_go_goose-1.2/py_go_goose/__init__.py
--rw-r--r--   0 dongmengnan   (501) staff       (20)    12554 2023-07-13 14:43:43.000000 py_go_goose-1.2/py_go_goose/build.py
--rw-r--r--   0 dongmengnan   (501) staff       (20)    48182 2023-07-13 14:43:43.000000 py_go_goose-1.2/py_go_goose/go.py
--rw-r--r--   0 dongmengnan   (501) staff       (20)     3110 2023-07-13 14:43:43.000000 py_go_goose-1.2/py_go_goose/go_goose.py
-drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 14:44:04.459739 py_go_goose-1.2/py_go_goose.egg-info/
--rw-r--r--   0 dongmengnan   (501) staff       (20)       96 2023-07-13 14:44:04.000000 py_go_goose-1.2/py_go_goose.egg-info/PKG-INFO
--rw-r--r--   0 dongmengnan   (501) staff       (20)      286 2023-07-13 14:44:04.000000 py_go_goose-1.2/py_go_goose.egg-info/SOURCES.txt
--rw-r--r--   0 dongmengnan   (501) staff       (20)        1 2023-07-13 14:44:04.000000 py_go_goose-1.2/py_go_goose.egg-info/dependency_links.txt
--rw-r--r--   0 dongmengnan   (501) staff       (20)       12 2023-07-13 14:44:04.000000 py_go_goose-1.2/py_go_goose.egg-info/top_level.txt
--rw-r--r--   0 dongmengnan   (501) staff       (20)       38 2023-07-13 14:44:04.460100 py_go_goose-1.2/setup.cfg
--rw-r--r--   0 dongmengnan   (501) staff       (20)      497 2023-07-13 14:41:54.000000 py_go_goose-1.2/setup.py
+drwxr-xr-x   0 guangnian  (1001) supergroup  (1001)        0 2023-07-13 16:27:10.028894 py_go_goose-1.3/
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)    11325 2023-07-13 14:45:24.000000 py_go_goose-1.3/LICENSE
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)       60 2023-07-13 16:22:53.000000 py_go_goose-1.3/MANIFEST.in
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)      292 2023-07-13 16:27:10.028894 py_go_goose-1.3/PKG-INFO
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)     2663 2023-07-13 14:45:24.000000 py_go_goose-1.3/README.md
+drwxr-xr-x   0 guangnian  (1001) supergroup  (1001)        0 2023-07-13 16:27:10.021894 py_go_goose-1.3/go_goose/
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)      337 2023-07-13 14:45:24.000000 py_go_goose-1.3/go_goose/go_goose.go
+drwxr-xr-x   0 guangnian  (1001) supergroup  (1001)        0 2023-07-13 16:27:10.027894 py_go_goose-1.3/py_go_goose/
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)     1464 2023-07-13 16:05:38.000000 py_go_goose-1.3/py_go_goose/Makefile
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)        0 2023-07-13 16:05:38.000000 py_go_goose-1.3/py_go_goose/__init__.py
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)    10934 2023-07-13 16:05:43.000000 py_go_goose-1.3/py_go_goose/_go_goose.cpython-38-x86_64-linux-gnu.h
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)  9357152 2023-07-13 16:05:43.000000 py_go_goose-1.3/py_go_goose/_go_goose.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)    12554 2023-07-13 16:05:38.000000 py_go_goose-1.3/py_go_goose/build.py
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)    48182 2023-07-13 16:05:38.000000 py_go_goose-1.3/py_go_goose/go.py
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)    87230 2023-07-13 16:05:41.000000 py_go_goose-1.3/py_go_goose/go_goose.c
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)    29845 2023-07-13 16:05:38.000000 py_go_goose-1.3/py_go_goose/go_goose.go
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)     3110 2023-07-13 16:05:38.000000 py_go_goose-1.3/py_go_goose/go_goose.py
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)    10934 2023-07-13 16:05:41.000000 py_go_goose-1.3/py_go_goose/go_goose_go.h
+drwxr-xr-x   0 guangnian  (1001) supergroup  (1001)        0 2023-07-13 16:27:10.027894 py_go_goose-1.3/py_go_goose.egg-info/
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)      292 2023-07-13 16:27:10.000000 py_go_goose-1.3/py_go_goose.egg-info/PKG-INFO
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)      485 2023-07-13 16:27:10.000000 py_go_goose-1.3/py_go_goose.egg-info/SOURCES.txt
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)        1 2023-07-13 16:27:10.000000 py_go_goose-1.3/py_go_goose.egg-info/dependency_links.txt
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)       12 2023-07-13 16:27:10.000000 py_go_goose-1.3/py_go_goose.egg-info/top_level.txt
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)       38 2023-07-13 16:27:10.028894 py_go_goose-1.3/setup.cfg
+-rw-r--r--   0 guangnian  (1001) supergroup  (1001)      400 2023-07-13 16:25:48.000000 py_go_goose-1.3/setup.py
```

### Comparing `py_go_goose-1.2/LICENSE` & `py_go_goose-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_go_goose-1.2/README.md` & `py_go_goose-1.3/README.md`

 * *Files identical despite different names*

### Comparing `py_go_goose-1.2/py_go_goose/build.py` & `py_go_goose-1.3/py_go_goose/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,18 +73,18 @@
 mod.add_function('Slice_float64_len', retval('int'), [param('int64_t', 'handle')])
 mod.add_function('Slice_float64_elem', retval('double'), [param('int64_t', 'handle'), param('int', 'idx')])
 mod.add_function('Slice_float64_subslice', retval('int64_t'), [param('int64_t', 'handle'), param('int', 'st'), param('int', 'ed')])
 mod.add_function('Slice_float64_set', None, [param('int64_t', 'handle'), param('int', 'idx'), param('double', 'value')])
 mod.add_function('Slice_float64_append', None, [param('int64_t', 'handle'), param('double', 'value')])
 mod.add_function('Slice_int_CTor', retval('int64_t'), [])
 mod.add_function('Slice_int_len', retval('int'), [param('int64_t', 'handle')])
-mod.add_function('Slice_int_elem', retval('int64_t'), [param('int64_t', 'handle'), param('int', 'idx')])
+mod.add_function('Slice_int_elem', retval('int'), [param('int64_t', 'handle'), param('int', 'idx')])
 mod.add_function('Slice_int_subslice', retval('int64_t'), [param('int64_t', 'handle'), param('int', 'st'), param('int', 'ed')])
-mod.add_function('Slice_int_set', None, [param('int64_t', 'handle'), param('int', 'idx'), param('int64_t', 'value')])
-mod.add_function('Slice_int_append', None, [param('int64_t', 'handle'), param('int64_t', 'value')])
+mod.add_function('Slice_int_set', None, [param('int64_t', 'handle'), param('int', 'idx'), param('int', 'value')])
+mod.add_function('Slice_int_append', None, [param('int64_t', 'handle'), param('int', 'value')])
 mod.add_function('Slice_int16_CTor', retval('int64_t'), [])
 mod.add_function('Slice_int16_len', retval('int'), [param('int64_t', 'handle')])
 mod.add_function('Slice_int16_elem', retval('int16_t'), [param('int64_t', 'handle'), param('int', 'idx')])
 mod.add_function('Slice_int16_subslice', retval('int64_t'), [param('int64_t', 'handle'), param('int', 'st'), param('int', 'ed')])
 mod.add_function('Slice_int16_set', None, [param('int64_t', 'handle'), param('int', 'idx'), param('int16_t', 'value')])
 mod.add_function('Slice_int16_append', None, [param('int64_t', 'handle'), param('int16_t', 'value')])
 mod.add_function('Slice_int32_CTor', retval('int64_t'), [])
@@ -115,18 +115,18 @@
 mod.add_function('Slice_string_len', retval('int'), [param('int64_t', 'handle')])
 mod.add_function('Slice_string_elem', retval('char*'), [param('int64_t', 'handle'), param('int', 'idx')])
 mod.add_function('Slice_string_subslice', retval('int64_t'), [param('int64_t', 'handle'), param('int', 'st'), param('int', 'ed')])
 mod.add_function('Slice_string_set', None, [param('int64_t', 'handle'), param('int', 'idx'), param('char*', 'value')])
 mod.add_function('Slice_string_append', None, [param('int64_t', 'handle'), param('char*', 'value')])
 mod.add_function('Slice_uint_CTor', retval('int64_t'), [])
 mod.add_function('Slice_uint_len', retval('int'), [param('int64_t', 'handle')])
-mod.add_function('Slice_uint_elem', retval('uint64_t'), [param('int64_t', 'handle'), param('int', 'idx')])
+mod.add_function('Slice_uint_elem', retval('unsigned int'), [param('int64_t', 'handle'), param('int', 'idx')])
 mod.add_function('Slice_uint_subslice', retval('int64_t'), [param('int64_t', 'handle'), param('int', 'st'), param('int', 'ed')])
-mod.add_function('Slice_uint_set', None, [param('int64_t', 'handle'), param('int', 'idx'), param('uint64_t', 'value')])
-mod.add_function('Slice_uint_append', None, [param('int64_t', 'handle'), param('uint64_t', 'value')])
+mod.add_function('Slice_uint_set', None, [param('int64_t', 'handle'), param('int', 'idx'), param('unsigned int', 'value')])
+mod.add_function('Slice_uint_append', None, [param('int64_t', 'handle'), param('unsigned int', 'value')])
 mod.add_function('Slice_uint16_CTor', retval('int64_t'), [])
 mod.add_function('Slice_uint16_len', retval('int'), [param('int64_t', 'handle')])
 mod.add_function('Slice_uint16_elem', retval('uint16_t'), [param('int64_t', 'handle'), param('int', 'idx')])
 mod.add_function('Slice_uint16_subslice', retval('int64_t'), [param('int64_t', 'handle'), param('int', 'st'), param('int', 'ed')])
 mod.add_function('Slice_uint16_set', None, [param('int64_t', 'handle'), param('int', 'idx'), param('uint16_t', 'value')])
 mod.add_function('Slice_uint16_append', None, [param('int64_t', 'handle'), param('uint16_t', 'value')])
 mod.add_function('Slice_uint32_CTor', retval('int64_t'), [])
```

### Comparing `py_go_goose-1.2/py_go_goose/go.py` & `py_go_goose-1.3/py_go_goose/go.py`

 * *Files identical despite different names*

### Comparing `py_go_goose-1.2/py_go_goose/go_goose.py` & `py_go_goose-1.3/py_go_goose/go_goose.py`

 * *Files identical despite different names*

