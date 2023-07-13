# Comparing `tmp/hukudo-3.2.0.tar.gz` & `tmp/hukudo-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hukudo-3.2.0.tar", last modified: Wed May 31 11:55:43 2023, max compression
+gzip compressed data, was "hukudo-3.3.0.tar", last modified: Thu Jul 13 08:18:07 2023, max compression
```

## Comparing `hukudo-3.2.0.tar` & `hukudo-3.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.190870 hukudo-3.2.0/
--rw-rw-r--   0 felix     (1337) felix     (1337)     1077 2022-04-05 09:56:29.000000 hukudo-3.2.0/LICENSE
--rw-rw-r--   0 felix     (1337) felix     (1337)     1246 2023-05-31 11:55:43.190870 hukudo-3.2.0/PKG-INFO
--rw-rw-r--   0 felix     (1337) felix     (1337)      890 2022-09-08 11:45:30.000000 hukudo-3.2.0/README.md
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.182870 hukudo-3.2.0/hukudo/
--rw-rw-r--   0 felix     (1337) felix     (1337)       22 2023-05-31 11:55:42.000000 hukudo-3.2.0/hukudo/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     5305 2023-03-13 12:19:59.000000 hukudo-3.2.0/hukudo/chromedriver.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2235 2022-09-09 10:11:07.000000 hukudo-3.2.0/hukudo/cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)       43 2022-06-07 10:45:57.000000 hukudo-3.2.0/hukudo/exc.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      636 2022-09-08 11:32:36.000000 hukudo-3.2.0/hukudo/filesystem.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.186870 hukudo-3.2.0/hukudo/gitlab/
--rw-rw-r--   0 felix     (1337) felix     (1337)        0 2022-07-20 19:31:40.000000 hukudo-3.2.0/hukudo/gitlab/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      745 2022-07-20 19:31:40.000000 hukudo-3.2.0/hukudo/gitlab/api.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      723 2022-07-20 19:31:40.000000 hukudo-3.2.0/hukudo/gitlab/cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      430 2022-07-20 19:31:40.000000 hukudo-3.2.0/hukudo/gitlab/jobs.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.186870 hukudo-3.2.0/hukudo/grafana/
--rw-rw-r--   0 felix     (1337) felix     (1337)       55 2022-03-10 15:35:16.000000 hukudo-3.2.0/hukudo/grafana/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     3652 2023-05-31 11:31:40.000000 hukudo-3.2.0/hukudo/grafana/api.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2981 2023-05-31 11:40:08.000000 hukudo-3.2.0/hukudo/grafana/cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      263 2022-06-07 15:19:07.000000 hukudo-3.2.0/hukudo/grafana/demo.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      141 2022-06-08 10:23:35.000000 hukudo-3.2.0/hukudo/grafana/errors.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      647 2022-06-08 15:07:18.000000 hukudo-3.2.0/hukudo/grafana/models.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     1076 2022-06-08 11:13:22.000000 hukudo-3.2.0/hukudo/log.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.186870 hukudo-3.2.0/hukudo/pypi/
--rw-rw-r--   0 felix     (1337) felix     (1337)      384 2022-09-09 10:11:07.000000 hukudo-3.2.0/hukudo/pypi/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      187 2022-09-09 10:12:16.000000 hukudo-3.2.0/hukudo/pypi/cli.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.186870 hukudo-3.2.0/hukudo/xls/
--rw-rw-r--   0 felix     (1337) felix     (1337)       38 2023-04-13 15:49:31.000000 hukudo-3.2.0/hukudo/xls/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2392 2021-11-03 18:22:13.000000 hukudo-3.2.0/hukudo/xls/edi.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2417 2021-12-01 09:56:40.000000 hukudo-3.2.0/hukudo/xls/fmt.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     4839 2023-04-13 15:56:59.000000 hukudo-3.2.0/hukudo/xls/sheet.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2029 2023-04-13 15:49:32.000000 hukudo-3.2.0/hukudo/xls/table.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.182870 hukudo-3.2.0/hukudo.egg-info/
--rw-rw-r--   0 felix     (1337) felix     (1337)     1246 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/PKG-INFO
--rw-rw-r--   0 felix     (1337) felix     (1337)      923 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/SOURCES.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)        1 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/dependency_links.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)       43 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/entry_points.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)      533 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/requires.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)        7 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/top_level.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)      386 2023-03-13 12:33:26.000000 hukudo-3.2.0/pyproject.toml
--rw-rw-r--   0 felix     (1337) felix     (1337)      753 2023-05-31 11:55:43.190870 hukudo-3.2.0/setup.cfg
--rw-rw-r--   0 felix     (1337) felix     (1337)      348 2023-03-13 12:33:26.000000 hukudo-3.2.0/setup.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.190870 hukudo-3.2.0/tests/
--rw-rw-r--   0 felix     (1337) felix     (1337)     2833 2022-06-08 16:07:14.000000 hukudo-3.2.0/tests/test_chromedriver.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      305 2022-06-08 13:34:36.000000 hukudo-3.2.0/tests/test_cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      613 2022-07-20 19:31:40.000000 hukudo-3.2.0/tests/test_gitlab.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     5455 2022-10-26 12:58:40.000000 hukudo-3.2.0/tests/test_grafana.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      666 2022-09-08 11:39:19.000000 hukudo-3.2.0/tests/test_keepn.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      144 2022-06-08 15:28:39.000000 hukudo-3.2.0/tests/test_log.py
--rw-rw-r--   0 felix     (1337) felix     (1337)       80 2022-06-08 10:38:01.000000 hukudo-3.2.0/tests/test_pypi.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      436 2021-11-03 14:53:39.000000 hukudo-3.2.0/tests/test_xls.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      127 2023-04-13 15:51:20.000000 hukudo-3.2.0/tests/test_xls_edi.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      717 2023-04-13 16:24:52.000000 hukudo-3.2.0/tests/test_xls_sheet.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-07-13 08:18:07.071310 hukudo-3.3.0/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1077 2022-04-05 09:56:29.000000 hukudo-3.3.0/LICENSE
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1246 2023-07-13 08:18:07.071310 hukudo-3.3.0/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      890 2022-09-08 11:45:30.000000 hukudo-3.3.0/README.md
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-07-13 08:18:07.071310 hukudo-3.3.0/hukudo/
+-rw-rw-r--   0 felix     (1000) felix     (1000)       22 2023-07-13 08:18:06.000000 hukudo-3.3.0/hukudo/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     5305 2023-03-13 12:19:59.000000 hukudo-3.3.0/hukudo/chromedriver.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2235 2022-09-09 10:11:07.000000 hukudo-3.3.0/hukudo/cli.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)       43 2022-06-07 10:45:57.000000 hukudo-3.3.0/hukudo/exc.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      636 2022-09-08 11:32:36.000000 hukudo-3.3.0/hukudo/filesystem.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-07-13 08:18:07.071310 hukudo-3.3.0/hukudo/gitlab/
+-rw-rw-r--   0 felix     (1000) felix     (1000)        0 2022-07-20 19:31:40.000000 hukudo-3.3.0/hukudo/gitlab/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      745 2022-07-20 19:31:40.000000 hukudo-3.3.0/hukudo/gitlab/api.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      723 2022-07-20 19:31:40.000000 hukudo-3.3.0/hukudo/gitlab/cli.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      430 2022-07-20 19:31:40.000000 hukudo-3.3.0/hukudo/gitlab/jobs.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-07-13 08:18:07.071310 hukudo-3.3.0/hukudo/grafana/
+-rw-rw-r--   0 felix     (1000) felix     (1000)       55 2022-03-10 15:35:16.000000 hukudo-3.3.0/hukudo/grafana/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     3652 2023-05-31 11:31:40.000000 hukudo-3.3.0/hukudo/grafana/api.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2981 2023-05-31 11:40:08.000000 hukudo-3.3.0/hukudo/grafana/cli.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      263 2022-06-07 15:19:07.000000 hukudo-3.3.0/hukudo/grafana/demo.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      141 2022-06-08 10:23:35.000000 hukudo-3.3.0/hukudo/grafana/errors.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      673 2023-07-13 08:13:00.000000 hukudo-3.3.0/hukudo/grafana/models.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1076 2022-06-08 11:13:22.000000 hukudo-3.3.0/hukudo/log.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-07-13 08:18:07.071310 hukudo-3.3.0/hukudo/pypi/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      384 2022-09-09 10:11:07.000000 hukudo-3.3.0/hukudo/pypi/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      187 2022-09-09 10:12:16.000000 hukudo-3.3.0/hukudo/pypi/cli.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-07-13 08:18:07.071310 hukudo-3.3.0/hukudo/xls/
+-rw-rw-r--   0 felix     (1000) felix     (1000)       38 2023-04-13 15:49:31.000000 hukudo-3.3.0/hukudo/xls/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2392 2021-11-03 18:22:13.000000 hukudo-3.3.0/hukudo/xls/edi.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2417 2021-12-01 09:56:40.000000 hukudo-3.3.0/hukudo/xls/fmt.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     4839 2023-04-13 15:56:59.000000 hukudo-3.3.0/hukudo/xls/sheet.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2029 2023-04-13 15:49:32.000000 hukudo-3.3.0/hukudo/xls/table.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-07-13 08:18:07.071310 hukudo-3.3.0/hukudo.egg-info/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1246 2023-07-13 08:18:07.000000 hukudo-3.3.0/hukudo.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      923 2023-07-13 08:18:07.000000 hukudo-3.3.0/hukudo.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-07-13 08:18:07.000000 hukudo-3.3.0/hukudo.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       43 2023-07-13 08:18:07.000000 hukudo-3.3.0/hukudo.egg-info/entry_points.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)      533 2023-07-13 08:18:07.000000 hukudo-3.3.0/hukudo.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        7 2023-07-13 08:18:07.000000 hukudo-3.3.0/hukudo.egg-info/top_level.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)      386 2023-03-13 12:33:26.000000 hukudo-3.3.0/pyproject.toml
+-rw-rw-r--   0 felix     (1000) felix     (1000)      753 2023-07-13 08:18:07.071310 hukudo-3.3.0/setup.cfg
+-rw-rw-r--   0 felix     (1000) felix     (1000)      348 2023-03-13 12:33:26.000000 hukudo-3.3.0/setup.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-07-13 08:18:07.071310 hukudo-3.3.0/tests/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2833 2022-06-08 16:07:14.000000 hukudo-3.3.0/tests/test_chromedriver.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      305 2022-06-08 13:34:36.000000 hukudo-3.3.0/tests/test_cli.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      613 2022-07-20 19:31:40.000000 hukudo-3.3.0/tests/test_gitlab.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     5606 2023-07-13 08:16:43.000000 hukudo-3.3.0/tests/test_grafana.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      666 2022-09-08 11:39:19.000000 hukudo-3.3.0/tests/test_keepn.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      144 2022-06-08 15:28:39.000000 hukudo-3.3.0/tests/test_log.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)       80 2022-06-08 10:38:01.000000 hukudo-3.3.0/tests/test_pypi.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      436 2021-11-03 14:53:39.000000 hukudo-3.3.0/tests/test_xls.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      127 2023-04-13 15:51:20.000000 hukudo-3.3.0/tests/test_xls_edi.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      717 2023-04-13 16:24:52.000000 hukudo-3.3.0/tests/test_xls_sheet.py
```

### Comparing `hukudo-3.2.0/LICENSE` & `hukudo-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/PKG-INFO` & `hukudo-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hukudo
-Version: 3.2.0
+Version: 3.3.0
 Home-page: https://gitlab.com/hukudo/lib/
 Author: hukudo GmbH
 Author-email: python@hukudo.de
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: pypi
```

### Comparing `hukudo-3.2.0/README.md` & `hukudo-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/chromedriver.py` & `hukudo-3.3.0/hukudo/chromedriver.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/cli.py` & `hukudo-3.3.0/hukudo/cli.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/filesystem.py` & `hukudo-3.3.0/hukudo/filesystem.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/gitlab/api.py` & `hukudo-3.3.0/hukudo/gitlab/api.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/gitlab/cli.py` & `hukudo-3.3.0/hukudo/gitlab/cli.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/grafana/api.py` & `hukudo-3.3.0/hukudo/grafana/api.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/grafana/cli.py` & `hukudo-3.3.0/hukudo/grafana/cli.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/grafana/models.py` & `hukudo-3.3.0/hukudo/grafana/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     def __init__(self, raw, base_url):
         super().__init__(raw)
         base = str(base_url).rstrip('/')
         self.url = f'{base}/d/{self.uid}'
 
     def export(self, path):
         path = Path(path)
