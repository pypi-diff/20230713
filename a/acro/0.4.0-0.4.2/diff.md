# Comparing `tmp/acro-0.4.0.tar.gz` & `tmp/acro-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acro-0.4.0.tar", last modified: Tue Jul 11 11:27:04 2023, max compression
+gzip compressed data, was "acro-0.4.2.tar", last modified: Thu Jul 13 13:22:01 2023, max compression
```

## Comparing `acro-0.4.0.tar` & `acro-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:27:04.854569 acro-0.4.0/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2023-07-11 11:22:02.000000 acro-0.4.0/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-11 11:27:04.854569 acro-0.4.0/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2227 2023-07-11 11:22:02.000000 acro-0.4.0/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:27:04.854569 acro-0.4.0/acro/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-07-11 11:22:02.000000 acro-0.4.0/acro/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    32413 2023-07-11 11:22:02.000000 acro-0.4.0/acro/acro.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1072 2023-07-11 11:22:02.000000 acro-0.4.0/acro/default.yaml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19383 2023-07-11 11:22:02.000000 acro-0.4.0/acro/record.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10320 2023-07-11 11:22:02.000000 acro-0.4.0/acro/utils.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       49 2023-07-11 11:22:02.000000 acro-0.4.0/acro/version.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:27:04.854569 acro-0.4.0/acro.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      339 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-11 11:27:04.854569 acro-0.4.0/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-07-11 11:22:14.000000 acro-0.4.0/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:27:04.854569 acro-0.4.0/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:22:02.000000 acro-0.4.0/test/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2056 2023-07-11 11:22:02.000000 acro-0.4.0/test/stata.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14281 2023-07-11 11:22:02.000000 acro-0.4.0/test/test_initial.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9013 2023-07-11 11:22:02.000000 acro-0.4.0/test/test_stata_interface.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-13 13:22:01.486328 acro-0.4.2/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2023-07-11 11:22:02.000000 acro-0.4.2/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-13 13:22:01.486328 acro-0.4.2/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2227 2023-07-13 09:47:17.000000 acro-0.4.2/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-13 13:22:01.486328 acro-0.4.2/acro/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-07-11 11:22:02.000000 acro-0.4.2/acro/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    32494 2023-07-13 13:10:29.000000 acro-0.4.2/acro/acro.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1072 2023-07-11 11:22:02.000000 acro-0.4.2/acro/default.yaml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19460 2023-07-13 13:10:29.000000 acro-0.4.2/acro/record.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10320 2023-07-13 09:50:52.000000 acro-0.4.2/acro/utils.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       49 2023-07-13 13:18:59.000000 acro-0.4.2/acro/version.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-13 13:22:01.486328 acro-0.4.2/acro.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-13 13:22:01.000000 acro-0.4.2/acro.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      339 2023-07-13 13:22:01.000000 acro-0.4.2/acro.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-13 13:22:01.000000 acro-0.4.2/acro.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-07-13 13:22:01.000000 acro-0.4.2/acro.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-07-13 13:22:01.000000 acro-0.4.2/acro.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-13 13:22:01.486328 acro-0.4.2/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-07-13 13:18:53.000000 acro-0.4.2/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-13 13:22:01.486328 acro-0.4.2/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:22:02.000000 acro-0.4.2/test/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2056 2023-07-13 09:47:17.000000 acro-0.4.2/test/stata.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14281 2023-07-13 09:47:17.000000 acro-0.4.2/test/test_initial.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9013 2023-07-13 09:47:17.000000 acro-0.4.2/test/test_stata_interface.py
```

### Comparing `acro-0.4.0/LICENSE` & `acro-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acro-0.4.0/PKG-INFO` & `acro-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.4.0
+Version: 0.4.2
 Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acro-0.4.0/README.md` & `acro-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `acro-0.4.0/acro/acro.py` & `acro-0.4.2/acro/acro.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pandas import DataFrame
 from statsmodels.discrete.discrete_model import BinaryResultsWrapper
 from statsmodels.iolib.table import SimpleTable
 from statsmodels.regression.linear_model import RegressionResultsWrapper
 
 from . import utils
 from .record import Records
+from .version import __version__
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("acro")
 warnings.simplefilter(action="ignore", category=FutureWarning)
 
 
 class ACRO:
@@ -58,14 +59,15 @@
         self.config: dict = {}
         self.results: Records = Records()
         self.suppress: bool = suppress
         path = pathlib.Path(__file__).with_name(config + ".yaml")
         logger.debug("path: %s", path)
         with open(path, encoding="utf-8") as handle:
             self.config = yaml.load(handle, Loader=yaml.loader.SafeLoader)
+        logger.info("version: %s", __version__)
         logger.info("config: %s", self.config)
         logger.info("automatic suppression: %s", self.suppress)
         # set globals needed for aggregation functions
         utils.THRESHOLD = self.config["safe_threshold"]
         utils.SAFE_PRATIO_P = self.config["safe_pratio_p"]
         utils.SAFE_NK_N = self.config["safe_nk_n"]
         utils.SAFE_NK_K = self.config["safe_nk_k"]
```

### Comparing `acro-0.4.0/acro/default.yaml` & `acro-0.4.2/acro/default.yaml`

 * *Files identical despite different names*

### Comparing `acro-0.4.0/acro/record.py` & `acro-0.4.2/acro/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,14 +334,15 @@
             command="custom",
             summary="review",
             outcome=DataFrame(),
             output=[os.path.normpath(filename)],
             comments=None if comment is None else [comment],
         )
         self.results[output.uid] = output
+        logger.info("add_custom(): %s", output.uid)
 
     def rename(self, old: str, new: str) -> None:
         """Rename an output.
 
         Parameters
         ----------
         old : str
@@ -403,21 +404,22 @@
         print(outputs)
         return outputs
 
     def validate_outputs(self) -> None:
         """Prompts researcher to complete any required fields."""
         for _, record in self.results.items():
             if record.status != "pass" and record.exception == "":
-                print(
-                    f"{str(record)}\n"
-                    f"The status of the record above is: {record.status}.\n"
-                    "Please explain why an exception should be granted.\n"
+                logger.info(
+                    "\n%s\n"
+                    "The status of the record above is: %s.\n"
+                    "Please explain why an exception should be granted.\n",
+                    str(record),
+                    record.status,
                 )
                 record.exception = input("")
-                print("")
 
     def finalise(self, path: str, ext: str) -> None:
         """Creates a results file for checking.
 
         Parameters
         ----------
         path : str
```

### Comparing `acro-0.4.0/acro/utils.py` & `acro-0.4.2/acro/utils.py`

 * *Files identical despite different names*

### Comparing `acro-0.4.0/acro.egg-info/PKG-INFO` & `acro-0.4.2/acro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.4.0
+Version: 0.4.2
 Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acro-0.4.0/setup.py` & `acro-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="acro",
-    version="0.4.0",
+    version="0.4.2",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="ACRO: Tools for the Automatic Checking of Research Outputs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/ACRO",
```

### Comparing `acro-0.4.0/test/stata.py` & `acro-0.4.2/test/stata.py`

 * *Files identical despite different names*

### Comparing `acro-0.4.0/test/test_initial.py` & `acro-0.4.2/test/test_initial.py`

 * *Files identical despite different names*

### Comparing `acro-0.4.0/test/test_stata_interface.py` & `acro-0.4.2/test/test_stata_interface.py`

 * *Files identical despite different names*

