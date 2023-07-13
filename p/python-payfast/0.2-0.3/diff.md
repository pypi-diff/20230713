# Comparing `tmp/python-payfast-0.2.tar.gz` & `tmp/python-payfast-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-payfast-0.2.tar", last modified: Thu Jul 13 11:03:22 2023, max compression
+gzip compressed data, was "python-payfast-0.3.tar", last modified: Thu Jul 13 11:08:02 2023, max compression
```

## Comparing `python-payfast-0.2.tar` & `python-payfast-0.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.604309 python-payfast-0.2/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-06-06 20:50:53.000000 python-payfast-0.2/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       72 2023-06-12 19:59:05.000000 python-payfast-0.2/MANIFEST.in
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 11:03:22.604309 python-payfast-0.2/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      143 2023-07-12 09:54:32.000000 python-payfast-0.2/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.300309 python-payfast-0.2/payfast/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2438 2023-07-13 10:58:29.000000 python-payfast-0.2/payfast/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.364309 python-payfast-0.2/payfast/api/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-07 11:51:53.000000 python-payfast-0.2/payfast/api/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      533 2023-06-21 18:57:35.000000 python-payfast-0.2/payfast/api/refunds.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    27537 2023-07-13 10:57:04.000000 python-payfast-0.2/payfast/api/subscriptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8005 2023-06-21 18:48:00.000000 python-payfast-0.2/payfast/api/transactions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      566 2023-06-12 19:22:21.000000 python-payfast-0.2/payfast/apps.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6188 2023-07-10 13:53:24.000000 python-payfast-0.2/payfast/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2614 2023-07-12 07:27:56.000000 python-payfast-0.2/payfast/callbacks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7060 2023-07-12 07:29:04.000000 python-payfast-0.2/payfast/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1210 2023-07-10 13:24:31.000000 python-payfast-0.2/payfast/constants.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2188 2023-07-10 14:27:12.000000 python-payfast-0.2/payfast/decorators.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1908 2023-06-21 19:24:26.000000 python-payfast-0.2/payfast/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    11812 2023-07-10 14:13:51.000000 python-payfast-0.2/payfast/itn.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      251 2023-06-21 18:47:03.000000 python-payfast-0.2/payfast/logging.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15853 2023-07-11 07:47:49.000000 python-payfast-0.2/payfast/payment.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2111 2023-06-08 18:38:43.000000 python-payfast-0.2/payfast/security_checks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3313 2023-07-10 14:21:32.000000 python-payfast-0.2/payfast/serialization.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      376 2023-06-19 18:50:19.000000 python-payfast-0.2/payfast/signals.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2761 2023-06-15 13:28:20.000000 python-payfast-0.2/payfast/signature.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:21.576307 python-payfast-0.2/payfast/templates/
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.396309 python-payfast-0.2/payfast/templates/payfast/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      285 2023-07-10 12:50:03.000000 python-payfast-0.2/payfast/templates/payfast/form.html
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      299 2023-06-12 20:32:31.000000 python-payfast-0.2/payfast/templates/payfast/sandbox.html
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      419 2023-07-10 12:49:49.000000 python-payfast-0.2/payfast/templates.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      544 2023-06-14 16:50:45.000000 python-payfast-0.2/payfast/timezone.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      618 2023-06-13 13:20:57.000000 python-payfast-0.2/payfast/urls.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     4071 2023-07-12 08:10:34.000000 python-payfast-0.2/payfast/utils.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1577 2023-07-12 08:09:37.000000 python-payfast-0.2/payfast/validation.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5009 2023-07-10 13:58:41.000000 python-payfast-0.2/payfast/views.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.432309 python-payfast-0.2/python_payfast.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1215 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      102 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-07-13 11:03:22.604309 python-payfast-0.2/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1804 2023-06-15 12:19:47.000000 python-payfast-0.2/setup.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.512309 python-payfast-0.2/tests/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-06 18:42:13.000000 python-payfast-0.2/tests/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.560309 python-payfast-0.2/tests/api/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:55:21.000000 python-payfast-0.2/tests/api/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      436 2023-06-12 18:51:32.000000 python-payfast-0.2/tests/api/test_subscriptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      563 2023-06-12 18:11:31.000000 python-payfast-0.2/tests/api/test_transactions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:58.000000 python-payfast-0.2/tests/test_base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:53.000000 python-payfast-0.2/tests/test_callbacks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:58.000000 python-payfast-0.2/tests/test_conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:35.000000 python-payfast-0.2/tests/test_constants.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:02:08.000000 python-payfast-0.2/tests/test_exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1541 2023-07-12 09:51:05.000000 python-payfast-0.2/tests/test_itn.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      300 2023-06-12 18:51:58.000000 python-payfast-0.2/tests/test_payfast.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      431 2023-06-12 19:22:34.000000 python-payfast-0.2/tests/test_payment.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:36.000000 python-payfast-0.2/tests/test_security_checks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:46.000000 python-payfast-0.2/tests/test_signature.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:05.000000 python-payfast-0.2/tests/test_templates.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:20.000000 python-payfast-0.2/tests/test_timezone.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:26.000000 python-payfast-0.2/tests/test_utils.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.941416 python-payfast-0.3/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-06-06 20:50:53.000000 python-payfast-0.3/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       72 2023-06-12 19:59:05.000000 python-payfast-0.3/MANIFEST.in
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 11:08:02.941416 python-payfast-0.3/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      143 2023-07-12 09:54:32.000000 python-payfast-0.3/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/payfast/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2438 2023-07-13 11:07:33.000000 python-payfast-0.3/payfast/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/payfast/api/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-07 11:51:53.000000 python-payfast-0.3/payfast/api/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      533 2023-06-21 18:57:35.000000 python-payfast-0.3/payfast/api/refunds.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    27538 2023-07-13 11:06:53.000000 python-payfast-0.3/payfast/api/subscriptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8005 2023-06-21 18:48:00.000000 python-payfast-0.3/payfast/api/transactions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      566 2023-06-12 19:22:21.000000 python-payfast-0.3/payfast/apps.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6188 2023-07-10 13:53:24.000000 python-payfast-0.3/payfast/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2614 2023-07-12 07:27:56.000000 python-payfast-0.3/payfast/callbacks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7060 2023-07-12 07:29:04.000000 python-payfast-0.3/payfast/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1210 2023-07-10 13:24:31.000000 python-payfast-0.3/payfast/constants.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2188 2023-07-10 14:27:12.000000 python-payfast-0.3/payfast/decorators.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1908 2023-06-21 19:24:26.000000 python-payfast-0.3/payfast/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    11812 2023-07-10 14:13:51.000000 python-payfast-0.3/payfast/itn.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      251 2023-06-21 18:47:03.000000 python-payfast-0.3/payfast/logging.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15853 2023-07-11 07:47:49.000000 python-payfast-0.3/payfast/payment.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2111 2023-06-08 18:38:43.000000 python-payfast-0.3/payfast/security_checks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3313 2023-07-10 14:21:32.000000 python-payfast-0.3/payfast/serialization.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      376 2023-06-19 18:50:19.000000 python-payfast-0.3/payfast/signals.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2761 2023-06-15 13:28:20.000000 python-payfast-0.3/payfast/signature.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.933416 python-payfast-0.3/payfast/templates/
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/payfast/templates/payfast/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      285 2023-07-10 12:50:03.000000 python-payfast-0.3/payfast/templates/payfast/form.html
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      299 2023-06-12 20:32:31.000000 python-payfast-0.3/payfast/templates/payfast/sandbox.html
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      419 2023-07-10 12:49:49.000000 python-payfast-0.3/payfast/templates.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      544 2023-06-14 16:50:45.000000 python-payfast-0.3/payfast/timezone.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      618 2023-06-13 13:20:57.000000 python-payfast-0.3/payfast/urls.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     4071 2023-07-12 08:10:34.000000 python-payfast-0.3/payfast/utils.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1577 2023-07-12 08:09:37.000000 python-payfast-0.3/payfast/validation.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5009 2023-07-10 13:58:41.000000 python-payfast-0.3/payfast/views.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/python_payfast.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1215 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      102 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-07-13 11:08:02.000000 python-payfast-0.3/python_payfast.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-07-13 11:08:02.941416 python-payfast-0.3/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1804 2023-06-15 12:19:47.000000 python-payfast-0.3/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.937416 python-payfast-0.3/tests/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-06 18:42:13.000000 python-payfast-0.3/tests/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:08:02.941416 python-payfast-0.3/tests/api/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:55:21.000000 python-payfast-0.3/tests/api/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      436 2023-06-12 18:51:32.000000 python-payfast-0.3/tests/api/test_subscriptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      563 2023-06-12 18:11:31.000000 python-payfast-0.3/tests/api/test_transactions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:58.000000 python-payfast-0.3/tests/test_base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:53.000000 python-payfast-0.3/tests/test_callbacks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:58.000000 python-payfast-0.3/tests/test_conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:35.000000 python-payfast-0.3/tests/test_constants.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:02:08.000000 python-payfast-0.3/tests/test_exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1541 2023-07-12 09:51:05.000000 python-payfast-0.3/tests/test_itn.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      300 2023-06-12 18:51:58.000000 python-payfast-0.3/tests/test_payfast.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      431 2023-06-12 19:22:34.000000 python-payfast-0.3/tests/test_payment.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:36.000000 python-payfast-0.3/tests/test_security_checks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:46.000000 python-payfast-0.3/tests/test_signature.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:05.000000 python-payfast-0.3/tests/test_templates.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:20.000000 python-payfast-0.3/tests/test_timezone.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:26.000000 python-payfast-0.3/tests/test_utils.py
```

### Comparing `python-payfast-0.2/LICENSE` & `python-payfast-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/PKG-INFO` & `python-payfast-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-payfast
-Version: 0.2
+Version: 0.3
 Summary: A very opinionated Python client library for the PayFast API.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-payfast-0.2/payfast/__init__.py` & `python-payfast-0.3/payfast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from payfast.api.subscriptions import Subscriptions, Card
 from payfast.api.transactions import Transactions, CCTransactions
 from payfast.api.refunds import Refunds
 
 
 
 
