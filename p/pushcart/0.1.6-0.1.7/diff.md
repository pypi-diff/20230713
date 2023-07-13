# Comparing `tmp/pushcart-0.1.6.tar.gz` & `tmp/pushcart-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart-0.1.6.tar", max compression
+gzip compressed data, was "pushcart-0.1.7.tar", max compression
```

## Comparing `pushcart-0.1.6.tar` & `pushcart-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-01-06 07:28:13.250337 pushcart-0.1.6/LICENSE
--rw-r--r--   0        0        0       70 2023-01-06 07:28:13.250337 pushcart-0.1.6/README.md
--rw-r--r--   0        0        0      694 2023-01-06 07:28:13.250337 pushcart-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      780 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/__init__.py
--rw-r--r--   0        0        0      192 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/configuration/__init__.py
--rw-r--r--   0        0        0      521 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/configuration/delta.py
--rw-r--r--   0        0        0     4505 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/configuration/pipeline.py
--rw-r--r--   0        0        0      104 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/configuration/presets/pipeline.py
--rw-r--r--   0        0        0     5871 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/configuration/presets/release.py
--rw-r--r--   0        0        0      521 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/configuration/table.py
--rw-r--r--   0        0        0      251 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/configuration/validation/__init__.py
--rw-r--r--   0        0        0    10095 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/configuration/validation/common.py
--rw-r--r--   0        0        0     2003 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/dbutils.py
--rw-r--r--   0        0        0     1657 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/pipeline.py
--rw-r--r--   0        0        0    11145 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/release.py
--rw-r--r--   0        0        0      130 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/sources/__init__.py
--rw-r--r--   0        0        0      259 2023-01-06 07:28:13.250337 pushcart-0.1.6/src/pushcart/sources/table.py
--rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 pushcart-0.1.6/setup.py
--rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 pushcart-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-08 07:35:44.283369 pushcart-0.1.7/LICENSE
+-rw-r--r--   0        0        0       80 2023-07-08 07:35:44.303369 pushcart-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 07:34:25.976683 pushcart-0.1.7/pushcart/__init__.py
+-rw-r--r--   0        0        0    13589 2023-07-13 19:37:18.998215 pushcart-0.1.7/pushcart/metadata.py
+-rw-r--r--   0        0        0     1318 2023-07-13 08:57:41.740193 pushcart-0.1.7/pushcart/utils.py
+-rw-r--r--   0        0        0     2543 2023-07-13 19:41:53.261558 pushcart-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 pushcart-0.1.7/PKG-INFO
```

### Comparing `pushcart-0.1.6/LICENSE` & `pushcart-0.1.7/LICENSE`

 * *Files identical despite different names*

