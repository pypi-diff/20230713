# Comparing `tmp/pytest-testmon-2.0.8.tar.gz` & `tmp/pytest-testmon-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-testmon-2.0.8.tar", last modified: Thu May 18 06:49:44 2023, max compression
+gzip compressed data, was "pytest-testmon-2.0.9.tar", last modified: Fri Jun  9 10:56:34 2023, max compression
```

## Comparing `pytest-testmon-2.0.8.tar` & `pytest-testmon-2.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-18 06:49:44.223853 pytest-testmon-2.0.8/
--rw-r--r--   0 tibor      (502) staff       (20)    34633 2023-01-17 15:34:55.000000 pytest-testmon-2.0.8/LICENSE
--rw-r--r--   0 tibor      (502) staff       (20)       74 2023-05-02 14:55:45.000000 pytest-testmon-2.0.8/MANIFEST.in
--rw-r--r--   0 tibor      (502) staff       (20)     2429 2023-05-18 06:49:44.223936 pytest-testmon-2.0.8/PKG-INFO
--rw-r--r--   0 tibor      (502) staff       (20)     1208 2023-05-02 14:55:45.000000 pytest-testmon-2.0.8/README.md
--rw-r--r--   0 tibor      (502) staff       (20)     1619 2023-05-18 06:49:21.000000 pytest-testmon-2.0.8/pyproject.toml
-drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-18 06:49:44.221526 pytest-testmon-2.0.8/pytest_testmon.egg-info/
--rw-r--r--   0 tibor      (502) staff       (20)     2429 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/PKG-INFO
--rw-r--r--   0 tibor      (502) staff       (20)      463 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/SOURCES.txt
--rw-r--r--   0 tibor      (502) staff       (20)        1 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/dependency_links.txt
--rw-r--r--   0 tibor      (502) staff       (20)       51 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/entry_points.txt
--rw-r--r--   0 tibor      (502) staff       (20)       28 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/requires.txt
--rw-r--r--   0 tibor      (502) staff       (20)        8 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/top_level.txt
--rw-r--r--   0 tibor      (502) staff       (20)     1219 2023-05-18 06:49:44.224236 pytest-testmon-2.0.8/setup.cfg
--rw-r--r--   0 tibor      (502) staff       (20)       69 2023-05-18 06:49:21.000000 pytest-testmon-2.0.8/setup.py
-drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-18 06:49:44.223487 pytest-testmon-2.0.8/testmon/
--rw-r--r--   0 tibor      (502) staff       (20)       44 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/__init__.py
--rw-r--r--   0 tibor      (502) staff       (20)     2149 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/common.py
--rw-r--r--   0 tibor      (502) staff       (20)     3786 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/configure.py
--rw-r--r--   0 tibor      (502) staff       (20)    22743 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/db.py
--rw-r--r--   0 tibor      (502) staff       (20)     8052 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/process_code.py
--rw-r--r--   0 tibor      (502) staff       (20)    16979 2023-05-18 06:49:21.000000 pytest-testmon-2.0.8/testmon/pytest_testmon.py
--rw-r--r--   0 tibor      (502) staff       (20)    19133 2023-05-18 06:49:21.000000 pytest-testmon-2.0.8/testmon/testmon_core.py
--rw-r--r--   0 tibor      (502) staff       (20)     1232 2023-01-18 05:16:27.000000 pytest-testmon-2.0.8/testmon/tox_testmon.py
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-06-09 10:56:34.522885 pytest-testmon-2.0.9/
+-rw-r--r--   0 tibor      (502) staff       (20)    34633 2023-01-17 15:34:55.000000 pytest-testmon-2.0.9/LICENSE
+-rw-r--r--   0 tibor      (502) staff       (20)       74 2023-05-02 14:55:45.000000 pytest-testmon-2.0.9/MANIFEST.in
+-rw-r--r--   0 tibor      (502) staff       (20)     2429 2023-06-09 10:56:34.522946 pytest-testmon-2.0.9/PKG-INFO
+-rw-r--r--   0 tibor      (502) staff       (20)     1208 2023-05-02 14:55:45.000000 pytest-testmon-2.0.9/README.md
+-rw-r--r--   0 tibor      (502) staff       (20)     1619 2023-06-09 10:44:58.000000 pytest-testmon-2.0.9/pyproject.toml
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-06-09 10:56:34.520551 pytest-testmon-2.0.9/pytest_testmon.egg-info/
+-rw-r--r--   0 tibor      (502) staff       (20)     2429 2023-06-09 10:56:34.000000 pytest-testmon-2.0.9/pytest_testmon.egg-info/PKG-INFO
+-rw-r--r--   0 tibor      (502) staff       (20)      463 2023-06-09 10:56:34.000000 pytest-testmon-2.0.9/pytest_testmon.egg-info/SOURCES.txt
+-rw-r--r--   0 tibor      (502) staff       (20)        1 2023-06-09 10:56:34.000000 pytest-testmon-2.0.9/pytest_testmon.egg-info/dependency_links.txt
+-rw-r--r--   0 tibor      (502) staff       (20)       51 2023-06-09 10:56:34.000000 pytest-testmon-2.0.9/pytest_testmon.egg-info/entry_points.txt
+-rw-r--r--   0 tibor      (502) staff       (20)       28 2023-06-09 10:56:34.000000 pytest-testmon-2.0.9/pytest_testmon.egg-info/requires.txt
+-rw-r--r--   0 tibor      (502) staff       (20)        8 2023-06-09 10:56:34.000000 pytest-testmon-2.0.9/pytest_testmon.egg-info/top_level.txt
+-rw-r--r--   0 tibor      (502) staff       (20)     1219 2023-06-09 10:56:34.523205 pytest-testmon-2.0.9/setup.cfg
+-rw-r--r--   0 tibor      (502) staff       (20)       69 2023-06-09 10:44:58.000000 pytest-testmon-2.0.9/setup.py
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-06-09 10:56:34.522279 pytest-testmon-2.0.9/testmon/
+-rw-r--r--   0 tibor      (502) staff       (20)       44 2023-06-09 10:44:59.000000 pytest-testmon-2.0.9/testmon/__init__.py
+-rw-r--r--   0 tibor      (502) staff       (20)     2313 2023-06-09 10:46:44.000000 pytest-testmon-2.0.9/testmon/common.py
+-rw-r--r--   0 tibor      (502) staff       (20)     3786 2023-06-09 10:44:59.000000 pytest-testmon-2.0.9/testmon/configure.py
+-rw-r--r--   0 tibor      (502) staff       (20)    22648 2023-06-09 10:44:59.000000 pytest-testmon-2.0.9/testmon/db.py
+-rw-r--r--   0 tibor      (502) staff       (20)     8052 2023-06-09 10:44:58.000000 pytest-testmon-2.0.9/testmon/process_code.py
+-rw-r--r--   0 tibor      (502) staff       (20)    17423 2023-06-09 10:44:58.000000 pytest-testmon-2.0.9/testmon/pytest_testmon.py
+-rw-r--r--   0 tibor      (502) staff       (20)    19133 2023-06-09 10:44:58.000000 pytest-testmon-2.0.9/testmon/testmon_core.py
+-rw-r--r--   0 tibor      (502) staff       (20)     1232 2023-01-18 05:16:27.000000 pytest-testmon-2.0.9/testmon/tox_testmon.py
```

### Comparing `pytest-testmon-2.0.8/LICENSE` & `pytest-testmon-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.8/PKG-INFO` & `pytest-testmon-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testmon
-Version: 2.0.8
+Version: 2.0.9
 Summary: selects tests affected by changed files and methods
 Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic
 Author-email: Tibor Arpas <tibor@testmon.org>
 License: AGPL
 Project-URL: Source, https://github.com/tarpas/pytest-testmon
 Keywords: testing,pytest,plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.8 Summary: selects
+Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.9 Summary: selects
 tests affected by changed files and methods Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic Author-email: Tibor Arpas
 testmon.org> License: AGPL Project-URL: Source, https://github.com/tarpas/
 pytest-testmon Keywords: testing,pytest,plugin Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
```

### Comparing `pytest-testmon-2.0.8/README.md` & `pytest-testmon-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.8/pyproject.toml` & `pytest-testmon-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.8/pytest_testmon.egg-info/PKG-INFO` & `pytest-testmon-2.0.9/pytest_testmon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testmon
-Version: 2.0.8
+Version: 2.0.9
 Summary: selects tests affected by changed files and methods
 Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic
 Author-email: Tibor Arpas <tibor@testmon.org>
 License: AGPL
 Project-URL: Source, https://github.com/tarpas/pytest-testmon
 Keywords: testing,pytest,plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.8 Summary: selects
+Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.9 Summary: selects
 tests affected by changed files and methods Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic Author-email: Tibor Arpas
 testmon.org> License: AGPL Project-URL: Source, https://github.com/tarpas/
 pytest-testmon Keywords: testing,pytest,plugin Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
```

### Comparing `pytest-testmon-2.0.8/setup.cfg` & `pytest-testmon-2.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.8/testmon/common.py` & `pytest-testmon-2.0.9/testmon/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 import re
 
 try:
     import importlib.metadata
 
     def get_system_packages_raw():
         return (
-            f"{pkg.metadata['Name']} {pkg.version}"
+            (pkg.metadata["Name"], pkg.version)
             for pkg in importlib.metadata.distributions()
         )
 
 except ImportError:
     import pkg_resources
 
     def get_system_packages_raw():
-        return (
-            f"{pkg.project_name} {pkg.version}" for pkg in pkg_resources.working_set
-        )
+        return ((pkg.project_name, pkg.version) for pkg in pkg_resources.working_set)
 
 
 from pathlib import Path
 
 
 def dummy():
     pass
@@ -31,16 +29,24 @@
     logging.basicConfig(format="%(levelname)s: %(message)s.", level=logging.WARNING)
     return logging.getLogger(name)
 
 
 logger = get_logger(__name__)
 
 
