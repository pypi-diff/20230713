# Comparing `tmp/python-payfast-0.3.tar.gz` & `tmp/python-payfast-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-payfast-0.3.tar", last modified: Thu Jul 13 11:08:02 2023, max compression
+gzip compressed data, was "python-payfast-0.5.tar", last modified: Thu Jul 13 15:09:26 2023, max compression
```

## Comparing `python-payfast-0.3.tar` & `python-payfast-0.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.941416 python-payfast-0.3/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-06-06 20:50:53.000000 python-payfast-0.3/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       72 2023-06-12 19:59:05.000000 python-payfast-0.3/MANIFEST.in
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 11:08:02.941416 python-payfast-0.3/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      143 2023-07-12 09:54:32.000000 python-payfast-0.3/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/payfast/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2438 2023-07-13 11:07:33.000000 python-payfast-0.3/payfast/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/payfast/api/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-07 11:51:53.000000 python-payfast-0.3/payfast/api/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      533 2023-06-21 18:57:35.000000 python-payfast-0.3/payfast/api/refunds.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    27538 2023-07-13 11:06:53.000000 python-payfast-0.3/payfast/api/subscriptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8005 2023-06-21 18:48:00.000000 python-payfast-0.3/payfast/api/transactions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      566 2023-06-12 19:22:21.000000 python-payfast-0.3/payfast/apps.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6188 2023-07-10 13:53:24.000000 python-payfast-0.3/payfast/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2614 2023-07-12 07:27:56.000000 python-payfast-0.3/payfast/callbacks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7060 2023-07-12 07:29:04.000000 python-payfast-0.3/payfast/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1210 2023-07-10 13:24:31.000000 python-payfast-0.3/payfast/constants.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2188 2023-07-10 14:27:12.000000 python-payfast-0.3/payfast/decorators.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1908 2023-06-21 19:24:26.000000 python-payfast-0.3/payfast/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    11812 2023-07-10 14:13:51.000000 python-payfast-0.3/payfast/itn.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      251 2023-06-21 18:47:03.000000 python-payfast-0.3/payfast/logging.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15853 2023-07-11 07:47:49.000000 python-payfast-0.3/payfast/payment.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2111 2023-06-08 18:38:43.000000 python-payfast-0.3/payfast/security_checks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3313 2023-07-10 14:21:32.000000 python-payfast-0.3/payfast/serialization.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      376 2023-06-19 18:50:19.000000 python-payfast-0.3/payfast/signals.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2761 2023-06-15 13:28:20.000000 python-payfast-0.3/payfast/signature.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.933416 python-payfast-0.3/payfast/templates/
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/payfast/templates/payfast/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      285 2023-07-10 12:50:03.000000 python-payfast-0.3/payfast/templates/payfast/form.html
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      299 2023-06-12 20:32:31.000000 python-payfast-0.3/payfast/templates/payfast/sandbox.html
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      419 2023-07-10 12:49:49.000000 python-payfast-0.3/payfast/templates.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      544 2023-06-14 16:50:45.000000 python-payfast-0.3/payfast/timezone.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      618 2023-06-13 13:20:57.000000 python-payfast-0.3/payfast/urls.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     4071 2023-07-12 08:10:34.000000 python-payfast-0.3/payfast/utils.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1577 2023-07-12 08:09:37.000000 python-payfast-0.3/payfast/validation.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5009 2023-07-10 13:58:41.000000 python-payfast-0.3/payfast/views.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/python_payfast.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1215 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      102 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-07-13 11:08:02.941416 python-payfast-0.3/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1804 2023-06-15 12:19:47.000000 python-payfast-0.3/setup.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/tests/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-06 18:42:13.000000 python-payfast-0.3/tests/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.941416 python-payfast-0.3/tests/api/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:55:21.000000 python-payfast-0.3/tests/api/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      436 2023-06-12 18:51:32.000000 python-payfast-0.3/tests/api/test_subscriptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      563 2023-06-12 18:11:31.000000 python-payfast-0.3/tests/api/test_transactions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:58.000000 python-payfast-0.3/tests/test_base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:53.000000 python-payfast-0.3/tests/test_callbacks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:58.000000 python-payfast-0.3/tests/test_conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:35.000000 python-payfast-0.3/tests/test_constants.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:02:08.000000 python-payfast-0.3/tests/test_exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1541 2023-07-12 09:51:05.000000 python-payfast-0.3/tests/test_itn.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      300 2023-06-12 18:51:58.000000 python-payfast-0.3/tests/test_payfast.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      431 2023-06-12 19:22:34.000000 python-payfast-0.3/tests/test_payment.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:36.000000 python-payfast-0.3/tests/test_security_checks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:46.000000 python-payfast-0.3/tests/test_signature.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:05.000000 python-payfast-0.3/tests/test_templates.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:20.000000 python-payfast-0.3/tests/test_timezone.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:26.000000 python-payfast-0.3/tests/test_utils.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.181051 python-payfast-0.5/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-06-06 20:50:53.000000 python-payfast-0.5/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       72 2023-06-12 19:59:05.000000 python-payfast-0.5/MANIFEST.in
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 15:09:26.177051 python-payfast-0.5/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      143 2023-07-12 09:54:32.000000 python-payfast-0.5/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.173051 python-payfast-0.5/payfast/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2441 2023-07-13 15:08:36.000000 python-payfast-0.5/payfast/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.173051 python-payfast-0.5/payfast/api/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-07 11:51:53.000000 python-payfast-0.5/payfast/api/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      533 2023-06-21 18:57:35.000000 python-payfast-0.5/payfast/api/refunds.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    27368 2023-07-13 14:36:03.000000 python-payfast-0.5/payfast/api/subscriptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8005 2023-06-21 18:48:00.000000 python-payfast-0.5/payfast/api/transactions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      566 2023-06-12 19:22:21.000000 python-payfast-0.5/payfast/apps.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6242 2023-07-13 15:00:50.000000 python-payfast-0.5/payfast/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2614 2023-07-12 07:27:56.000000 python-payfast-0.5/payfast/callbacks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7301 2023-07-13 15:08:13.000000 python-payfast-0.5/payfast/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1210 2023-07-10 13:24:31.000000 python-payfast-0.5/payfast/constants.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2188 2023-07-10 14:27:12.000000 python-payfast-0.5/payfast/decorators.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1908 2023-06-21 19:24:26.000000 python-payfast-0.5/payfast/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    11812 2023-07-10 14:13:51.000000 python-payfast-0.5/payfast/itn.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      251 2023-06-21 18:47:03.000000 python-payfast-0.5/payfast/logging.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15833 2023-07-13 13:57:00.000000 python-payfast-0.5/payfast/payment.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2111 2023-06-08 18:38:43.000000 python-payfast-0.5/payfast/security_checks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3308 2023-07-13 13:57:13.000000 python-payfast-0.5/payfast/serialization.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      376 2023-06-19 18:50:19.000000 python-payfast-0.5/payfast/signals.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2761 2023-06-15 13:28:20.000000 python-payfast-0.5/payfast/signature.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.169051 python-payfast-0.5/payfast/templates/
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.173051 python-payfast-0.5/payfast/templates/payfast/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      285 2023-07-10 12:50:03.000000 python-payfast-0.5/payfast/templates/payfast/form.html
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      299 2023-06-12 20:32:31.000000 python-payfast-0.5/payfast/templates/payfast/sandbox.html
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      419 2023-07-10 12:49:49.000000 python-payfast-0.5/payfast/templates.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      544 2023-06-14 16:50:45.000000 python-payfast-0.5/payfast/timezone.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      618 2023-06-13 13:20:57.000000 python-payfast-0.5/payfast/urls.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     4071 2023-07-12 08:10:34.000000 python-payfast-0.5/payfast/utils.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1577 2023-07-12 08:09:37.000000 python-payfast-0.5/payfast/validation.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5009 2023-07-10 13:58:41.000000 python-payfast-0.5/payfast/views.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.177051 python-payfast-0.5/python_payfast.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1215 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      102 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-07-13 15:09:26.181051 python-payfast-0.5/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1804 2023-06-15 12:19:47.000000 python-payfast-0.5/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.177051 python-payfast-0.5/tests/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-06 18:42:13.000000 python-payfast-0.5/tests/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.177051 python-payfast-0.5/tests/api/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:55:21.000000 python-payfast-0.5/tests/api/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      436 2023-06-12 18:51:32.000000 python-payfast-0.5/tests/api/test_subscriptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      563 2023-06-12 18:11:31.000000 python-payfast-0.5/tests/api/test_transactions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:58.000000 python-payfast-0.5/tests/test_base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:53.000000 python-payfast-0.5/tests/test_callbacks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:58.000000 python-payfast-0.5/tests/test_conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:35.000000 python-payfast-0.5/tests/test_constants.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:02:08.000000 python-payfast-0.5/tests/test_exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1541 2023-07-12 09:51:05.000000 python-payfast-0.5/tests/test_itn.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      300 2023-06-12 18:51:58.000000 python-payfast-0.5/tests/test_payfast.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      431 2023-06-12 19:22:34.000000 python-payfast-0.5/tests/test_payment.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:36.000000 python-payfast-0.5/tests/test_security_checks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:46.000000 python-payfast-0.5/tests/test_signature.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:05.000000 python-payfast-0.5/tests/test_templates.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:20.000000 python-payfast-0.5/tests/test_timezone.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:26.000000 python-payfast-0.5/tests/test_utils.py
```

### Comparing `python-payfast-0.3/LICENSE` & `python-payfast-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/PKG-INFO` & `python-payfast-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-payfast
-Version: 0.3
+Version: 0.5
 Summary: A very opinionated Python client library for the PayFast API.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-payfast-0.3/payfast/__init__.py` & `python-payfast-0.5/payfast/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     SubscriptionPayment,
     TokenizedPayment,
     TokenizedSub,
 )
 from payfast.base import RequestsTransport
 from payfast.logging import configure_logging
 from payfast.exceptions import PayFastException
