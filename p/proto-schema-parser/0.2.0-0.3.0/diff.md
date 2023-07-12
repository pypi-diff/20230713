# Comparing `tmp/proto_schema_parser-0.2.0.tar.gz` & `tmp/proto_schema_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proto_schema_parser-0.2.0.tar", last modified: Wed Jun 21 16:07:59 2023, max compression
+gzip compressed data, was "proto_schema_parser-0.3.0.tar", last modified: Wed Jul 12 22:37:02 2023, max compression
```

## Comparing `proto_schema_parser-0.2.0.tar` & `proto_schema_parser-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1072 2023-06-19 20:44:40.014912 proto_schema_parser-0.2.0/LICENSE
--rw-r--r--   0        0        0     2405 2023-06-21 16:07:40.720467 proto_schema_parser-0.2.0/README.md
--rw-r--r--   0        0        0      157 2023-06-21 15:58:39.952033 proto_schema_parser-0.2.0/proto_schema_parser/__init__.py
--rw-r--r--   0        0        0    22913 2023-06-21 15:58:03.887400 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.interp
--rw-r--r--   0        0        0    22385 2023-06-21 15:58:03.887777 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.py
--rw-r--r--   0        0        0     1285 2023-06-21 15:58:03.888019 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.tokens
--rw-r--r--   0        0        0    29665 2023-06-21 15:58:03.888363 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.interp
--rw-r--r--   0        0        0   268632 2023-06-21 15:58:03.889387 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.py
--rw-r--r--   0        0        0     1285 2023-06-21 15:58:03.889520 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.tokens
--rw-r--r--   0        0        0    30623 2023-06-21 15:58:03.889721 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParserListener.py
--rw-r--r--   0        0        0    18134 2023-06-21 15:58:03.889910 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParserVisitor.py
--rw-r--r--   0        0        0        0 2023-06-21 15:58:03.889952 proto_schema_parser-0.2.0/proto_schema_parser/antlr/__init__.py
--rw-r--r--   0        0        0     4469 2023-06-21 16:07:40.720880 proto_schema_parser-0.2.0/proto_schema_parser/ast.py
--rw-r--r--   0        0        0     8977 2023-06-21 16:07:40.721184 proto_schema_parser-0.2.0/proto_schema_parser/parser.py
--rw-r--r--   0        0        0     1237 2023-06-21 16:07:59.283537 proto_schema_parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    20338 2023-06-21 16:07:40.721458 proto_schema_parser-0.2.0/tests/test_parser.py
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 proto_schema_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-21 16:26:36.335196 proto_schema_parser-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2900 2023-07-12 22:36:53.969176 proto_schema_parser-0.3.0/README.md
+-rw-r--r--   0        0        0      157 2023-06-21 16:26:36.349553 proto_schema_parser-0.3.0/proto_schema_parser/__init__.py
+-rw-r--r--   0        0        0    22913 2023-06-21 16:26:36.349777 proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufLexer.interp
+-rw-r--r--   0        0        0    22385 2023-06-21 16:26:36.350000 proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufLexer.py
+-rw-r--r--   0        0        0     1285 2023-06-21 16:26:36.350099 proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufLexer.tokens
+-rw-r--r--   0        0        0    29665 2023-06-21 16:26:36.350277 proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParser.interp
+-rw-r--r--   0        0        0   268632 2023-06-21 16:26:36.350935 proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParser.py
+-rw-r--r--   0        0        0     1285 2023-06-21 16:26:36.351032 proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParser.tokens
+-rw-r--r--   0        0        0    30623 2023-06-21 16:26:36.351215 proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParserListener.py
+-rw-r--r--   0        0        0    18134 2023-06-21 16:26:36.351314 proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParserVisitor.py
+-rw-r--r--   0        0        0        0 2023-06-21 16:26:36.351356 proto_schema_parser-0.3.0/proto_schema_parser/antlr/__init__.py
+-rw-r--r--   0        0        0     4469 2023-06-21 16:26:36.351474 proto_schema_parser-0.3.0/proto_schema_parser/ast.py
+-rw-r--r--   0        0        0     6897 2023-07-12 22:36:53.969562 proto_schema_parser-0.3.0/proto_schema_parser/generator.py
+-rw-r--r--   0        0        0     8977 2023-06-21 16:26:36.351581 proto_schema_parser-0.3.0/proto_schema_parser/parser.py
+-rw-r--r--   0        0        0     1393 2023-07-12 22:37:02.154849 proto_schema_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8838 2023-07-12 22:36:53.969960 proto_schema_parser-0.3.0/tests/test_generator.py
+-rw-r--r--   0        0        0    20338 2023-06-21 16:26:36.351833 proto_schema_parser-0.3.0/tests/test_parser.py
+-rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 proto_schema_parser-0.3.0/PKG-INFO
```

### Comparing `proto_schema_parser-0.2.0/LICENSE` & `proto_schema_parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/README.md` & `proto_schema_parser-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Protobuf Schema Parser
 
-Protobuf Schema Parser is a pure-Python library that parses Protobuf schemas into an abstract syntax tree (AST).
+Protobuf Schema Parser is a pure-Python library that parses and writes Protobuf schemas to and from an abstract syntax tree (AST).
 
