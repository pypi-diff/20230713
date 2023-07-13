# Comparing `tmp/kevlar-system-inspector-1.1.0a1.tar.gz` & `tmp/kevlar-system-inspector-1.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-s4dsz_p2/kevlar-system-inspector-1.1.0a1.tar", last modified: Mon Jul 10 21:23:19 2023, max compression
+gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-0cbdsw9x/kevlar-system-inspector-1.1.0a2.tar", last modified: Thu Jul 13 14:56:21 2023, max compression
```

## Comparing `kevlar-system-inspector-1.1.0a1.tar` & `kevlar-system-inspector-1.1.0a2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5089 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4058 2023-05-16 13:17:40.000000 kevlar-system-inspector-1.1.0a1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/scripts/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/scripts/kevlar-system-inspector
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/
--rw-rw-rw-   0 root         (0) root         (0)     6827 2023-06-16 17:53:59.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     6310 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    16780 2023-06-16 18:06:26.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/console.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-13 18:38:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6821 2023-06-16 14:27:46.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/output.py
--rw-rw-rw-   0 root         (0) root         (0)    11579 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/resources/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/sysinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/failures.rst
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/html5-template.txt
--rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-16 17:50:38.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/report.rst
--rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/starlab.css
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-16 18:06:26.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/successes.rst
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-16 14:24:35.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/summary.rst
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/warnings.rst
--rw-rw-rw-   0 root         (0) root         (0)     5360 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_allowlisting.py
--rw-rw-rw-   0 root         (0) root         (0)     7875 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_kernel_config.py
--rw-rw-rw-   0 root         (0) root         (0)      650 2023-06-16 19:17:04.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_kernel_sandboxing.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2023-06-16 17:50:38.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_offline_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     6668 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_secure_networking.py
--rw-rw-rw-   0 root         (0) root         (0)     2000 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-06 18:45:08.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/access.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     4226 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/kconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-06-13 16:06:35.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     3943 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/mount.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/systemd.py
--rw-rw-rw-   0 root         (0) root         (0)     2825 2023-07-06 18:45:08.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/workdir.py
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-16 13:17:40.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5089 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5089 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4058 2023-05-16 13:17:40.000000 kevlar-system-inspector-1.1.0a2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/scripts/kevlar-system-inspector
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/
+-rw-rw-rw-   0 root         (0) root         (0)     6025 2023-07-12 20:42:05.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6310 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    16780 2023-06-16 18:06:26.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/console.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-13 18:38:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-12 20:42:05.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/output.py
+-rw-rw-rw-   0 root         (0) root         (0)    11579 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/sysinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/failures.rst
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/html5-template.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-16 17:50:38.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/report.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/starlab.css
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-16 18:06:26.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/successes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-16 14:24:35.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/summary.rst
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/warnings.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5360 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_allowlisting.py
+-rw-rw-rw-   0 root         (0) root         (0)     7875 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_kernel_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-06-16 19:17:04.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_kernel_sandboxing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2023-06-16 17:50:38.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_offline_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6668 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_secure_networking.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-06 18:45:08.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/access.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/kconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-06-13 16:06:35.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/mount.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2825 2023-07-06 18:45:08.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/workdir.py
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-13 12:59:23.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5089 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/top_level.txt
```

### Comparing `kevlar-system-inspector-1.1.0a1/LICENSE` & `kevlar-system-inspector-1.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/PKG-INFO` & `kevlar-system-inspector-1.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `kevlar-system-inspector-1.1.0a1/README.rst` & `kevlar-system-inspector-1.1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/setup.cfg` & `kevlar-system-inspector-1.1.0a2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kevlar-system-inspector
-version = 1.1.0a1
+version = 1.1.0a2
 author = Star Lab
 author_email = info@starlab.io
 url = https://www.starlab.io/explore-kevlar-system-inspector
 license = MIT
 license_files = LICENSE
 description = A security scanner for Linux systems
 long_description = file: README.rst
```

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/__init__.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 import pytest
 
 from .console import ConsoleProgress
 from .report import KevlarReporter
 from .output import (
     HtmlReporter,
     RstReporter,
-    ConsoleTestLister,
-    CsvTestLister,
     ConsoleReporter,
     TextReporter,
     SummaryReporter,
 )
 from .version import get_version
 
 DEFAULT_OUTPUT_FILE = "kevlar-system-inspector-report.txt"
