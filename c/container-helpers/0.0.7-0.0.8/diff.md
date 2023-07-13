# Comparing `tmp/container_helpers-0.0.7.tar.gz` & `tmp/container_helpers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container_helpers-0.0.7.tar", max compression
+gzip compressed data, was "container_helpers-0.0.8.tar", max compression
```

## Comparing `container_helpers-0.0.7.tar` & `container_helpers-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-07-11 07:04:41.390212 container_helpers-0.0.7/LICENSE
--rw-r--r--   0        0        0      438 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/__init__.py
--rw-r--r--   0        0        0     1239 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/data_types.py
--rw-r--r--   0        0        0        0 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/providers/__init__.py
--rw-r--r--   0        0        0      190 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/providers/base.py
--rw-r--r--   0        0        0      773 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/providers/helpers.py
--rw-r--r--   0        0        0     5119 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/providers/podman.py
--rw-r--r--   0        0        0      388 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/services/__init__.py
--rw-r--r--   0        0        0     2720 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/services/base.py
--rw-r--r--   0        0        0     4470 2023-07-11 07:04:41.390212 container_helpers-0.0.7/containers/services/windows.py
--rw-r--r--   0        0        0      568 2023-07-11 07:04:41.390212 container_helpers-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 container_helpers-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-13 01:23:31.198634 container_helpers-0.0.8/LICENSE
+-rw-r--r--   0        0        0      438 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/__init__.py
+-rw-r--r--   0        0        0     1280 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/data_types.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/providers/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/providers/base.py
+-rw-r--r--   0        0        0      773 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/providers/helpers.py
+-rw-r--r--   0        0        0     5285 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/providers/podman.py
+-rw-r--r--   0        0        0      388 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/services/__init__.py
+-rw-r--r--   0        0        0     2720 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/services/base.py
+-rw-r--r--   0        0        0     4470 2023-07-13 01:23:31.198634 container_helpers-0.0.8/containers/services/windows.py
+-rw-r--r--   0        0        0      568 2023-07-13 01:23:31.198634 container_helpers-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 container_helpers-0.0.8/PKG-INFO
```

### Comparing `container_helpers-0.0.7/LICENSE` & `container_helpers-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.7/containers/data_types.py` & `container_helpers-0.0.8/containers/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,8 +46,9 @@
     remove: bool = False
     environ: typing.Dict[str, str] = dataclasses.field(default_factory=dict)
     work_dir: typing.Optional[PathType] = None
     mounts: typing.List[Mount] = dataclasses.field(default_factory=list)
     user: typing.Optional[str] = None
     group: typing.Optional[str] = None
     network: typing.Optional[str] = None
+    timeout: typing.Optional[int] = None
     security_options: typing.Optional[SecurityOptions] = None
```

### Comparing `container_helpers-0.0.7/containers/providers/helpers.py` & `container_helpers-0.0.8/containers/providers/helpers.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.7/containers/providers/podman.py` & `container_helpers-0.0.8/containers/providers/podman.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,18 @@
         if container.tty:
             tty_args = ("--tty",)
 
         remove_args = tuple()
         if container.remove:
             remove_args = ("--rm",)
 
+        timeout_args = tuple()
+        if container.timeout is not None:
+            timeout_args = ("--timeout", str(container.timeout))
+
         user_args = tuple()
         if container.user is not None:
             user_group = str(container.user)
             if container.group is not None:
                 user_group += f":{container.group}"
             user_args = ("--user", user_group)
 
@@ -138,14 +142,15 @@
             )
         )
         args = (
             *base_args,
             *interactive_args,
             *tty_args,
             *remove_args,
+            *timeout_args,
             *env_args,
             *user_args,
             *work_dir_args,
             *network_args,
             *security_options_args,
             *mount_args,
             container.image,
```

### Comparing `container_helpers-0.0.7/containers/services/base.py` & `container_helpers-0.0.8/containers/services/base.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.7/containers/services/windows.py` & `container_helpers-0.0.8/containers/services/windows.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.7/pyproject.toml` & `container_helpers-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "container-helpers"
-version = "0.0.7"
+version = "0.0.8"
 description = "Helpers for running docker or podman containers easily in Python"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/container-helpers"
 packages = [{include = "containers"}]
 
 [tool.poetry.dependencies]
```

### Comparing `container_helpers-0.0.7/PKG-INFO` & `container_helpers-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-helpers
-Version: 0.0.7
+Version: 0.0.8
 Summary: Helpers for running docker or podman containers easily in Python
 Home-page: https://github.com/LaunchPlatform/container-helpers
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