-from payfast.api.subscriptions import Subscriptions, Card
+from payfast.api.subscriptions import Subscriptions, Cards
 from payfast.api.transactions import Transactions, CCTransactions
 from payfast.api.refunds import Refunds
 
 
 
 
-__version__ = '0.3'
+__version__ = '0.5'
 __title__ = 'python-payfast'
 
 
 
 
 class PayFast:
 
@@ -41,15 +41,15 @@
         self.base_uri = settings.API_ROOT
         self.api_version = version
         args = [version]
         kwargs = {'transport_class': self.TRANSPORT_CLASS}
 
         self.subscriptions = Subscriptions(*args, **kwargs)
         self.subs = Subscriptions(*args, **kwargs) # alias
-        self.card = Card(*args, **kwargs)
+        self.cards = Cards(*args, **kwargs)
 
         self.transactions = Transactions(*args, **kwargs)
         self.cc_transactions = CCTransactions(*args, **kwargs)
 
         self.refunds = Refunds(*args, **kwargs)
         self.refund = self.refunds.create # alias
```

### Comparing `python-payfast-0.3/payfast/api/refunds.py` & `python-payfast-0.5/payfast/api/refunds.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/api/subscriptions.py` & `python-payfast-0.5/payfast/api/subscriptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,41 +238,29 @@
             # REMOVE HACK
             return self.sub.cancel()
         return self.sub.update(amount=self.amount)
 
 
 
 
