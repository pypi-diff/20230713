# Comparing `tmp/sayswho-0.1.0.tar.gz` & `tmp/sayswho-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayswho-0.1.0.tar", max compression
+gzip compressed data, was "sayswho-0.1.1.tar", max compression
```

## Comparing `sayswho-0.1.0.tar` & `sayswho-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6691 2023-07-13 01:44:10.471016 sayswho-0.1.0/README.md
--rw-r--r--   0        0        0      328 2023-07-13 01:19:10.697193 sayswho-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 15:12:54.639435 sayswho-0.1.0/src/sayswho/__init__.py
--rw-r--r--   0        0        0     9717 2023-07-12 21:53:15.324024 sayswho-0.1.0/src/sayswho/attribution_helpers.py
--rw-r--r--   0        0        0     2540 2023-07-07 00:46:44.215252 sayswho-0.1.0/src/sayswho/constants.py
--rw-r--r--   0        0        0     5292 2023-07-12 22:02:43.820694 sayswho-0.1.0/src/sayswho/quote_helpers.py
--rw-r--r--   0        0        0     7670 2023-07-12 20:55:04.784484 sayswho-0.1.0/src/sayswho/quotes.py
--rw-r--r--   0        0        0     5884 2023-07-13 01:25:00.345184 sayswho-0.1.0/src/sayswho/sayswho.py
--rw-r--r--   0        0        0     7205 1970-01-01 00:00:00.000000 sayswho-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5550 2023-07-13 20:59:18.464577 sayswho-0.1.1/README.md
+-rw-r--r--   0        0        0      505 2023-07-13 21:12:45.529345 sayswho-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 15:12:54.639435 sayswho-0.1.1/src/sayswho/__init__.py
+-rw-r--r--   0        0        0     9717 2023-07-12 21:53:15.324024 sayswho-0.1.1/src/sayswho/attribution_helpers.py
+-rw-r--r--   0        0        0     2540 2023-07-07 00:46:44.215252 sayswho-0.1.1/src/sayswho/constants.py
+-rw-r--r--   0        0        0     5292 2023-07-12 22:02:43.820694 sayswho-0.1.1/src/sayswho/quote_helpers.py
+-rw-r--r--   0        0        0     7670 2023-07-12 20:55:04.784484 sayswho-0.1.1/src/sayswho/quotes.py
+-rw-r--r--   0        0        0     5884 2023-07-13 01:25:00.345184 sayswho-0.1.1/src/sayswho/sayswho.py
+-rw-r--r--   0        0        0     6341 1970-01-01 00:00:00.000000 sayswho-0.1.1/PKG-INFO
```

### Comparing `sayswho-0.1.0/src/sayswho/attribution_helpers.py` & `sayswho-0.1.1/src/sayswho/attribution_helpers.py`

 * *Files identical despite different names*

### Comparing `sayswho-0.1.0/src/sayswho/constants.py` & `sayswho-0.1.1/src/sayswho/constants.py`

 * *Files identical despite different names*

### Comparing `sayswho-0.1.0/src/sayswho/quote_helpers.py` & `sayswho-0.1.1/src/sayswho/quote_helpers.py`

 * *Files identical despite different names*

### Comparing `sayswho-0.1.0/src/sayswho/quotes.py` & `sayswho-0.1.1/src/sayswho/quotes.py`

 * *Files identical despite different names*

### Comparing `sayswho-0.1.0/src/sayswho/sayswho.py` & `sayswho-0.1.1/src/sayswho/sayswho.py`

 * *Files identical despite different names*

