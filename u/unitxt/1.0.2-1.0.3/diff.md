# Comparing `tmp/unitxt-1.0.2.tar.gz` & `tmp/unitxt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-1.0.2.tar", last modified: Wed Jul 12 10:40:38 2023, max compression
+gzip compressed data, was "unitxt-1.0.3.tar", last modified: Thu Jul 13 12:56:46 2023, max compression
```

## Comparing `unitxt-1.0.2.tar` & `unitxt-1.0.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-12 10:40:38.786075 unitxt-1.0.2/
--rw-rw-r--   0 elron    (605371) tslm      (3127)    11357 2023-07-11 12:24:16.000000 unitxt-1.0.2/LICENSE
--rw-rw-r--   0 elron    (605371) tslm      (3127)       33 2023-07-11 12:24:16.000000 unitxt-1.0.2/MANIFEST.in
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2242 2023-07-12 10:40:38.785474 unitxt-1.0.2/PKG-INFO
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1810 2023-07-12 07:15:30.000000 unitxt-1.0.2/README.md
--rw-rw-r--   0 elron    (605371) tslm      (3127)      118 2023-07-12 07:33:22.000000 unitxt-1.0.2/pyproject.toml
--rw-rw-r--   0 elron    (605371) tslm      (3127)       38 2023-07-12 10:40:38.786188 unitxt-1.0.2/setup.cfg
--rw-rw-r--   0 elron    (605371) tslm      (3127)      811 2023-07-12 10:40:35.000000 unitxt-1.0.2/setup.py
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-12 10:40:38.695540 unitxt-1.0.2/src/
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-12 10:40:38.777942 unitxt-1.0.2/src/unitxt/
--rw-rw-r--   0 elron    (605371) tslm      (3127)      129 2023-07-12 10:12:58.000000 unitxt-1.0.2/src/unitxt/__init__.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     5949 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/artifact.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      944 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/blocks.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      535 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/card.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2786 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/catalog.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/collections.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2948 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/common.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2831 2023-07-12 10:02:38.000000 unitxt-1.0.2/src/unitxt/dataset.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/file_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      399 2023-07-12 09:44:41.000000 unitxt-1.0.2/src/unitxt/fusion.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1686 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/generator_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      656 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/instructions.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      659 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/load.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      669 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/loaders.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     4579 2023-07-12 10:10:40.000000 unitxt-1.0.2/src/unitxt/metric.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     4244 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/metrics.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      935 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/normalizers.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     8441 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/operator.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     7075 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/operators.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      201 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/processors.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      428 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/recipe.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1384 2023-07-12 10:15:26.000000 unitxt-1.0.2/src/unitxt/register.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2041 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/schema.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)    11051 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/split_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     3556 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/splitters.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6556 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/stream.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      567 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/task.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6351 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/templates.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6768 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/text_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      246 2023-07-12 09:26:30.000000 unitxt-1.0.2/src/unitxt/utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1327 2023-07-12 09:48:17.000000 unitxt-1.0.2/src/unitxt/validate.py
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-12 10:40:38.784101 unitxt-1.0.2/src/unitxt.egg-info/
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2242 2023-07-12 10:40:38.779922 unitxt-1.0.2/src/unitxt.egg-info/PKG-INFO
--rw-rw-r--   0 elron    (605371) tslm      (3127)      931 2023-07-12 10:40:38.781000 unitxt-1.0.2/src/unitxt.egg-info/SOURCES.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)        1 2023-07-12 10:40:38.781620 unitxt-1.0.2/src/unitxt.egg-info/dependency_links.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)       66 2023-07-12 10:40:38.783545 unitxt-1.0.2/src/unitxt.egg-info/requires.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)        7 2023-07-12 10:40:38.784195 unitxt-1.0.2/src/unitxt.egg-info/top_level.txt
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-13 12:56:46.970772 unitxt-1.0.3/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)    11357 2023-07-11 12:24:16.000000 unitxt-1.0.3/LICENSE
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       33 2023-07-11 12:24:16.000000 unitxt-1.0.3/MANIFEST.in
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2437 2023-07-13 12:56:46.970439 unitxt-1.0.3/PKG-INFO
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2005 2023-07-13 09:36:28.000000 unitxt-1.0.3/README.md
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      118 2023-07-12 07:33:22.000000 unitxt-1.0.3/pyproject.toml
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       38 2023-07-13 12:56:46.970882 unitxt-1.0.3/setup.cfg
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      811 2023-07-13 12:56:06.000000 unitxt-1.0.3/setup.py
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-13 12:56:46.953632 unitxt-1.0.3/src/
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-13 12:56:46.967549 unitxt-1.0.3/src/unitxt/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      129 2023-07-12 10:12:58.000000 unitxt-1.0.3/src/unitxt/__init__.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6331 2023-07-13 09:36:28.000000 unitxt-1.0.3/src/unitxt/artifact.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      944 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/blocks.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      535 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/card.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     3240 2023-07-13 11:06:45.000000 unitxt-1.0.3/src/unitxt/catalog.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/collections.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2948 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/common.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     3868 2023-07-13 09:38:45.000000 unitxt-1.0.3/src/unitxt/dataclass.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2905 2023-07-13 12:49:32.000000 unitxt-1.0.3/src/unitxt/dataset.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/file_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      398 2023-07-12 10:44:35.000000 unitxt-1.0.3/src/unitxt/fusion.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1686 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/generator_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      656 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/instructions.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      407 2023-07-13 09:36:28.000000 unitxt-1.0.3/src/unitxt/load.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      669 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/loaders.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     4628 2023-07-13 12:49:45.000000 unitxt-1.0.3/src/unitxt/metric.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     4244 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/metrics.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      935 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/normalizers.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     8441 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/operator.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     7075 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/operators.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      201 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/processors.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      428 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/recipe.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1856 2023-07-13 11:09:36.000000 unitxt-1.0.3/src/unitxt/register.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2041 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/schema.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)    11051 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/split_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     3556 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/splitters.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6556 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/stream.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      567 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/task.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6351 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/templates.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6768 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/text_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      238 2023-07-13 09:36:28.000000 unitxt-1.0.3/src/unitxt/utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1327 2023-07-12 10:44:34.000000 unitxt-1.0.3/src/unitxt/validate.py
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-13 12:56:46.969839 unitxt-1.0.3/src/unitxt.egg-info/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2437 2023-07-13 12:56:46.967954 unitxt-1.0.3/src/unitxt.egg-info/PKG-INFO
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      955 2023-07-13 12:56:46.968276 unitxt-1.0.3/src/unitxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)        1 2023-07-13 12:56:46.968791 unitxt-1.0.3/src/unitxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       66 2023-07-13 12:56:46.969413 unitxt-1.0.3/src/unitxt.egg-info/requires.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)        7 2023-07-13 12:56:46.969940 unitxt-1.0.3/src/unitxt.egg-info/top_level.txt
```

### Comparing `unitxt-1.0.2/LICENSE` & `unitxt-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/PKG-INFO` & `unitxt-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 We aspire to be simple, adaptable and transperant. 
 
 Unitxt builds on separation. Separation allows adding a dataset, without knowing anything about the models using it. Separation allows training without caring for preprocessing, switching models without loading the data differently and changing formats (instruction\ICL\etc.) without changing anything else. 
 
 # 
 [![version](https://img.shields.io/pypi/v/unitxt)](https://pypi.org/project/unitxt/)  ![license](https://img.shields.io/github/license/ibm/unitxt)  ![python](https://img.shields.io/badge/python-3.8%20|%203.9-blue)  ![tests](https://img.shields.io/github/actions/workflow/status/ibm/unitxt/tests.yml?branch=main&label=tests)
 ![Read the Docs](https://img.shields.io/readthedocs/unitxt)
+[![downloads](https://static.pepy.tech/personalized-badge/unitxt?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/unitxt)
 
 
 # Installation 🦄
 
 ```bash
   pip install unitxt
 ```
```

### Comparing `unitxt-1.0.2/README.md` & `unitxt-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 We aspire to be simple, adaptable and transperant. 
 
 Unitxt builds on separation. Separation allows adding a dataset, without knowing anything about the models using it. Separation allows training without caring for preprocessing, switching models without loading the data differently and changing formats (instruction\ICL\etc.) without changing anything else. 
 
 # 
 [![version](https://img.shields.io/pypi/v/unitxt)](https://pypi.org/project/unitxt/)  ![license](https://img.shields.io/github/license/ibm/unitxt)  ![python](https://img.shields.io/badge/python-3.8%20|%203.9-blue)  ![tests](https://img.shields.io/github/actions/workflow/status/ibm/unitxt/tests.yml?branch=main&label=tests)
 ![Read the Docs](https://img.shields.io/readthedocs/unitxt)
+[![downloads](https://static.pepy.tech/personalized-badge/unitxt?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/unitxt)
 
 
 # Installation 🦄
 
 ```bash
   pip install unitxt
 ```
```

### Comparing `unitxt-1.0.2/setup.py` & `unitxt-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
     
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="unitxt",
-    version="1.0.2",
+    version="1.0.3",
     author="IBM Research",
     author_email="elron.bandel@ibm.com",
     description="Load any mixture of text to text data in one line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ibm/unitxt",
     packages=setuptools.find_packages('src'),
```

### Comparing `unitxt-1.0.2/src/unitxt/artifact.py` & `unitxt-1.0.3/src/unitxt/artifact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 import inspect
 import json
 import os
 import pkgutil
-import re
 from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass, field, fields
 from typing import final
 
+from .text_utils import camel_to_snake_case, is_camel_case
+
 
 class AbstractField:
     pass
 
 
-from .text_utils import camel_to_snake_case, is_camel_case
-
-artifactories = []
+class Artifactories(object):
+    def __new__(cls):
+        if not hasattr(cls, 'instance'):
+            cls.instance = super(Artifactories, cls).__new__(cls)
+            cls.instance.artifactories = []
+
+        return cls.instance
+
+    def __iter__(self):
+        return iter(self.artifactories)
+
+    def __next__(self):
+        return next(self.artifactories)
+
+    def register_atrifactory(self, artifactory):
+        assert isinstance(artifactory, Artifactory), "Artifactory must be an instance of Artifactory"
+        assert hasattr(artifactory, "__contains__"), "Artifactory must have __contains__ method"
+        assert hasattr(artifactory, "__getitem__"), "Artifactory must have __getitem__ method"
+        self.artifactories.append(artifactory)
 
 
 class BaseArtifact(ABC):
     _class_register = {}
 
     @classmethod
     def is_artifact_dict(cls, d):
@@ -73,15 +90,15 @@
 
         for field in fields(self):
             # check if field.type is class and if it is subclass of BaseArtifact
             if isinstance(field.type, type) and issubclass(field.type, BaseArtifact):
                 value = getattr(self, field.name)
                 if isinstance(value, str):
                     artifact, artifactory = fetch_artifact(value)
-                    assert artifact is not None, f"Artifact {value} does not exist, in {artifactories}"
+                    assert artifact is not None, f"Artifact {value} does not exist, in {Artifactories()}"
                     print(f"Artifact {value} is fetched from {artifactory}")
                     setattr(self, field.name, artifact)
 
         self.prepare()
         self.verify()
 
     def to_dict(self):
@@ -158,26 +175,19 @@
         return f"Artifact {self.name} does not exist, in artifactories:{self.artifactories}"
 
 
 def fetch_artifact(name):
     if Artifact.is_artifact_file(name):
         return Artifact.load(name), None
     else:
-        for artifactory in artifactories:
+        for artifactory in Artifactories():
             if name in artifactory:
                 return artifactory[name], artifactory
 
-    raise UnitxtArtifactNotFoundError(name, artifactories)
-
-
-def register_atrifactory(artifactory):
-    assert isinstance(artifactory, Artifactory), "Artifactory must be an instance of Artifactory"
-    assert hasattr(artifactory, "__contains__"), "Artifactory must have __contains__ method"
-    assert hasattr(artifactory, "__getitem__"), "Artifactory must have __getitem__ method"
-    artifactories.append(artifactory)
+    raise UnitxtArtifactNotFoundError(name, Artifactories().artifactories)
 
 
 def register_all_artifacts(path):
     for loader, module_name, is_pkg in pkgutil.walk_packages(path):
         print(__name__)
         if module_name == __name__:
             continue
```

### Comparing `unitxt-1.0.2/src/unitxt/blocks.py` & `unitxt-1.0.3/src/unitxt/blocks.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/card.py` & `unitxt-1.0.3/src/unitxt/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/collections.py` & `unitxt-1.0.3/src/unitxt/collections.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/common.py` & `unitxt-1.0.3/src/unitxt/common.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/dataset.py` & `unitxt-1.0.3/src/unitxt/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .artifact import __file__ as _
 from .artifact import fetch_artifact
 from .blocks import __file__ as _
 from .card import __file__ as _
 from .catalog import __file__ as _
 from .collections import __file__ as _
 from .common import __file__ as _
+from .dataclass import __file__ as _
 from .file_utils import __file__ as _
 from .fusion import __file__ as _
 from .generator_utils import __file__ as _
 from .instructions import __file__ as _
 from .load import __file__ as _
 from .loaders import __file__ as _
 from .metric import __file__ as _
@@ -42,14 +43,15 @@
         return None
 
 
 def parse(query: str):
     """
     Parses a query of the form 'key1=value1,key2=value2,...' into a dictionary.
     """
+    query = query.replace("@", "::")
     result = {}
     for kv in query.split(","):
         parts = kv.split("=")
         if parts[1].isdigit():
             result[parts[0]] = int(parts[1])
         elif parts[1].replace(".", "", 1).isdigit():
             result[parts[0]] = float(parts[1])
```

### Comparing `unitxt-1.0.2/src/unitxt/file_utils.py` & `unitxt-1.0.3/src/unitxt/file_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/generator_utils.py` & `unitxt-1.0.3/src/unitxt/generator_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/instructions.py` & `unitxt-1.0.3/src/unitxt/instructions.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/loaders.py` & `unitxt-1.0.3/src/unitxt/loaders.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/metric.py` & `unitxt-1.0.3/src/unitxt/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .artifact import __file__ as _
 from .blocks import __file__ as _
 from .card import __file__ as _
 from .catalog import __file__ as _
 from .collections import __file__ as _
 from .common import __file__ as _
+from .dataclass import __file__ as _
 from .file_utils import __file__ as _
 from .fusion import __file__ as _
 from .generator_utils import __file__ as _
 from .instructions import __file__ as _
 from .load import __file__ as _
 from .loaders import __file__ as _
 from .metrics import __file__ as _
@@ -92,15 +93,15 @@
 
 class MetricRecipe(SequntialOperatorInitilizer):
     def prepare(self):
         register_all_artifacts()
         self.steps = [
             FromPredictionsAndOriginalData(),
             ApplyValueOperatorsField(
-                value_field="prediction", operators_field="processors", default_operators=["to_string"]
+                value_field="prediction", operators_field="processors", default_operators=["processors::to_string"]
             ),
             SplitByValue(["group"]),
             ApplyStreamOperatorsField(
                 "metrics",
                 reversed=True,
             ),
             MultiStreamScoreMean(),
```

### Comparing `unitxt-1.0.2/src/unitxt/metrics.py` & `unitxt-1.0.3/src/unitxt/metrics.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/normalizers.py` & `unitxt-1.0.3/src/unitxt/normalizers.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/operator.py` & `unitxt-1.0.3/src/unitxt/operator.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/operators.py` & `unitxt-1.0.3/src/unitxt/operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/register.py` & `unitxt-1.0.3/src/unitxt/register.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,61 @@
-import inspect
-import os
 import importlib
 import inspect
+import os
 
-from .artifact import Artifact
+from .artifact import Artifact, Artifactories
+from .catalog import LocalCatalog, GithubCatalog, PATHS_SEP
 from .utils import Singleton
+
+
+UNITXT_ARTIFACTORIES_ENV_VAR = 'UNITXT_ARTIFACTORIES'
+
 # Usage
-non_registered_files = ['__init__.py', 'artifact.py', 'utils.py', 'register.py', 'metric.py', 'dataset.py', 'blocks.py']
+non_registered_files = [
+    "__init__.py",
+    "artifact.py",
+    "utils.py",
+    "register.py",
+    "metric.py",
+    "dataset.py",
+    "blocks.py",
+]
+
+
+def _register_all_catalogs():
+    Artifactories().register_atrifactory(LocalCatalog())
+    if UNITXT_ARTIFACTORIES_ENV_VAR in os.environ:
+        for path in os.environ[UNITXT_ARTIFACTORIES_ENV_VAR].split(PATHS_SEP):
+            Artifactories().register_atrifactory(LocalCatalog(location=path))
+    Artifactories().register_atrifactory(GithubCatalog())
 
 def _register_all_artifacts():
-    
     dir = os.path.dirname(__file__)
     file_name = os.path.basename(__file__)
-    
+
     for file in os.listdir(dir):
-        if file.endswith('.py') and file not in non_registered_files and file != file_name:
-            module_name = file.replace('.py', '')
-            
-            module = importlib.import_module('.' + module_name, __package__)
-            
+        if file.endswith(".py") and file not in non_registered_files and file != file_name:
+            module_name = file.replace(".py", "")
+
+            module = importlib.import_module("." + module_name, __package__)
+
             for name, obj in inspect.getmembers(module):
                 # Make sure the object is a class
                 if inspect.isclass(obj):
                     # Make sure the class is a subclass of Artifact (but not Artifact itself)
                     if issubclass(obj, Artifact) and obj is not Artifact:
                         Artifact.register_class(obj)
-            
 
-class ProjectArtifactRegisterer(Singleton):
-    
+
+class ProjectArtifactRegisterer(metaclass=Singleton):
     def __init__(self):
-        
-        if not hasattr(self, '_registered'):
+        if not hasattr(self, "_registered"):
             self._registered = False
-        
+
         if not self._registered:
+            _register_all_catalogs()
             _register_all_artifacts()
             self._registered = True
-            
+
 
 def register_all_artifacts():
-    ProjectArtifactRegisterer()
+    ProjectArtifactRegisterer()
```

### Comparing `unitxt-1.0.2/src/unitxt/schema.py` & `unitxt-1.0.3/src/unitxt/schema.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/split_utils.py` & `unitxt-1.0.3/src/unitxt/split_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/splitters.py` & `unitxt-1.0.3/src/unitxt/splitters.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/stream.py` & `unitxt-1.0.3/src/unitxt/stream.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/task.py` & `unitxt-1.0.3/src/unitxt/task.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/templates.py` & `unitxt-1.0.3/src/unitxt/templates.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/text_utils.py` & `unitxt-1.0.3/src/unitxt/text_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.2/src/unitxt/validate.py` & `unitxt-1.0.3/src/unitxt/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC
 from dataclasses import field
 from typing import Any, Dict
 
 from datasets import Dataset, Features, Sequence, Value
 
-from .operator import  StreamInstanceOperator
+from .operator import StreamInstanceOperator
+
 
 class Validator(ABC):
     pass
 
 
 class ValidateSchema(Validator, StreamInstanceOperator):
     schema: Features = None
```

### Comparing `unitxt-1.0.2/src/unitxt.egg-info/PKG-INFO` & `unitxt-1.0.3/src/unitxt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 We aspire to be simple, adaptable and transperant. 
 
 Unitxt builds on separation. Separation allows adding a dataset, without knowing anything about the models using it. Separation allows training without caring for preprocessing, switching models without loading the data differently and changing formats (instruction\ICL\etc.) without changing anything else. 
 
 # 
 [![version](https://img.shields.io/pypi/v/unitxt)](https://pypi.org/project/unitxt/)  ![license](https://img.shields.io/github/license/ibm/unitxt)  ![python](https://img.shields.io/badge/python-3.8%20|%203.9-blue)  ![tests](https://img.shields.io/github/actions/workflow/status/ibm/unitxt/tests.yml?branch=main&label=tests)
 ![Read the Docs](https://img.shields.io/readthedocs/unitxt)
+[![downloads](https://static.pepy.tech/personalized-badge/unitxt?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/unitxt)
 
 
 # Installation 🦄
 
 ```bash
   pip install unitxt
 ```
```

### Comparing `unitxt-1.0.2/src/unitxt.egg-info/SOURCES.txt` & `unitxt-1.0.3/src/unitxt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/unitxt/__init__.py
 src/unitxt/artifact.py
 src/unitxt/blocks.py
 src/unitxt/card.py
 src/unitxt/catalog.py
 src/unitxt/collections.py
 src/unitxt/common.py
+src/unitxt/dataclass.py
 src/unitxt/dataset.py
 src/unitxt/file_utils.py
 src/unitxt/fusion.py
 src/unitxt/generator_utils.py
 src/unitxt/instructions.py
 src/unitxt/load.py
 src/unitxt/loaders.py
```

