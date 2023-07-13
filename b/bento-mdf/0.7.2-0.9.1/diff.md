# Comparing `tmp/bento_mdf-0.7.2.tar.gz` & `tmp/bento_mdf-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_mdf-0.7.2.tar", max compression
+gzip compressed data, was "bento_mdf-0.9.1.tar", max compression
```

## Comparing `bento_mdf-0.7.2.tar` & `bento_mdf-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     4774 2023-02-13 22:09:03.146259 bento_mdf-0.7.2/README.md
--rwxr-xr-x   0        0        0     2936 2023-05-23 17:21:20.349476 bento_mdf-0.7.2/bin/load-mdf.py
--rwxr-xr-x   0        0        0     1918 2023-02-13 22:09:03.147706 bento_mdf-0.7.2/bin/test-mdf.py
--rw-r--r--   0        0        0     1848 2023-05-23 21:47:12.034021 bento_mdf-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       48 2023-02-13 22:09:03.157582 bento_mdf-0.7.2/src/bento_mdf/__init__.py
--rw-r--r--   0        0        0     9129 2023-02-13 22:09:03.158593 bento_mdf-0.7.2/src/bento_mdf/diff.py
--rw-r--r--   0        0        0    29005 2023-05-23 21:45:45.813530 bento_mdf-0.7.2/src/bento_mdf/mdf.py
--rw-r--r--   0        0        0     8110 2023-02-13 22:09:03.160193 bento_mdf-0.7.2/src/bento_mdf/validator.py
--rw-r--r--   0        0        0     5899 1970-01-01 00:00:00.000000 bento_mdf-0.7.2/setup.py
--rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 bento_mdf-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     4691 2023-07-13 20:51:45.079756 bento_mdf-0.9.1/README.md
+-rwxr-xr-x   0        0        0     2936 2023-07-13 20:51:45.079756 bento_mdf-0.9.1/bin/load-mdf.py
+-rwxr-xr-x   0        0        0     1918 2023-07-13 20:51:45.079756 bento_mdf-0.9.1/bin/test-mdf.py
+-rw-r--r--   0        0        0     1848 2023-07-13 20:51:45.079756 bento_mdf-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-07-13 20:51:45.079756 bento_mdf-0.9.1/src/bento_mdf/__init__.py
+-rw-r--r--   0        0        0     9158 2023-07-13 20:51:45.079756 bento_mdf-0.9.1/src/bento_mdf/diff.py
+-rw-r--r--   0        0        0    29005 2023-07-13 20:51:45.079756 bento_mdf-0.9.1/src/bento_mdf/mdf.py
+-rw-r--r--   0        0        0     8110 2023-07-13 20:51:45.079756 bento_mdf-0.9.1/src/bento_mdf/validator.py
+-rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 bento_mdf-0.9.1/PKG-INFO
```

### Comparing `bento_mdf-0.7.2/README.md` & `bento_mdf-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This directory provides ``test-mdf.py``, a standalone command line MDF validator.
 
 ## Installation
 
 Install the latest version (including scripts below) from GitHub using
 an up-to-date pip:
 