-The lexer and parser are autogenerated from [Buf](https://buf.build/)'s ANTLR [lexer and parser](https://github.com/bufbuild/protobuf.com/tree/main/examples/antlr) grammar files. The library then `proto_schema_parser.parser.Parser` to parse the [CST into an AST](https://stackoverflow.com/questions/29971097/how-to-create-ast-with-antlr4).
+The library uses `proto_schema_parser.parser.Parser` to parse the [CST into an AST](https://stackoverflow.com/questions/29971097/how-to-create-ast-with-antlr4). The `proto_schema_parser.generator.Generator` class converts the AST back into a CST (a Protobuf schema string).
+
+_The lexer and parser are autogenerated from [Buf](https://buf.build/)'s ANTLR [lexer and parser](https://github.com/bufbuild/protobuf.com/tree/main/examples/antlr) grammar files._
 
 ## Features
 
 - ✅ proto2 and proto3 support
 - ✅ message, field, enum, optional, required, repeated
 - ✅ import, package, oneof, map, and option
 - ✅ group and extend (in proto2)
@@ -58,14 +60,33 @@
                                       Field(name='result_per_page',
                                             number=3,
                                             type='int32',
                                             cardinality=None,
                                             options=[])])])
 ```
 
+To write the AST back to a protobuf schema, create a `Generator` object and call the `generate` method:
+
+```python
+from proto_schema_parser.generator import Generator
+
+proto = Generator().generate(result)
+```
+
+This will print:
+
+```proto
+syntax = "proto3";
+message SearchRequest {
+  string query = 1;
+  int32 page_number = 2;
+  int32 result_per_page = 3;
+}
+```
+
 ## Contributing
 
 I welcome contributions!
 
 - Submit a PR and I'll review it as soon as I can.
 - Open an issue if you find a bug or have a feature request.
```

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.interp` & `proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufLexer.interp`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.py` & `proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufLexer.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.tokens` & `proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufLexer.tokens`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.interp` & `proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParser.interp`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.py` & `proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParser.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.tokens` & `proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParser.tokens`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParserListener.py` & `proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParserListener.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParserVisitor.py` & `proto_schema_parser-0.3.0/proto_schema_parser/antlr/ProtobufParserVisitor.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/ast.py` & `proto_schema_parser-0.3.0/proto_schema_parser/ast.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/proto_schema_parser/parser.py` & `proto_schema_parser-0.3.0/proto_schema_parser/parser.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/pyproject.toml` & `proto_schema_parser-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "proto-schema-parser"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Pure Python Protobuf 3 .proto Parser"
 authors = [
     { name = "Chris Riccomini", email = "criccomini@apache.org" },
 ]
 dependencies = [
     "antlr4-python3-runtime>=4.13.0",
 ]
@@ -29,14 +29,22 @@
     "isort>=5.12.0",
     "pylint>=2.17.4",
     "pyright>=1.1.314",
 ]
 
 [tool.pdm.scripts]
 antlr = "java -Xmx500M -cp antlr/antlr-4.13.0-complete.jar org.antlr.v4.Tool -Dlanguage=Python3 -visitor -o proto_schema_parser -lib proto_schema_parser/antlr antlr/ProtobufLexer.g4 antlr/ProtobufParser.g4"
+black = "black proto_schema_parser/ tests/"
+isort = "isort proto_schema_parser/ tests/"
+
+[tool.pdm.scripts.style]
+composite = [
+    "black",
+    "isort",
+]
 
 [tool.black]
 exclude = "proto_schema_parser/antlr/"
 
 [tool.isort]
 profile = "black"
 case_sensitive = true
```

### Comparing `proto_schema_parser-0.2.0/tests/test_parser.py` & `proto_schema_parser-0.3.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.2.0/PKG-INFO` & `proto_schema_parser-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: proto-schema-parser
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Pure Python Protobuf 3 .proto Parser
 Author-Email: Chris Riccomini <criccomini@apache.org>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: antlr4-python3-runtime>=4.13.0
 Description-Content-Type: text/markdown
 
 # Protobuf Schema Parser
 
-Protobuf Schema Parser is a pure-Python library that parses Protobuf schemas into an abstract syntax tree (AST).
+Protobuf Schema Parser is a pure-Python library that parses and writes Protobuf schemas to and from an abstract syntax tree (AST).
 
-The lexer and parser are autogenerated from [Buf](https://buf.build/)'s ANTLR [lexer and parser](https://github.com/bufbuild/protobuf.com/tree/main/examples/antlr) grammar files. The library then `proto_schema_parser.parser.Parser` to parse the [CST into an AST](https://stackoverflow.com/questions/29971097/how-to-create-ast-with-antlr4).
+The library uses `proto_schema_parser.parser.Parser` to parse the [CST into an AST](https://stackoverflow.com/questions/29971097/how-to-create-ast-with-antlr4). The `proto_schema_parser.generator.Generator` class converts the AST back into a CST (a Protobuf schema string).
+
+_The lexer and parser are autogenerated from [Buf](https://buf.build/)'s ANTLR [lexer and parser](https://github.com/bufbuild/protobuf.com/tree/main/examples/antlr) grammar files._
 
 ## Features
 
 - ✅ proto2 and proto3 support
 - ✅ message, field, enum, optional, required, repeated
 - ✅ import, package, oneof, map, and option
 - ✅ group and extend (in proto2)
@@ -68,14 +70,33 @@
                                       Field(name='result_per_page',
                                             number=3,
                                             type='int32',
                                             cardinality=None,
                                             options=[])])])
 ```
 
+To write the AST back to a protobuf schema, create a `Generator` object and call the `generate` method:
+
+```python
+from proto_schema_parser.generator import Generator
+
+proto = Generator().generate(result)
+```
+
+This will print:
+
+```proto
+syntax = "proto3";
+message SearchRequest {
+  string query = 1;
+  int32 page_number = 2;
+  int32 result_per_page = 3;
+}
+```
+
 ## Contributing
 
 I welcome contributions!
 
 - Submit a PR and I'll review it as soon as I can.
 - Open an issue if you find a bug or have a feature request.
```

