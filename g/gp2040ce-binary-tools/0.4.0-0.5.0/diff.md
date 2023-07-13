# Comparing `tmp/gp2040ce-binary-tools-0.4.0.tar.gz` & `tmp/gp2040ce-binary-tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2040ce-binary-tools-0.4.0.tar", last modified: Sun Jul  9 16:10:35 2023, max compression
+gzip compressed data, was "gp2040ce-binary-tools-0.5.0.tar", last modified: Thu Jul 13 00:26:11 2023, max compression
```

## Comparing `gp2040ce-binary-tools-0.4.0.tar` & `gp2040ce-binary-tools-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/
--rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce-binary-tools-0.4.0/.gitattributes
--rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce-binary-tools-0.4.0/.gitignore
--rw-r--r--   0 bss       (1026) bss       (1000)     1077 2023-06-20 17:56:42.000000 gp2040ce-binary-tools-0.4.0/LICENSE
--rw-r--r--   0 bss       (1026) bss       (1000)     6593 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     5893 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/README.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.632900 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/
--rw-r--r--   0 bss       (1026) bss       (1000)     6593 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     1141 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
--rw-r--r--   0 bss       (1026) bss       (1000)        1 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      226 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/entry_points.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      277 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/requires.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       18 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/top_level.txt
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.633900 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/
--rw-r--r--   0 bss       (1026) bss       (1000)     2093 2023-06-26 20:39:01.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)      160 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/_version.py
--rw-r--r--   0 bss       (1026) bss       (1000)     6666 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)      712 2023-06-30 07:04:59.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/config_tree.css
--rw-r--r--   0 bss       (1026) bss       (1000)    17641 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     8426 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/pico.py
--rw-r--r--   0 bss       (1026) bss       (1000)     8893 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2349 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/pyproject.toml
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.633900 gp2040ce-binary-tools-0.4.0/requirements/
--rw-r--r--   0 bss       (1026) bss       (1000)     3991 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/requirements/requirements-dev.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      991 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/requirements/requirements.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       38 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/setup.cfg
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.633900 gp2040ce-binary-tools-0.4.0/tests/
--rw-r--r--   0 bss       (1026) bss       (1000)     1222 2023-06-28 19:59:12.000000 gp2040ce-binary-tools-0.4.0/tests/conftest.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.634900 gp2040ce-binary-tools-0.4.0/tests/test-files/
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    22122 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7378 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2023-07-01 19:13:13.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/nanopb_pb2.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    12702 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     4135 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2023-06-21 00:57:38.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     2046 2023-06-30 06:50:33.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/test-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)   727084 2023-06-26 19:51:10.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/test-firmware.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     8192 2023-07-01 21:47:58.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/test-storage-area.bin
--rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-06-29 19:56:04.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/test-whole-board.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     6039 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/tests/test_builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2798 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/tests/test_commands.py
--rw-r--r--   0 bss       (1026) bss       (1000)     6687 2023-07-01 22:06:16.000000 gp2040ce-binary-tools-0.4.0/tests/test_gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1321 2023-06-21 00:57:38.000000 gp2040ce-binary-tools-0.4.0/tests/test_package.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9649 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/tests/test_pico.py
--rw-r--r--   0 bss       (1026) bss       (1000)     6590 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/tests/test_storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1604 2023-06-28 19:59:12.000000 gp2040ce-binary-tools-0.4.0/tox.ini
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-13 00:26:11.499867 gp2040ce-binary-tools-0.5.0/
+-rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce-binary-tools-0.5.0/.gitattributes
+-rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce-binary-tools-0.5.0/.gitignore
+-rw-r--r--   0 bss       (1026) bss       (1000)     2815 2023-07-13 00:17:59.000000 gp2040ce-binary-tools-0.5.0/CHANGELOG.md
+-rw-r--r--   0 bss       (1026) bss       (1000)     1077 2023-06-20 17:56:42.000000 gp2040ce-binary-tools-0.5.0/LICENSE
+-rw-r--r--   0 bss       (1026) bss       (1000)     7126 2023-07-13 00:26:11.499867 gp2040ce-binary-tools-0.5.0/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     6319 2023-07-12 22:46:50.000000 gp2040ce-binary-tools-0.5.0/README.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-13 00:26:11.490867 gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/
+-rw-r--r--   0 bss       (1026) bss       (1000)     7126 2023-07-13 00:26:11.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     1154 2023-07-13 00:26:11.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)        1 2023-07-13 00:26:11.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      282 2023-07-13 00:26:11.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/entry_points.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      289 2023-07-13 00:26:11.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/requires.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       18 2023-07-13 00:26:11.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/top_level.txt
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-13 00:26:11.490867 gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2093 2023-06-26 20:39:01.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      160 2023-07-13 00:26:11.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/_version.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9902 2023-07-12 23:31:46.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      712 2023-06-30 07:04:59.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/config_tree.css
+-rw-r--r--   0 bss       (1026) bss       (1000)    19282 2023-07-12 22:49:08.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     8935 2023-07-12 21:31:16.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/pico.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9676 2023-07-12 22:47:41.000000 gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2521 2023-07-13 00:21:00.000000 gp2040ce-binary-tools-0.5.0/pyproject.toml
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-13 00:26:11.490867 gp2040ce-binary-tools-0.5.0/requirements/
+-rw-r--r--   0 bss       (1026) bss       (1000)     4532 2023-07-11 16:44:22.000000 gp2040ce-binary-tools-0.5.0/requirements/requirements-dev.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      991 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.5.0/requirements/requirements.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       38 2023-07-13 00:26:11.499867 gp2040ce-binary-tools-0.5.0/setup.cfg
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-13 00:26:11.491866 gp2040ce-binary-tools-0.5.0/tests/
+-rw-r--r--   0 bss       (1026) bss       (1000)     1222 2023-06-28 19:59:12.000000 gp2040ce-binary-tools-0.5.0/tests/conftest.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-13 00:26:11.492866 gp2040ce-binary-tools-0.5.0/tests/test-files/
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-13 00:26:11.499867 gp2040ce-binary-tools-0.5.0/tests/test-files/pb2-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    22122 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/pb2-files/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     7378 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/pb2-files/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2023-07-01 19:13:13.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/pb2-files/nanopb_pb2.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-13 00:26:11.499867 gp2040ce-binary-tools-0.5.0/tests/test-files/proto-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    12702 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/proto-files/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     4135 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/proto-files/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2023-06-21 00:57:38.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/proto-files/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     2046 2023-06-30 06:50:33.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/test-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)   727084 2023-06-26 19:51:10.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/test-firmware.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     8192 2023-07-01 21:47:58.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/test-storage-area.bin
+-rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-06-29 19:56:04.000000 gp2040ce-binary-tools-0.5.0/tests/test-files/test-whole-board.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     8771 2023-07-12 23:31:56.000000 gp2040ce-binary-tools-0.5.0/tests/test_builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2823 2023-07-12 22:44:08.000000 gp2040ce-binary-tools-0.5.0/tests/test_commands.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     8761 2023-07-12 05:06:41.000000 gp2040ce-binary-tools-0.5.0/tests/test_gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1321 2023-06-21 00:57:38.000000 gp2040ce-binary-tools-0.5.0/tests/test_package.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    10887 2023-07-12 22:32:48.000000 gp2040ce-binary-tools-0.5.0/tests/test_pico.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     6590 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.5.0/tests/test_storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1604 2023-06-28 19:59:12.000000 gp2040ce-binary-tools-0.5.0/tox.ini
```

### Comparing `gp2040ce-binary-tools-0.4.0/.gitignore` & `gp2040ce-binary-tools-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/LICENSE` & `gp2040ce-binary-tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/PKG-INFO` & `gp2040ce-binary-tools-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: gp2040ce-binary-tools
-Version: 0.4.0
-Summary: Tools for working with GP2040-CE firmware and storage binaries.
-Author-email: "Brian S. Stephan" <bss@incorporeal.org>
-License: MIT
-Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
-Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # GP2040-CE Binary Tools
 
 Tools for working with GP2040-CE binary dumps.
 
 ## Dependencies
 
 Interacting with your board (e.g. getting dumps, etc.) requires [picotool](https://github.com/raspberrypi/picotool), and
@@ -73,29 +55,43 @@
 
 `concatenate` combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
 section .bin or config (with footer) .bin, and produces a properly-offset .bin file suitable for flashing to a board.
 This may be useful to ensure the board is flashed with a particular configuration, for instances such as producing a
 binary to flash many boards with a particular configuration (specific customizations, etc.), or keeping documented
 backups of what you're testing with during development.
 
+The produced binary can be written to a file with `--new-binary-filename FILENAME` or straight to a RP2040 in BOOTSEL
+ mode with `--usb`.
+
 Sample usage:
 
 ```
-% concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin new-firmware-with-config.bin
+% concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin --new-binary-filename new-firmware-with-config.bin
 ```
 
 ### dump-config
 
 `dump-config` replaces the need for picotool in order to make a copy of the GP2040-CE configuration as a binary file.
 This could be used with the other tools, or just to keep a backup.
 
 Sample usage:
 
 ```
-% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename `date +%Y%m%d`-config-backup.bin
+% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto `date +%Y%m%d`-config-backup.bin
+```
+
+### dump-gp2040ce
+
+`dump-gp2040ce` replaces the need for picotool in order to make a copy of a board's full GP2040-CE image as a binary file.
+This could be used with the other tools, or just to keep a backup.
+
+Sample usage:
+
+```
+% dump-gp2040ce `date +%Y%m%d`-backup.bin
 ```
 
 ### visualize-storage
 
 `visualize-storage` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
 storage section, and prints it out for visual inspection or diffing with other tools. It can also find the storage
 section from a GP2040-CE whole board dump, if you have that instead. Usage is simple; just connect your board in BOOTSEL
```

### Comparing `gp2040ce-binary-tools-0.4.0/README.md` & `gp2040ce-binary-tools-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: gp2040ce-binary-tools
+Version: 0.5.0
+Summary: Tools for working with GP2040-CE firmware and storage binaries.
+Author-email: "Brian S. Stephan" <bss@incorporeal.org>
+License: MIT
+Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
+Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
+Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Utilities
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # GP2040-CE Binary Tools
 
 Tools for working with GP2040-CE binary dumps.
 
 ## Dependencies
 
 Interacting with your board (e.g. getting dumps, etc.) requires [picotool](https://github.com/raspberrypi/picotool), and
@@ -55,29 +74,43 @@
 
 `concatenate` combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
 section .bin or config (with footer) .bin, and produces a properly-offset .bin file suitable for flashing to a board.
 This may be useful to ensure the board is flashed with a particular configuration, for instances such as producing a
 binary to flash many boards with a particular configuration (specific customizations, etc.), or keeping documented
 backups of what you're testing with during development.
 
+The produced binary can be written to a file with `--new-binary-filename FILENAME` or straight to a RP2040 in BOOTSEL
+ mode with `--usb`.
+
 Sample usage:
 
 ```
-% concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin new-firmware-with-config.bin
+% concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin --new-binary-filename new-firmware-with-config.bin
 ```
 
 ### dump-config
 
 `dump-config` replaces the need for picotool in order to make a copy of the GP2040-CE configuration as a binary file.
 This could be used with the other tools, or just to keep a backup.
 
 Sample usage:
 
 ```
-% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename `date +%Y%m%d`-config-backup.bin
+% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto `date +%Y%m%d`-config-backup.bin
+```
+
+### dump-gp2040ce
+
+`dump-gp2040ce` replaces the need for picotool in order to make a copy of a board's full GP2040-CE image as a binary file.
+This could be used with the other tools, or just to keep a backup.
+
+Sample usage:
+
+```
+% dump-gp2040ce `date +%Y%m%d`-backup.bin
 ```
 
 ### visualize-storage
 
 `visualize-storage` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
 storage section, and prints it out for visual inspection or diffing with other tools. It can also find the storage
 section from a GP2040-CE whole board dump, if you have that instead. Usage is simple; just connect your board in BOOTSEL
```

### Comparing `gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/PKG-INFO` & `gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: MIT
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
+Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
@@ -73,29 +74,43 @@
 
 `concatenate` combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
 section .bin or config (with footer) .bin, and produces a properly-offset .bin file suitable for flashing to a board.
 This may be useful to ensure the board is flashed with a particular configuration, for instances such as producing a
 binary to flash many boards with a particular configuration (specific customizations, etc.), or keeping documented
 backups of what you're testing with during development.
 
+The produced binary can be written to a file with `--new-binary-filename FILENAME` or straight to a RP2040 in BOOTSEL
+ mode with `--usb`.
+
 Sample usage:
 
 ```
-% concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin new-firmware-with-config.bin
+% concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin --new-binary-filename new-firmware-with-config.bin
 ```
 
 ### dump-config
 
 `dump-config` replaces the need for picotool in order to make a copy of the GP2040-CE configuration as a binary file.
 This could be used with the other tools, or just to keep a backup.
 
 Sample usage:
 
 ```
-% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename `date +%Y%m%d`-config-backup.bin
+% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto `date +%Y%m%d`-config-backup.bin
+```
+
+### dump-gp2040ce
+
+`dump-gp2040ce` replaces the need for picotool in order to make a copy of a board's full GP2040-CE image as a binary file.
+This could be used with the other tools, or just to keep a backup.
+
+Sample usage:
+
+```
+% dump-gp2040ce `date +%Y%m%d`-backup.bin
 ```
 
 ### visualize-storage
 
 `visualize-storage` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
 storage section, and prints it out for visual inspection or diffing with other tools. It can also find the storage
 section from a GP2040-CE whole board dump, if you have that instead. Usage is simple; just connect your board in BOOTSEL
```

### Comparing `gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/SOURCES.txt` & `gp2040ce-binary-tools-0.5.0/gp2040ce_binary_tools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitattributes
 .gitignore
+CHANGELOG.md
 LICENSE
 README.md
 pyproject.toml
 tox.ini
 gp2040ce_binary_tools.egg-info/PKG-INFO
 gp2040ce_binary_tools.egg-info/SOURCES.txt
 gp2040ce_binary_tools.egg-info/dependency_links.txt
```

### Comparing `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/__init__.py` & `gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/config_tree.css` & `gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/config_tree.css`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/gui.py` & `gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from textual.screen import ModalScreen
 from textual.validation import Number
 from textual.widgets import Button, Footer, Header, Input, Label, Pretty, Select, Tree
 from textual.widgets.tree import TreeNode
 
 from gp2040ce_bintools import core_parser, handler
 from gp2040ce_bintools.builder import write_new_config_to_filename, write_new_config_to_usb
-from gp2040ce_bintools.storage import get_config_from_file, get_config_from_usb
+from gp2040ce_bintools.pico import get_bootsel_endpoints, read
+from gp2040ce_bintools.storage import (STORAGE_MEMORY_ADDRESS, STORAGE_SIZE, ConfigReadError, get_config,
+                                       get_config_from_file, get_new_config)
 
 logger = logging.getLogger(__name__)
 
 
 class EditScreen(ModalScreen):
     """Do an input prompt by way of an overlaid screen."""
 
@@ -126,34 +128,35 @@
         ('q', 'quit', "Quit"),
     ]
     CSS_PATH = "config_tree.css"
     TITLE = "GP2040-CE Configuration Editor"
 
     def __init__(self, *args, **kwargs):
         """Initialize config."""
+        # disable normal logging and enable console logging
+        logger.debug("reconfiguring logging...")
+        root = logging.getLogger()
+        root.setLevel(logging.DEBUG)
+        root.removeHandler(handler)
+        root.addHandler(TextualHandler())
+
         self.config_filename = kwargs.pop('config_filename', None)
-        self.whole_board = kwargs.pop('whole_board', False)
         self.usb = kwargs.pop('usb', False)
-        # load the config
+        self.whole_board = kwargs.pop('whole_board', False)
+        self.create_new = kwargs.pop('create_new', False)
+
+        super().__init__(*args, **kwargs)
+        self._load_config()
+
         if self.usb:
-            self.config, self.endpoint_out, self.endpoint_in = get_config_from_usb()
             self.source_name = (f"DEVICE ID {hex(self.endpoint_out.device.idVendor)}:"
                                 f"{hex(self.endpoint_out.device.idProduct)} "
                                 f"on bus {self.endpoint_out.device.bus} address {self.endpoint_out.device.address}")
         else:
-            self.config = get_config_from_file(self.config_filename, whole_board=self.whole_board)
             self.source_name = self.config_filename
-        super().__init__(*args, **kwargs)
-
-        # disable normal logging and enable console logging if we're not headless
-        logger.debug("reconfiguring logging...")
-        root = logging.getLogger()
-        root.setLevel(logging.DEBUG)
-        root.removeHandler(handler)
-        root.addHandler(TextualHandler())
 
     def compose(self) -> ComposeResult:
         """Compose the UI."""
         yield Header()
         yield Footer()
         yield Tree("Root")
 
@@ -166,15 +169,15 @@
         missing_fields = [f for f in self.config.DESCRIPTOR.fields
                           if f not in [fp for fp, vp in self.config.ListFields()]]
         for field_descriptor, field_value in sorted(self.config.ListFields(), key=lambda f: f[0].name):
             child_is_message = ConfigEditor._descriptor_is_message(field_descriptor)
             ConfigEditor._add_node(tree.root, self.config, field_descriptor, field_value,
                                    value_is_config=child_is_message)
         for child_field_descriptor in sorted(missing_fields, key=lambda f: f.name):
-            child_is_message = ConfigEditor._descriptor_is_message(field_descriptor)
+            child_is_message = ConfigEditor._descriptor_is_message(child_field_descriptor)
             ConfigEditor._add_node(tree.root, self.config, child_field_descriptor,
                                    getattr(self.config, child_field_descriptor.name),
                                    value_is_config=child_is_message)
         tree.root.expand()
 
     def on_tree_node_selected(self, node_event: Tree.NodeSelected) -> None:
         """Take the appropriate action for this type of node."""
@@ -308,14 +311,43 @@
             node.data = (parent_config, field_descriptor, field_value)
             node.set_label(pb_field_to_node_label(field_descriptor, field_value))
             logger.debug(self.config)
         else:
             logger.debug("opening edit screen for %s", field_descriptor.name)
             self.push_screen(EditScreen(node, field_value))
 
+    def _load_config(self):
+        """Based on how this was initialized, get the config in a variety of ways."""
+        if self.usb:
+            try:
+                self.endpoint_out, self.endpoint_in = get_bootsel_endpoints()
+                config_binary = read(self.endpoint_out, self.endpoint_in, STORAGE_MEMORY_ADDRESS, STORAGE_SIZE)
+                self.config = get_config(bytes(config_binary))
+            except ConfigReadError:
+                if self.create_new:
+                    logger.warning("creating new config as the read one was invalid!")
+                    self.config = get_new_config()
+                else:
+                    raise
+        else:
+            try:
+                self.config = get_config_from_file(self.config_filename, whole_board=self.whole_board)
+            except FileNotFoundError:
+                if self.create_new:
+                    logger.warning("creating new config as the read one was invalid!")
+                    self.config = get_new_config()
+                else:
+                    raise
+            except ConfigReadError:
+                if self.create_new:
+                    logger.warning("creating new config as the read one was invalid!")
+                    self.config = get_new_config()
+                else:
+                    raise
+
 
 def pb_field_to_node_label(field_descriptor, field_value):
     """Provide the pretty label for a tree node.
 
     Args:
         field_descriptor: protobuf field for determining the type
         field_value: value to render
@@ -350,20 +382,23 @@
 
 def edit_config():
     """Edit the configuration in an interactive fashion."""
     parser = argparse.ArgumentParser(
         description="Utilize a GUI to view and alter the contents of a GP2040-CE configuration.",
         parents=[core_parser],
     )
+    parser.add_argument('--whole-board', action='store_true', help="indicate the binary file is a whole board dump")
+    parser.add_argument('--new-if-not-found', action='store_true', default=True,
+                        help="if the file/USB device doesn't have a config section, start a new one (default: enabled)")
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument('--usb', action='store_true', help="retrieve the config from a Pico board connected over USB "
                                                           "and in BOOTSEL mode")
     group.add_argument('--filename', help=".bin file of a GP2040-CE board's config + footer or entire storage section, "
                                           "or of a GP2040-CE's whole board dump if --whole-board is specified")
-    parser.add_argument('--whole-board', action='store_true', help="indicate the binary file is a whole board dump")
     args, _ = parser.parse_known_args()
 
     if args.usb:
-        app = ConfigEditor(usb=True)
+        app = ConfigEditor(usb=True, create_new=args.new_if_not_found)
     else:
-        app = ConfigEditor(config_filename=args.filename, whole_board=args.whole_board)
+        app = ConfigEditor(config_filename=args.filename, whole_board=args.whole_board,
+                           create_new=args.new_if_not_found)
     app.run()
```

### Comparing `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/pico.py` & `gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/pico.py`

 * *Files 8% similar despite different names*

```diff
@@ -194,29 +194,42 @@
 
     Args:
         out_endpoint: the out direction USB endpoint to write to
         in_endpoint: the in direction USB endpoint to read from
         location: memory address of where to start reading from
         content: the data to write
     """
-    if (location % 256) != 0:
-        raise PicoAlignmentError("writes must start at 256 byte boundaries, please pad or align as appropriate!")
+    chunk_size = 4096
+    write_location = location
+    write_size = 0
+
+    if (location % chunk_size) != 0:
+        raise PicoAlignmentError(f"writes must start at {chunk_size} byte boundaries, "
+                                 f"please pad or align as appropriate!")
 
     # set up the data
     command_size = 8
+    size = len(content)
 
     exclusive_access(out_end, in_end, is_exclusive=True)
-    exit_xip(out_end, in_end)
-    erase(out_end, in_end, location, len(content))
-    exit_xip(out_end, in_end)
-    pico_token = 1
-    logger.debug("writing %s bytes to %s", len(content), location)
-    payload = struct.pack(PICOBOOT_CMD_STRUCT + PICOBOOT_CMD_READ_SUFFIX_STRUCT,
-                          PICO_MAGIC, pico_token, PICO_COMMANDS['WRITE'], command_size, len(content),
-                          location, len(content))
-    logger.debug("WRITE: %s", payload)
-    out_end.write(payload)
-    logger.debug("actually writing bytes now...")
-    out_end.write(content)
-    res = in_end.read(256)
-    logger.debug("res: %s", res)
+    while write_size < size:
+        pico_token = 1
+        to_write = content[write_size:(write_size + chunk_size)]
+
+        exit_xip(out_end, in_end)
+        logger.debug("erasing %s bytes at %s", len(to_write), hex(write_location))
+        erase(out_end, in_end, write_location, len(to_write))
+
+        logger.debug("writing %s bytes to %s", len(to_write), hex(write_location))
+        payload = struct.pack(PICOBOOT_CMD_STRUCT + PICOBOOT_CMD_READ_SUFFIX_STRUCT,
+                              PICO_MAGIC, pico_token, PICO_COMMANDS['WRITE'], command_size, len(to_write),
+                              write_location, len(to_write))
+        logger.debug("WRITE: %s", payload)
+        out_end.write(payload)
+        logger.debug("actually writing bytes now...")
+        logger.debug("payload: %s", to_write)
+        out_end.write(bytes(to_write))
+        res = in_end.read(chunk_size)
+        logger.debug("res: %s", res)
+        write_size += chunk_size
+        write_location += chunk_size
     exclusive_access(out_end, in_end, is_exclusive=False)
```

### Comparing `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/storage.py` & `gp2040ce-binary-tools-0.5.0/gp2040ce_bintools/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,27 @@
 
 
 #################
 # LIBRARY ITEMS #
 #################
 
 
-class ConfigCrcError(ValueError):
+class ConfigReadError(ValueError):
+    """General exception for failing to read/verify the GP2040-CE config for some reason."""
+
+
+class ConfigCrcError(ConfigReadError):
     """Exception raised when the CRC checksum in the footer doesn't match the actual content's."""
 
 
-class ConfigLengthError(ValueError):
+class ConfigLengthError(ConfigReadError):
     """Exception raised when a length sanity check fails."""
 
 
-class ConfigMagicError(ValueError):
+class ConfigMagicError(ConfigReadError):
     """Exception raised when the config section does not have the magic value in its footer."""
 
 
 def get_config(content: bytes) -> Message:
     """Read the config from a GP2040-CE storage section.
 
     Args:
@@ -61,32 +65,40 @@
     Returns:
         the discovered config size, config CRC checksum, and magic from the config footer
     Raises:
         ConfigLengthError, ConfigMagicError: if the provided bytes are not a config footer
     """
     # last 12 bytes are the footer
     logger.debug("length of content to look for footer in: %s", len(content))
+    logger.debug("content searching in for a footer: %s", content)
     if len(content) < FOOTER_SIZE:
         raise ConfigLengthError(f"provided content ({len(content)} bytes) is not large enough to have a config footer!")
 
     footer = content[-FOOTER_SIZE:]
     logger.debug("suspected footer magic: %s", footer[-4:])
     if footer[-4:] != FOOTER_MAGIC:
         raise ConfigMagicError("content's magic is not as expected!")
 
     config_size = int.from_bytes(reversed(footer[:4]), 'big')
     config_crc = int.from_bytes(reversed(footer[4:8]), 'big')
     config_magic = f'0x{footer[8:12].hex()}'
 
     # more sanity checks
+    logger.debug("length of content + footer: %s", len(content))
     if len(content) < config_size + FOOTER_SIZE:
         raise ConfigLengthError(f"provided content ({len(content)} bytes) is not large enough according to the "
                                 f"config footer!")
 
-    content_crc = binascii.crc32(content[-(config_size + 12):-12])
+    logger.debug("config size according to footer: %s", config_size)
+
+    content_config = content[-(config_size + 12):-12]
+    content_crc = binascii.crc32(content_config)
+    logger.debug("content used to calculate CRC: %s", content_config)
+    logger.debug("calculated config CRC: %s", content_crc)
+    logger.debug("expected config CRC: %s", config_crc)
     if config_crc != content_crc:
         raise ConfigCrcError(f"provided content CRC checksum {content_crc} does not match footer's expected CRC "
                              f"checksum {config_crc}!")
 
     logger.debug("detected footer (size:%s, crc:%s, magic:%s", config_size, config_crc, config_magic)
     return config_size, config_crc, config_magic
 
@@ -146,14 +158,24 @@
         raise ConfigLengthError("provided content is not large enough to have a storage section!")
 
     logger.debug("returning bytes from %s to %s", hex(STORAGE_BINARY_LOCATION),
                  hex(STORAGE_BINARY_LOCATION + STORAGE_SIZE))
     return content[STORAGE_BINARY_LOCATION:(STORAGE_BINARY_LOCATION + STORAGE_SIZE)]
 
 
+def get_new_config() -> Message:
+    """Wrap the creation of a new Config message.
+
+    Returns:
+        the initialized Config
+    """
+    config_pb2 = get_config_pb2()
+    return config_pb2.Config()
+
+
 def pad_config_to_storage_size(config: bytes) -> bytearray:
     """Provide a copy of the config (with footer) padded with zero bytes to be the proper storage section size.
 
     Args:
         firmware: the config section binary to process
     Returns:
         the resulting padded binary as a bytearray
@@ -186,36 +208,36 @@
 
 def dump_config():
     """Save the GP2040-CE's configuration to a binary file."""
     parser = argparse.ArgumentParser(
         description="Read the configuration section from a USB device and save it to a binary file.",
         parents=[core_parser],
     )
-    parser.add_argument('--filename', help=".bin file to save the GP2040-CE board's config section to")
+    parser.add_argument('binary_filename', help=".bin file to save the GP2040-CE board's config section to")
     args, _ = parser.parse_known_args()
     config, _, _ = get_config_from_usb()
-    with open(args.filename, 'wb') as out_file:
+    with open(args.binary_filename, 'wb') as out_file:
         out_file.write(serialize_config_with_footer(config))
 
 
 def visualize():
     """Print the contents of GP2040-CE's storage."""
     parser = argparse.ArgumentParser(
         description="Read the configuration section from a dump of a GP2040-CE board's storage section and print out "
                     "its contents.",
         parents=[core_parser],
     )
+    parser.add_argument('--whole-board', action='store_true', help="indicate the binary file is a whole board dump")
+    parser.add_argument('--json', action='store_true', help="print the config out as a JSON document")
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument('--usb', action='store_true', help="retrieve the config from a Pico board connected over USB "
                                                           "and in BOOTSEL mode")
     group.add_argument('--filename', help=".bin file of a GP2040-CE board's storage section, bytes "
                                           "101FE000-10200000, or of a GP2040-CE's whole board dump "
                                           "if --whole-board is specified")
-    parser.add_argument('--whole-board', action='store_true', help="indicate the binary file is a whole board dump")
-    parser.add_argument('--json', action='store_true', help="print the config out as a JSON document")
     args, _ = parser.parse_known_args()
 
     if args.usb:
         config, _, _ = get_config_from_usb()
     else:
         config = get_config_from_file(args.filename, whole_board=args.whole_board)
```

### Comparing `gp2040ce-binary-tools-0.4.0/pyproject.toml` & `gp2040ce-binary-tools-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,28 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/OpenStickCommunity/gp2040ce-binary-tools"
+"Changelog" = "https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues"
 
 
 [project.optional-dependencies]
 dev = ["bandit", "decorator", "flake8", "flake8-blind-except", "flake8-builtins", "flake8-docstrings",
        "flake8-executable", "flake8-fixme", "flake8-isort", "flake8-logging-format", "flake8-mutable",
        "flake8-pyproject", "mypy", "pip-tools", "pytest", "pytest-asyncio", "pytest-cov", "setuptools-scm",
-       "tox"]
+       "textual-dev", "tox"]
 
 [project.scripts]
 concatenate = "gp2040ce_bintools.builder:concatenate"
 dump-config = "gp2040ce_bintools.storage:dump_config"
+dump-gp2040ce = "gp2040ce_bintools.builder:dump_gp2040ce"
 edit-config = "gp2040ce_bintools.gui:edit_config"
 visualize-storage = "gp2040ce_bintools.storage:visualize"
 
 [tool.flake8]
 enable-extensions = "G,M"
 exclude = [".tox/", "venv/", "_version.py", "tests/test-files/"]
 extend-ignore = "T101"
```

### Comparing `gp2040ce-binary-tools-0.4.0/requirements/requirements-dev.txt` & `gp2040ce-binary-tools-0.5.0/requirements/requirements-dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=requirements/requirements-dev.txt
 #
+aiohttp==3.8.4
+    # via textual-dev
+aiosignal==1.3.1
+    # via aiohttp
+async-timeout==4.0.2
+    # via aiohttp
+attrs==23.1.0
+    # via aiohttp
 bandit==1.7.5
     # via gp2040ce-binary-tools (pyproject.toml)
 build==0.10.0
     # via pip-tools
 cachetools==5.3.1
     # via tox
 chardet==5.1.0
     # via tox
+charset-normalizer==3.2.0
+    # via aiohttp
 click==8.1.3
-    # via pip-tools
+    # via
+    #   pip-tools
+    #   textual-dev
 colorama==0.4.6
     # via tox
 coverage[toml]==7.2.7
     # via pytest-cov
 decorator==5.1.1
     # via gp2040ce-binary-tools (pyproject.toml)
 distlib==0.3.6
@@ -51,22 +63,28 @@
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-logging-format==0.9.0
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-mutable==1.2.0
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-pyproject==1.2.3
     # via gp2040ce-binary-tools (pyproject.toml)
+frozenlist==1.3.3
+    # via
+    #   aiohttp
+    #   aiosignal
 gitdb==4.0.10
     # via gitpython
 gitpython==3.1.31
     # via bandit
 grpcio==1.56.0
     # via grpcio-tools
 grpcio-tools==1.56.0
     # via gp2040ce-binary-tools (pyproject.toml)
+idna==3.4
+    # via yarl
 importlib-metadata==6.7.0
     # via textual
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via flake8-isort
 linkify-it-py==2.0.2
@@ -78,14 +96,20 @@
     #   textual
 mccabe==0.7.0
     # via flake8
 mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
+msgpack==1.0.5
+    # via textual-dev
+multidict==6.0.4
+    # via
+    #   aiohttp
+    #   yarl
 mypy==1.4.1
     # via gp2040ce-binary-tools (pyproject.toml)
 mypy-extensions==1.0.0
     # via mypy
 packaging==23.1
     # via
     #   build
@@ -141,14 +165,18 @@
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
 stevedore==5.1.0
     # via bandit
 textual==0.29.0
+    # via
+    #   gp2040ce-binary-tools (pyproject.toml)
+    #   textual-dev
+textual-dev==1.0.1
     # via gp2040ce-binary-tools (pyproject.toml)
 tomli==2.0.1
     # via
     #   build
     #   coverage
     #   flake8-pyproject
     #   mypy
@@ -161,19 +189,22 @@
 tox==4.6.3
     # via gp2040ce-binary-tools (pyproject.toml)
 typing-extensions==4.7.1
     # via
     #   mypy
     #   setuptools-scm
     #   textual
+    #   textual-dev
 uc-micro-py==1.0.2
     # via linkify-it-py
 virtualenv==20.23.1
     # via tox
 wheel==0.40.0
     # via pip-tools
+yarl==1.9.2
+    # via aiohttp
 zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `gp2040ce-binary-tools-0.4.0/requirements/requirements.txt` & `gp2040ce-binary-tools-0.5.0/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/conftest.py` & `gp2040ce-binary-tools-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/config_pb2.py` & `gp2040ce-binary-tools-0.5.0/tests/test-files/pb2-files/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/enums_pb2.py` & `gp2040ce-binary-tools-0.5.0/tests/test-files/pb2-files/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/nanopb_pb2.py` & `gp2040ce-binary-tools-0.5.0/tests/test-files/pb2-files/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/config.proto` & `gp2040ce-binary-tools-0.5.0/tests/test-files/proto-files/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/enums.proto` & `gp2040ce-binary-tools-0.5.0/tests/test-files/proto-files/enums.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/nanopb.proto` & `gp2040ce-binary-tools-0.5.0/tests/test-files/proto-files/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/test-config.bin` & `gp2040ce-binary-tools-0.5.0/tests/test-files/test-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/test-firmware.bin` & `gp2040ce-binary-tools-0.5.0/tests/test-files/test-firmware.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/test-storage-area.bin` & `gp2040ce-binary-tools-0.5.0/tests/test-files/test-storage-area.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test-files/test-whole-board.bin` & `gp2040ce-binary-tools-0.5.0/tests/test-files/test-whole-board.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test_builder.py` & `gp2040ce-binary-tools-0.5.0/tests/test_builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import sys
 import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 
 from gp2040ce_bintools import get_config_pb2
-from gp2040ce_bintools.builder import (FirmwareLengthError, combine_firmware_and_config, pad_firmware_up_to_storage,
-                                       replace_config_in_binary, write_new_config_to_filename, write_new_config_to_usb)
+from gp2040ce_bintools.builder import (FirmwareLengthError, combine_firmware_and_config,
+                                       concatenate_firmware_and_storage_files, get_gp2040ce_from_usb,
+                                       pad_firmware_up_to_storage, replace_config_in_binary,
+                                       write_new_config_to_filename, write_new_config_to_usb)
 from gp2040ce_bintools.storage import get_config, get_config_footer, get_storage_section, serialize_config_with_footer
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
 @decorator
 def with_pb2s(test, *args, **kwargs):
@@ -22,20 +24,50 @@
 
     test(*args, **kwargs)
 
     sys.path.pop()
     del sys.modules['config_pb2']
 
 
+def test_concatenate_to_file(tmp_path):
+    """Test that we write a file as expected."""
+    tmp_file = os.path.join(tmp_path, 'concat.bin')
+    firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
+    config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
+    concatenate_firmware_and_storage_files(firmware_file, config_file, combined_filename=tmp_file)
+    with open(tmp_file, 'rb') as file:
+        content = file.read()
+    assert len(content) == 2 * 1024 * 1024
+
+
+def test_concatenate_to_usb(tmp_path):
+    """Test that we write a file as expected."""
+    firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
+    config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
+    end_out, end_in = mock.MagicMock(), mock.MagicMock()
+    with mock.patch('gp2040ce_bintools.builder.get_bootsel_endpoints', return_value=(end_out, end_in)):
+        with mock.patch('gp2040ce_bintools.builder.write') as mock_write:
+            concatenate_firmware_and_storage_files(firmware_file, config_file, usb=True)
+
+    assert mock_write.call_args.args[2] == 0x10000000
+    assert len(mock_write.call_args.args[3]) == 2 * 1024 * 1024
+
+
 def test_padding_firmware(firmware_binary):
     """Test that firmware is padded to the expected size."""
     padded = pad_firmware_up_to_storage(firmware_binary)
     assert len(padded) == 2088960
 
 
+def test_padding_firmware_can_truncate():
+    """Test that firmware is padded to the expected size."""
+    padded = pad_firmware_up_to_storage(bytearray(b'\x00' * 4 * 1024 * 1024), or_truncate=True)
+    assert len(padded) == 2088960
+
+
 def test_firmware_plus_storage(firmware_binary, storage_dump):
     """Test that combining firmware and storage produces a valid combined binary."""
     whole_board = combine_firmware_and_config(firmware_binary, storage_dump)
     # if this is valid, we should be able to find the storage and footer again
     storage = get_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 2032
@@ -46,14 +78,23 @@
     whole_board = combine_firmware_and_config(firmware_binary, config_binary)
     # if this is valid, we should be able to find the storage and footer again
     storage = get_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 2032
 
 
+def test_chunky_firmware_plus_config_binary(config_binary):
+    """Test that combining giant firmware and storage produces a valid combined binary."""
+    whole_board = combine_firmware_and_config(bytearray(b'\x00' * 4 * 1024 * 1024), config_binary, replace_extra=True)
+    # if this is valid, we should be able to find the storage and footer again
+    storage = get_storage_section(whole_board)
+    footer_size, _, _ = get_config_footer(storage)
+    assert footer_size == 2032
+
+
 def test_replace_config_in_binary(config_binary):
     """Test that a config binary is placed in the storage location of a source binary to overwrite."""
     whole_board = replace_config_in_binary(bytearray(b'\x00' * 3 * 1024 * 1024), config_binary)
     assert len(whole_board) == 3 * 1024 * 1024
     # if this is valid, we should be able to find the storage and footer again
     storage = get_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
@@ -143,10 +184,27 @@
     config = get_config(config_binary)
     serialized = serialize_config_with_footer(config)
     end_out, end_in = mock.MagicMock(), mock.MagicMock()
     with mock.patch('gp2040ce_bintools.builder.write') as mock_write:
         write_new_config_to_usb(config, end_out, end_in)
 
     # check that it got padded
-    padded_serialized = bytearray(b'\x00' * 4) + serialized
-    assert mock_write.call_args.args[2] % 256 == 0
+    assert len(serialized) == 2044
+    padded_serialized = bytearray(b'\x00' * 2052) + serialized
+    assert mock_write.call_args.args[2] % 4096 == 0
     assert mock_write.call_args.args[3] == padded_serialized
+
+
+def test_get_gp2040ce_from_usb():
+    """Test we attempt to read from the proper location over USB."""
+    mock_out = mock.MagicMock()
+    mock_out.device.idVendor = 0xbeef
+    mock_out.device.idProduct = 0xcafe
+    mock_out.device.bus = 1
+    mock_out.device.address = 2
+    mock_in = mock.MagicMock()
+    with mock.patch('gp2040ce_bintools.builder.get_bootsel_endpoints', return_value=(mock_out, mock_in)) as mock_get:
+        with mock.patch('gp2040ce_bintools.builder.read') as mock_read:
+            config, _, _ = get_gp2040ce_from_usb()
+
+    mock_get.assert_called_once()
+    mock_read.assert_called_with(mock_out, mock_in, 0x10000000, 2 * 1024 * 1024)
```

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test_commands.py` & `gp2040ce-binary-tools-0.5.0/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     assert 'Read the configuration section from a dump of a GP2040-CE board' in result.stdout
 
 
 def test_concatenate_invocation(tmpdir):
     """Test that a normal invocation against a dump works."""
     out_filename = os.path.join(tmpdir, 'out.bin')
     _ = run(['concatenate', 'tests/test-files/test-firmware.bin', 'tests/test-files/test-storage-area.bin',
-             out_filename])
+             '--new-binary-filename', out_filename])
     with open(out_filename, 'rb') as out_file, open('tests/test-files/test-storage-area.bin', 'rb') as storage_file:
         out = out_file.read()
         storage = storage_file.read()
     assert out[2088960:2097152] == storage
 
 
 def test_storage_dump_invocation():
