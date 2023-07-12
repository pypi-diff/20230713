# Comparing `tmp/efrem_utils-0.0.2.tar.gz` & `tmp/efrem_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.0.2.tar", max compression
+gzip compressed data, was "efrem_utils-0.0.4.tar", max compression
```

## Comparing `efrem_utils-0.0.2.tar` & `efrem_utils-0.0.4.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      936 2023-07-12 18:37:07.019654 efrem_utils-0.0.2/efrem_utils.py
--rw-r--r--   0        0        0      299 2023-07-12 18:39:13.218589 efrem_utils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      104 2023-07-12 18:35:53.881437 efrem_utils-0.0.2/README.md
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 efrem_utils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2172 2023-07-12 23:36:57.351657 efrem_utils-0.0.4/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-12 23:00:01.757005 efrem_utils-0.0.4/LICENSE
+-rw-r--r--   0        0        0      299 2023-07-12 23:38:05.880367 efrem_utils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      191 2023-07-12 23:33:11.941559 efrem_utils-0.0.4/README.md
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 efrem_utils-0.0.4/PKG-INFO
```

