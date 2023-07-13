# Comparing `tmp/foursight-3.5.0.2b9.tar.gz` & `tmp/foursight-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.5.0.2b9.tar", max compression
+gzip compressed data, was "foursight-3.5.2.tar", max compression
```

## Comparing `foursight-3.5.0.2b9.tar` & `foursight-3.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.5.0.2b9/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.5.0.2b9/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.5.0.2b9/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.5.0.2b9/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    54860 2023-07-07 22:27:54.136755 foursight-3.5.0.2b9/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.5.0.2b9/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    62768 2023-07-07 22:27:54.137645 foursight-3.5.0.2b9/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.5.0.2b9/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.5.0.2b9/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.5.0.2b9/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.5.0.2b9/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    15663 2023-06-09 17:46:33.623749 foursight-3.5.0.2b9/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.5.0.2b9/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.5.0.2b9/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.5.0.2b9/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.5.0.2b9/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.5.0.2b9/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137844 2023-07-07 22:27:48.841661 foursight-3.5.0.2b9/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.5.0.2b9/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.5.0.2b9/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1322 2023-07-13 21:23:28.500882 foursight-3.5.0.2b9/pyproject.toml
--rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 foursight-3.5.0.2b9/setup.py
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 foursight-3.5.0.2b9/PKG-INFO
+-rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-3.5.2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-3.5.2/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1055 2023-01-19 17:19:39.269034 foursight-3.5.2/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-3.5.2/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54860 2023-06-21 14:22:50.333640 foursight-3.5.2/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-3.5.2/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    62768 2023-06-21 14:22:50.335968 foursight-3.5.2/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37766 2023-01-19 17:19:39.271725 foursight-3.5.2/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-3.5.2/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-3.5.2/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-3.5.2/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-3.5.2/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-3.5.2/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2022-11-16 16:53:13.427051 foursight-3.5.2/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 17:19:30.850214 foursight-3.5.2/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2022-11-16 16:53:13.428402 foursight-3.5.2/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-3.5.2/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 17:19:39.276361 foursight-3.5.2/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-3.5.2/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45209 2023-04-19 19:52:24.091978 foursight-3.5.2/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   128320 2023-07-11 18:30:23.521392 foursight-3.5.2/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 17:19:39.282546 foursight-3.5.2/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137844 2023-05-23 18:05:48.756394 foursight-3.5.2/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-3.5.2/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-3.5.2/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1259 2023-07-11 18:30:23.521976 foursight-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 foursight-3.5.2/setup.py
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 foursight-3.5.2/PKG-INFO
```

### Comparing `foursight-3.5.0.2b9/LICENSE.txt` & `foursight-3.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/app_utils.py` & `foursight-3.5.2/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/check_schedules.py` & `foursight-3.5.2/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/check_setup.json` & `foursight-3.5.2/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.5.2/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.5.2/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.5.2/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.5.2/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,16 @@
     # check indexing queue
     check, skip = wfr_utils.check_indexing(check, connection)
     if skip:
         return check
     # check number of total workflow runs in the past 6h
     check, n_runs_available = wfr_utils.limit_number_of_runs(check, my_auth)
     if n_runs_available == 0:
+        check.brief_output.append('Runs are limited due to docker pull rate limit')
+        check.status = 'WARN'
         return check
 
     # Build the query
     query = '/search/?status=uploading&status=upload failed&status!=archived&status!=archived to project'
     # add file type
     f_type = kwargs.get('file_type')
     query += '&type=' + f_type
@@ -315,14 +317,16 @@
     # check indexing queue
     check, skip = wfr_utils.check_indexing(check, connection)
     if skip:
         return check
     # check number of total workflow runs in the past 6h
     check, n_runs_available = wfr_utils.limit_number_of_runs(check, my_auth)
     if n_runs_available == 0:
