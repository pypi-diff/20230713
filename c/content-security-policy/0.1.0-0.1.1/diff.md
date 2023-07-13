# Comparing `tmp/content_security_policy-0.1.0.tar.gz` & `tmp/content_security_policy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "content_security_policy-0.1.0.tar", max compression
+gzip compressed data, was "content_security_policy-0.1.1.tar", max compression
```

## Comparing `content_security_policy-0.1.0.tar` & `content_security_policy-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,23 @@
--rw-r--r--   0        0        0        0 2023-06-30 11:54:25.522623 content_security_policy-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-30 11:52:48.818470 content_security_policy-0.1.0/content_security_policy/__init__.py
--rw-r--r--   0        0        0      278 2023-06-30 11:54:56.016215 content_security_policy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 content_security_policy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-10 13:55:31.659648 content_security_policy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4038 2023-07-13 10:01:58.088186 content_security_policy-0.1.1/README.md
+-rw-r--r--   0        0        0      224 2023-07-12 16:56:24.453214 content_security_policy-0.1.1/content_security_policy/__init__.py
+-rw-r--r--   0        0        0    10837 2023-07-13 10:02:57.541729 content_security_policy-0.1.1/content_security_policy/base_classes.py
+-rw-r--r--   0        0        0     2124 2023-07-12 16:59:09.394212 content_security_policy-0.1.1/content_security_policy/constants.py
+-rw-r--r--   0        0        0     4619 2023-07-13 10:02:38.701662 content_security_policy-0.1.1/content_security_policy/directives.py
+-rw-r--r--   0        0        0      341 2023-07-11 06:46:33.557664 content_security_policy-0.1.1/content_security_policy/exceptions.py
+-rw-r--r--   0        0        0     3884 2023-07-13 09:44:20.601790 content_security_policy-0.1.1/content_security_policy/parse.py
+-rw-r--r--   0        0        0     5544 2023-07-13 09:01:51.089047 content_security_policy-0.1.1/content_security_policy/patterns.py
+-rw-r--r--   0        0        0     1476 2023-07-05 19:33:38.880448 content_security_policy-0.1.1/content_security_policy/test/__pycache__/test_directives.cpython-311.pyc
+-rw-r--r--   0        0        0     2854 2023-07-12 21:53:07.512121 content_security_policy-0.1.1/content_security_policy/test/__pycache__/test_parsing.cpython-311.pyc
+-rw-r--r--   0        0        0    10842 2023-07-13 10:01:59.724859 content_security_policy-0.1.1/content_security_policy/test/__pycache__/test_policy.cpython-311.pyc
+-rw-r--r--   0        0        0     3312 2023-07-13 08:16:16.620689 content_security_policy-0.1.1/content_security_policy/test/__pycache__/test_source_list_directives.cpython-311.pyc
+-rw-r--r--   0        0        0     3289 2023-07-12 14:49:31.496701 content_security_policy-0.1.1/content_security_policy/test/__pycache__/test_values.cpython-311.pyc
+-rw-r--r--   0        0        0      595 2023-07-05 19:28:34.286675 content_security_policy-0.1.1/content_security_policy/test/test_directives.py
+-rw-r--r--   0        0        0     1680 2023-07-12 21:51:31.774951 content_security_policy-0.1.1/content_security_policy/test/test_parsing.py
+-rw-r--r--   0        0        0     5108 2023-07-13 10:01:58.058186 content_security_policy-0.1.1/content_security_policy/test/test_policy.py
+-rw-r--r--   0        0        0     1185 2023-07-13 09:44:20.565123 content_security_policy-0.1.1/content_security_policy/test/test_source_list_directives.py
+-rw-r--r--   0        0        0     1290 2023-07-12 14:49:18.963366 content_security_policy-0.1.1/content_security_policy/test/test_values.py
+-rw-r--r--   0        0        0      905 2023-07-13 08:06:11.533259 content_security_policy-0.1.1/content_security_policy/utils.py
+-rw-r--r--   0        0        0    10465 2023-07-12 21:53:01.408756 content_security_policy-0.1.1/content_security_policy/values.py
+-rw-r--r--   0        0        0      397 2023-07-13 10:08:41.726341 content_security_policy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4500 1970-01-01 00:00:00.000000 content_security_policy-0.1.1/PKG-INFO
```

