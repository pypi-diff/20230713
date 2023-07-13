# Comparing `tmp/puwifi-1.0.4.tar.gz` & `tmp/puwifi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puwifi-1.0.4.tar", last modified: Thu Jul 13 09:28:48 2023, max compression
+gzip compressed data, was "puwifi-1.0.5.tar", last modified: Thu Jul 13 09:34:14 2023, max compression
```

## Comparing `puwifi-1.0.4.tar` & `puwifi-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:28:48.084236 puwifi-1.0.4/
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.4/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:28:48.074236 puwifi-1.0.4/.github/
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.4/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:28:48.074236 puwifi-1.0.4/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.4/.github/workflows/pylint.yml
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.4/.pylintrc
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3867 2023-07-13 09:28:48.084236 puwifi-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3259 2023-07-10 18:08:53.000000 puwifi-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:28:48.074236 puwifi-1.0.4/puwifi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3867 2023-07-13 09:28:48.000000 puwifi-1.0.4/puwifi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-13 09:28:48.000000 puwifi-1.0.4/puwifi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:28:48.000000 puwifi-1.0.4/puwifi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-13 09:28:48.000000 puwifi-1.0.4/puwifi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-13 09:28:48.000000 puwifi-1.0.4/puwifi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 09:28:48.000000 puwifi-1.0.4/puwifi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9135 2023-07-13 09:27:14.000000 puwifi-1.0.4/puwifi.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-13 09:27:28.000000 puwifi-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.4/renovate.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 09:28:48.084236 puwifi-1.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:34:14.814235 puwifi-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.5/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:34:14.814235 puwifi-1.0.5/.github/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.5/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:34:14.814235 puwifi-1.0.5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.5/.github/workflows/pylint.yml
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.5/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-07-13 09:34:14.814235 puwifi-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-10 18:08:53.000000 puwifi-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:34:14.814235 puwifi-1.0.5/puwifi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9136 2023-07-13 09:32:09.000000 puwifi-1.0.5/puwifi.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-13 09:34:07.000000 puwifi-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.5/renovate.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 09:34:14.814235 puwifi-1.0.5/setup.cfg
```

### Comparing `puwifi-1.0.4/.github/workflows/codeql-analysis.yml` & `puwifi-1.0.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.4/.github/workflows/pylint.yml` & `puwifi-1.0.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.4/.gitignore` & `puwifi-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.4/.pylintrc` & `puwifi-1.0.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.4/LICENSE` & `puwifi-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.4/PKG-INFO` & `puwifi-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puwifi
-Version: 1.0.4
+Version: 1.0.5
 Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
 Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
 Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
 Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `puwifi-1.0.4/README.md` & `puwifi-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.4/puwifi.egg-info/PKG-INFO` & `puwifi-1.0.5/puwifi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puwifi
-Version: 1.0.4
+Version: 1.0.5
 Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
 Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
 Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
 Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `puwifi-1.0.4/puwifi.py` & `puwifi-1.0.5/puwifi.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """class for wifi utils"""
     def __init__(self, username, password, host, port):
         self.username = username
         self.password = password
         self.host = host
         self.port = port
 
-    def pw_request(cls,
+    def pw_request(self,
                 method,
                 username,
                 password,
                 host, port,
                 timeout) -> list:
         """request method: sends request to wifi host
```

### Comparing `puwifi-1.0.4/pyproject.toml` & `puwifi-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="puwifi"
-version="1.0.4"
+version="1.0.5"
 
 authors = [
     { name="SaicharanKandukuri", email="saicharankandukuri1x1@gmail.com"}
 ]
 
 description = "⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever"
 readme = "README.md"
```

