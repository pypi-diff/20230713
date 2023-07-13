# Comparing `tmp/pepdbagent-0.5.1.tar.gz` & `tmp/pepdbagent-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepdbagent-0.5.1.tar", last modified: Tue Jul 11 15:19:50 2023, max compression
+gzip compressed data, was "pepdbagent-0.5.2.tar", last modified: Thu Jul 13 16:11:43 2023, max compression
```

## Comparing `pepdbagent-0.5.1.tar` & `pepdbagent-0.5.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/pepdbagent/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/pepdbagent/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/modules/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/modules/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/pepdbagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pepdbagent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/pepdbagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 15:19:50.000000 pepdbagent-0.5.1/pepdbagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:50.792789 pepdbagent-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-11 15:19:37.000000 pepdbagent-0.5.1/tests/test_pepagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.128439 pepdbagent-0.5.2/pepdbagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/pepdbagent/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/modules/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/modules/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/pepdbagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/pepdbagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/tests/test_pepagent.py
```

### Comparing `pepdbagent-0.5.1/LICENSE.txt` & `pepdbagent-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/PKG-INFO` & `pepdbagent-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.5.1
+Version: 0.5.2
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.5.1/README.md` & `pepdbagent-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/pepdbagent/db_utils.py` & `pepdbagent-0.5.2/pepdbagent/db_utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/pepdbagent/exceptions.py` & `pepdbagent-0.5.2/pepdbagent/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/pepdbagent/models.py` & `pepdbagent-0.5.2/pepdbagent/models.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/pepdbagent/modules/annotation.py` & `pepdbagent-0.5.2/pepdbagent/modules/annotation.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/pepdbagent/modules/namespace.py` & `pepdbagent-0.5.2/pepdbagent/modules/namespace.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/pepdbagent/modules/project.py` & `pepdbagent-0.5.2/pepdbagent/modules/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
 import json
 import logging
 from typing import Union, List, NoReturn
 
 import peppy
-import sqlalchemy
 from sqlalchemy import Engine, and_, delete, insert, or_, select, update
 from sqlalchemy.exc import IntegrityError, NoResultFound
 from sqlalchemy.orm import Session
 from sqlalchemy import Select
 
 from peppy.const import SAMPLE_RAW_DICT_KEY, SUBSAMPLE_RAW_LIST_KEY, CONFIG_KEY
 
@@ -221,23 +220,23 @@
         :param update_only: if project exists overwrite it, otherwise do nothing.  [Default: False]
         :param description: description of the project
         :return: None
         """
         proj_dict = project.to_dict(extended=True, orient="records")
         if not description:
             description = project.description
-        proj_dict["_config"]["description"] = description
+        proj_dict[CONFIG_KEY]["description"] = description
 
         namespace = namespace.lower()
         if name:
             name = name.lower()
             proj_name = name
-            proj_dict["_config"]["name"] = project.name
-        elif proj_dict["_config"]["name"]:
-            proj_name = proj_dict["_config"]["name"].lower()
+            proj_dict[CONFIG_KEY]["name"] = proj_name
+        elif proj_dict[CONFIG_KEY]["name"]:
+            proj_name = proj_dict[CONFIG_KEY]["name"].lower()
         else:
             raise ValueError(f"Name of the project wasn't provided. Project will not be uploaded.")
 
         proj_digest = create_digest(proj_dict)
         number_of_samples = len(project.samples)
 
         if update_only:
@@ -327,26 +326,29 @@
         :return: None
         """
         proj_name = proj_name.lower()
         namespace = namespace.lower()
         if self.exists(namespace=namespace, name=proj_name, tag=tag):
             _LOGGER.info(f"Updating {proj_name} project...")
             statement = self._create_select_statement(proj_name, namespace, tag)
+
             with Session(self._sa_engine) as session:
                 found_prj = session.scalars(statement).one()
 
                 if found_prj:
                     _LOGGER.debug(
                         f"Project has been found: {found_prj.namespace}, {found_prj.name}"
                     )
 
                     found_prj.digest = project_digest
                     found_prj.number_of_samples = number_of_samples
                     found_prj.private = private
                     found_prj.pep_schema = pep_schema
+                    found_prj.last_update_date = datetime.datetime.now(datetime.timezone.utc)
+                    found_prj.description = project_dict[CONFIG_KEY].get("description")
 
                     # Deleting old samples and subsamples
                     if found_prj.samples_mapping:
                         for sample in found_prj.samples_mapping:
                             _LOGGER.info(f"deleting samples: {str(sample)}")
                             session.delete(sample)
```

### Comparing `pepdbagent-0.5.1/pepdbagent/pepdbagent.py` & `pepdbagent-0.5.2/pepdbagent/pepdbagent.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/pepdbagent/utils.py` & `pepdbagent-0.5.2/pepdbagent/utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/pepdbagent.egg-info/PKG-INFO` & `pepdbagent-0.5.2/pepdbagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.5.1
+Version: 0.5.2
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.5.1/pepdbagent.egg-info/SOURCES.txt` & `pepdbagent-0.5.2/pepdbagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/setup.py` & `pepdbagent-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/tests/conftest.py` & `pepdbagent-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.1/tests/test_pepagent.py` & `pepdbagent-0.5.2/tests/test_pepagent.py`

 * *Files identical despite different names*