-class Subscription:
+class SubscriptionBase:
 
     def __init__(self, data):
         if not isinstance(data, dict):
             # The data argument would generally come straight from the
             # RequestsTransport response. Therefore, if the transport
             # somehow handles the response incorrectly a boolean or
             # some other type might be used instead of a dictionary.
             raise ValueError(
                 '"data" argument for "Subscription" must be a dictionary.'
             )
 
         self.data = data
-        fields = [
-            'amount',
-            'cycles',
-            'cycles_complete',
-            'frequency',
-            'run_date',
-            'status',
-            'status_reason',
-            'status_text',
-            'token',
-            'subscription_type',
-        ]
         values = {}
-        for field in fields:
+        for field, value in data.items():
             value = data.get(field, None)
             if field == 'amount':
                 # PayFast returns the amount in cents.
                 # Convert it to something more obvious.
                 self.amount_cents = int(value)
                 value = Decimal(value) / Decimal(100)
                 value = value.quantize(Decimal('1.00'))
@@ -281,18 +269,50 @@
                 value = datetime.fromisoformat(value)
                 value = timezone.normalize(value)
 
             if field in ['cycles', 'cycles_complete', 'frequency', 'status']:
                 value = int(value)
 
             setattr(self, field, value)
-        self.freq = self.frequency
+
+        if hasattr(self, 'frequency'):
+            self.freq = self.frequency
 
 
     @property
