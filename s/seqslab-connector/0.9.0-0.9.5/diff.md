# Comparing `tmp/seqslab-connector-0.9.0.tar.gz` & `tmp/seqslab-connector-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslab-connector-0.9.0.tar", last modified: Fri May 26 08:12:52 2023, max compression
+gzip compressed data, was "seqslab-connector-0.9.5.tar", last modified: Thu Jul 13 09:32:27 2023, max compression
```

## Comparing `seqslab-connector-0.9.0.tar` & `seqslab-connector-0.9.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.834075 seqslab-connector-0.9.0/seqslab/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/hive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/seqslab/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/sqlalchemy/hive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/seqslab/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/seqslab/superset/seqslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/seqslab_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 08:12:52.000000 seqslab-connector-0.9.0/seqslab_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-26 08:12:52.838075 seqslab-connector-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-26 08:12:37.000000 seqslab-connector-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:27.322686 seqslab-connector-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-13 09:32:27.322686 seqslab-connector-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:27.318686 seqslab-connector-0.9.5/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/seqslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/seqslab/hive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:27.318686 seqslab-connector-0.9.5/seqslab/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/seqslab/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/seqslab/sqlalchemy/hive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:27.322686 seqslab-connector-0.9.5/seqslab/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/seqslab/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/seqslab/superset/seqslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:27.322686 seqslab-connector-0.9.5/seqslab_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-13 09:32:27.000000 seqslab-connector-0.9.5/seqslab_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 09:32:27.000000 seqslab-connector-0.9.5/seqslab_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:32:27.000000 seqslab-connector-0.9.5/seqslab_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 09:32:27.000000 seqslab-connector-0.9.5/seqslab_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-13 09:32:27.000000 seqslab-connector-0.9.5/seqslab_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 09:32:27.000000 seqslab-connector-0.9.5/seqslab_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-13 09:32:27.322686 seqslab-connector-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-13 09:32:14.000000 seqslab-connector-0.9.5/setup.py
```

### Comparing `seqslab-connector-0.9.0/LICENSE` & `seqslab-connector-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslab-connector-0.9.0/PKG-INFO` & `seqslab-connector-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-connector
-Version: 0.9.0
+Version: 0.9.5
 Summary: Atgenomix SeqsLab Connector for Python
 Home-page: https://github.com/atgenomix/seqslab-connector
 Author: Allen Chang
 Author-email: allen.chang@atgenomix.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-connector
```

### Comparing `seqslab-connector-0.9.0/README.md` & `seqslab-connector-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `seqslab-connector-0.9.0/seqslab/hive.py` & `seqslab-connector-0.9.5/seqslab/hive.py`

 * *Files identical despite different names*

### Comparing `seqslab-connector-0.9.0/seqslab/sqlalchemy/hive.py` & `seqslab-connector-0.9.5/seqslab/sqlalchemy/hive.py`

 * *Files identical despite different names*

### Comparing `seqslab-connector-0.9.0/seqslab/superset/seqslab.py` & `seqslab-connector-0.9.5/seqslab/superset/seqslab.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """
 Superset db engine specs for SeqsLab
 """
-
+from superset.db_engine_specs import BaseEngineSpec
 from superset.db_engine_specs.hive import HiveEngineSpec
+from superset.exceptions import SupersetException
+from superset import sql_parse
 
 
 class SeqsLabHiveEngineSpec(HiveEngineSpec):
     engine_name = "Atgenomix SeqsLab Interactive Job"
 
     engine = "seqslab"
     drivers = {"hive": "Hive driver for interactive job"}
@@ -40,7 +42,15 @@
         "P1W": "date_trunc('week', {col})",
         "P1M": "date_trunc('month', {col})",
         "P3M": "date_trunc('quarter', {col})",
         "P1Y": "date_trunc('year', {col})",
         "P1W/1970-01-03T00:00:00Z": "date_trunc('week', {col} + interval '1 day') + interval '5 days'",
         "1969-12-28T00:00:00Z/P1W": "date_trunc('week', {col} + interval '1 day') - interval '1 day'",
     }
+
+    @staticmethod
+    def execute(  # type: ignore
+        cursor, query: str, **kwargs
+    ):  # pylint: disable=arguments-differ
+        if not BaseEngineSpec.is_readonly_query(sql_parse.ParsedQuery(query)):
+            raise SupersetException("DML operation is currently not supported")
+        HiveEngineSpec.execute(cursor, query, **kwargs)
```

### Comparing `seqslab-connector-0.9.0/seqslab_connector.egg-info/PKG-INFO` & `seqslab-connector-0.9.5/seqslab_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-connector
-Version: 0.9.0
+Version: 0.9.5
 Summary: Atgenomix SeqsLab Connector for Python
 Home-page: https://github.com/atgenomix/seqslab-connector
 Author: Allen Chang
 Author-email: allen.chang@atgenomix.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-connector
```

### Comparing `seqslab-connector-0.9.0/setup.py` & `seqslab-connector-0.9.5/setup.py`

 * *Files identical despite different names*

