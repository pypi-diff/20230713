# Comparing `tmp/chartreuse-4.3.2.tar.gz` & `tmp/chartreuse-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartreuse-4.3.2.tar", last modified: Mon Jul  3 06:48:47 2023, max compression
+gzip compressed data, was "chartreuse-4.3.3.tar", last modified: Thu Jul 13 10:13:15 2023, max compression
```

## Comparing `chartreuse-4.3.2.tar` & `chartreuse-4.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-03 06:48:37.000000 chartreuse-4.3.2/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 06:48:37.000000 chartreuse-4.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 06:48:47.191141 chartreuse-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-03 06:48:37.000000 chartreuse-4.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 06:48:37.000000 chartreuse-4.3.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 06:48:37.000000 chartreuse-4.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 06:48:47.195141 chartreuse-4.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-03 06:48:37.000000 chartreuse-4.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/src/chartreuse/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/chartreuse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4101 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/chartreuse_upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/src/chartreuse/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6307 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/utils/alembic_migration_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/src/chartreuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:13:15.788343 chartreuse-4.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-13 10:13:05.000000 chartreuse-4.3.3/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 10:13:05.000000 chartreuse-4.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 10:13:15.788343 chartreuse-4.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-13 10:13:05.000000 chartreuse-4.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 10:13:05.000000 chartreuse-4.3.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-13 10:13:05.000000 chartreuse-4.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-13 10:13:15.788343 chartreuse-4.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-13 10:13:05.000000 chartreuse-4.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:13:15.784343 chartreuse-4.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:13:15.788343 chartreuse-4.3.3/src/chartreuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 10:13:05.000000 chartreuse-4.3.3/src/chartreuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-13 10:13:05.000000 chartreuse-4.3.3/src/chartreuse/chartreuse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4101 2023-07-13 10:13:05.000000 chartreuse-4.3.3/src/chartreuse/chartreuse_upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:13:15.788343 chartreuse-4.3.3/src/chartreuse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-13 10:13:05.000000 chartreuse-4.3.3/src/chartreuse/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6393 2023-07-13 10:13:05.000000 chartreuse-4.3.3/src/chartreuse/utils/alembic_migration_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:13:15.788343 chartreuse-4.3.3/src/chartreuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 10:13:15.000000 chartreuse-4.3.3/src/chartreuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-13 10:13:15.000000 chartreuse-4.3.3/src/chartreuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:13:15.000000 chartreuse-4.3.3/src/chartreuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-13 10:13:15.000000 chartreuse-4.3.3/src/chartreuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-13 10:13:15.000000 chartreuse-4.3.3/src/chartreuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 10:13:15.000000 chartreuse-4.3.3/src/chartreuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:13:15.000000 chartreuse-4.3.3/src/chartreuse.egg-info/zip-safe
```

### Comparing `chartreuse-4.3.2/LICENCE.md` & `chartreuse-4.3.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.2/README.md` & `chartreuse-4.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
       ...
       patroni_postgresql: bool = "patroni_postgresql" in context.get_x_argument(as_dictionary=True)
         ...
         with connectable.connect() as connection:
           ...
           with context.begin_transaction():
             if patroni_postgresql:
-              context.execute("SET ROLE wiremind_owner")
+              context.execute(text("SET ROLE wiremind_owner"))
             context.run_migrations()
        ...
       ```
 2. Chartreuse in pre-upgrade mode:
     - When running Chartreuse in pre-upgrade mode (`upgradeBeforeDeployment: true`), it will not start running (The Chartreuse Pod will hang in `Init` state) until one PG Pod (and ES Pod if ES is used) is running, so make sure these Pods are available to Chartreuse. To fix that:
       - You will need to delete the Chartreuse Job so the upgrade can resume and fix you PG and ES pods (or create them if they don't exist), then you can redeploy so your migrations can run.
       - You can also try the `upgradeBeforeDeployment: false` mode (maybe temporarily).
```

### Comparing `chartreuse-4.3.2/setup.cfg` & `chartreuse-4.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.2/setup.py` & `chartreuse-4.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.2/src/chartreuse/chartreuse.py` & `chartreuse-4.3.3/src/chartreuse/chartreuse.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.2/src/chartreuse/chartreuse_upgrade.py` & `chartreuse-4.3.3/src/chartreuse/chartreuse_upgrade.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.2/src/chartreuse/utils/alembic_migration_helper.py` & `chartreuse-4.3.3/src/chartreuse/utils/alembic_migration_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import re
 from subprocess import SubprocessError
 from time import sleep, time
 from typing import List
 
 import sqlalchemy
+from sqlalchemy import inspect, text
 from sqlalchemy.pool import NullPool
 from wiremind_kubernetes.utils import run_command
 
 logger = logging.getLogger(__name__)
 
 
 class AlembicMigrationHelper:
@@ -42,15 +43,17 @@
             self._configure()
 
         self.is_migration_needed = self._check_migration_needed()
 
     def _configure(self) -> None:
         with open("%s/%s" % (self.alembic_directory_path, self.alembic_config_file_path), "r") as f:
             content = f.read()
-            content_new = re.sub("(sqlalchemy.url.*=.*){1}", r"sqlalchemy.url=%s" % self.database_url, content, flags=re.M)
+            content_new = re.sub(
+                "(sqlalchemy.url.*=.*){1}", r"sqlalchemy.url=%s" % self.database_url, content, flags=re.M
+            )
         if content != content_new:
             with open("%s/%s" % (self.alembic_directory_path, self.alembic_config_file_path), "w") as f:
                 f.write(content_new)
             logger.info("alembic.ini was configured.")
         else:
             raise SubprocessError("configuration of alembic.ini has failed (alembic.ini is unchanged)")
 
@@ -75,15 +78,15 @@
 
         while time() - start_time < wait_timeout:
             try:
                 # Yes, we may create a connection each time.
                 with engine.connect() as connection:
                     transac = connection.begin()
                     # TODO: Use scalar_one() once sqlachemly >= 1.4
-                    _id = connection.execute(";".join(default_privileges_checks)).scalar()
+                    _id = connection.execute(text(";".join(default_privileges_checks))).scalar()
                     assert _id == 1
                     transac.rollback()
                 logger.info(
                     "The role wiremind_owner_user was created and the default privileges"
                     " were set by the postgres-operator."
                 )
                 return
@@ -97,15 +100,15 @@
                 sleep(2)
         raise Exception(
             f"I'm fed up! Waited {wait_timeout}s for postgres-operator to configure the"
             f" Postgres database. Start by checking the postgres-operator logs."
         )
 
     def _get_table_list(self) -> List[str]:
-        return sqlalchemy.create_engine(self.database_url).table_names()
+        return inspect(sqlalchemy.create_engine(self.database_url)).get_table_names()
 
     def is_postgres_empty(self) -> bool:
         table_list = self._get_table_list()
         logger.info(f"Tables in the database: {table_list}")
         # Don't count "alembic" table
         table_name = "alembic_version"
         if table_name in table_list:
```

### Comparing `chartreuse-4.3.2/src/chartreuse.egg-info/SOURCES.txt` & `chartreuse-4.3.3/src/chartreuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

