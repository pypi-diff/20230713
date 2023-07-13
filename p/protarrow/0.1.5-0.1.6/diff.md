# Comparing `tmp/protarrow-0.1.5.tar.gz` & `tmp/protarrow-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protarrow-0.1.5.tar", max compression
+gzip compressed data, was "protarrow-0.1.6.tar", max compression
```

## Comparing `protarrow-0.1.5.tar` & `protarrow-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10140 2023-05-09 16:12:07.359680 protarrow-0.1.5/LICENSE
--rw-r--r--   0        0        0     3022 2023-05-09 16:12:07.359680 protarrow-0.1.5/README.md
--rw-r--r--   0        0        0      754 2023-05-09 16:12:32.163744 protarrow-0.1.5/protarrow/__init__.py
--rw-r--r--   0        0        0    19405 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/arrow_to_proto.py
--rw-r--r--   0        0        0     7596 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/cast_to_proto.py
--rw-r--r--   0        0        0     1236 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/common.py
--rw-r--r--   0        0        0     4621 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/message_extractor.py
--rw-r--r--   0        0        0    18792 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/proto_to_arrow.py
--rw-r--r--   0        0        0     1858 2023-05-09 16:12:32.159743 protarrow-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4285 1970-01-01 00:00:00.000000 protarrow-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10140 2023-07-13 11:19:23.064791 protarrow-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3022 2023-07-13 11:19:23.064791 protarrow-0.1.6/README.md
+-rw-r--r--   0        0        0      754 2023-07-13 11:19:46.945755 protarrow-0.1.6/protarrow/__init__.py
+-rw-r--r--   0        0        0    19405 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/arrow_to_proto.py
+-rw-r--r--   0        0        0     7596 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/cast_to_proto.py
+-rw-r--r--   0        0        0     1236 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/common.py
+-rw-r--r--   0        0        0     4621 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/message_extractor.py
+-rw-r--r--   0        0        0    18960 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/proto_to_arrow.py
+-rw-r--r--   0        0        0     1859 2023-07-13 11:19:46.941755 protarrow-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.1.6/PKG-INFO
```

### Comparing `protarrow-0.1.5/LICENSE` & `protarrow-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.5/README.md` & `protarrow-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.5/protarrow/__init__.py` & `protarrow-0.1.6/protarrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from protarrow.proto_to_arrow import (
     message_type_to_schema,
     message_type_to_struct_type,
     messages_to_record_batch,
     messages_to_table,
 )
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 __all__ = [
     "MessageExtractor",
     "ProtarrowConfig",
     "cast_record_batch",
     "cast_struct_array",
     "cast_table",
     "message_type_to_schema",
```

### Comparing `protarrow-0.1.5/protarrow/arrow_to_proto.py` & `protarrow-0.1.6/protarrow/arrow_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.5/protarrow/cast_to_proto.py` & `protarrow-0.1.6/protarrow/cast_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.5/protarrow/common.py` & `protarrow-0.1.6/protarrow/common.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.5/protarrow/message_extractor.py` & `protarrow-0.1.6/protarrow/message_extractor.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.5/protarrow/proto_to_arrow.py` & `protarrow-0.1.6/protarrow/proto_to_arrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,26 +218,28 @@
         return lambda x: x
 
     elif is_binary_enum(data_type):
         values_by_number = {
             k: bytes(v.name, encoding="UTF-8")
             for k, v in enum_descriptor.values_by_number.items()
         }
+        fallback = values_by_number[enum_descriptor.values[0].number]
 
         def converter(x: int) -> bytes:
-            return values_by_number[x]
+            return values_by_number.get(x, fallback)
 
         return converter
     elif is_string_enum(data_type):
         values_by_number = {
             k: v.name for k, v in enum_descriptor.values_by_number.items()
         }
+        fallback = values_by_number[enum_descriptor.values[0].number]
 
         def converter(x: int) -> bytes:
-            return values_by_number[x]
+            return values_by_number.get(x, fallback)
 
         return converter
     else:
         raise TypeError(data_type)
 
 
 def field_descriptor_to_field(
```

### Comparing `protarrow-0.1.5/pyproject.toml` & `protarrow-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "protarrow"
-version = "0.1.5"
+version = "0.1.6"
 description = "Convert from protobuf to arrow and back"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "protarrow" }
 ]
 readme = "README.md"
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 keywords = ["apache-arrow", "protobuf", "data"]
 
 [tool.poetry.dependencies]
 googleapis-common-protos = ">=1.53.0"
 protobuf = ">=3.20.1"
-pyarrow = ">=8.0.0"
+pyarrow = ">=12.0.0"
 python = ">=3.8,<3.12"
 
 [tool.poetry.group.dev.dependencies]
 Jinja2 = ">=3.1.2"
 black = "^22.10.0"
 coverage = ">=6.5.0"
 flake8 = ">=5.0.4"
```

### Comparing `protarrow-0.1.5/PKG-INFO` & `protarrow-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protarrow
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convert from protobuf to arrow and back
 Home-page: https://github.com/tradewelltech/protarrow
 License: Apache-2.0
 Keywords: apache-arrow,protobuf,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
@@ -14,21 +14,17 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: googleapis-common-protos (>=1.53.0)
 Requires-Dist: protobuf (>=3.20.1)
-Requires-Dist: pyarrow (>=8.0.0)
+Requires-Dist: pyarrow (>=12.0.0)
 Project-URL: Documentation, https://protarrow.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/tradewelltech/protarrow
 Description-Content-Type: text/markdown
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Python Version][versions-image]][versions-url]
 [![Github Stars][stars-image]][stars-url]
```

