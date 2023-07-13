# Comparing `tmp/odd_dbt-0.1.8.tar.gz` & `tmp/odd_dbt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odd_dbt-0.1.8.tar", max compression
+gzip compressed data, was "odd_dbt-0.1.9.tar", max compression
```

## Comparing `odd_dbt-0.1.8.tar` & `odd_dbt-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/LICENSE
--rw-r--r--   0        0        0     1709 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/__init__.py
--rw-r--r--   0        0        0     1990 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/app.py
--rw-r--r--   0        0        0     2181 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/context.py
--rw-r--r--   0        0        0      155 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/errors.py
--rw-r--r--   0        0        0        0 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/mapper/__init__.py
--rw-r--r--   0        0        0     1585 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/mapper/data_source.py
--rw-r--r--   0        0        0     4251 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/mapper/dbt_test.py
--rw-r--r--   0        0        0     1242 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/mapper/status_reason.py
--rw-r--r--   0        0        0      152 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/models/__init__.py
--rw-r--r--   0        0        0      240 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/models/manifest.py
--rw-r--r--   0        0        0      704 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/models/profile.py
--rw-r--r--   0        0        0      764 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/models/project.py
--rw-r--r--   0        0        0      607 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/models/result.py
--rw-r--r--   0        0        0      591 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/models/run_results.py
--rw-r--r--   0        0        0      283 2023-03-13 07:45:47.000000 odd_dbt-0.1.8/odd_dbt/utils/__init__.py
--rw-r--r--   0        0        0      940 2023-03-13 07:46:04.000000 odd_dbt-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 odd_dbt-0.1.8/setup.py
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 odd_dbt-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1709 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/__init__.py
+-rw-r--r--   0        0        0     1990 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/app.py
+-rw-r--r--   0        0        0     2181 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/context.py
+-rw-r--r--   0        0        0      155 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/errors.py
+-rw-r--r--   0        0        0        0 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/mapper/__init__.py
+-rw-r--r--   0        0        0     1585 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/mapper/data_source.py
+-rw-r--r--   0        0        0     4251 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/mapper/dbt_test.py
+-rw-r--r--   0        0        0     1242 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/mapper/status_reason.py
+-rw-r--r--   0        0        0      152 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/models/__init__.py
+-rw-r--r--   0        0        0      240 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/models/manifest.py
+-rw-r--r--   0        0        0      704 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/models/profile.py
+-rw-r--r--   0        0        0      764 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/models/project.py
+-rw-r--r--   0        0        0      607 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/models/result.py
+-rw-r--r--   0        0        0      591 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/models/run_results.py
+-rw-r--r--   0        0        0      283 2023-03-13 08:28:28.000000 odd_dbt-0.1.9/odd_dbt/utils/__init__.py
+-rw-r--r--   0        0        0      904 2023-03-13 08:28:48.000000 odd_dbt-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 odd_dbt-0.1.9/setup.py
+-rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 odd_dbt-0.1.9/PKG-INFO
```

### Comparing `odd_dbt-0.1.8/LICENSE` & `odd_dbt-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/README.md` & `odd_dbt-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/app.py` & `odd_dbt-0.1.9/odd_dbt/app.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/context.py` & `odd_dbt-0.1.9/odd_dbt/context.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/mapper/data_source.py` & `odd_dbt-0.1.9/odd_dbt/mapper/data_source.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/mapper/dbt_test.py` & `odd_dbt-0.1.9/odd_dbt/mapper/dbt_test.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/mapper/status_reason.py` & `odd_dbt-0.1.9/odd_dbt/mapper/status_reason.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/models/profile.py` & `odd_dbt-0.1.9/odd_dbt/models/profile.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/models/project.py` & `odd_dbt-0.1.9/odd_dbt/models/project.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/models/result.py` & `odd_dbt-0.1.9/odd_dbt/models/result.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/odd_dbt/models/run_results.py` & `odd_dbt-0.1.9/odd_dbt/models/run_results.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.1.8/pyproject.toml` & `odd_dbt-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odd-dbt"
-version = "0.1.8"
+version = "0.1.9"
 description = "OpenDataDiscovery Action for dbt"
 authors = ["Mateusz Kulas <mkulas@provectus.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ['Open Data Discovery', 'dbt', "Metadata", "Data Discovery", "Data Observability"]
 packages = [{include = "odd_dbt"}]
 
@@ -17,15 +17,14 @@
 oddrn-generator = "^0.1.70"
 funcy = "^1.17"
 sqlalchemy = "^1.4.46"
 psycopg2 = "^2.9.5"
 loguru = "^0.6.0"
 typer = {extras = ["all"], version = "^0.7.0"}
 dbt-snowflake = "^1.4.1"
-snowflake-connector-python = "^2.8"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 pre-commit = "^3.1.0"
 
 [build-system]
```

### Comparing `odd_dbt-0.1.8/setup.py` & `odd_dbt-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,23 @@
  'dbt-redshift>=1.4.0,<2.0.0',
  'dbt-snowflake>=1.4.1,<2.0.0',
  'funcy>=1.17,<2.0',
  'loguru>=0.6.0,<0.7.0',
  'odd-models>=2.0.23,<3.0.0',
  'oddrn-generator>=0.1.70,<0.2.0',
  'psycopg2>=2.9.5,<3.0.0',
- 'snowflake-connector-python>=2.8,<3.0',
  'sqlalchemy>=1.4.46,<2.0.0',
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['odd_dbt_test = odd_dbt.app:app']}
 
 setup_kwargs = {
     'name': 'odd-dbt',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'OpenDataDiscovery Action for dbt',
     'long_description': '# OpenDataDiscovery dbt tests metadata collecting\n[![PyPI version](https://badge.fury.io/py/odd-dbt.svg)](https://badge.fury.io/py/odd-dbt)\n\nLibrary used for running dbt tests and injecting them as entities to ODD platform. \n\n## Supported data sources\n| Source    |\n|-----------| \n| Snowflake | \n| Redshift  |\n| Postgres  |\n\n## Requirements\nLibrary to inject Quality Tests entities requires presence of corresponding with them datasets entities in the platform.  \nFor example: if you want to inject data quality test of Snowflake table, you need to have entity of that table present in the platform.\n\n## Supported tests\nLibrary supports for basics tests provided by dbt. \n- `unique`: values in the column should be unique\n- `not_null`: values in the column should not contain null values\n- `accepted_values`: column should only contain values from list specified in the test config\n- `relationships`: each value in the select column of the model exists as a specified field in the reference table (also known as referential integrity)\n\n## ODDRN generation for datasets\nhost_settings of ODDRN generators required for source datasets are loaded from `.dbt/profiles.yml`.  \nProfiles inside the file looks different for each type of data source.  \n**Snowflake** host_settings value is created from field `account`. Field value should be `<account_identifier>`  \nFor example the URL for an account uses the following format: `<account_identifier>`.snowflakecomputing.com  \nExample Snowflake account identifier `hj1234.eu-central-1`.  \n**Redshift** and **Postgres** host_settings are loaded from field `host` field.  \nExample Redshift host: `redshift-cluster-example.123456789.eu-central-1.redshift.amazonaws.com`  ',
     'author': 'Mateusz Kulas',
     'author_email': 'mkulas@provectus.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `odd_dbt-0.1.8/PKG-INFO` & `odd_dbt-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odd-dbt
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenDataDiscovery Action for dbt
 License: Apache-2.0
 Keywords: Open Data Discovery,dbt,Metadata,Data Discovery,Data Observability
 Author: Mateusz Kulas
 Author-email: mkulas@provectus.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,15 +17,14 @@
 Requires-Dist: dbt-redshift (>=1.4.0,<2.0.0)
 Requires-Dist: dbt-snowflake (>=1.4.1,<2.0.0)
 Requires-Dist: funcy (>=1.17,<2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: odd-models (>=2.0.23,<3.0.0)
 Requires-Dist: oddrn-generator (>=0.1.70,<0.2.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
-Requires-Dist: snowflake-connector-python (>=2.8,<3.0)
 Requires-Dist: sqlalchemy (>=1.4.46,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # OpenDataDiscovery dbt tests metadata collecting
 [![PyPI version](https://badge.fury.io/py/odd-dbt.svg)](https://badge.fury.io/py/odd-dbt)
```

