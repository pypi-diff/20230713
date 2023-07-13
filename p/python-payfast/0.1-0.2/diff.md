# Comparing `tmp/python-payfast-0.1.tar.gz` & `tmp/python-payfast-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-payfast-0.1.tar", last modified: Wed Jul 12 09:55:25 2023, max compression
+gzip compressed data, was "python-payfast-0.2.tar", last modified: Thu Jul 13 11:03:22 2023, max compression
```

## Comparing `python-payfast-0.1.tar` & `python-payfast-0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-12 09:55:25.839209 python-payfast-0.1/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-06-06 20:50:53.000000 python-payfast-0.1/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       72 2023-06-12 19:59:05.000000 python-payfast-0.1/MANIFEST.in
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-12 09:55:25.839209 python-payfast-0.1/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      143 2023-07-12 09:54:32.000000 python-payfast-0.1/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-12 09:55:25.831208 python-payfast-0.1/payfast/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2390 2023-07-12 07:27:49.000000 python-payfast-0.1/payfast/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-12 09:55:25.835209 python-payfast-0.1/payfast/api/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-07 11:51:53.000000 python-payfast-0.1/payfast/api/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      533 2023-06-21 18:57:35.000000 python-payfast-0.1/payfast/api/refunds.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    27459 2023-07-12 09:53:02.000000 python-payfast-0.1/payfast/api/subscriptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8005 2023-06-21 18:48:00.000000 python-payfast-0.1/payfast/api/transactions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      566 2023-06-12 19:22:21.000000 python-payfast-0.1/payfast/apps.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6188 2023-07-10 13:53:24.000000 python-payfast-0.1/payfast/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2614 2023-07-12 07:27:56.000000 python-payfast-0.1/payfast/callbacks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7060 2023-07-12 07:29:04.000000 python-payfast-0.1/payfast/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1210 2023-07-10 13:24:31.000000 python-payfast-0.1/payfast/constants.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2188 2023-07-10 14:27:12.000000 python-payfast-0.1/payfast/decorators.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1908 2023-06-21 19:24:26.000000 python-payfast-0.1/payfast/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    11812 2023-07-10 14:13:51.000000 python-payfast-0.1/payfast/itn.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      251 2023-06-21 18:47:03.000000 python-payfast-0.1/payfast/logging.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15853 2023-07-11 07:47:49.000000 python-payfast-0.1/payfast/payment.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2111 2023-06-08 18:38:43.000000 python-payfast-0.1/payfast/security_checks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3313 2023-07-10 14:21:32.000000 python-payfast-0.1/payfast/serialization.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      376 2023-06-19 18:50:19.000000 python-payfast-0.1/payfast/signals.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2761 2023-06-15 13:28:20.000000 python-payfast-0.1/payfast/signature.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-12 09:55:25.827208 python-payfast-0.1/payfast/templates/
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-12 09:55:25.835209 python-payfast-0.1/payfast/templates/payfast/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      285 2023-07-10 12:50:03.000000 python-payfast-0.1/payfast/templates/payfast/form.html
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      299 2023-06-12 20:32:31.000000 python-payfast-0.1/payfast/templates/payfast/sandbox.html
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      419 2023-07-10 12:49:49.000000 python-payfast-0.1/payfast/templates.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      544 2023-06-14 16:50:45.000000 python-payfast-0.1/payfast/timezone.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      618 2023-06-13 13:20:57.000000 python-payfast-0.1/payfast/urls.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     4071 2023-07-12 08:10:34.000000 python-payfast-0.1/payfast/utils.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1577 2023-07-12 08:09:37.000000 python-payfast-0.1/payfast/validation.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5009 2023-07-10 13:58:41.000000 python-payfast-0.1/payfast/views.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-12 09:55:25.835209 python-payfast-0.1/python_payfast.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-12 09:55:25.000000 python-payfast-0.1/python_payfast.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1215 2023-07-12 09:55:25.000000 python-payfast-0.1/python_payfast.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-07-12 09:55:25.000000 python-payfast-0.1/python_payfast.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      102 2023-07-12 09:55:25.000000 python-payfast-0.1/python_payfast.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-07-12 09:55:25.000000 python-payfast-0.1/python_payfast.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-07-12 09:55:25.839209 python-payfast-0.1/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1804 2023-06-15 12:19:47.000000 python-payfast-0.1/setup.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-12 09:55:25.839209 python-payfast-0.1/tests/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-06 18:42:13.000000 python-payfast-0.1/tests/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-12 09:55:25.839209 python-payfast-0.1/tests/api/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:55:21.000000 python-payfast-0.1/tests/api/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      436 2023-06-12 18:51:32.000000 python-payfast-0.1/tests/api/test_subscriptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      563 2023-06-12 18:11:31.000000 python-payfast-0.1/tests/api/test_transactions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:58.000000 python-payfast-0.1/tests/test_base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:53.000000 python-payfast-0.1/tests/test_callbacks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:58.000000 python-payfast-0.1/tests/test_conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:35.000000 python-payfast-0.1/tests/test_constants.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:02:08.000000 python-payfast-0.1/tests/test_exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1541 2023-07-12 09:51:05.000000 python-payfast-0.1/tests/test_itn.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      300 2023-06-12 18:51:58.000000 python-payfast-0.1/tests/test_payfast.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      431 2023-06-12 19:22:34.000000 python-payfast-0.1/tests/test_payment.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:36.000000 python-payfast-0.1/tests/test_security_checks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:46.000000 python-payfast-0.1/tests/test_signature.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:05.000000 python-payfast-0.1/tests/test_templates.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:20.000000 python-payfast-0.1/tests/test_timezone.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:26.000000 python-payfast-0.1/tests/test_utils.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.604309 python-payfast-0.2/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-06-06 20:50:53.000000 python-payfast-0.2/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       72 2023-06-12 19:59:05.000000 python-payfast-0.2/MANIFEST.in
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 11:03:22.604309 python-payfast-0.2/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      143 2023-07-12 09:54:32.000000 python-payfast-0.2/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.300309 python-payfast-0.2/payfast/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2438 2023-07-13 10:58:29.000000 python-payfast-0.2/payfast/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.364309 python-payfast-0.2/payfast/api/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-07 11:51:53.000000 python-payfast-0.2/payfast/api/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      533 2023-06-21 18:57:35.000000 python-payfast-0.2/payfast/api/refunds.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    27537 2023-07-13 10:57:04.000000 python-payfast-0.2/payfast/api/subscriptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8005 2023-06-21 18:48:00.000000 python-payfast-0.2/payfast/api/transactions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      566 2023-06-12 19:22:21.000000 python-payfast-0.2/payfast/apps.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6188 2023-07-10 13:53:24.000000 python-payfast-0.2/payfast/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2614 2023-07-12 07:27:56.000000 python-payfast-0.2/payfast/callbacks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7060 2023-07-12 07:29:04.000000 python-payfast-0.2/payfast/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1210 2023-07-10 13:24:31.000000 python-payfast-0.2/payfast/constants.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2188 2023-07-10 14:27:12.000000 python-payfast-0.2/payfast/decorators.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1908 2023-06-21 19:24:26.000000 python-payfast-0.2/payfast/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    11812 2023-07-10 14:13:51.000000 python-payfast-0.2/payfast/itn.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      251 2023-06-21 18:47:03.000000 python-payfast-0.2/payfast/logging.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15853 2023-07-11 07:47:49.000000 python-payfast-0.2/payfast/payment.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2111 2023-06-08 18:38:43.000000 python-payfast-0.2/payfast/security_checks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3313 2023-07-10 14:21:32.000000 python-payfast-0.2/payfast/serialization.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      376 2023-06-19 18:50:19.000000 python-payfast-0.2/payfast/signals.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2761 2023-06-15 13:28:20.000000 python-payfast-0.2/payfast/signature.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:21.576307 python-payfast-0.2/payfast/templates/
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.396309 python-payfast-0.2/payfast/templates/payfast/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      285 2023-07-10 12:50:03.000000 python-payfast-0.2/payfast/templates/payfast/form.html
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      299 2023-06-12 20:32:31.000000 python-payfast-0.2/payfast/templates/payfast/sandbox.html
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      419 2023-07-10 12:49:49.000000 python-payfast-0.2/payfast/templates.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      544 2023-06-14 16:50:45.000000 python-payfast-0.2/payfast/timezone.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      618 2023-06-13 13:20:57.000000 python-payfast-0.2/payfast/urls.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     4071 2023-07-12 08:10:34.000000 python-payfast-0.2/payfast/utils.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1577 2023-07-12 08:09:37.000000 python-payfast-0.2/payfast/validation.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5009 2023-07-10 13:58:41.000000 python-payfast-0.2/payfast/views.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.432309 python-payfast-0.2/python_payfast.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1215 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      102 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-07-13 11:03:21.000000 python-payfast-0.2/python_payfast.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-07-13 11:03:22.604309 python-payfast-0.2/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1804 2023-06-15 12:19:47.000000 python-payfast-0.2/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.512309 python-payfast-0.2/tests/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-06 18:42:13.000000 python-payfast-0.2/tests/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 11:03:22.560309 python-payfast-0.2/tests/api/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:55:21.000000 python-payfast-0.2/tests/api/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      436 2023-06-12 18:51:32.000000 python-payfast-0.2/tests/api/test_subscriptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      563 2023-06-12 18:11:31.000000 python-payfast-0.2/tests/api/test_transactions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:58.000000 python-payfast-0.2/tests/test_base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:53.000000 python-payfast-0.2/tests/test_callbacks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:58.000000 python-payfast-0.2/tests/test_conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:35.000000 python-payfast-0.2/tests/test_constants.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:02:08.000000 python-payfast-0.2/tests/test_exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1541 2023-07-12 09:51:05.000000 python-payfast-0.2/tests/test_itn.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      300 2023-06-12 18:51:58.000000 python-payfast-0.2/tests/test_payfast.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      431 2023-06-12 19:22:34.000000 python-payfast-0.2/tests/test_payment.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:36.000000 python-payfast-0.2/tests/test_security_checks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:46.000000 python-payfast-0.2/tests/test_signature.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:05.000000 python-payfast-0.2/tests/test_templates.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:20.000000 python-payfast-0.2/tests/test_timezone.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:26.000000 python-payfast-0.2/tests/test_utils.py
```

### Comparing `python-payfast-0.1/LICENSE` & `python-payfast-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/PKG-INFO` & `python-payfast-0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-payfast
-Version: 0.1
+Version: 0.2
 Summary: A very opinionated Python client library for the PayFast API.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-payfast-0.1/payfast/__init__.py` & `python-payfast-0.2/payfast/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     SubscriptionPayment,
     TokenizedPayment,
     TokenizedSub,
 )
 from payfast.base import RequestsTransport
 from payfast.logging import configure_logging
 from payfast.exceptions import PayFastException
