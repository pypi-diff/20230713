# Comparing `tmp/antgen-0.2.1.tar.gz` & `tmp/antgen-0.2.2.tar.gz`

## Comparing `antgen-0.2.1.tar` & `antgen-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 antgen-0.2.1/.gitignore
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 antgen-0.2.1/LICENSE
--rw-r--r--   0        0        0    18577 2020-02-02 00:00:00.000000 antgen-0.2.1/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 antgen-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    18829 2020-02-02 00:00:00.000000 antgen-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 antgen-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 antgen-0.2.2/LICENSE
+-rw-r--r--   0        0        0    18577 2020-02-02 00:00:00.000000 antgen-0.2.2/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 antgen-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    18829 2020-02-02 00:00:00.000000 antgen-0.2.2/PKG-INFO
```

### Comparing `antgen-0.2.1/LICENSE` & `antgen-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antgen-0.2.1/README.md` & `antgen-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `antgen-0.2.1/pyproject.toml` & `antgen-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "antgen"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Nuno Velosa", email="nunovelosa@hotmail.com" },
 ]
 description = "This tool generates synthetic macroscopic load signatures for their use in conjunction with NILM (load disaggregation) tools."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `antgen-0.2.1/PKG-INFO` & `antgen-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antgen
-Version: 0.2.1
+Version: 0.2.2
 Summary: This tool generates synthetic macroscopic load signatures for their use in conjunction with NILM (load disaggregation) tools.
 Project-URL: Homepage, https://gitlab.com/nunovelosa/antgen
 Project-URL: Bug Tracker, https://gitlab.com/nunovelosa/antgen/issues
 Author-email: Nuno Velosa <nunovelosa@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