```

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test_gui.py` & `gp2040ce-binary-tools-0.5.0/tests/test_gui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Test the Textual GUI."""
 import os
 import sys
+import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 from textual.widgets import Tree
 
+from gp2040ce_bintools import get_config_pb2
 from gp2040ce_bintools.gui import ConfigEditor
-from gp2040ce_bintools.storage import get_config_from_file
+from gp2040ce_bintools.storage import ConfigReadError, get_config, get_config_from_file
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
 @decorator
 async def with_pb2s(test, *args, **kwargs):
     """Wrap a test with precompiled pb2 files on the path."""
@@ -22,14 +24,55 @@
 
     sys.path.pop()
     del sys.modules['config_pb2']
 
 
 @pytest.mark.asyncio
 @with_pb2s
+async def test_load_configs():
+    """Test a variety of ways the editor may get initialized."""
+    test_config_filename = os.path.join(HERE, 'test-files/test-config.bin')
+    empty_config = get_config_pb2().Config()
+    with open(test_config_filename, 'rb') as file_:
+        test_config_binary = file_.read()
+    test_config = get_config(test_config_binary)
+
+    app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-config.bin'))
+    assert app.config == test_config
+
+    app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-config.binooooooo'), create_new=True)
+    assert app.config == empty_config
+
+    with pytest.raises(FileNotFoundError):
+        app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-config.binooooooo'))
+
+    app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-firmware.bin'), create_new=True)
+    assert app.config == empty_config
+
+    with pytest.raises(ConfigReadError):
+        app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-firmware.bin'))
+
+    with mock.patch('gp2040ce_bintools.gui.get_bootsel_endpoints', return_value=(mock.MagicMock(), mock.MagicMock())):
+        with mock.patch('gp2040ce_bintools.gui.read', return_value=b'\x00'):
+            with pytest.raises(ConfigReadError):
+                app = ConfigEditor(usb=True)
+
+    with mock.patch('gp2040ce_bintools.gui.get_bootsel_endpoints', return_value=(mock.MagicMock(), mock.MagicMock())):
+        with mock.patch('gp2040ce_bintools.gui.read', return_value=b'\x00'):
+            app = ConfigEditor(usb=True, create_new=True)
+    assert app.config == empty_config
+
+    with mock.patch('gp2040ce_bintools.gui.get_bootsel_endpoints', return_value=(mock.MagicMock(), mock.MagicMock())):
+        with mock.patch('gp2040ce_bintools.gui.read', return_value=test_config_binary):
+            app = ConfigEditor(usb=True)
+    assert app.config == test_config
+
+
+@pytest.mark.asyncio
+@with_pb2s
 async def test_simple_tree_building():
     """Test some basics of the config tree being built."""
     app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-config.bin'))
     async with app.run_test() as pilot:
         check_node = pilot.app.query_one(Tree).root.children[2]
         assert "boardVersion = 'v0.7.2'" in check_node.label
         parent_config, field_descriptor, field_value = check_node.data
```

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test_package.py` & `gp2040ce-binary-tools-0.5.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test_pico.py` & `gp2040ce-binary-tools-0.5.0/tests/test_pico.py`

 * *Files 12% similar despite different names*

```diff
@@ -174,21 +174,42 @@
     end_out, end_in = mock.MagicMock(), mock.MagicMock()
     _ = pico.write(end_out, end_in, 0x101FE000, b'\x00\x01\x02\x03')
 
     expected_writes = [
         mock.call(struct.pack('<LLBBxxLL12x', 0x431fd10b, 1, 0x1, 1, 0, 1)),
         mock.call(struct.pack('<LLBBxxL16x', 0x431fd10b, 1, 0x6, 0, 0)),
         mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x3, 8, 0, 0x101FE000, 4)),