-	pip install bento_mdf@git+https://github.com/CBIIT/bento-mdf.git#egg=subdir\&subdirectory=drivers/python
+	pip install bento-mdf
 
 ## Scripts
 
 Scripts [`test-mdf.py`](./test-mdf.py) and
 [`load-mdf.py`](./load-mdf.py) are included in the
 distribution. `test-mdf` is a verbose validator that can be used to
 find issues in a set of local MDFs using the [MDF
```

### Comparing `bento_mdf-0.7.2/bin/load-mdf.py` & `bento_mdf-0.9.1/bin/load-mdf.py`

 * *Files identical despite different names*

### Comparing `bento_mdf-0.7.2/bin/test-mdf.py` & `bento_mdf-0.9.1/bin/test-mdf.py`

 * *Files identical despite different names*

### Comparing `bento_mdf-0.7.2/pyproject.toml` & `bento_mdf-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bento-mdf"
-version = "0.7.2"
+version = "0.9.1"
 description = "Python driver/validator for Bento Model Description Format"
 authors = [
     { name="Mark A. Jensen", email = "mark.jensen@nih.gov"}
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
@@ -14,15 +14,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/CBIIT/bento-mdf"
 "Bug Tracker" = "https://github.com/CBIIT/bento-mdf/issues"
 
 [tool.poetry]
 name = "bento-mdf"
-version = "0.7.2"
+version = "0.9.1"
 description = "Python driver/validator for Bento Model Description Format"
 authors = [
     "Mark A. Jensen <mark.jensen@nih.gov>"
 ]
 license = "Apache 2.0"
 readme = "README.md"
 include = ["logs/log.ini"]
```

### Comparing `bento_mdf-0.7.2/src/bento_mdf/diff.py` & `bento_mdf-0.9.1/src/bento_mdf/diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-import sys
 import logging
 import os.path
+import sys
+
 sys.path.append("..")
+from warnings import warn
+
 from bento_mdf.mdf import MDF
 from bento_meta.objects import *
-from warnings import warn
+
 # NOTE: the diff class was changed from keeping the final data structure "result"
 #       from being 'set' based to being 'list' so that it could be dumped into
 #       json structure (which is incompatible with sets)
 
 
 class Diff:
     """for manipulating the final result data structure when diff models"""
@@ -111,17 +114,17 @@
 
     logging.info("point A")
     # set_trace()
 
     for thing in sets:
         aset = set(getattr(mdl_a, thing))
         bset = set(getattr(mdl_b, thing))
-        sets[thing]["a"] = sorted(list(set(aset - bset)))
-        sets[thing]["b"] = sorted(list(set(bset - aset)))
-        sets[thing]["common"] = sorted(list(set(aset & bset)))
+        sets[thing]["a"] = list(set(aset - bset))
+        sets[thing]["b"] = list(set(bset - aset))
+        sets[thing]["common"] = list(set(aset & bset))
 
         logging.debug("ok, where is {} at?".format(thing))
         logging.debug("aset is {}".format(aset))
         logging.debug("bset is {}".format(bset))
 
         logging.debug(" you want a:{}".format(sets[thing]["a"]))
         logging.debug(" you want b:{}".format(sets[thing]["b"]))
@@ -151,16 +154,16 @@
                     logging.info("...comparing simple {}".format(getattr(b_ent, att)))
                     continue
                 else:
                     diff_.update_result(
                         thing,
                         entk,
                         att,
-                        sorted(getattr(a_ent, att)),
-                        sorted(getattr(b_ent, att)),
+                        getattr(a_ent, att),
+                        getattr(b_ent, att),
                     )
 
             # try and see if the "object" type is the same?
             #     a_att,b_att are things like "valuesets", "properties"
             logging.info("...object")
             for att in obj_atts:
                 a_att = getattr(a_ent, att)
@@ -175,51 +178,52 @@
                 if type(a_att) == type(b_att):
                     if type(a_att) == ValueSet:  # kludge for ValueSet+Terms
                         if diff_.valuesets_are_different(a_att, b_att):
                             diff_.update_result(
                                 thing,
                                 entk,
                                 att,
-                                sorted(list(set(a_att.terms) - set(b_att.terms))),
-                                sorted(list(set(b_att.terms) - set(a_att.terms))),
+                                list(set(a_att.terms) - set(b_att.terms)),
+                                list(set(b_att.terms) - set(a_att.terms)),
                             )
                     # items are something-other-than valuesets
+                    # items are concepts
+                    elif type(a_att) == Concept:
+                        continue  # new concept nanos generated when Model loaded so can't compare???
                     elif getattr(a_att, "handle"):
                         if a_att.handle == b_att.handle:
                             continue
                         else:
-                            diff_.update_result(
-                                thing, entk, att, sorted(a_att), sorted(b_att)
-                            )
+                            diff_.update_result(thing, entk, att, a_att, b_att)
                     else:
                         warn(
                             "can't handle attribute with type {}".format(
                                 type(a_att).__name__
                             )
                         )
                         logging.warning(
                             "can't handle attribute with type {}".format(
                                 type(a_att).__name__
                             )
                         )
                 else:
-                    diff_.update_result(thing, entk, att, sorted(a_att), sorted(b_att))
+                    diff_.update_result(thing, entk, att, a_att, b_att)
 
             # try and see if the "collection" set is the same?
             logging.info("...collection")
             for att in coll_atts:
                 aset = set(getattr(a_ent, att))
                 bset = set(getattr(b_ent, att))
                 if aset != bset:
                     diff_.update_result(
                         thing,
                         entk,
                         att,
-                        sorted(list(set(aset - bset))),
-                        sorted(list(set(bset - aset))),
+                        list(set(aset - bset)),
+                        list(set(bset - aset)),
                     )
 
     logging.info("done")
     diff_.finalize_result()
     return diff_.result
```

### Comparing `bento_mdf-0.7.2/src/bento_mdf/mdf.py` & `bento_mdf-0.9.1/src/bento_mdf/mdf.py`

 * *Files identical despite different names*

### Comparing `bento_mdf-0.7.2/src/bento_mdf/validator.py` & `bento_mdf-0.9.1/src/bento_mdf/validator.py`

 * *Files identical despite different names*

### Comparing `bento_mdf-0.7.2/setup.py` & `bento_mdf-0.9.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,149 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bento-mdf
+Version: 0.9.1
+Summary: Python driver/validator for Bento Model Description Format
+License: Apache 2.0
+Author: Mark A. Jensen
+Author-email: mark.jensen@nih.gov
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bento-meta (>=0.1.3)
+Requires-Dist: delfick-project (>=0.7.9,<0.8.0)
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Requires-Dist: pyyaml (>=6)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Description-Content-Type: text/markdown
+
+bento_mdf
+=======
+
+Python 3 drivers for the graph [Model Description Format](https://github.com/CBIIT/bento-mdf)
+
+This directory provides ``test-mdf.py``, a standalone command line MDF validator.
+
+## Installation
+
+Install the latest version (including scripts below) from GitHub using
+an up-to-date pip:
+
+	pip install bento-mdf
+
+## Scripts
+
+Scripts [`test-mdf.py`](./test-mdf.py) and
+[`load-mdf.py`](./load-mdf.py) are included in the
+distribution. `test-mdf` is a verbose validator that can be used to
+find issues in a set of local MDFs using the [MDF
+JSONSchema](../../schema/mdf-schema.yaml). `load-mdf` will load a
+valid set of MDFs into an existing [Neo4j](https://neo4j.com) [Metamodel Database](https://github.com/CBIIT/bento-meta).
+
+
+## `test-mdf` Usage
+
+    $ test-mdf.py -h
+    usage: test-mdf.py [-h] [--schema SCHEMA] [--quiet] [--log-file LOG_FILE]
+                       mdf-file [mdf-file ...]
+
+    Validate MDF against JSONSchema
+
+    positional arguments:
+      mdf-file             MDF yaml files for validation
+
+    optional arguments:
+      -h, --help           show this help message and exit
+      --schema SCHEMA      MDF JSONschema file
+      --quiet              Suppress output; return only exit value
+      --log-file LOG_FILE  Log file name
+
+See "Validator Notes" below.
+
+## `load-mdf` Usage
+
+    $ ./load-mdf.py -h
+    usage: load-mdf.py [-h] --commit COMMIT [--handle HANDLE] [--user USER] [--passw PASSW]
+                       [--bolt BoltURL] [--put]
+                       [MDF-FILE ...]
+
+    Load model in MDF into an MDB
+
+    positional arguments:
+      MDF-FILE         MDF file(s)/url(s)
+
+    optional arguments:
+      -h, --help       show this help message and exit
+      --commit COMMIT  commit SHA1 for MDF instance (if any)
+      --handle HANDLE  model handle
+      --user USER      MDB username
+      --passw PASSW    MDB password
+      --bolt BoltURL   MDB Bolt url endpoint (specify as 'bolt://...')
+      --put            Load model to database
+
+## Validator `test-mdf.py`Notes
+
+The ``--schema`` argument is optional. ``test-mdf.py`` will automatically retrieve the latest [mdf-schema.yaml](../../schema/mdf-schema.yaml) in the master branch of [this repo](https://github.com/CBIIT/bento-mdf).
+
+The script tests both the syntax of the YAML (for both schema and MDF files), and the validity of the files with respect to the JSONSchema (for both schema and MDF files).
+
+The errors are as emitted from the [PyYaml](https://pyyaml.org/wiki/PyYAMLDocumentation) and [jsonschema](https://python-jsonschema.readthedocs.io/en/stable/) packages, and can be rather obscure.
+
+* Successful test
+
+        $ test-mdf.py samples/ctdc_model_file.yaml samples/ctdc_model_properties_file.yaml 
+        Checking schema YAML =====
+        Checking as a JSON schema =====
+        Checking instance YAML =====
+        Checking instance against schema =====
+
+* Bad YAML syntax
+
+        $ test-mdf.py samples/ctdc_model_bad.yaml samples/ctdc_model_properties_file.yaml 
+        Checking schema YAML =====
+        Checking as a JSON schema =====
+        Checking instance YAML =====
+        YAML error in 'samples/ctdc_model_bad.yaml':
+        while parsing a block mapping
+          in "samples/ctdc_model_bad.yaml", line 1, column 1
+        expected <block end>, but found '<block mapping start>'
+          in "samples/ctdc_model_bad.yaml", line 3, column 3
+
+* Schema-invalid YAML
+
+        $ test-mdf.py samples/ctdc_model_file_invalid.yaml samples/ctdc_model_properties_file.yaml 
+        Checking schema YAML =====
+        Checking as a JSON schema =====
+        Checking instance YAML =====
+        Checking instance against schema =====
+        ['show_node', 'specimen_id', 'biopsy_sequence_number', 'specimen_type'] is not of type 'object'
+        
+        Failed validating 'type' in schema['properties']['Nodes']['additionalProperties']:
+            {'$id': '#nodeSpec',
+             'properties': {'Category': {'$ref': '#/defs/snake_case_id'},
+                            'Props': {'oneOf': [{'items': {'$ref': '#/defs/snake_case_id'},
+                                                 'type': 'array',
+                                                 'uniqueItems': True},
+                                                {'type': 'null'}]},
+                            'Tags': {'$ref': '#/defs/tagsSpec'}},
+             'required': ['Props'],
+             'type': 'object'}
+        
+        On instance['Nodes']['specimen']:
+            ['show_node', 'specimen_id', 'biopsy_sequence_number', 'specimen_type']
+
+## Testing the tester
+
+The validator code itself can be tested as follows:
+
+    pip install tox
+    cd bento-mdf/validators/mdf-validate
+    tox
 
-package_dir = \
-{'': 'src'}
 
-packages = \
-['bento_mdf']
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['bento-meta>=0.1.3',
- 'delfick-project>=0.7.9,<0.8.0',
- 'jsonschema>=4.17.3,<5.0.0',
- 'pyyaml>=6',
- 'requests>=2.28.2,<3.0.0',
- 'tqdm>=4.64.1,<5.0.0']
-
-scripts = \
-['bin/test-mdf.py', 'bin/load-mdf.py']
-
-setup_kwargs = {
-    'name': 'bento-mdf',
-    'version': '0.7.2',
-    'description': 'Python driver/validator for Bento Model Description Format',
-    'long_description': 'bento_mdf\n=======\n\nPython 3 drivers for the graph [Model Description Format](https://github.com/CBIIT/bento-mdf)\n\nThis directory provides ``test-mdf.py``, a standalone command line MDF validator.\n\n## Installation\n\nInstall the latest version (including scripts below) from GitHub using\nan up-to-date pip:\n\n\tpip install bento_mdf@git+https://github.com/CBIIT/bento-mdf.git#egg=subdir\\&subdirectory=drivers/python\n\n## Scripts\n\nScripts [`test-mdf.py`](./test-mdf.py) and\n[`load-mdf.py`](./load-mdf.py) are included in the\ndistribution. `test-mdf` is a verbose validator that can be used to\nfind issues in a set of local MDFs using the [MDF\nJSONSchema](../../schema/mdf-schema.yaml). `load-mdf` will load a\nvalid set of MDFs into an existing [Neo4j](https://neo4j.com) [Metamodel Database](https://github.com/CBIIT/bento-meta).\n\n\n## `test-mdf` Usage\n\n    $ test-mdf.py -h\n    usage: test-mdf.py [-h] [--schema SCHEMA] [--quiet] [--log-file LOG_FILE]\n                       mdf-file [mdf-file ...]\n\n    Validate MDF against JSONSchema\n\n    positional arguments:\n      mdf-file             MDF yaml files for validation\n\n    optional arguments:\n      -h, --help           show this help message and exit\n      --schema SCHEMA      MDF JSONschema file\n      --quiet              Suppress output; return only exit value\n      --log-file LOG_FILE  Log file name\n\nSee "Validator Notes" below.\n\n## `load-mdf` Usage\n\n    $ ./load-mdf.py -h\n    usage: load-mdf.py [-h] --commit COMMIT [--handle HANDLE] [--user USER] [--passw PASSW]\n                       [--bolt BoltURL] [--put]\n                       [MDF-FILE ...]\n\n    Load model in MDF into an MDB\n\n    positional arguments:\n      MDF-FILE         MDF file(s)/url(s)\n\n    optional arguments:\n      -h, --help       show this help message and exit\n      --commit COMMIT  commit SHA1 for MDF instance (if any)\n      --handle HANDLE  model handle\n      --user USER      MDB username\n      --passw PASSW    MDB password\n      --bolt BoltURL   MDB Bolt url endpoint (specify as \'bolt://...\')\n      --put            Load model to database\n\n## Validator `test-mdf.py`Notes\n\nThe ``--schema`` argument is optional. ``test-mdf.py`` will automatically retrieve the latest [mdf-schema.yaml](../../schema/mdf-schema.yaml) in the master branch of [this repo](https://github.com/CBIIT/bento-mdf).\n\nThe script tests both the syntax of the YAML (for both schema and MDF files), and the validity of the files with respect to the JSONSchema (for both schema and MDF files).\n\nThe errors are as emitted from the [PyYaml](https://pyyaml.org/wiki/PyYAMLDocumentation) and [jsonschema](https://python-jsonschema.readthedocs.io/en/stable/) packages, and can be rather obscure.\n\n* Successful test\n\n        $ test-mdf.py samples/ctdc_model_file.yaml samples/ctdc_model_properties_file.yaml \n        Checking schema YAML =====\n        Checking as a JSON schema =====\n        Checking instance YAML =====\n        Checking instance against schema =====\n\n* Bad YAML syntax\n\n        $ test-mdf.py samples/ctdc_model_bad.yaml samples/ctdc_model_properties_file.yaml \n        Checking schema YAML =====\n        Checking as a JSON schema =====\n        Checking instance YAML =====\n        YAML error in \'samples/ctdc_model_bad.yaml\':\n        while parsing a block mapping\n          in "samples/ctdc_model_bad.yaml", line 1, column 1\n        expected <block end>, but found \'<block mapping start>\'\n          in "samples/ctdc_model_bad.yaml", line 3, column 3\n\n* Schema-invalid YAML\n\n        $ test-mdf.py samples/ctdc_model_file_invalid.yaml samples/ctdc_model_properties_file.yaml \n        Checking schema YAML =====\n        Checking as a JSON schema =====\n        Checking instance YAML =====\n        Checking instance against schema =====\n        [\'show_node\', \'specimen_id\', \'biopsy_sequence_number\', \'specimen_type\'] is not of type \'object\'\n        \n        Failed validating \'type\' in schema[\'properties\'][\'Nodes\'][\'additionalProperties\']:\n            {\'$id\': \'#nodeSpec\',\n             \'properties\': {\'Category\': {\'$ref\': \'#/defs/snake_case_id\'},\n                            \'Props\': {\'oneOf\': [{\'items\': {\'$ref\': \'#/defs/snake_case_id\'},\n                                                 \'type\': \'array\',\n                                                 \'uniqueItems\': True},\n                                                {\'type\': \'null\'}]},\n                            \'Tags\': {\'$ref\': \'#/defs/tagsSpec\'}},\n             \'required\': [\'Props\'],\n             \'type\': \'object\'}\n        \n        On instance[\'Nodes\'][\'specimen\']:\n            [\'show_node\', \'specimen_id\', \'biopsy_sequence_number\', \'specimen_type\']\n\n## Testing the tester\n\nThe validator code itself can be tested as follows:\n\n    pip install tox\n    cd bento-mdf/validators/mdf-validate\n    tox\n\n\n\n\n',
-    'author': 'Mark A. Jensen',
-    'author_email': 'mark.jensen@nih.gov',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'scripts': scripts,
-    'python_requires': '>=3.8,<4.0',
-}
 
 
-setup(**setup_kwargs)
```