-from payfast.api.subscriptions import Subscriptions
+from payfast.api.subscriptions import Subscriptions, Card
 from payfast.api.transactions import Transactions, CCTransactions
 from payfast.api.refunds import Refunds
 
 
 
 
-__version__ = '0.1'
+__version__ = '0.2'
 __title__ = 'python-payfast'
 
 
 
 
 class PayFast:
 
@@ -41,14 +41,15 @@
         self.base_uri = settings.API_ROOT
         self.api_version = version
         args = [version]
         kwargs = {'transport_class': self.TRANSPORT_CLASS}
 
         self.subscriptions = Subscriptions(*args, **kwargs)
         self.subs = Subscriptions(*args, **kwargs) # alias
+        self.card = Card(*args, **kwargs)
 
         self.transactions = Transactions(*args, **kwargs)
         self.cc_transactions = CCTransactions(*args, **kwargs)
 
         self.refunds = Refunds(*args, **kwargs)
         self.refund = self.refunds.create # alias
```

### Comparing `python-payfast-0.1/payfast/api/refunds.py` & `python-payfast-0.2/payfast/api/refunds.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/api/subscriptions.py` & `python-payfast-0.2/payfast/api/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,27 +553,84 @@
         from payfast import PayFast
         payfast = PayFast()
         return payfast.subscriptions.update(self.token, **kwargs)
 
 
 
 