-        mock.call(struct.pack('<LLBBxxL16x', 0x431fd10b, 1, 0x6, 0, 0)),
         mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x5, 8, 4, 0x101FE000, 4)),
         mock.call(b'\x00\x01\x02\x03'),
         mock.call(struct.pack('<LLBBxxLL12x', 0x431fd10b, 1, 0x1, 1, 0, 0)),
     ]
     end_out.write.assert_has_calls(expected_writes)
-    assert end_in.read.call_count == 6
+    assert end_in.read.call_count == 5
+
+
+def test_write_chunked():
+    """Test that we can write to a board in BOOTSEL mode."""
+    end_out, end_in = mock.MagicMock(), mock.MagicMock()
+    payload = bytearray(b'\x00\x01\x02\x03' * 1024)
+    _ = pico.write(end_out, end_in, 0x10100000, payload * 2)
+
+    expected_writes = [
+        mock.call(struct.pack('<LLBBxxLL12x', 0x431fd10b, 1, 0x1, 1, 0, 1)),
+        mock.call(struct.pack('<LLBBxxL16x', 0x431fd10b, 1, 0x6, 0, 0)),
+        mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x3, 8, 0, 0x10100000, 4096)),
+        mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x5, 8, 4096, 0x10100000, 4096)),
+        mock.call(bytes(payload)),
+        mock.call(struct.pack('<LLBBxxL16x', 0x431fd10b, 1, 0x6, 0, 0)),
+        mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x3, 8, 0, 0x10100000 + 4096, 4096)),
+        mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x5, 8, 4096, 0x10100000 + 4096, 4096)),
+        mock.call(bytes(payload)),
+        mock.call(struct.pack('<LLBBxxLL12x', 0x431fd10b, 1, 0x1, 1, 0, 0)),
+    ]
+    end_out.write.assert_has_calls(expected_writes)
+    assert end_in.read.call_count == 8
 
 
 def test_misaligned_write():
     """Test that we can't write to a board at invalid memory addresses."""
     end_out, end_in = mock.MagicMock(), mock.MagicMock()
     with pytest.raises(pico.PicoAlignmentError):
         _ = pico.write(end_out, end_in, 0x101FE001, b'\x00\x01\x02\x03')