+    def is_active(self):
+        if self.status_text == constants.SubscriptionStatus.ACTIVE.value:
+            return True
+        return False
+
+
+    @property
+    def is_cancelled(self):
+        if self.status_text == constants.SubscriptionStatus.CANCELLED.value:
+            return True
+        return False
+
+
+    def cancel(self):
+        from payfast import PayFast
+        payfast = PayFast()
+        return payfast.subscriptions.cancel(self.token)
+
+
+    def update_card_link(self, return_url=None) -> str:
+        from payfast import PayFast
+        payfast = PayFast()
+        return payfast.subscriptions.update_card_link(self.token, return_url)
+
+
+
+
+class Subscription(SubscriptionBase):
+
+    @property
     def start_date(self):
         if self.cycles_complete == 0:
             return self.run_date
         cycles_complete = self.freq_delta * self.cycles_complete
         start = self.run_date - cycles_complete
         return start
 
@@ -303,52 +323,23 @@
             return
         cycles = self.freq_delta * self.cycles
         end = self.start_date + cycles
         return end
 
 
     @property
-    def is_tokenized(self):
-        sub_type = self.subscription_type
-        if sub_type == str(constants.SubscriptionType.TOKENIZATION.value):
-            return True
-        return False
-
-
-    @property
-    def is_subscription(self):
-        return not self.is_tokenized
-
-
-    @property
-    def is_active(self):
-        if self.status_text == constants.SubscriptionStatus.ACTIVE.value:
-            return True
-        return False
-
-
-    @property
-    def is_cancelled(self):
-        if self.status_text == constants.SubscriptionStatus.CANCELLED.value:
-            return True
-        return False
-
-
-    @property
     def is_trial(self):
         """
         A subscription is in a free trial if:
 
         - ``cycles_complete`` is smaller than 1. This means that
           the customer has not completed a billing cycle yet and;
 
         - ``run_date`` is in the future.
         """
-        if self.is_tokenized:
-            return False
         now = timezone.now().date()
         run_date = self.run_date.date()
         if self.cycles_complete < 1:
             return True
         return False
 
 
@@ -371,18 +362,14 @@
     def upgrade(
         self,
         amount,
         item_name,
         upgrade_to_period: list=None,
         **kwargs
     ) -> Upgrade:
-        if self.is_tokenized:
-            raise PayFastException(
-                f'Cannot upgrade tokenized subscription (type 2) "{self.token}"'
-            )
         upgrade = Upgrade(
             sub=self,
             amount=amount,
             item_name=item_name,
             upgrade_to_period=upgrade_to_period,
             **kwargs,
         )
@@ -400,19 +387,14 @@
         #. Update this subscription using the PayFast API.
 
         :param amount: The amount to downgrade to.
         """
         from payfast import PayFast
         payfast = PayFast()
 
-        if self.is_tokenized:
-            raise PayFastException(
-                f'Cannot downgrade tokenized subscription (type 2) "{self.token}"'
-            )
-
         if settings.PAYFAST_UPDATE_BUG:
             raise PayFastException(
                 'Cannot downgrade subscription until the PayFast '
                 'update bug is fixed. Cancel the subscription, then '
                 'have the user start a new subscription.'
             )
 
@@ -429,20 +411,14 @@
         kwargs['amount_cents'] = amount_cents
         return payfast.subscriptions.update(
             self.token,
             **kwargs,
         )
 
 
-    def cancel(self):
-        from payfast import PayFast
-        payfast = PayFast()
-        return payfast.subscriptions.cancel(self.token)
-
-
     def is_unpaid(self):
         """
         According to PayFast support the subscription ``run_date``
         won't be changed after payment failures. The ``run_date``
         will only be updated after a successful payment.
         """
         now = timezone.now().date()
@@ -539,33 +515,38 @@
             )
 
         new_run_date = run_date.replace(day=day)
         payfast.subscriptions.update(self.token, run_date=new_run_date)
         return True
 
 
-    def update_card_link(self, return_url=None) -> str:
-        from payfast import PayFast
-        payfast = PayFast()
-        return payfast.subscriptions.update_card_link(self.token, return_url)
-
-
     def update(self, **kwargs):
         from payfast import PayFast
         payfast = PayFast()
         return payfast.subscriptions.update(self.token, **kwargs)
 
 
 
 
-class SubscriptionBase:
+class Card(SubscriptionBase):
+    pass
+
+
+
+
+class SubscriptionBaseResource:
 
     key = 'subscriptions'
 
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.is_card = False
+
+
     def fetch(self, *args, **kwargs):
         """
         Just an alias for ``get`` because this is what the endpoint is
         called on PayFast's API.
         """
         return self.get(*args, **kwargs)
 
@@ -615,14 +596,24 @@
             }
 
         :rtype: Subscription
         """
         uri = urljoin([self.uri, token, 'fetch'])
         response = self.request('GET', uri)
         data = response.payload
