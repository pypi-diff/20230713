# Comparing `tmp/oarepo-model-builder-nr-1.0.8.tar.gz` & `tmp/oarepo-model-builder-nr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-nr-1.0.8.tar", last modified: Tue Mar 14 14:41:18 2023, max compression
+gzip compressed data, was "oarepo-model-builder-nr-1.0.9.tar", last modified: Tue Mar 14 19:15:30 2023, max compression
```

## Comparing `oarepo-model-builder-nr-1.0.8.tar` & `oarepo-model-builder-nr-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:41:18.946903 oarepo-model-builder-nr-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 14:41:18.946903 oarepo-model-builder-nr-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:41:18.942903 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:41:18.946903 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/models/nr_common_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/models/nr_datatypes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/models/nr_documents.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:41:18.946903 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 14:41:18.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-14 14:41:18.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:41:18.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-14 14:41:18.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:40:23.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-14 14:41:18.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-14 14:41:18.000000 oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-14 14:41:18.946903 oarepo-model-builder-nr-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 14:40:07.000000 oarepo-model-builder-nr-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:15:30.121938 oarepo-model-builder-nr-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 19:15:30.121938 oarepo-model-builder-nr-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:15:30.121938 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:15:30.121938 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/models/nr_common_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/models/nr_datatypes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/models/nr_documents.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:15:30.121938 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 19:15:30.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-14 19:15:30.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:15:30.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-14 19:15:30.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:14:36.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-14 19:15:30.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-14 19:15:30.000000 oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-14 19:15:30.121938 oarepo-model-builder-nr-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:14:23.000000 oarepo-model-builder-nr-1.0.9/setup.py
```

### Comparing `oarepo-model-builder-nr-1.0.8/PKG-INFO` & `oarepo-model-builder-nr-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-nr
-Version: 1.0.8
+Version: 1.0.9
 Summary: "A model builder plugin with Czech National Repository compatible metadata schema"
 Home-page: https://github.com/Narodni-repozitar/oarepo-model-builder-nr
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio Czech NR model builder
 Platform: any
```

### Comparing `oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/models/nr_common_metadata.yaml` & `oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/models/nr_common_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/models/nr_datatypes.yaml` & `oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/models/nr_datatypes.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr/models/nr_documents.yaml` & `oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr/models/nr_documents.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
               imports:
                 - import: nr_metadata.documents.services.records.ui_schema.NRDegreeGrantorUISchema
           marshmallow:
             schema-class: nr_metadata.documents.services.records.schema.NRDegreeGrantorSchema
             imports:
               - import: nr_metadata.documents.services.records.schema.NRDegreeGrantorSchema
           type: taxonomy
-          vocabulary-type: degreeGrantor
+          vocabulary-type: institutions
           label.cs: Instituce / grantor
           label.en: Degree grantor
         studyFields[]:
           type: keyword
           ^label.cs: Oblasti studia
           ^label.en: Study fields
     collection:
```

### Comparing `oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/PKG-INFO` & `oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-nr
-Version: 1.0.8
+Version: 1.0.9
 Summary: "A model builder plugin with Czech National Repository compatible metadata schema"
 Home-page: https://github.com/Narodni-repozitar/oarepo-model-builder-nr
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio Czech NR model builder
 Platform: any
```

### Comparing `oarepo-model-builder-nr-1.0.8/oarepo_model_builder_nr.egg-info/SOURCES.txt` & `oarepo-model-builder-nr-1.0.9/oarepo_model_builder_nr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-nr-1.0.8/setup.cfg` & `oarepo-model-builder-nr-1.0.9/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-nr
-version = 1.0.8
+version = 1.0.9
 description = "A model builder plugin with Czech National Repository compatible metadata schema"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio Czech NR model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```