@@ -201,20 +222,24 @@
     with pytest.raises(pico.PicoAlignmentError):
         _ = pico.write(end_out, end_in, 0x101FE040, b'\x00\x01\x02\x03')
     with pytest.raises(pico.PicoAlignmentError):
         _ = pico.write(end_out, end_in, 0x101FE080, b'\x00\x01\x02\x03')
     with pytest.raises(pico.PicoAlignmentError):
         _ = pico.write(end_out, end_in, 0x101FE0FF, b'\x00\x01\x02\x03')
 
-    _ = pico.write(end_out, end_in, 0x101FE100, b'\x00\x01\x02\x03')
+    # 256 byte alignment is what is desired, but see comments around there for
+    # why only 4096 seems to work right...
+    with pytest.raises(pico.PicoAlignmentError):
+        _ = pico.write(end_out, end_in, 0x101FE100, b'\x00\x01\x02\x03')
+
+    _ = pico.write(end_out, end_in, 0x101FF000, b'\x00\x01\x02\x03')
 
     expected_writes = [
         mock.call(struct.pack('<LLBBxxLL12x', 0x431fd10b, 1, 0x1, 1, 0, 1)),
         mock.call(struct.pack('<LLBBxxL16x', 0x431fd10b, 1, 0x6, 0, 0)),
-        mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x3, 8, 0, 0x101FE100, 4)),
-        mock.call(struct.pack('<LLBBxxL16x', 0x431fd10b, 1, 0x6, 0, 0)),
-        mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x5, 8, 4, 0x101FE100, 4)),
+        mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x3, 8, 0, 0x101FF000, 4)),
+        mock.call(struct.pack('<LLBBxxLLL8x', 0x431fd10b, 1, 0x5, 8, 4, 0x101FF000, 4)),
         mock.call(b'\x00\x01\x02\x03'),
         mock.call(struct.pack('<LLBBxxLL12x', 0x431fd10b, 1, 0x1, 1, 0, 0)),
     ]
     end_out.write.assert_has_calls(expected_writes)
-    assert end_in.read.call_count == 6
+    assert end_in.read.call_count == 5
```

### Comparing `gp2040ce-binary-tools-0.4.0/tests/test_storage.py` & `gp2040ce-binary-tools-0.5.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.4.0/tox.ini` & `gp2040ce-binary-tools-0.5.0/tox.ini`

 * *Files identical despite different names*