+        check.brief_output.append('Runs are limited due to docker pull rate limit')
+        check.status = 'WARN'
         return check
 
     # Build the query (skip to be uploaded by workflow)
     query = ("/search/?type=File&file_format.file_format=fastq&quality_metric.uuid=No+value"
              "&status=pre-release&status=released&status=released%20to%20project&status=uploaded")
     # fastqc not properly reporting for long reads
     skip_instruments = ['PromethION', 'GridION', 'MinION', 'PacBio RS II']
@@ -2084,14 +2088,16 @@
     # check indexing queue
     check, skip = wfr_utils.check_indexing(check, connection)
     if skip:
         return check
     # check number of total workflow runs in the past 6h
     check, n_runs_available = wfr_utils.limit_number_of_runs(check, my_auth)
     if n_runs_available == 0:
+        check.brief_output.append('Runs are limited due to docker pull rate limit')
+        check.status = 'WARN'
         return check
 
     query = ('/search/?status=uploaded&status=pre-release&status=released+to+project&status=released'
              '&type=FileFastq&file_format.file_format=fastq&file_first_line=No value&status=restricted')
 
     # The search
     print('About to query ES for files')
```

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.5.2/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dcicutils import ff_utils
 from dcicutils.env_utils import prod_bucket_env_for_app
-import boto3
 import re
 import requests
 import json
 import datetime
 import time
 import itertools
 import random
 from difflib import SequenceMatcher
+import boto3
 from .helpers import wrangler_utils
 from collections import Counter
 from oauth2client.service_account import ServiceAccountCredentials
 import gspread
 import pandas as pd
 from collections import OrderedDict
 import uuid
```

### Comparing `foursight-3.5.0.2b9/chalicelib_fourfront/package.py` & `foursight-3.5.2/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.2b9/pyproject.toml` & `foursight-3.5.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [tool.poetry]
 name = "foursight"
-version = "3.5.0.2b9"
+version = "3.5.2"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-#dcicutils = "^7.5.1"
-dcicutils = "7.6.0.1b4"
+dcicutils = "^7.5.0"
 click = "^7.1.2"
 PyJWT = "^2.5.0"
 Jinja2 = "2.10.1"
 MarkupSafe = "1.1.1"
 google-api-python-client = "^1.7.4"
 geocoder = "1.38.1"
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 tibanna_ff = ">=0.22.5"
 ## adding foursight-core
 # use below for deployment
-#foursight-core = "4.3.0.2b6"
-foursight-core = "4.3.0.1b54"
+foursight-core = "^4.3.0"
 # use below for tests but not for deployment
 # foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="master" }
 pytest = "5.1.2"
 gspread = ">=3.6.0"
 oauth2client = ">=4.1.3"
 pandas = ">=1.1.4"
```

### Comparing `foursight-3.5.0.2b9/setup.py` & `foursight-3.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 {'': ['*']}
 
 install_requires = \
 ['Jinja2==2.10.1',
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'click>=7.1.2,<8.0.0',
- 'dcicutils==7.6.0.1b4',
+ 'dcicutils>=7.5.0,<8.0.0',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
- 'foursight-core==4.3.0.1b54',
+ 'foursight-core>=4.3.0,<5.0.0',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.7.4,<2.0.0',
  'gspread>=3.6.0',
  'oauth2client>=4.1.3',
  'pandas>=1.1.4',
  'pytest==5.1.2',
@@ -34,15 +34,15 @@
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight',
-    'version': '3.5.0.2b9',
+    'version': '3.5.2',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight-3.5.0.2b9/PKG-INFO` & `foursight-3.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.5.0.2b9
+Version: 3.5.2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: dcicutils (==7.6.0.1b4)
+Requires-Dist: dcicutils (>=7.5.0,<8.0.0)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.3.0.1b54)
+Requires-Dist: foursight-core (>=4.3.0,<5.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.7.4,<2.0.0)
 Requires-Dist: gspread (>=3.6.0)
 Requires-Dist: oauth2client (>=4.1.3)
 Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: pytest (==5.1.2)
```

