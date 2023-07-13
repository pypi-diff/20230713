# Comparing `tmp/types_awscrt-0.16.3.tar.gz` & `tmp/types_awscrt-0.16.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_awscrt-0.16.3.tar", max compression
+gzip compressed data, was "types_awscrt-0.16.4.tar", max compression
```

## Comparing `types_awscrt-0.16.3.tar` & `types_awscrt-0.16.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/LICENSE
--rw-r--r--   0        0        0     1423 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/README.md
--rw-r--r--   0        0        0      289 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/__init__.pyi
--rw-r--r--   0        0        0      438 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/_test.pyi
--rw-r--r--   0        0        0     4673 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/auth.pyi
--rw-r--r--   0        0        0      128 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/checksums.pyi
--rw-r--r--   0        0        0       94 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/common.pyi
--rw-r--r--   0        0        0      594 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/crypto.pyi
--rw-r--r--   0        0        0     1707 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/eventstream/__init__.pyi
--rw-r--r--   0        0        0     3714 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/eventstream/rpc.pyi
--rw-r--r--   0        0        0      234 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/exceptions.pyi
--rw-r--r--   0        0        0     4713 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/http.pyi
--rw-r--r--   0        0        0     4721 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/io.pyi
--rw-r--r--   0        0        0     4090 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/mqtt.pyi
--rw-r--r--   0        0        0    11852 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/mqtt5.pyi
--rw-r--r--   0        0        0        0 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/py.typed
--rw-r--r--   0        0        0     3531 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/s3.pyi
--rw-r--r--   0        0        0     3414 2022-12-27 01:19:47.164513 types_awscrt-0.16.3/awscrt-stubs/websocket.pyi
--rw-r--r--   0        0        0     2411 2022-12-27 01:20:23.532106 types_awscrt-0.16.3/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 types_awscrt-0.16.3/setup.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 types_awscrt-0.16.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/LICENSE
+-rw-r--r--   0        0        0     1423 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/README.md
+-rw-r--r--   0        0        0      289 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/__init__.pyi
+-rw-r--r--   0        0        0      438 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/_test.pyi
+-rw-r--r--   0        0        0     4673 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/auth.pyi
+-rw-r--r--   0        0        0      128 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/checksums.pyi
+-rw-r--r--   0        0        0       94 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/common.pyi
+-rw-r--r--   0        0        0      594 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/crypto.pyi
+-rw-r--r--   0        0        0     1707 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/eventstream/__init__.pyi
+-rw-r--r--   0        0        0     3714 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/eventstream/rpc.pyi
+-rw-r--r--   0        0        0      234 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     4713 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/http.pyi
+-rw-r--r--   0        0        0     4721 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/io.pyi
+-rw-r--r--   0        0        0     4090 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/mqtt.pyi
+-rw-r--r--   0        0        0    11852 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/mqtt5.pyi
+-rw-r--r--   0        0        0        0 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/py.typed
+-rw-r--r--   0        0        0     3531 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/s3.pyi
+-rw-r--r--   0        0        0     3414 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/websocket.pyi
+-rw-r--r--   0        0        0     2411 2023-01-14 01:20:04.250548 types_awscrt-0.16.4/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 types_awscrt-0.16.4/setup.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 types_awscrt-0.16.4/PKG-INFO
```

### Comparing `types_awscrt-0.16.3/LICENSE` & `types_awscrt-0.16.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/README.md` & `types_awscrt-0.16.4/README.md`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/auth.pyi` & `types_awscrt-0.16.4/awscrt-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/crypto.pyi` & `types_awscrt-0.16.4/awscrt-stubs/crypto.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/eventstream/__init__.pyi` & `types_awscrt-0.16.4/awscrt-stubs/eventstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/eventstream/rpc.pyi` & `types_awscrt-0.16.4/awscrt-stubs/eventstream/rpc.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/http.pyi` & `types_awscrt-0.16.4/awscrt-stubs/http.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/io.pyi` & `types_awscrt-0.16.4/awscrt-stubs/io.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/mqtt.pyi` & `types_awscrt-0.16.4/awscrt-stubs/mqtt.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/mqtt5.pyi` & `types_awscrt-0.16.4/awscrt-stubs/mqtt5.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/s3.pyi` & `types_awscrt-0.16.4/awscrt-stubs/s3.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/awscrt-stubs/websocket.pyi` & `types_awscrt-0.16.4/awscrt-stubs/websocket.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.3/pyproject.toml` & `types_awscrt-0.16.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.isort]
 profile = "black"
 line_length = 100
 src_paths = []
 
 [tool.poetry]
 name = "types-awscrt"
-version = "0.16.3"
+version = "0.16.4"
 description = "Type annotations and code completion for awscrt"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/types-awscrt"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
```

### Comparing `types_awscrt-0.16.3/setup.py` & `types_awscrt-0.16.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['awscrt-stubs']
 
 package_data = \
 {'': ['*'], 'awscrt-stubs': ['eventstream/*']}
 
 setup_kwargs = {
     'name': 'types-awscrt',
-    'version': '0.16.3',
+    'version': '0.16.4',
     'description': 'Type annotations and code completion for awscrt',
     'long_description': '# types-awscrt\n\n[![PyPI - types-awscrt](https://img.shields.io/pypi/v/types-awscrt.svg?color=blue&label=types-awscrt)](https://pypi.org/project/types-awscrt)\n[![PyPI - awscrt](https://img.shields.io/pypi/v/awscrt.svg?color=blue&label=awscrt)](https://pypi.org/project/awscrt)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-awscrt.svg?color=blue)](https://pypi.org/project/types-awscrt)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-awscrt?color=blue)](https://pypistats.org/packages/types-awscrt)\n\n![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)\n\nType annotations and code completion for [awscrt](https://pypi.org/project/awscrt/) package.\nThis package is a part of [mypy_boto3_builder](https://github.com/youtype/mypy_boto3_builder) project.\n\n## Installation\n\n```bash\npython -m pip install types-awscrt\n```\n\n## Usage\n\nUse [mypy](https://github.com/python/mypy) or [pyright](https://github.com/microsoft/pyright) for type checking.\n\n### Latest changes\n\nFull changelog can be found in [Releases](https://github.com/youtype/types-awscrt/releases).\n\n## Versioning\n\n`types-awscrt` version is the same as related `awscrt` version and follows\n[PEP 440](https://www.python.org/dev/peps/pep-0440/) format.\n\n## Support and contributing\n\nPlease reports any bugs or request new features in\n[types-awscrt](https://github.com/youtype/types-awscrt/issues/) repository.\n',
     'author': 'Vlad Emelianov',
     'author_email': 'vlad.emelianov.nz@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://youtype.github.io/mypy_boto3_builder/',
```

### Comparing `types_awscrt-0.16.3/PKG-INFO` & `types_awscrt-0.16.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-awscrt
-Version: 0.16.3
+Version: 0.16.4
 Summary: Type annotations and code completion for awscrt
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: awscrt,type-annotations,pyright,mypy,boto3
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.7,<4.0
```

