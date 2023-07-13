# Comparing `tmp/types-jsonschema-4.7.0.tar.gz` & `tmp/types-jsonschema-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-jsonschema-4.7.0.tar", last modified: Fri Jul 15 09:18:34 2022, max compression
+gzip compressed data, was "types-jsonschema-4.9.0.tar", last modified: Fri Aug  5 12:38:37 2022, max compression
```

## Comparing `types-jsonschema-4.7.0.tar` & `types-jsonschema-4.9.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 09:18:34.561653 types-jsonschema-4.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-07-15 09:18:33.000000 types-jsonschema-4.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-15 09:18:33.000000 types-jsonschema-4.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-07-15 09:18:34.561653 types-jsonschema-4.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 09:18:34.557653 types-jsonschema-4.7.0/jsonschema-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-15 09:18:33.000000 types-jsonschema-4.7.0/jsonschema-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/_format.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/_legacy_validators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/_reflect.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/_types.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/_validators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/protocols.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-07-15 09:18:23.000000 types-jsonschema-4.7.0/jsonschema-stubs/validators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-15 09:18:34.561653 types-jsonschema-4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-15 09:18:33.000000 types-jsonschema-4.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 09:18:34.561653 types-jsonschema-4.7.0/types_jsonschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-07-15 09:18:34.000000 types-jsonschema-4.7.0/types_jsonschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-07-15 09:18:34.000000 types-jsonschema-4.7.0/types_jsonschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 09:18:34.000000 types-jsonschema-4.7.0/types_jsonschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-15 09:18:34.000000 types-jsonschema-4.7.0/types_jsonschema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 12:38:37.578902 types-jsonschema-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-08-05 12:38:37.000000 types-jsonschema-4.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-05 12:38:37.000000 types-jsonschema-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-08-05 12:38:37.578902 types-jsonschema-4.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 12:38:37.578902 types-jsonschema-4.9.0/jsonschema-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-05 12:38:37.000000 types-jsonschema-4.9.0/jsonschema-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/_legacy_validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/_validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/protocols.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-08-05 12:38:19.000000 types-jsonschema-4.9.0/jsonschema-stubs/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 12:38:37.578902 types-jsonschema-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-08-05 12:38:37.000000 types-jsonschema-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 12:38:37.578902 types-jsonschema-4.9.0/types_jsonschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-08-05 12:38:37.000000 types-jsonschema-4.9.0/types_jsonschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-08-05 12:38:37.000000 types-jsonschema-4.9.0/types_jsonschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 12:38:37.000000 types-jsonschema-4.9.0/types_jsonschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-05 12:38:37.000000 types-jsonschema-4.9.0/types_jsonschema.egg-info/top_level.txt
```

### Comparing `types-jsonschema-4.7.0/CHANGELOG.md` & `types-jsonschema-4.9.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## 4.9.0 (2022-08-05)
+
+[stubsabot] Bump jsonschema to 4.9.* (#8491)
+
+* [stubsabot] Bump jsonschema to 4.9.*
+
+* Remove jsonschema._reflect
+
+Co-authored-by: stubsabot <>
+Co-authored-by: Sebastian Rittau <srittau@rittau.biz>
+
 ## 4.7.0 (2022-07-15)
 
 [stubsabot] Bump jsonschema to 4.7.* (#8299)
 
 ## 4.6.0 (2022-06-26)
 
 Bump jsonschema to 4.6.* (#8161)
```

### Comparing `types-jsonschema-4.7.0/PKG-INFO` & `types-jsonschema-4.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-jsonschema
-Version: 4.7.0
+Version: 4.9.0
 Summary: Typing stubs for jsonschema
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/jsonschema.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `jsonschema` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `jsonschema`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/jsonschema. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `e90ee8e0d9d2a60975dff3c95d20643e133823b5`.
+This package was generated from typeshed commit `892796a7945cad5e9eeb91766694fb327eda5b7d`.
```

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/__init__.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/_format.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/_format.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/_legacy_validators.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/_legacy_validators.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/_types.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/_types.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/_utils.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/_utils.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/_validators.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/_validators.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/cli.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/cli.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/exceptions.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/protocols.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/protocols.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/jsonschema-stubs/validators.pyi` & `types-jsonschema-4.9.0/jsonschema-stubs/validators.pyi`

 * *Files identical despite different names*

### Comparing `types-jsonschema-4.7.0/setup.py` & `types-jsonschema-4.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 This is a PEP 561 type stub package for the `jsonschema` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `jsonschema`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/jsonschema. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `e90ee8e0d9d2a60975dff3c95d20643e133823b5`.
+This package was generated from typeshed commit `892796a7945cad5e9eeb91766694fb327eda5b7d`.
 '''.lstrip()
 
 setup(name=name,
-      version="4.7.0",
+      version="4.9.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/jsonschema.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['jsonschema-stubs'],
-      package_data={'jsonschema-stubs': ['__init__.pyi', '_format.pyi', '_legacy_validators.pyi', '_reflect.pyi', '_types.pyi', '_utils.pyi', '_validators.pyi', 'cli.pyi', 'exceptions.pyi', 'protocols.pyi', 'validators.pyi', 'METADATA.toml']},
+      package_data={'jsonschema-stubs': ['__init__.pyi', '_format.pyi', '_legacy_validators.pyi', '_types.pyi', '_utils.pyi', '_validators.pyi', 'cli.pyi', 'exceptions.pyi', 'protocols.pyi', 'validators.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-jsonschema-4.7.0/types_jsonschema.egg-info/PKG-INFO` & `types-jsonschema-4.9.0/types_jsonschema.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-jsonschema
-Version: 4.7.0
+Version: 4.9.0
 Summary: Typing stubs for jsonschema
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/jsonschema.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `jsonschema` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `jsonschema`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/jsonschema. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `e90ee8e0d9d2a60975dff3c95d20643e133823b5`.
+This package was generated from typeshed commit `892796a7945cad5e9eeb91766694fb327eda5b7d`.
```

### Comparing `types-jsonschema-4.7.0/types_jsonschema.egg-info/SOURCES.txt` & `types-jsonschema-4.9.0/types_jsonschema.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 CHANGELOG.md
 MANIFEST.in
 setup.py
 jsonschema-stubs/METADATA.toml
 jsonschema-stubs/__init__.pyi
 jsonschema-stubs/_format.pyi
 jsonschema-stubs/_legacy_validators.pyi
-jsonschema-stubs/_reflect.pyi
 jsonschema-stubs/_types.pyi
 jsonschema-stubs/_utils.pyi
 jsonschema-stubs/_validators.pyi
 jsonschema-stubs/cli.pyi
 jsonschema-stubs/exceptions.pyi
 jsonschema-stubs/protocols.pyi
 jsonschema-stubs/validators.pyi
```