-def get_system_packages():
-    return ", ".join(sorted(set(get_system_packages_raw())))
+def get_system_packages(ignore=None):
+    return ", ".join(
+        sorted(
+            {
+                f"{package} {version}"
+                for (package, version) in get_system_packages_raw()
+                if not ignore or not package in ignore
+            }
+        )
+    )
 
 
 def drop_patch_version(system_packages):
     return re.sub(
         r"\b([\w_-]+\s\d+\.\d+)\.\w+\b",
         r"\1",
         system_packages,
```

### Comparing `pytest-testmon-2.0.8/testmon/configure.py` & `pytest-testmon-2.0.9/testmon/configure.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.8/testmon/db.py` & `pytest-testmon-2.0.9/testmon/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,22 +87,22 @@
                 "UPDATE file_fp SET mtime=?, fsha=? WHERE id = ?", new_mtimes
             )
 
     def finish_execution(self, exec_id, duration=None, select=True):
         self.update_saving_stats(exec_id, select)
         self.fetch_or_create_file_fp.cache_clear()
         with self.con as con:
-            con.execute(
-                """
-                DELETE FROM file_fp
+            self.vacuum_file_fp(con)
+
+    def vacuum_file_fp(self, con):
+        con.execute(
+            """ DELETE FROM file_fp
                 WHERE id NOT IN (
-                    SELECT DISTINCT fingerprint_id FROM test_execution_file_fp
-                )
-                """
-            )
+                    SELECT DISTINCT fingerprint_id FROM test_execution_file_fp) """
+        )
 
     def fetch_current_run_stats(self, exec_id):
         with self.con as con:
             cursor = con.cursor()
             run_saved_tests, run_saved_time = cursor.execute(
                 f"""
                     SELECT count(*), sum(te.duration) FROM test_execution te
@@ -267,24 +267,21 @@
                         record["filename"],
                         record["fsha"],
                         checksums_to_blob(record["method_checksums"]),
                     )
 
                     test_execution_file_fps.append((te_id, fingerprint_id))
                     files_fshas.add((record["filename"], record["fsha"]))
-            cursor.executemany(
-                "INSERT INTO test_execution_file_fp VALUES (?, ?)",
-                test_execution_file_fps,
-            )
-            self.fetch_or_create_file_fp.cache_clear()
-            cursor.execute(
-                "DELETE FROM file_fp WHERE "
-                "    id NOT IN (select fingerprint_id from test_execution_file_fp)"
-            )
-            self.insert_into_suite_files_fshas(con, exec_id, files_fshas)
+            if test_execution_file_fps:
+                cursor.executemany(
+                    "INSERT INTO test_execution_file_fp VALUES (?, ?)",
+                    test_execution_file_fps,
+                )
+                self.fetch_or_create_file_fp.cache_clear()
+                self.insert_into_suite_files_fshas(con, exec_id, files_fshas)
 
     def insert_into_suite_files_fshas(self, con, exec_id, files_fshas):
         pass
 
     def _fetch_data_version(self):
         con = self.con
```

### Comparing `pytest-testmon-2.0.8/testmon/process_code.py` & `pytest-testmon-2.0.9/testmon/process_code.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.8/testmon/pytest_testmon.py` & `pytest-testmon-2.0.9/testmon/pytest_testmon.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,15 +107,16 @@
         dest="tmnet",
         help=(
             "This is used for internal beta. Please don't use. You can go to https://www.testmon.net/ to register."
         ),
     )
 
     parser.addini("environment_expression", "environment expression", default="")
-    parser.addini("testmon_url", "URL of the testmon.net api server.")
+    parser.addini("testmon_ignore_dependencies", "ignore dependencies", default=[])
+    parser.addini("tmnet_url", "URL of the testmon.net api server.")
     parser.addini("tmnet_api_key", "testmon api key")
 
 
 def testmon_options(config):
     result = []
     for label in [
         "testmon",
@@ -127,17 +128,25 @@
     return result
 
 
 def init_testmon_data(config):
     environment = config.getoption("environment_expression") or eval_environment(
         config.getini("environment_expression")
     )
-    system_packages = get_system_packages()
+    ignore_dependencies_arg = config.getini("testmon_ignore_dependencies")
+    if type(ignore_dependencies_arg) in (list, tuple):
+        ignore_dependencies = ignore_dependencies_arg
+    elif "\n" in ignore_dependencies_arg:
+        ignore_dependencies = ignore_dependencies_arg.split("\n")
+    else:
+        ignore_dependencies = None
 
-    url = config.getini("testmon_url")
+    system_packages = get_system_packages(ignore=ignore_dependencies)
+
+    url = config.getini("tmnet_url")
     rpc_proxy = None
 
     if config.testmon_config.tmnet or getattr(config, "tmnet", None):
         rpc_proxy = getattr(config, "tmnet", None)
 
         if not url:
             url = "https://api1.testmon.net/"
```

### Comparing `pytest-testmon-2.0.8/testmon/testmon_core.py` & `pytest-testmon-2.0.9/testmon/testmon_core.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.8/testmon/tox_testmon.py` & `pytest-testmon-2.0.9/testmon/tox_testmon.py`

 * *Files identical despite different names*