@@ -109,29 +107,14 @@
              will print plain output when redirected to a file or pipe. The
              value 'always' will always print formatted output, and 'never'
              will always print plain output.
              """,
     )
 
     parser.add_argument(
-        "--list-tests",
-        action="store",
-        nargs="?",
-        const=True,
-        help="""
-             List the tests without running them. Note that this may show
-             additional tests not mentioned in the report as we only show
-             active security issues that are relevent to your operating
-             system.
-
-             If given a file name, writes a CSV to that file.
-             """,
-    )
-
-    parser.add_argument(
         "--version",
         action="version",
         version=f"Kevlar System Inspector: {get_version()}",
     )
 
     # Undocumented options:
     #   --debug: turn on regular pytest output
@@ -152,36 +135,29 @@
     if not any([args.output, args.output_console, args.output_html, args.output_rst]):
         # Default: text report only
         args.output = DEFAULT_OUTPUT_FILE
 
     # To isolate from any conftest.py or directories with test_*.py in them,
     # use path rather than --pyargs, and explicitly set the root directory.
     pytest_args = [_THIS_DIR, "--rootdir", _THIS_DIR]
-    plugins: List[Any] = [Tweaks()]
-
-    if args.list_tests:
-        if isinstance(args.list_tests, str):
-            plugins.append(CsvTestLister(args.list_tests))
-        else:
-            plugins.append(ConsoleTestLister())
-        pytest_args.append("--collect-only")
+    plugins: List[Any] = [
+        Tweaks(),
+        KevlarReporter(force_fail=args.force_fail_all),
+        ConsoleProgress(),
+    ]
+    if args.output:
+        plugins.append(TextReporter(args.output))
+    if args.output_html:
+        plugins.append(HtmlReporter(args.output_html))
+    if args.output_rst:
+        plugins.append(RstReporter(args.output_rst))
+    if args.output_console:
+        plugins.append(ConsoleReporter())
     else:
-        plugins.extend(
-            [KevlarReporter(force_fail=args.force_fail_all), ConsoleProgress()]
-        )
-        if args.output:
-            plugins.append(TextReporter(args.output))
-        if args.output_html:
-            plugins.append(HtmlReporter(args.output_html))
-        if args.output_rst:
-            plugins.append(RstReporter(args.output_rst))
-        if args.output_console:
-            plugins.append(ConsoleReporter())
-        else:
-            plugins.append(SummaryReporter())
+        plugins.append(SummaryReporter())
 
     if args.debug_coverage:
         try:
             import pytest_cov  # type: ignore # noqa: 401
         except ImportError:
             parser.error("ptest-cov module not installed. Cannot generate coverage.")
         pytest_args.extend(
```

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/conftest.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/conftest.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/console.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/console.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/decorators.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/decorators.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/report.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/report.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/sysinfo.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/sysinfo.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/failures.rst` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/failures.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/report.rst` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/report.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/starlab.css` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/starlab.css`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/summary.rst` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/summary.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_allowlisting.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_allowlisting.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_kernel_config.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_kernel_config.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_kernel_sandboxing.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_kernel_sandboxing.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_offline_integrity.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_offline_integrity.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_secure_networking.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_secure_networking.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_systemd_syscall_filtering.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_systemd_syscall_filtering.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/__init__.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/elf.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/elf.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/kconfig.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/kconfig.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/modules.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/modules.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/mount.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/mount.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/systemd.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/systemd.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/workdir.py` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/workdir.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/PKG-INFO` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/SOURCES.txt` & `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