+        if isinstance(data, dict):
+            if 'token' not in data:
+                data['token'] = token
+            sub_type = constants.SubscriptionType.TOKENIZATION.value
+            if 'frequency' in data:
+                sub_type = constants.SubscriptionType.REGULAR.value
+            data['subscription_type'] = sub_type
+
+        if self.is_card:
+            return Card(data)
         return Subscription(data)
 
 
     def cancel(self, token):
         """
         PUT /subscriptions/:token/cancel
 
@@ -673,15 +664,15 @@
         if return_url:
             uri = f'{uri}?return={return_url}'
         return uri
 
 
 
 
-class Subscriptions(SubscriptionBase, Resource):
+class Subscriptions(SubscriptionBaseResource, Resource):
 
 
     def pause(self, token):
         """
         PUT /subscriptions/:token/pause
 
         :rtype: bool
@@ -801,15 +792,21 @@
 
     def new(self, *args, **kwargs):
         return SubscriptionPayment(*args, **kwargs)
 
 
 
 
-class Card(SubscriptionBase, Resource):
+class Cards(SubscriptionBaseResource, Resource):
+
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.is_card = True
+
 
     def charge(
         self,
         token,
         amount: Decimal,
         item_name,
         item_description=None,
```

### Comparing `python-payfast-0.3/payfast/api/transactions.py` & `python-payfast-0.5/payfast/api/transactions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/apps.py` & `python-payfast-0.5/payfast/apps.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/base.py` & `python-payfast-0.5/payfast/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
         self.json = {}
         self.http_status = response.status_code
         try:
             self.json = response.json()
         except requests.JSONDecodeError:
             self.text = response.content.decode()
+        logger.debug(json.dumps(self.json, indent=4))
 
         if isinstance(self.json, dict):
             self.code = self.json.get('code', 0)
             self.status = self.json.get('status', '')
             self.data = self.json.get('data', {})
 
             self.response = self.data.get('response', None)
```

### Comparing `python-payfast-0.3/payfast/callbacks.py` & `python-payfast-0.5/payfast/callbacks.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/conf.py` & `python-payfast-0.5/payfast/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,37 +69,41 @@
 
 
 class Settings:
 
     DEBUG = config('PAYFAST_DEBUG', cast=bool, default=True)
     USE_PAYFAST_SANDBOX = DEBUG
 
+    DEFAULT_MERCHANT_ID = 10005195
+    DEFAULT_MERCHANT_KEY = 'cfd5vff7cvxpp'
+    DEFAULT_SALT_PASSPHRASE = '123456789A_bcdefgh'
+
     PAYFAST_HOST = None
     PROCESS_URL = None
     if USE_PAYFAST_SANDBOX:
         PAYFAST_HOST = 'sandbox.payfast.co.za'
     else:
         PAYFAST_HOST = 'www.payfast.co.za'
     API_ROOT = 'https://api.payfast.co.za'
 
     # Might only be set in Django, add defaults
-    MERCHANT_ID = config('PAYFAST_MERCHANT_ID', cast=int)
-    MERCHANT_KEY = config('PAYFAST_MERCHANT_KEY')
-    SALT_PASSPHRASE = config('PAYFAST_SALT_PASSPHRASE')
+    MERCHANT_ID = config('PAYFAST_MERCHANT_ID', default=DEFAULT_MERCHANT_ID, cast=int)
+    MERCHANT_KEY = config('PAYFAST_MERCHANT_KEY', default=DEFAULT_MERCHANT_KEY)
+    SALT_PASSPHRASE = config('PAYFAST_SALT_PASSPHRASE', default=DEFAULT_SALT_PASSPHRASE)
 
     if len(SALT_PASSPHRASE) > 32:
         raise ValueError(
             'Your PayFast "SALT_PASSPHRASE" setting must be no longer than '
             '32 characters'
         )
 
     if DEBUG:
-        MERCHANT_ID = 10005195
-        MERCHANT_KEY = 'cfd5vff7cvxpp'
-        SALT_PASSPHRASE = '123456789A_bcdefgh'
+        MERCHANT_ID = DEFAULT_MERCHANT_ID
+        MERCHANT_KEY = DEFAULT_MERCHANT_KEY
+        SALT_PASSPHRASE = DEFAULT_SALT_PASSPHRASE
 
     PROCESS_URL = f'https://{PAYFAST_HOST}/eng/process'
     VALIDATE_URL = f'https://{PAYFAST_HOST}/eng/query/validate'
 
     PAYFAST_NETWORKS_DEFAULT = [
         '197.97.145.144/28',
         '41.74.179.192/27',
```

### Comparing `python-payfast-0.3/payfast/constants.py` & `python-payfast-0.5/payfast/constants.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/decorators.py` & `python-payfast-0.5/payfast/decorators.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/exceptions.py` & `python-payfast-0.5/payfast/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/itn.py` & `python-payfast-0.5/payfast/itn.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/payment.py` & `python-payfast-0.5/payfast/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         value = json.dumps({
             'user_id': self.user_id,
             'plan_id': self.plan_id,
 
             'trial': trial,
             'run_date': getattr(self, 'billing_date', None),
             'recurring_amount': getattr(self, 'recurring_amount', None),
-            'is_tokenized': getattr(self, 'is_tokenized_card', False),
+            'is_tokenized': getattr(self, 'is_tokenized', False),
         }, cls=PayFastJSONEncoder)
         length = len(value)
         if length > 255:
             raise ValueError(
                 f'"custom_str1" exceeds PayFast character limit of 255. '
                 f'Length: {length}. '
                 f'custom_str1: {value}. '
@@ -434,15 +434,15 @@
         self.frequency = frequency
         self.cycles = kwargs.get('cycles', constants.Cycles.INDEFINITE.value)
         try:
             int(self.cycles)
         except:
             raise
         self.subscription_type = constants.SubscriptionType.REGULAR.value
-        self.is_tokenized_card = False
+        self.is_tokenized = False
 
         self.billing_date = kwargs.get('billing_date', timezone.now())
         self.recurring_amount = kwargs.get('recurring_amount', None)
         if not amount and not self.recurring_amount:
             raise ValueError(
                 'You must provide a value for "recurring_amount" argument '
                 'if no value is provided for "amount".'
@@ -464,27 +464,27 @@
 
 
 
 class TokenizedPayment(Payment):
 
     def __init__(self, amount, item_name, **kwargs):
         self.subscription_type = constants.SubscriptionType.TOKENIZATION.value
-        self.is_tokenized_card = True
+        self.is_tokenized = True
         super().__init__(amount, item_name, **kwargs)
 
 
 
 
 # TODO REVIEW
 class TokenizedSub(SubscriptionPayment):
 
     def __init__(self, amount, item_name, **kwargs):
         super().__init__(amount, item_name, **kwargs)
         self.subscription_type = constants.SubscriptionType.TOKENIZATION.value
-        self.is_tokenized_card = True
+        self.is_tokenized = True
         del self.frequency
         del self.cycles
         del self.recurring_amount
         # Prep again
         self.data_for_payfast = self.prep()
```

### Comparing `python-payfast-0.3/payfast/security_checks.py` & `python-payfast-0.5/payfast/security_checks.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/serialization.py` & `python-payfast-0.5/payfast/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 ]
 boolean_fields = [
     'email_confirmation',
     # 'subscription_notify_email',
     # 'subscription_notify_webhook',
     # 'subscription_notify_buyer',
 
-    'is_tokenized_card',
+    'is_tokenized',
 ]
 
 
 
 
 class PayFastJSONEncoder(json.JSONEncoder):
```

### Comparing `python-payfast-0.3/payfast/signature.py` & `python-payfast-0.5/payfast/signature.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/timezone.py` & `python-payfast-0.5/payfast/timezone.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/urls.py` & `python-payfast-0.5/payfast/urls.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/utils.py` & `python-payfast-0.5/payfast/utils.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/validation.py` & `python-payfast-0.5/payfast/validation.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/payfast/views.py` & `python-payfast-0.5/payfast/views.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/python_payfast.egg-info/PKG-INFO` & `python-payfast-0.5/python_payfast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-payfast
-Version: 0.3
+Version: 0.5
 Summary: A very opinionated Python client library for the PayFast API.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-payfast-0.3/python_payfast.egg-info/SOURCES.txt` & `python-payfast-0.5/python_payfast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/setup.py` & `python-payfast-0.5/setup.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/tests/api/test_transactions.py` & `python-payfast-0.5/tests/api/test_transactions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.3/tests/test_itn.py` & `python-payfast-0.5/tests/test_itn.py`

 * *Files identical despite different names*

