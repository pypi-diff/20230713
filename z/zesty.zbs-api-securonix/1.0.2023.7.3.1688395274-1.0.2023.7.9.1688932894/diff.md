# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.7.3.1688395274.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.7.9.1688932894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.7.3.1688395274.tar", last modified: Mon Jul  3 14:41:14 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.7.9.1688932894.tar", last modified: Sun Jul  9 20:01:35 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274.tar` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    16171 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    14309 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-03 14:40:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-03 14:41:14.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16536 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    14309 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-09 19:29:49.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-09 20:01:34.000000 zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.7.3.1688395274
+Version: 1.0.2023.7.9.1688932894
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/README.md` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/setup.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/ManagedFS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import time
+from enum import Enum, auto
 from typing import Dict, List, Optional, Union
 from uuid import UUID as _UUID
 from uuid import uuid4
 
-from sqlalchemy import TIMESTAMP, INT
+from sqlalchemy import Enum as sa_ENUM
+from sqlalchemy import INT
+from sqlalchemy.sql.schema import ForeignKey
 from sqlalchemy.dialects.postgresql import ARRAY, UUID
 
 try:
     from sqlalchemy import Column, String, case, cast, engine, func, or_
     from sqlalchemy.dialects.postgresql import (BIGINT, BOOLEAN, FLOAT, JSON,
                                                 TIMESTAMP, VARCHAR)
     from sqlalchemy.ext.declarative import declarative_base
@@ -272,50 +275,72 @@
         return f"{actual_sorting_column} {sorting_order}"
 
 
 class ManagedFs(ManagedFsMixin, BaseMixin, Base):
     __tablename__ = "managed_filesystems"
 
 
+class MigrationStatus(Enum):
+    Active = auto()
+    Aborted = auto()
+    Completed = auto()
+    Failed = auto()
+
+
 class RunningMigrations(BaseMixin, Base):
     __tablename__ = "active_migration"
 
     fs_id = Column(VARCHAR)
     migration_uuid = Column(UUID(as_uuid=True), nullable=False, primary_key=True)
+    finished_at = Column(TIMESTAMP, nullable=True)
+    account_id = Column(VARCHAR, default=None)
+    region = Column(VARCHAR(255))
 
     reboot = Column(BOOLEAN, default=False)
     # array of day numbers when reboot is allowed 0-6
     days = Column(ARRAY(VARCHAR))
     # timeframe from-to in %I:%M %p
     from_ = Column(VARCHAR)
     to = Column(VARCHAR)
 
-    status = Column(VARCHAR, nullable=False, server_default="Active")
-    is_rebooting = Column(BOOLEAN, default=False)
+    status = Column(sa_ENUM(MigrationStatus), nullable=False, server_default=MigrationStatus.Active.name)
+    is_rebooting = Column(BOOLEAN, default=False)  # TODO: can this be deleted?
+
+    snapshot_id = Column(VARCHAR(255))
+    snapshot_remove_after = Column(INT, nullable=True)  # in days
+    snapshot_create_started_at = Column(TIMESTAMP, nullable=True)
+    snapshot_deleted_at = Column(TIMESTAMP, nullable=True)
 
-    # Snapshot and ebs deletion in days
-    ebs_remove_after = Column(INT, nullable=True)
-    snapshot_remove_after = Column(INT, nullable=True)
+    ebs_id = Column(VARCHAR(255))
+    ebs_remove_after = Column(INT, nullable=True)  # in days
+    ebs_detached_at = Column(TIMESTAMP, nullable=True)
+    ebs_deleted_at = Column(TIMESTAMP, nullable=True)
 
     def __init__(
             self,
             fs_id: str,
             migration_uuid: _UUID,
+            account_id: str = None,
+            region: str = None,
             days: Optional[List[int]] = None,
             from_: Optional[str] = None,
             to: Optional[str] = None,
             reboot: bool = False,
+            status: MigrationStatus = MigrationStatus.Active,
             ebs_remove_after: int = 1,
             snapshot_remove_after: int = 7):
         self.migration_uuid = migration_uuid
         self.fs_id = fs_id
+        self.account_id = account_id
+        self.region = region
         self.days = days
         self.from_ = from_
         self.to = to
         self.reboot = reboot
+        self.status = status
         self.ebs_remove_after = ebs_remove_after
         self.snapshot_remove_after = snapshot_remove_after
 
     @staticmethod
     def new_migration(
             fs_id,
             days: Optional[List[int]] = None,
@@ -335,21 +360,22 @@
 
 
 class MigrationHistory(BaseMixin, Base):
     __tablename__ = "migration_history"
 
     time_start = Column(TIMESTAMP)
     time_end = Column(TIMESTAMP)
-    status = Column(VARCHAR)
     phase = Column(VARCHAR, primary_key=True)
     progress = Column(FLOAT)
     completed = Column(BOOLEAN)
     failed = Column(BOOLEAN)
+    failure_reason = Column(VARCHAR)
     fs_id = Column(VARCHAR)
-    migration_uuid = Column(UUID(as_uuid=True), nullable=False, primary_key=True)
+    migration_uuid = Column(UUID(as_uuid=True), ForeignKey("active_migration.migration_uuid",  ondelete="CASCADE"),
+                            nullable=False, primary_key=True, index=True)
     # should be returned from the agent in seconds
     estimated = Column(INT)
     name = Column(VARCHAR)
     weight = Column(INT)
     abortable = Column(BOOLEAN)
     index = Column(INT, primary_key=True)
 
@@ -387,15 +413,16 @@
 
 
 class MigrationActions(BaseMixin, Base):
     __tablename__ = "migration_actions"
 
     id = Column(INT, primary_key=True, autoincrement=True)
     fs_id = Column(VARCHAR)
-    migration_uuid = Column(UUID(as_uuid=True), nullable=True)
+    migration_uuid = Column(UUID(as_uuid=True), ForeignKey("active_migration.migration_uuid",  ondelete="CASCADE"),
+                            nullable=False)
     action = Column(VARCHAR)
     value = Column(VARCHAR)
 
     allowed_actions = ['start', 'reboot', 'reboot_now', 'abort']
 
     def __init__(self, fs_id, migration_uuid, action, value):
         self.fs_id = fs_id
@@ -405,30 +432,9 @@
 
     def set_action(self, action):
         if action not in self.allowed_actions:
             raise WrongActionException
         self.action = action
 
 
-class MigrationOrigin(BaseMixin, Base):
-    __tablename__ = 'migration_origins'
-
-    fs_id = Column(VARCHAR(255))
-    migration_uuid = Column(UUID(as_uuid=True), nullable=False, primary_key=True)
-    account_id = Column(VARCHAR, index=True, default=None)
-
-    region = Column(VARCHAR(255))
-    migration_finished_at = Column(TIMESTAMP, nullable=True)
-
-    snapshot_id = Column(VARCHAR(255))
-    snapshot_expire_after_days = Column(INT, nullable=True)
-    snapshot_create_started_at = Column(TIMESTAMP, nullable=True)
-    snapshot_deleted_at = Column(TIMESTAMP, nullable=True)
-
-    ebs_id = Column(VARCHAR(255))
-    ebs_expire_after_days = Column(INT, nullable=True)
-    ebs_detached_at = Column(TIMESTAMP, nullable=True)
-    ebs_deleted_at = Column(TIMESTAMP, nullable=True)
-
-
 def create_tables(engine: engine.base.Engine) -> None:
     Base.metadata.create_all(engine, checkfirst=True)
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/src/step_instructions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.7.3.1688395274
+Version: 1.0.2023.7.9.1688932894
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.3.1688395274/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.7.9.1688932894/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

