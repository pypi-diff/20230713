# Comparing `tmp/ovos-config-0.0.9a5.tar.gz` & `tmp/ovos-config-0.0.9a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-config-0.0.9a5.tar", last modified: Wed May 24 03:48:58 2023, max compression
+gzip compressed data, was "ovos-config-0.0.9a6.tar", last modified: Wed May 24 03:55:20 2023, max compression
```

## Comparing `ovos-config-0.0.9a5.tar` & `ovos-config-0.0.9a6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:48:58.644020 ovos-config-0.0.9a5/
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-24 03:48:58.644020 ovos-config-0.0.9a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:48:58.644020 ovos-config-0.0.9a5/ovos_config/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15910 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/mycroft.conf
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/ovos.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:48:58.644020 ovos-config-0.0.9a5/ovos_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/ovos_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 03:48:58.644020 ovos-config-0.0.9a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-24 03:48:58.000000 ovos-config-0.0.9a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:55:20.372952 ovos-config-0.0.9a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-24 03:55:20.372952 ovos-config-0.0.9a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:55:20.372952 ovos-config-0.0.9a6/ovos_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15910 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/mycroft.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/ovos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:55:20.372952 ovos-config-0.0.9a6/ovos_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/ovos_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 03:55:20.372952 ovos-config-0.0.9a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-24 03:55:20.000000 ovos-config-0.0.9a6/setup.py
```

### Comparing `ovos-config-0.0.9a5/PKG-INFO` & `ovos-config-0.0.9a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-config
-Version: 0.0.9a5
+Version: 0.0.9a6
 Summary: ovos-core configuration module
 Home-page: https://github.com/OpenVoiceOS/ovos-config
 License: Apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: extras
```

### Comparing `ovos-config-0.0.9a5/README.md` & `ovos-config-0.0.9a6/README.md`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a5/ovos_config/__main__.py` & `ovos-config-0.0.9a6/ovos_config/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a5/ovos_config/config.py` & `ovos-config-0.0.9a6/ovos_config/config.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a5/ovos_config/locale.py` & `ovos-config-0.0.9a6/ovos_config/locale.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a5/ovos_config/locations.py` & `ovos-config-0.0.9a6/ovos_config/locations.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a5/ovos_config/meta.py` & `ovos-config-0.0.9a6/ovos_config/meta.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a5/ovos_config/models.py` & `ovos-config-0.0.9a6/ovos_config/models.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a5/ovos_config/mycroft.conf` & `ovos-config-0.0.9a6/ovos_config/mycroft.conf`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.9a5/ovos_config.egg-info/PKG-INFO` & `ovos-config-0.0.9a6/ovos_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-config
-Version: 0.0.9a5
+Version: 0.0.9a6
 Summary: ovos-core configuration module
 Home-page: https://github.com/OpenVoiceOS/ovos-config
 License: Apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: extras
```

### Comparing `ovos-config-0.0.9a5/setup.py` & `ovos-config-0.0.9a6/setup.py`

 * *Files identical despite different names*