-        path.write_text(json.dumps(self.raw))
+        path.write_text(json.dumps(self.raw, sort_keys=True, indent=2))
```

### Comparing `hukudo-3.2.0/hukudo/log.py` & `hukudo-3.3.0/hukudo/log.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/xls/edi.py` & `hukudo-3.3.0/hukudo/xls/edi.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/xls/fmt.py` & `hukudo-3.3.0/hukudo/xls/fmt.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/xls/sheet.py` & `hukudo-3.3.0/hukudo/xls/sheet.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo/xls/table.py` & `hukudo-3.3.0/hukudo/xls/table.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo.egg-info/PKG-INFO` & `hukudo-3.3.0/hukudo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hukudo
-Version: 3.2.0
+Version: 3.3.0
 Home-page: https://gitlab.com/hukudo/lib/
 Author: hukudo GmbH
 Author-email: python@hukudo.de
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: pypi
```

### Comparing `hukudo-3.2.0/hukudo.egg-info/SOURCES.txt` & `hukudo-3.3.0/hukudo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/hukudo.egg-info/requires.txt` & `hukudo-3.3.0/hukudo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/setup.cfg` & `hukudo-3.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hukudo
-version = 3.2.0
+version = 3.3.0
 url = https://gitlab.com/hukudo/lib/
 author = hukudo GmbH
 author_email = python@hukudo.de
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
```

### Comparing `hukudo-3.2.0/tests/test_chromedriver.py` & `hukudo-3.3.0/tests/test_chromedriver.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/tests/test_gitlab.py` & `hukudo-3.3.0/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/tests/test_grafana.py` & `hukudo-3.3.0/tests/test_grafana.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,14 +167,18 @@
     assert 'https://grafana.dev.0-main.de/d/test-uid' in result.output
 
 
 def test_cli_dashboard_export_import(demo_env, tmp_path):
     run(demo_env, ['grafana', 'dashboard', 'export', str(tmp_path)])
     files = list(tmp_path.glob('*.json'))
     assert len(files) == 1
+    # formatted json is indented on line 2
+    contents = files[0].read_text()
+    line_2 = contents.split('\n')[1]
+    assert line_2.startswith('  ')
     for file in files:
         run(demo_env, ['grafana', 'dashboard', 'import', str(file)])
 
 
 def test_cli_config(demo_envfile):
     run(env={}, args=['grafana', '-c', demo_envfile, 'dashboard', 'list'])
```

### Comparing `hukudo-3.2.0/tests/test_keepn.py` & `hukudo-3.3.0/tests/test_keepn.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.2.0/tests/test_xls_sheet.py` & `hukudo-3.3.0/tests/test_xls_sheet.py`

 * *Files identical despite different names*

