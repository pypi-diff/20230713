# Comparing `tmp/hoppr_cop-1.1.8.tar.gz` & `tmp/hoppr_cop-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_cop-1.1.8.tar", max compression
+gzip compressed data, was "hoppr_cop-1.1.9.tar", max compression
```

## Comparing `hoppr_cop-1.1.8.tar` & `hoppr_cop-1.1.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1084 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/LICENSE.md
--rw-r--r--   0        0        0       55 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/combined/__init__.py
--rw-r--r--   0        0        0     3336 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/combined/cli.py
--rw-r--r--   0        0        0     4488 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/combined/combined_scanner.py
--rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/gemnasium/__init__.py
--rw-r--r--   0        0        0     9326 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/gemnasium/gemnasium_scanner.py
--rw-r--r--   0        0        0     1134 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/gemnasium/models.py
--rwxr-xr-x   0        0        0      113 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/gemnasium/semver
--rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/grype/__init__.py
--rw-r--r--   0        0        0     5953 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/grype/grype_scanner.py
--rw-r--r--   0        0        0     5289 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/grype/models.py
--rw-r--r--   0        0        0     9337 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/hoppr_plugin/hopprcop_plugin.py
--rw-r--r--   0        0        0      478 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/README.md
--rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/__init__.py
--rw-r--r--   0        0        0      832 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/__init__.py
--rw-r--r--   0        0        0     1029 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/exception.py
--rw-r--r--   0        0        0     9487 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/model.py
--rw-r--r--   0        0        0    11624 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/ossindex.py
--rw-r--r--   0        0        0      153 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/py.typed
--rw-r--r--   0        0        0     3147 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/serializer.py
--rw-r--r--   0        0        0     4923 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/oss_index_scanner.py
--rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/trivy/__init__.py
--rw-r--r--   0        0        0     5590 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/trivy/trivy_scanner.py
--rw-r--r--   0        0        0      854 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 hoppr_cop-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/LICENSE.md
+-rw-r--r--   0        0        0       55 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/combined/__init__.py
+-rw-r--r--   0        0        0     3336 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/combined/cli.py
+-rw-r--r--   0        0        0     4488 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/combined/combined_scanner.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/gemnasium/__init__.py
+-rw-r--r--   0        0        0     9326 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/gemnasium/gemnasium_scanner.py
+-rw-r--r--   0        0        0     1134 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/gemnasium/models.py
+-rwxr-xr-x   0        0        0      113 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/gemnasium/semver
+-rw-r--r--   0        0        0        0 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/grype/__init__.py
+-rw-r--r--   0        0        0     5953 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/grype/grype_scanner.py
+-rw-r--r--   0        0        0     5289 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/grype/models.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/hoppr_plugin/__init__.py
+-rw-r--r--   0        0        0     9337 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/hoppr_plugin/hopprcop_plugin.py
+-rw-r--r--   0        0        0      478 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/api/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/api/exception.py
+-rw-r--r--   0        0        0     9487 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/api/model.py
+-rw-r--r--   0        0        0    11624 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/api/ossindex.py
+-rw-r--r--   0        0        0      153 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/api/py.typed
+-rw-r--r--   0        0        0     3147 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/api/serializer.py
+-rw-r--r--   0        0        0     4923 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/ossindex/oss_index_scanner.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/trivy/__init__.py
+-rw-r--r--   0        0        0     5590 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/hopprcop/trivy/trivy_scanner.py
+-rw-r--r--   0        0        0      961 2023-07-13 20:05:09.000000 hoppr_cop-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 hoppr_cop-1.1.9/PKG-INFO
```

### Comparing `hoppr_cop-1.1.8/LICENSE.md` & `hoppr_cop-1.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/combined/cli.py` & `hoppr_cop-1.1.9/hopprcop/combined/cli.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/combined/combined_scanner.py` & `hoppr_cop-1.1.9/hopprcop/combined/combined_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/gemnasium/gemnasium_scanner.py` & `hoppr_cop-1.1.9/hopprcop/gemnasium/gemnasium_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/gemnasium/models.py` & `hoppr_cop-1.1.9/hopprcop/gemnasium/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/grype/grype_scanner.py` & `hoppr_cop-1.1.9/hopprcop/grype/grype_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/grype/models.py` & `hoppr_cop-1.1.9/hopprcop/grype/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/hoppr_plugin/hopprcop_plugin.py` & `hoppr_cop-1.1.9/hopprcop/hoppr_plugin/hopprcop_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/ossindex/api/__init__.py` & `hoppr_cop-1.1.9/hopprcop/ossindex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/ossindex/api/exception.py` & `hoppr_cop-1.1.9/hopprcop/ossindex/api/exception.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/ossindex/api/model.py` & `hoppr_cop-1.1.9/hopprcop/ossindex/api/model.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/ossindex/api/ossindex.py` & `hoppr_cop-1.1.9/hopprcop/ossindex/api/ossindex.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/ossindex/api/serializer.py` & `hoppr_cop-1.1.9/hopprcop/ossindex/api/serializer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/ossindex/oss_index_scanner.py` & `hoppr_cop-1.1.9/hopprcop/ossindex/oss_index_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/hopprcop/trivy/trivy_scanner.py` & `hoppr_cop-1.1.9/hopprcop/trivy/trivy_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.8/pyproject.toml` & `hoppr_cop-1.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr-cop"
-version = "1.1.8"
+version = "1.1.9"
 description = ""
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 [[tool.poetry.packages]]
 include = "hopprcop"
 
@@ -19,22 +19,25 @@
 tinydb = "^4.7.0"
 rich = ">12.5.1"
 mkdocs = "^1.3.1"
 mkdocs-mermaid2-plugin = "^0.6.0"
 hoppr = "^1.8.0"
 pytest = "7.3.1"
 coverage = "^7.0.0"
-hoppr-security-commons = "^0.0.13"
+hoppr-security-commons = "0.*"
 mkdocs-glightbox = "^0.3.1"
 pygments = "^2.14.0"
 pymdown-extensions = "^10.0.0"
 
 [tool.poetry.scripts]
 hoppr-cop = "hopprcop.combined.cli:app"
 
+[tool.poetry.plugins."hoppr.plugin"]
+hopprcop_plugin = "hopprcop.hoppr_plugin.hopprcop_plugin:HopprCopPlugin"
+
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 black = "^23.0.0"
 pylint = "^2.14.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `hoppr_cop-1.1.8/PKG-INFO` & `hoppr_cop-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: hoppr-cop
-Version: 1.1.8
+Version: 1.1.9
 Summary: 
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: coverage (>=7.0.0,<8.0.0)
 Requires-Dist: cvss (>=2.5,<3.0)
 Requires-Dist: hoppr (>=1.8.0,<2.0.0)
 Requires-Dist: hoppr-cyclonedx-models (>=0.4.7)
-Requires-Dist: hoppr-security-commons (>=0.0.13,<0.0.14)
+Requires-Dist: hoppr-security-commons (==0.*)
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0)
 Requires-Dist: mkdocs-glightbox (>=0.3.1,<0.4.0)
 Requires-Dist: mkdocs-mermaid2-plugin (>=0.6.0,<0.7.0)
 Requires-Dist: packageurl-python (>=0.10.1,<0.11.0)
 Requires-Dist: pygments (>=2.14.0,<3.0.0)
 Requires-Dist: pymdown-extensions (>=10.0.0,<11.0.0)
 Requires-Dist: pytest (==7.3.1)
```