-__version__ = '0.2'
+__version__ = '0.3'
 __title__ = 'python-payfast'
 
 
 
 
 class PayFast:
```

### Comparing `python-payfast-0.2/payfast/api/refunds.py` & `python-payfast-0.3/payfast/api/refunds.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/api/subscriptions.py` & `python-payfast-0.3/payfast/api/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,14 +566,66 @@
         """
         Just an alias for ``get`` because this is what the endpoint is
         called on PayFast's API.
         """
         return self.get(*args, **kwargs)
 
 
+    @cached
+    def get(self, token, **kwargs):
+        """
+        GET ``/subscriptions/:token/fetch``
+
+        Example response of a subscription managed by PayFast
+        (not adhoc tokenization):
+
+        .. code-block::
+
+            {
+                "code": 200,
+                "status": "success",
+                "data": {
+                    "response": {
+                        "amount": 1628,
+                        "cycles": 14,
+                        "cycles_complete": 9,
+                        "frequency": 3,
+                        "run_date": "2020-07-04T00:00:00+02:00",
+                        "status": 1,
+                        "status_reason": "",
+                        "status_text": "ACTIVE",
+                        "token": "a3b3ae55-ab8b-b388-df23-4e6882b86ce0"
+                    }
+                }
+            }
+
+        Example response of a tokenized subscription:
+
+        .. code-block::
+
+            {
+                "code": 200,
+                "status": "success",
+                "data": {
+                    "response": {
+                        "status": 1,
+                        "status_reason": "",
+                        "status_text": "ACTIVE"
+                    }
+                }
+            }
+
+        :rtype: Subscription
+        """
+        uri = urljoin([self.uri, token, 'fetch'])
+        response = self.request('GET', uri)
+        data = response.payload
+        return Subscription(data)
+
+
     def cancel(self, token):
         """
         PUT /subscriptions/:token/cancel
 
         If the subscription is already cancelled::
 
             {
@@ -623,65 +675,14 @@
         return uri
 
 
 
 
 class Subscriptions(SubscriptionBase, Resource):
 
-    @cached
-    def get(self, token, **kwargs):
-        """
-        GET ``/subscriptions/:token/fetch``
-
-        Example response of a subscription managed by PayFast
-        (not adhoc tokenization):
-
-        .. code-block::
-
-            {
-                "code": 200,
-                "status": "success",
-                "data": {
-                    "response": {
-                        "amount": 1628,
-                        "cycles": 14,
-                        "cycles_complete": 9,
-                        "frequency": 3,
-                        "run_date": "2020-07-04T00:00:00+02:00",
-                        "status": 1,
-                        "status_reason": "",
-                        "status_text": "ACTIVE",
-                        "token": "a3b3ae55-ab8b-b388-df23-4e6882b86ce0"
-                    }
-                }
-            }
-
-        Example response of a tokenized subscription:
-
-        .. code-block::
-
-            {
-                "code": 200,
-                "status": "success",
-                "data": {
-                    "response": {
-                        "status": 1,
-                        "status_reason": "",
-                        "status_text": "ACTIVE"
-                    }
-                }
-            }
-
-        :rtype: Subscription
-        """
-        uri = urljoin([self.uri, token, 'fetch'])
-        response = self.request('GET', uri)
-        data = response.payload
-        return Subscription(data)
-
 
     def pause(self, token):
         """
         PUT /subscriptions/:token/pause
 
         :rtype: bool
         """
```

### Comparing `python-payfast-0.2/payfast/api/transactions.py` & `python-payfast-0.3/payfast/api/transactions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/apps.py` & `python-payfast-0.3/payfast/apps.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/base.py` & `python-payfast-0.3/payfast/base.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/callbacks.py` & `python-payfast-0.3/payfast/callbacks.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/conf.py` & `python-payfast-0.3/payfast/conf.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/constants.py` & `python-payfast-0.3/payfast/constants.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/decorators.py` & `python-payfast-0.3/payfast/decorators.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/exceptions.py` & `python-payfast-0.3/payfast/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/itn.py` & `python-payfast-0.3/payfast/itn.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/payment.py` & `python-payfast-0.3/payfast/payment.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/security_checks.py` & `python-payfast-0.3/payfast/security_checks.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/serialization.py` & `python-payfast-0.3/payfast/serialization.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/signature.py` & `python-payfast-0.3/payfast/signature.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/timezone.py` & `python-payfast-0.3/payfast/timezone.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/urls.py` & `python-payfast-0.3/payfast/urls.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/utils.py` & `python-payfast-0.3/payfast/utils.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/validation.py` & `python-payfast-0.3/payfast/validation.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/payfast/views.py` & `python-payfast-0.3/payfast/views.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/python_payfast.egg-info/PKG-INFO` & `python-payfast-0.3/python_payfast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-payfast
-Version: 0.2
+Version: 0.3
 Summary: A very opinionated Python client library for the PayFast API.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-payfast-0.2/python_payfast.egg-info/SOURCES.txt` & `python-payfast-0.3/python_payfast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/setup.py` & `python-payfast-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/tests/api/test_transactions.py` & `python-payfast-0.3/tests/api/test_transactions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.2/tests/test_itn.py` & `python-payfast-0.3/tests/test_itn.py`

 * *Files identical despite different names*