-class Subscriptions(Resource):
+class SubscriptionBase:
 
     key = 'subscriptions'
 
 
     def fetch(self, *args, **kwargs):
         """
         Just an alias for ``get`` because this is what the endpoint is
         called on PayFast's API.
         """
         return self.get(*args, **kwargs)
 
 
+    def cancel(self, token):
+        """
+        PUT /subscriptions/:token/cancel
+
+        If the subscription is already cancelled::
+
+            {
+                "code": 400,
+                "status": "failed",
+                "data": {
+                    "response": false,
+                    "message": "Failure - The subscription status is cancelled"
+                }
+            }
+
+        :rtype: bool
+        """
+        uri = urljoin([self.uri, token, 'cancel'])
+        # TODO: handle "Failure - The subscription status is cancelled"
+        response = self.request('PUT', uri, raise_for_status=False)
+        if not response.ok:
+            cancel_msg = 'failure - the subscription status is cancelled'
+            if cancel_msg in response.message.lower():
+                # This would be a 400 status which is why we have to set
+                # raise_for_status to False. Override the values, because
+                # this subscription has already been cancelled so everything
+                # is okay.
+                #
+                # TODO REVIEW:
+                # Perhaps add a flag to the cancel method to raise an exception
+                # for this. However, this will be the default behaviour.
+                response.ok = True
+                response.code = 200
+                if response.payload is False:
+                    response.payload = True
+            else:
+                raise PayFastAPIException(response)
+        data = response.payload
+        cache_bust(token)
+        return data
+
+
+    def update_card_link(self, token, return_url=None) -> str:
+        """
+        This doesn't point to the PayFast API but it still fits here.
+        """
+        host = settings.PAYFAST_HOST
+        uri = f'https://{host}/eng/recurring/update/{token}'
+        if return_url:
+            uri = f'{uri}?return={return_url}'
+        return uri
+
+
+
+
+class Subscriptions(SubscriptionBase, Resource):
+
     @cached
     def get(self, token, **kwargs):
         """
         GET ``/subscriptions/:token/fetch``
 
         Example response of a subscription managed by PayFast
         (not adhoc tokenization):
@@ -644,56 +701,14 @@
         uri = urljoin([self.uri, token, 'unpause'])
         response = self.request('PUT', uri)
         data = response.payload
         cache_bust(token)
         return data
 
 
-    def cancel(self, token):
-        """
-        PUT /subscriptions/:token/cancel
-
-        If the subscription is already cancelled::
-
-            {
-                "code": 400,
-                "status": "failed",
-                "data": {
-                    "response": false,
-                    "message": "Failure - The subscription status is cancelled"
-                }
-            }
-
-        :rtype: bool
-        """
-        uri = urljoin([self.uri, token, 'cancel'])
-        # TODO: handle "Failure - The subscription status is cancelled"
-        response = self.request('PUT', uri, raise_for_status=False)
-        if not response.ok:
-            cancel_msg = 'failure - the subscription status is cancelled'
-            if cancel_msg in response.message.lower():
-                # This would be a 400 status which is why we have to set
-                # raise_for_status to False. Override the values, because
-                # this subscription has already been cancelled so everything
-                # is okay.
-                #
-                # TODO REVIEW:
-                # Perhaps add a flag to the cancel method to raise an exception
-                # for this. However, this will be the default behaviour.
-                response.ok = True
-                response.code = 200
-                if response.payload is False:
-                    response.payload = True
-            else:
-                raise PayFastAPIException(response)
-        data = response.payload
-        cache_bust(token)
-        return data
-
-
     def update(
         self,
         token,
         cycles: int=None,
         run_date: datetime=None,
         amount_cents: int=None,
         amount=None,
@@ -779,14 +794,22 @@
             raise
         data = response.payload
         cache_bust(token)
         callbacks._subscription_update(token, payload, success=True)
         return data
 
 
+    def new(self, *args, **kwargs):
+        return SubscriptionPayment(*args, **kwargs)
+
+
+
+
+class Card(SubscriptionBase, Resource):
+
     def charge(
         self,
         token,
         amount: Decimal,
         item_name,
         item_description=None,
         itn: bool=True, # TODO possibly change to send_itn
@@ -850,23 +873,8 @@
                 f'No PayFast payment ID was found in response payload. '
                 f'Payload: {data}'
             )
         return pf_payment_id
 
 
     def new(self, *args, **kwargs):
-        return SubscriptionPayment(*args, **kwargs)
-
-
-    def new_tokenized(self, *args, **kwargs):
         return TokenizedPayment(*args, **kwargs)
-
-
-    def update_card_link(self, token, return_url=None) -> str:
-        """
-        This doesn't point to the PayFast API but it still fits here.
-        """
-        host = settings.PAYFAST_HOST
-        uri = f'https://{host}/eng/recurring/update/{token}'
-        if return_url:
-            uri = f'{uri}?return={return_url}'
-        return uri
```

### Comparing `python-payfast-0.1/payfast/api/transactions.py` & `python-payfast-0.2/payfast/api/transactions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/apps.py` & `python-payfast-0.2/payfast/apps.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/base.py` & `python-payfast-0.2/payfast/base.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/callbacks.py` & `python-payfast-0.2/payfast/callbacks.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/conf.py` & `python-payfast-0.2/payfast/conf.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/constants.py` & `python-payfast-0.2/payfast/constants.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/decorators.py` & `python-payfast-0.2/payfast/decorators.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/exceptions.py` & `python-payfast-0.2/payfast/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/itn.py` & `python-payfast-0.2/payfast/itn.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/payment.py` & `python-payfast-0.2/payfast/payment.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/security_checks.py` & `python-payfast-0.2/payfast/security_checks.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/serialization.py` & `python-payfast-0.2/payfast/serialization.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/signature.py` & `python-payfast-0.2/payfast/signature.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/timezone.py` & `python-payfast-0.2/payfast/timezone.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/urls.py` & `python-payfast-0.2/payfast/urls.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/utils.py` & `python-payfast-0.2/payfast/utils.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/validation.py` & `python-payfast-0.2/payfast/validation.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/payfast/views.py` & `python-payfast-0.2/payfast/views.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/python_payfast.egg-info/PKG-INFO` & `python-payfast-0.2/python_payfast.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-payfast
-Version: 0.1
+Version: 0.2
 Summary: A very opinionated Python client library for the PayFast API.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-payfast-0.1/python_payfast.egg-info/SOURCES.txt` & `python-payfast-0.2/python_payfast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/setup.py` & `python-payfast-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/tests/api/test_transactions.py` & `python-payfast-0.2/tests/api/test_transactions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.1/tests/test_itn.py` & `python-payfast-0.2/tests/test_itn.py`

 * *Files identical despite different names*

