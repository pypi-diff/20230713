# Comparing `tmp/skale-contracts-0.0.1.dev678421197680222296.tar.gz` & `tmp/skale-contracts-0.0.1.dev8027846711168070537.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale-contracts-0.0.1.dev678421197680222296.tar", last modified: Wed Jul 12 14:56:04 2023, max compression
+gzip compressed data, was "skale-contracts-0.0.1.dev8027846711168070537.tar", last modified: Thu Jul 13 13:52:38 2023, max compression
```

## Comparing `skale-contracts-0.0.1.dev678421197680222296.tar` & `skale-contracts-0.0.1.dev8027846711168070537.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:56:04.266351 skale-contracts-0.0.1.dev678421197680222296/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-12 14:56:04.266351 skale-contracts-0.0.1.dev678421197680222296/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 14:55:49.000000 skale-contracts-0.0.1.dev678421197680222296/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 14:55:49.000000 skale-contracts-0.0.1.dev678421197680222296/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-12 14:56:04.266351 skale-contracts-0.0.1.dev678421197680222296/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:56:04.266351 skale-contracts-0.0.1.dev678421197680222296/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:56:04.266351 skale-contracts-0.0.1.dev678421197680222296/src/skale_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-12 14:56:04.000000 skale-contracts-0.0.1.dev678421197680222296/src/skale_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 14:56:04.000000 skale-contracts-0.0.1.dev678421197680222296/src/skale_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:56:04.000000 skale-contracts-0.0.1.dev678421197680222296/src/skale_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 14:56:04.000000 skale-contracts-0.0.1.dev678421197680222296/src/skale_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:56:04.000000 skale-contracts-0.0.1.dev678421197680222296/src/skale_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 14:55:57.000000 skale-contracts-0.0.1.dev678421197680222296/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:52:38.562816 skale-contracts-0.0.1.dev8027846711168070537/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-13 13:52:38.562816 skale-contracts-0.0.1.dev8027846711168070537/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 13:52:20.000000 skale-contracts-0.0.1.dev8027846711168070537/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 13:52:20.000000 skale-contracts-0.0.1.dev8027846711168070537/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-13 13:52:38.566816 skale-contracts-0.0.1.dev8027846711168070537/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:52:38.562816 skale-contracts-0.0.1.dev8027846711168070537/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:52:38.562816 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 13:52:29.000000 skale-contracts-0.0.1.dev8027846711168070537/version.txt
```

### Comparing `skale-contracts-0.0.1.dev678421197680222296/PKG-INFO` & `skale-contracts-0.0.1.dev8027846711168070537/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 0.0.1.dev678421197680222296
+Version: 0.0.1.dev8027846711168070537
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale-contracts-0.0.1.dev678421197680222296/setup.cfg` & `skale-contracts-0.0.1.dev8027846711168070537/setup.cfg`

 * *Files identical despite different names*

### Comparing `skale-contracts-0.0.1.dev678421197680222296/src/skale_contracts.egg-info/PKG-INFO` & `skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 0.0.1.dev678421197680222296
+Version: 0.0.1.dev8027846711168070537
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

