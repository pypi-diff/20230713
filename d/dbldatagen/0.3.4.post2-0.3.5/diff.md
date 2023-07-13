# Comparing `tmp/dbldatagen-0.3.4.post2.tar.gz` & `tmp/dbldatagen-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbldatagen-0.3.4.post2.tar", last modified: Tue Apr 18 23:02:02 2023, max compression
+gzip compressed data, was "dbldatagen-0.3.5.tar", last modified: Thu Jul 13 17:23:23 2023, max compression
```

## Comparing `dbldatagen-0.3.4.post2.tar` & `dbldatagen-0.3.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/dbldatagen/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/column_generation_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/column_spec_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    57532 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/datagen_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/datarange.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/daterange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/dbldatagen/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/data_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/exponential_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/function_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/nrange.py
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/schema_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/spark_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/text_generator_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    41986 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/text_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/dbldatagen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-18 23:02:02.000000 dbldatagen-0.3.4.post2/dbldatagen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 23:02:02.000000 dbldatagen-0.3.4.post2/dbldatagen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:02:02.000000 dbldatagen-0.3.4.post2/dbldatagen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 23:02:02.000000 dbldatagen-0.3.4.post2/dbldatagen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:23:23.115438 dbldatagen-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-07-13 17:23:23.115438 dbldatagen-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:23:23.115438 dbldatagen-0.3.5/dbldatagen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61074 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/column_generation_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/column_spec_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65625 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/datagen_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/datarange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/daterange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:23:23.115438 dbldatagen-0.3.5/dbldatagen/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/distributions/data_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/distributions/exponential_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/distributions/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/function_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/nrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/schema_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/spark_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/text_generator_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41986 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/text_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/dbldatagen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:23:23.115438 dbldatagen-0.3.5/dbldatagen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-07-13 17:23:23.000000 dbldatagen-0.3.5/dbldatagen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 17:23:23.000000 dbldatagen-0.3.5/dbldatagen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:23:23.000000 dbldatagen-0.3.5/dbldatagen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 17:23:23.000000 dbldatagen-0.3.5/dbldatagen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 17:23:23.115438 dbldatagen-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-13 17:22:12.000000 dbldatagen-0.3.5/setup.py
```

### Comparing `dbldatagen-0.3.4.post2/CHANGELOG.md` & `dbldatagen-0.3.5/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 # Databricks Labs Data Generator Release Notes
 
 ## Change History
 All notable changes to the Databricks Labs Data Generator will be documented in this file.
 
+### Version 0.3.5
+
+#### Changed
+* Added formatting of generated code as Html for script methods
+* Allow use of inferred types on `withColumn` method when `expr` attribute is used
+* Added ``withStructColumn`` method to allow simplified generation of struct and JSON columns
+* Modified pipfile to use newer version of package specifications
+
+### Version 0.3.4 Post 3
+
+### Changed
+* Build now uses Python 3.8.12. Updated build process to reflect that.
+
 ### Version 0.3.4 Post 2
 
 ### Fixed
 * Fix for use of values in columns of type array, map and struct 
 * Fix for generation of arrays via `numFeatures` and `structType` attributes when numFeatures has value of 1
 
+
 ### Version 0.3.4 Post 1
 
 ### Fixed
 * Fix for use and configuration of root logger 
 
 ### Acknowledgements
 Thanks to Marvin Schenkel for the contribution
@@ -134,15 +148,15 @@
 
 For example:
 
 `%pip install dbldatagen`
 
 To use an older DB runtime version in your notebook, you can use the following code in your notebook:
 
-```commandline
+```shell
 %pip install git+https://github.com/databrickslabs/dbldatagen@dbr_7_3_LTS_compat
 ```
 
 See the [Databricks runtime release notes](https://docs.databricks.com/release-notes/runtime/releases.html) 
  for the full list of dependencies used by the Databricks runtime.
 
 This can be found at : https://docs.databricks.com/release-notes/runtime/releases.html
```

### Comparing `dbldatagen-0.3.4.post2/CONTRIBUTING.md` & `dbldatagen-0.3.5/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 ## Package Dependencies
 See the contents of the file `python/require.txt` to see the Python package dependencies. 
 Dependent packages are not installed automatically by the `dbldatagen` package.
 
 ## Python compatibility
 
-The code has been tested with Python 3.8.10 and later.
+The code has been tested with Python 3.8.12 and later.
 
-Older releases were tested with Python 3.7.5 but as of this release, it requires the Databricks runtime 9.1 LTS or later
-which relies on Python 3.8.10
+Older releases were tested with Python 3.7.5 but as of this release, it requires the Databricks 
+runtime 9.1 LTS or later. 
 
 ## Checking your code for common issues
 
 Run `./lint.sh` from the project root directory to run various code style checks. 
 These are based on the use of `prospector`, `pylint` and related tools.
 
 ## Setting up your build environment
```

### Comparing `dbldatagen-0.3.4.post2/LICENSE` & `dbldatagen-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/PKG-INFO` & `dbldatagen-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.4.post2
+Version: 0.3.5
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post2/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.5/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4.post2/PULL_REQUEST_TEMPLATE.md` & `dbldatagen-0.3.5/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/README.md` & `dbldatagen-0.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post2/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.5/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/__init__.py` & `dbldatagen-0.3.5/dbldatagen/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,34 +21,37 @@
 the `DataGenerator` class.
 
 Most of the other classes are used for internal purposes only
 """
 
 from .data_generator import DataGenerator
 from .datagen_constants import DEFAULT_RANDOM_SEED, RANDOM_SEED_RANDOM, RANDOM_SEED_FIXED, \
-                               RANDOM_SEED_HASH_FIELD_NAME, MIN_PYTHON_VERSION, MIN_SPARK_VERSION
+                               RANDOM_SEED_HASH_FIELD_NAME, MIN_PYTHON_VERSION, MIN_SPARK_VERSION, \
+                               INFER_DATATYPE
 from .utils import ensure, topologicalSort, mkBoundsList, coalesce_values, \
-    deprecated, parse_time_interval, DataGenError, split_list_matching_condition, strip_margins
+    deprecated, parse_time_interval, DataGenError, split_list_matching_condition, strip_margins, \
+    json_value_from_path, system_time_millis
 from ._version import __version__
 from .column_generation_spec import ColumnGenerationSpec
 from .column_spec_options import ColumnSpecOptions
 from .data_analyzer import DataAnalyzer
 from .schema_parser import SchemaParser
 from .daterange import DateRange
 from .datarange import DataRange
 from .nrange import NRange
 from .function_builder import ColumnGeneratorBuilder
 from .spark_singleton import SparkSingleton
 from .text_generators import TemplateGenerator, ILText, TextGenerator
 from .text_generator_plugins import PyfuncText, PyfuncTextFactory, FakerTextFactory, fakerText
+from .html_utils import HtmlUtils
 
 __all__ = ["data_generator", "data_analyzer", "schema_parser", "daterange", "nrange",
            "column_generation_spec", "utils", "function_builder",
            "spark_singleton", "text_generators", "datarange", "datagen_constants",
-           "text_generator_plugins"
+           "text_generator_plugins", "html_utils"
            ]
 
 
 def python_version_check(python_version_expected):
     """Check against Python version
 
        Allows minimum version to be passed in to facilitate unit testing
```

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/_version.py` & `dbldatagen-0.3.5/dbldatagen/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     major, minor, patch, release, build = r.match(version).groups()
     version_info = VersionInfo(major, minor, patch, release, build)
     logger = logging.getLogger(__name__)
     logger.info("Version : %s", version_info)
     return version_info
 
 
-__version__ = "0.3.4post2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "0.3.5"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
 
 
 def _get_spark_version(sparkVersion):
     try:
         r = re.compile(r'(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>.*)')
         major, minor, patch, release = r.match(sparkVersion).groups()
```

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/column_generation_spec.py` & `dbldatagen-0.3.5/dbldatagen/column_generation_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 import pyspark.sql.functions as F
 
 from pyspark.sql.types import FloatType, IntegerType, StringType, DoubleType, BooleanType, \
     TimestampType, DataType, DateType, ArrayType, MapType, StructType
 
 from .column_spec_options import ColumnSpecOptions
 from .datagen_constants import RANDOM_SEED_FIXED, RANDOM_SEED_HASH_FIELD_NAME, RANDOM_SEED_RANDOM, \
-    DEFAULT_SEED_COLUMN, OPTION_RANDOM, OPTION_RANDOM_SEED, OPTION_RANDOM_SEED_METHOD
+    DEFAULT_SEED_COLUMN, OPTION_RANDOM, OPTION_RANDOM_SEED, OPTION_RANDOM_SEED_METHOD, INFER_DATATYPE
 
 from .daterange import DateRange
 from .distributions import Normal, DataDistribution
 from .nrange import NRange
 from .text_generators import TemplateGenerator
 from .utils import ensure, coalesce_values
+from .schema_parser import SchemaParser
 
 HASH_COMPUTE_METHOD = "hash"
 VALUES_COMPUTE_METHOD = "values"
 RAW_VALUES_COMPUTE_METHOD = "raw_values"
 AUTO_COMPUTE_METHOD = "auto"
+EXPR_OPTION = "expr"
 COMPUTE_METHOD_VALID_VALUES = [HASH_COMPUTE_METHOD,
                                AUTO_COMPUTE_METHOD,
                                VALUES_COMPUTE_METHOD,
                                RAW_VALUES_COMPUTE_METHOD]
 
 
 class ColumnGenerationSpec(object):
@@ -103,16 +105,26 @@
         self.debug = debug
 
         self._setup_logger()
 
         # set up default range and type for column
         self._dataRange = NRange(None, None, None)  # by default range of values for  column is unconstrained
 
+        self._inferDataType = False
         if colType is None:  # default to integer field if none specified
             colType = IntegerType()
+        elif colType == INFER_DATATYPE:
+            colType = StringType()  # default inferred data type to string until exact type is known
+            self._inferDataType = True
+
+            if EXPR_OPTION not in kwargs:
+                raise ValueError("Column generation spec must have `expr` attribute specified if datatype is inferred")
+
+        elif type(colType) == str:
+            colType = SchemaParser.columnTypeFromString(colType)
 
         assert isinstance(colType, DataType), f"colType `{colType}` is not instance of DataType"
 
         self._initialBuildPlan = []  # the build plan for the column - descriptive only
         self.executionHistory = []  # the execution history for the column
 
         self._seedColumnName = seedColumnName
@@ -396,14 +408,20 @@
 
     @property
     def textGenerator(self):
         """ Get the text generator for the column spec"""
         return self._textGenerator
 
     @property
+    def inferDatatype(self):
+        """ If True indicates that datatype should be inferred to be result of computing SQL expression
+        """
+        return self._inferDataType
+
+    @property
     def baseColumns(self):
         """ Return base columns as list of strings"""
 
         # if base column  is string and contains multiple columns, split them
         # other build list of columns if needed
         if type(self.baseColumn) is str and "," in self.baseColumn:
             return [x.strip() for x in self.baseColumn.split(",")]
@@ -1026,19 +1044,20 @@
             # for array, struct and map types, either value is provided via `expr` or via values
             if not type(self.datatype) in [ArrayType, MapType, StructType] or self.values is not None:
                 self._computeImpliedRangeIfNeeded(self.datatype)
 
             # TODO: add full support for date value generation
             if self.expr is not None:
                 # note use of SQL expression ignores range specifications
-                new_def = expr(self.expr).astype(self.datatype)
-
-                # record execution history
+                new_def = expr(self.expr)
                 self.executionHistory.append(f".. using SQL expression `{self.expr}` as base")
-                self.executionHistory.append(f".. casting to  `{self.datatype}`")
+
+                if not self._inferDataType:
+                    new_def = new_def.astype(self.datatype)
+                    self.executionHistory.append(f".. casting to  `{self.datatype}`")
             elif type(self.datatype) in [ArrayType, MapType, StructType] and self.values is None:
                 new_def = expr("NULL")
             elif self._dataRange is not None and self._dataRange.isFullyPopulated():
                 self.executionHistory.append(f".. computing ranged value: {self._dataRange}")
                 new_def = self._computeRangedColumn(base_column=self.baseColumn, datarange=self._dataRange,
                                                     is_random=col_is_rand)
             elif type(self.datatype) is DateType:
@@ -1079,14 +1098,30 @@
 
         new_def = self._applyFinalCastExpression(self.datatype, new_def)
 
         if percent_nulls is not None:
             new_def = self._applyComputePercentNullsExpression(new_def, percent_nulls)
         return new_def
 
+    def _onSelect(self, df):
+        """
+        The _onSelect method is called when the column specifications expression as produced by the
+        method ``_makeSingleGenerationExpression`` is used in a select statement.
+
+        :param df: Dataframe in which expression is used
+        :return: nothing
+
+        .. note:: The purpose of this method is to allow for introspection of information such as datatype
+                  which can only be determined when column specifications expression is used.
+        """
+        if self._inferDataType:
+            inferred_type = df.schema[self.name].dataType
+            self.logger.info("Inferred datatype for column %s as %s", self.name, str(inferred_type))
+            self._csOptions.options['type'] = inferred_type
+
     def _applyTextFormatExpression(self, new_def, sformat):
         # note :
         # while it seems like this could use a shared instance, this does not work if initialized
         # in a class method
         self.executionHistory.append(f".. applying column format  `{sformat}`")
         new_def = format_string(sformat, new_def)
         return new_def
@@ -1137,14 +1172,17 @@
         :returns: new column definition
         """
         self.executionHistory.append(f".. casting column [{self.name}] to  `{col_type}`")
 
         # cast the result to the appropriate type. For dates, cast first to timestamp, then to date
         if type(col_type) is DateType:
             new_def = new_def.astype(TimestampType()).astype(col_type)
+        elif self._inferDataType:
+            # dont apply cast when column has an inferred data type
+            pass
         else:
             new_def = new_def.astype(col_type)
 
         return new_def
 
     def _applyComputePercentNullsExpression(self, newDef, probabilityNulls):
         """Compute percentage nulls for column being generated
```

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/column_spec_options.py` & `dbldatagen-0.3.5/dbldatagen/column_spec_options.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/data_analyzer.py` & `dbldatagen-0.3.5/dbldatagen/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/data_generator.py` & `dbldatagen-0.3.5/dbldatagen/data_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 This file defines the `DataGenError` and `DataGenerator` classes
 """
 import copy
 import logging
 import re
 
 from pyspark.sql.types import LongType, IntegerType, StringType, StructType, StructField, DataType
-from .spark_singleton import SparkSingleton
+
+from ._version import _get_spark_version
 from .column_generation_spec import ColumnGenerationSpec
 from .datagen_constants import DEFAULT_RANDOM_SEED, RANDOM_SEED_FIXED, RANDOM_SEED_HASH_FIELD_NAME, \
-                               DEFAULT_SEED_COLUMN, SPARK_RANGE_COLUMN, MIN_SPARK_VERSION, \
-                               OPTION_RANDOM, OPTION_RANDOM_SEED, OPTION_RANDOM_SEED_METHOD
-
-from .utils import ensure, topologicalSort, DataGenError, deprecated, split_list_matching_condition
-from . _version import _get_spark_version
+    DEFAULT_SEED_COLUMN, SPARK_RANGE_COLUMN, MIN_SPARK_VERSION, \
+    OPTION_RANDOM, OPTION_RANDOM_SEED, OPTION_RANDOM_SEED_METHOD, \
+    INFER_DATATYPE
+from .html_utils import HtmlUtils
 from .schema_parser import SchemaParser
+from .spark_singleton import SparkSingleton
+from .utils import ensure, topologicalSort, DataGenError, deprecated, split_list_matching_condition
 
 _OLD_MIN_OPTION = 'min'
 _OLD_MAX_OPTION = 'max'
 
 _STREAMING_TIMESTAMP_COLUMN = "_source_timestamp"
 
 
@@ -57,15 +59,16 @@
 
     _allowed_keys = ["startingId", "rowCount", "output_id"]
 
     # set up logging
 
     # restrict spurious messages from java gateway
     logging.getLogger("py4j").setLevel(logging.WARNING)
-    #logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.NOTSET)
+
+    # logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.NOTSET)
 
     def __init__(self, sparkSession=None, name=None, randomSeedMethod=None,
                  rows=1000000, startingId=0, randomSeed=None, partitions=None, verbose=False,
                  batchSize=None, debug=False, seedColumnName=DEFAULT_SEED_COLUMN,
                  random=False,
                  **kwargs):
         """ Constructor for data generator object """
@@ -178,15 +181,15 @@
 
         Layout of version string must be compatible "xx.xx.xx.patch"
         """
         sparkVersionInfo = _get_spark_version(sparkVersion)
 
         if sparkVersionInfo < minSparkVersion:
             logging.warning(f"*** Minimum version of Python supported is {minSparkVersion} - found version %s ",
-                         sparkVersionInfo )
+                            sparkVersionInfo)
             return False
 
         return True
 
     def _setupSparkSession(self, sparkSession):
         """
         Set up spark session
@@ -484,20 +487,31 @@
         return [fd for fd in self._inferredSchemaFields if not self._columnSpecsByName[fd.name].isFieldOmitted]
 
     @property
     def schema(self):
         """ infer spark output schema definition from the field specifications
 
         :returns: Spark SQL `StructType` for schema
+
+        ..note::
+          If the data generation specification contains columns for which the datatype is inferred, the schema type
+          for inferred columns may not be correct until the build command has completed.
+
         """
         return StructType(self.schemaFields)
 
     @property
     def inferredSchema(self):
-        """ infer spark interim schema definition from the field specifications"""
+        """ infer spark interim schema definition from the field specifications
+
+        ..note::
+          If the data generation specification contains columns for which the datatype is inferred, the schema type
+          for inferred columns may not be correct until the build command has completed.
+
+        """
         self._checkFieldList()
         return StructType(self._inferredSchemaFields)
 
     def __getitem__(self, key):
         """ implement the built in derefernce by key behavior """
         ensure(key is not None, "key should be non-empty")
         return self._columnSpecsByName[key]
@@ -602,15 +616,16 @@
         :param fields: a string specifying an explicit field to match , or a list of strings specifying
                        explicit fields to match. May be omitted.
         :param matchTypes: a single Spark SQL datatype or list of Spark SQL data types to match. May be omitted.
         :returns: modified in-place instance of test data generator allowing for chaining of calls following
                   Builder pattern
 
         .. note::
-           matchTypes may also take SQL type strings or a list of SQL type strings such as "array<integer>"
+           matchTypes may also take SQL type strings or a list of SQL type strings such as "array<integer>". However,
+           you may not use ``INFER_DATYTYPE`` as part of the matchTypes list.
 
         You may also add a variety of options to further control the test data generation process.
         For full list of options, see :doc:`/reference/api/dbldatagen.column_spec_options`.
 
         """
         if fields is not None and type(fields) is str:
             fields = [fields]
@@ -640,14 +655,17 @@
             effective_fields = [x for x in effective_fields for y in patterns if re.search(y, x) is not None]
 
         if matchTypes is not None:
             effective_types = []
 
             for typ in matchTypes:
                 if isinstance(typ, str):
+                    if typ == INFER_DATATYPE:
+                        raise ValueError("You cannot use INFER_DATATYPE with the method `withColumnSpecs`")
+
                     effective_types.append(SchemaParser.columnTypeFromString(typ))
                 else:
                     effective_types.append(typ)
 
             effective_fields = [x for x in effective_fields for y in effective_types
                                 if self.getColumnType(x) == y]
 
@@ -757,14 +775,27 @@
 
         :param baseColumn: String or list of columns to control order of generation of columns. If not specified,
                            column is dependent on base seed column (which defaults to `id`)
 
         :returns: modified in-place instance of test data generator allowing for chaining of calls
                   following Builder pattern
 
+        .. note::
+           if the value ``None`` is used for the ``colType`` parameter, the method will try to use the underlying
+           datatype derived from the base columns.
+
+           If the value ``INFER_DATATYPE`` is used for the ``colType`` parameter and a SQL expression has been supplied
+           via the ``expr`` parameter, the method will try to infer the column datatype from the SQL expression when
+           the ``build()`` method is called.
+
+           Inferred data types can only be used if the ``expr`` parameter is specified.
+
+           Note that properties which return a schema based on the specification may not be accurate until the
+           ``build()`` method is called. Prior to this, the schema may indicate a default column type for those fields.
+
         You may also add a variety of additional options to further control the test data generation process.
         For full list of options, see :doc:`/reference/api/dbldatagen.column_spec_options`.
 
         """
         ensure(colName is not None, "Must specify column name for column")
         ensure(colType is not None, f"Must specify column type for column `{colName}`")
         if baseColumn is not None:
@@ -789,41 +820,149 @@
 
         if random is None:
             random = self._defaultRandom
 
         new_props = {}
         new_props.update(kwargs)
 
-        if type(colType) == str:
-            colType = SchemaParser.columnTypeFromString(colType)
-
         self.logger.info("effective range: %s, %s, %s args: %s", minValue, maxValue, step, kwargs)
         self.logger.info("adding column - `%s` with baseColumn : `%s`, implicit : %s , omit %s",
                          colName, baseColumn, implicit, omit)
-        self._generateColumnDefinition(colName, colType, minValue=minValue, maxValue=maxValue,
-                                       step=step, prefix=prefix, random=random,
-                                       distribution=distribution, baseColumn=baseColumn, dataRange=dataRange,
-                                       implicit=implicit, omit=omit, **new_props)
-        self._inferredSchemaFields.append(StructField(colName, colType, nullable))
+        newColumn = self._generateColumnDefinition(colName, colType, minValue=minValue, maxValue=maxValue,
+                                                   step=step, prefix=prefix, random=random,
+                                                   distribution=distribution, baseColumn=baseColumn,
+                                                   dataRange=dataRange,
+                                                   implicit=implicit, omit=omit, **new_props)
+
+        # note for inferred columns, the column type is initially sey to a StringType but may be superceded later
+        self._inferredSchemaFields.append(StructField(colName, newColumn.datatype, nullable))
         return self
 
+    def _mkSqlStructFromList(self, fields):
+        """
+        Create a SQL struct expression from a list of fields
+
+        :param fields: a list of elements that make up the SQL struct expression (each being a string or tuple)
+        :returns: SQL expression to generate the struct
+
+        .. note::
+          This method is used internally when creating struct columns. It is not intended for general use.
+
+          Each element of the list may be a simple string, or a tuple.
+          When the element is specified as a simple string, it must be the name of a previously defined column which
+          will be used as both the field name within the struct and the SQL expression to generate the field value.
+
+          When the element is specified as a tuple, it must be a tuple of two elements. The first element must be the
+          name of the field within the struct. The second element must be a SQL expression that will be used to generate
+          the field value, and may reference previously defined columns.
+        """
+        assert fields is not None and isinstance(fields, list), \
+            "Fields must be a non-empty list of fields that make up the struct elements"
+        assert len(fields) >= 1, "Fields must be a non-empty list of fields that make up the struct elements"
+
+        struct_expressions = []
+
+        for fieldSpec in fields:
+            if isinstance(fieldSpec, str):
+                struct_expressions.append(f"'{fieldSpec}'")
+                struct_expressions.append(fieldSpec)
+            elif isinstance(fieldSpec, tuple):
+                assert len(fieldSpec) == 2, "tuple must be field name and SQL expression strings"
+                assert isinstance(fieldSpec[0], str), "First element must be field name string"
+                assert isinstance(fieldSpec[1], str), "Second element must be field value SQL string"
+                struct_expressions.append(f"'{fieldSpec[0]}'")
+                struct_expressions.append(fieldSpec[1])
+
+        struct_expression = f"named_struct({','.join(struct_expressions)})"
+        return struct_expression
+
+    def _mkStructFromDict(self, fields):
+        assert fields is not None and isinstance(fields, dict), \
+            "Fields must be a non-empty dict of fields that make up the struct elements"
+        struct_expressions = []
+
+        for key, value in fields.items():
+            struct_expressions.append(f"'{key}'")
+            if isinstance(value, str):
+                struct_expressions.append(str(value))
+            elif isinstance(value, dict):
+                struct_expressions.append(self._mkStructFromDict(value))
+            elif isinstance(value, list):
+                array_expressions = ",".join([str(x) for x in value])
+                struct_expressions.append(f"array({array_expressions})")
+            else:
+                raise ValueError(f"Invalid field element for field `{key}`")
+
+        struct_expression = f"named_struct({','.join(struct_expressions)})"
+        return struct_expression
+
+    def withStructColumn(self, colName, fields=None, asJson=False, **kwargs):
+        """
+        Add a struct column to the synthetic data generation specification. This will add a new column composed of
+        a struct of the specified fields.
+
+        :param colName: name of column
+        :param fields: list of elements to compose as a struct valued column (each being a string or tuple), or a dict
+                          outlining the structure of the struct column
+        :param asJson: If False, generate a struct valued column. If True, generate a JSON string column
+        :param kwargs: keyword arguments to pass to the underlying column generators as per `withColumn`
+        :return: A modified in-place instance of data generator allowing for chaining of calls
+                  following the Builder pattern
+
+        .. note::
+            Additional options for the field specification may be specified as keyword arguments.
+
+            The fields specification specified by the `fields` argument may be :
+
+            - A list of field references (`strings`) which will be used as both the field name and the SQL expression
+            - A list of tuples of the form **(field_name, field_expression)** where `field_name` is the name of the
+              field. In that case, the `field_expression` string should be a SQL expression to generate the field value
+            - A Python dict outlining the structure of the struct column. The keys of the dict are the field names
+
+            When using the `dict` form of the field specifications, a field whose value is a list will be treated
+            as creating a SQL array literal.
+
+        """
+        assert fields is not None and isinstance(fields, (list, dict)), \
+            "Fields argument must be a list of field specifications or dict outlining the target structure "
+        assert type(colName) is str and len(colName) > 0, "Must specify a column name"
+
+        if isinstance(fields, list):
+            assert len(fields) > 0, \
+                "Must specify at least one field for struct column"
+            struct_expr = self._mkSqlStructFromList(fields)
+        elif isinstance(fields, dict):
+            struct_expr = self._mkStructFromDict(fields)
+        else:
+            raise ValueError(f"Invalid field specification for struct column `{colName}`")
+
+        if asJson:
+            output_expr = f"to_json({struct_expr})"
+            newDf = self.withColumn(colName, StringType(), expr=output_expr,  **kwargs)
+        else:
+            newDf = self.withColumn(colName, INFER_DATATYPE, expr=struct_expr, **kwargs)
+
+        return newDf
+
     def _generateColumnDefinition(self, colName, colType=None, baseColumn=None,
                                   implicit=False, omit=False, nullable=True, **kwargs):
         """ generate field definition and column spec
 
         .. note:: Any time that a new column definition is added,
                   we'll mark that the build plan needs to be regenerated.
            For our purposes, the build plan determines the order of column generation etc.
 
-        :returns: modified in-place instance of test data generator allowing for chaining of calls
-                  following Builder pattern
+        :returns: Newly added column_spec
         """
         if colType is None:
             colType = self.getColumnType(baseColumn)
 
+            if colType == INFER_DATATYPE:
+                raise ValueError("When base column(s) have inferred datatype, you must specify the column type")
+
         new_props = {}
         new_props.update(kwargs)
 
         # if the column  has the option `random` set to true
         # then use the instance level random seed
         # otherwise use the default random seed for the class
         if OPTION_RANDOM_SEED in new_props:
@@ -868,15 +1007,15 @@
             self._allColumnSpecs.remove(x)
 
         self._allColumnSpecs.append(column_spec)
 
         # mark that the build plan needs to be regenerated
         self._markForPlanRegen()
 
-        return self
+        return column_spec
 
     def _getBaseDataFrame(self, startId=0, streaming=False, options=None):
         """ generate the base data frame and seed column (which defaults to `id`) , partitioning the data if necessary
 
         This is used when generating the test data.
 
         A base data frame is created and then each of the additional columns are generated, according to
@@ -949,15 +1088,15 @@
         self.logger.info("dependency list: %s", str(dependency_ordering))
 
         self._buildOrder = list(
             topologicalSort(dependency_ordering, flatten=False, initial_columns=[self._seedColumnName]))
 
         self.logger.info("columnBuildOrder: %s", str(self._buildOrder))
 
-        self._buildOrder = self._adjustBuildOrderForSqlDependencies(self._buildOrder,  self._columnSpecsByName)
+        self._buildOrder = self._adjustBuildOrderForSqlDependencies(self._buildOrder, self._columnSpecsByName)
 
         return self._buildOrder
 
     def _adjustBuildOrderForSqlDependencies(self, buildOrder, columnSpecsByName):
         """ Adjust column build order according to the following heuristics
 
         1: if the column being built in a specific build order phase has a SQL expression and it references
@@ -1124,28 +1263,30 @@
             self.executionHistory.append("registering temp view")
             self.logger.info("Registering temporary view [%s]", self.name)
             df1.createOrReplaceTempView(self.name)
             self.logger.info("Registered!")
 
         return df1
 
+    # noinspection PyProtectedMember
     def _buildColumnExpressionsWithSelects(self, df1):
         """
         Build column generation expressions with selects
         :param df1: dataframe for base data generator
         :return: new dataframe
 
         The data generator build plan is separated into `rounds` of expressions. Each round consists of
         expressions that are generated using a single `select` operation
         """
         self.executionHistory.append("Generating data with selects")
         # generation with selects may be more efficient as less intermediate data frames
         # are generated resulting in shorter lineage
         for colNames in self.build_order:
             build_round = ["*"]
+            column_specs_applied = []
             inx_col = 0
             self.executionHistory.append(f"building stage for columns: {colNames}")
             for colName in colNames:
                 col1 = self._columnSpecsByName[colName]
                 column_generators = col1.makeGenerationExpressions()
                 self.executionHistory.extend(col1.executionHistory)
                 if type(column_generators) is list and len(column_generators) == 1:
@@ -1153,17 +1294,22 @@
                 elif type(column_generators) is list and len(column_generators) > 1:
                     i = 0
                     for cg in column_generators:
                         build_round.append(cg.alias(f'{colName}_{i}'))
                         i += 1
                 else:
                     build_round.append(column_generators.alias(colName))
+                column_specs_applied.append(col1)
                 inx_col = inx_col + 1
 
             df1 = df1.select(*build_round)
+
+            # apply any post select processing
+            for cs in column_specs_applied:
+                cs._onSelect(df1)
         return df1
 
     def _sqlTypeFromSparkType(self, dt):
         """Get sql type for spark type
            :param dt: instance of Spark SQL type such as IntegerType()
         """
         return dt.simpleString()
@@ -1183,21 +1329,22 @@
             if isUpdate:
                 results.append(f"{substitution_col}={new_val}")
             else:
                 results.append(f"{new_val}")
 
         return ", ".join(results)
 
-    def scriptTable(self, name=None, location=None, tableFormat="delta"):
+    def scriptTable(self, name=None, location=None, tableFormat="delta", asHtml=False):
         """ generate create table script suitable for format of test data set
 
         :param name: name of table to use in generated script
         :param location: path to location of data. If specified (default is None), will generate
                          an external table definition.
         :param tableFormat: table format for table
+        :param asHtml: if true, generate output suitable for use with `displayHTML` method in notebook environment
         :returns: SQL string for scripted table
         """
         assert name is not None, "`name` must be specified"
 
         self.computeBuildPlan()
 
         output_columns = self.getOutputColumnNamesAndTypes()
@@ -1215,22 +1362,29 @@
         results.append(",\n".join(col_expressions))
         results.append(")")
         results.append(f"using {tableFormat}")
 
         if location is not None:
             results.append(f"location '{location}'")
 
-        return "\n".join(results)
+        results = "\n".join(results)
+
+        if asHtml:
+            results = HtmlUtils.formatCodeAsHtml(results)
+
+        return results
 
     def scriptMerge(self, tgtName=None, srcName=None, updateExpr=None, delExpr=None, joinExpr=None, timeExpr=None,
                     insertExpr=None,
                     useExplicitNames=True,
                     updateColumns=None, updateColumnExprs=None,
                     insertColumns=None, insertColumnExprs=None,
-                    srcAlias="src", tgtAlias="tgt"):
+                    srcAlias="src", tgtAlias="tgt",
+                    asHtml=False
+                    ):
         """ generate merge table script suitable for format of test data set
 
         :param tgtName: name of target table to use in generated script
         :param tgtAlias: alias for target table - defaults to `tgt`
         :param srcName: name of source table to use in generated script
         :param srcAlias: alias for source table - defaults to `src`
         :param updateExpr: optional string representing updated condition. If not present, then
@@ -1249,14 +1403,15 @@
             target table. This should have the form [ ("insert_column_name", "insert column expr"), ...]
         :param updateColumns: List of strings designating columns to update.
                                If not supplied, uses all columns defined in spec
         :param updateColumnExprs: Optional list of strings designating designating column expressions for update.
             By default, will use src column as update value for
             target table. This should have the form [ ("update_column_name", "update column expr"), ...]
         :param useExplicitNames: If True, generate explicit column names in insert and update statements
+        :param asHtml: if true, generate output suitable for use with `displayHTML` method in notebook environment
         :returns: SQL string for scripted merge statement
         """
         assert tgtName is not None, "you must specify a target table"
         assert srcName is not None, "you must specify a source table"
         assert joinExpr is not None, "you must specify a join expression"
 
         self.computeBuildPlan()
@@ -1323,8 +1478,13 @@
                           self._mkInsertOrUpdateStatement(columns=insertColumns, srcAlias=srcAlias,
                                                           substitutions=insertColumnExprs, isUpdate=False)
                           + ")"
                           )
 
         results.append(ins_clause)
 
-        return "\n".join(results)
+        result = "\n".join(results)
+
+        if asHtml:
+            result = HtmlUtils.formatCodeAsHtml(results)
+
+        return result
```

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/datagen_constants.py` & `dbldatagen-0.3.5/dbldatagen/datagen_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,7 +37,9 @@
 MIN_PYTHON_VERSION = (3, 8)
 MIN_SPARK_VERSION = (3, 1, 2)
 
 # options for randon data generation
 OPTION_RANDOM = "random"
 OPTION_RANDOM_SEED_METHOD = "randomSeedMethod"
 OPTION_RANDOM_SEED = "randomSeed"
+
+INFER_DATATYPE = "__infer__"
```

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/datarange.py` & `dbldatagen-0.3.5/dbldatagen/datarange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/daterange.py` & `dbldatagen-0.3.5/dbldatagen/daterange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/distributions/__init__.py` & `dbldatagen-0.3.5/dbldatagen/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/distributions/beta.py` & `dbldatagen-0.3.5/dbldatagen/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/distributions/data_distribution.py` & `dbldatagen-0.3.5/dbldatagen/distributions/data_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/distributions/exponential_distribution.py` & `dbldatagen-0.3.5/dbldatagen/distributions/exponential_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/distributions/gamma.py` & `dbldatagen-0.3.5/dbldatagen/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/distributions/normal_distribution.py` & `dbldatagen-0.3.5/dbldatagen/distributions/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/function_builder.py` & `dbldatagen-0.3.5/dbldatagen/function_builder.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/nrange.py` & `dbldatagen-0.3.5/dbldatagen/nrange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/schema_parser.py` & `dbldatagen-0.3.5/dbldatagen/schema_parser.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/spark_singleton.py` & `dbldatagen-0.3.5/dbldatagen/spark_singleton.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/text_generator_plugins.py` & `dbldatagen-0.3.5/dbldatagen/text_generator_plugins.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/text_generators.py` & `dbldatagen-0.3.5/dbldatagen/text_generators.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post2/dbldatagen/utils.py` & `dbldatagen-0.3.5/dbldatagen/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 """
 This file defines the `DataGenError` classes and utility functions
 
 These are meant for internal use only
 """
 
 import functools
+import json
+import re
+import time
 import warnings
 from datetime import timedelta
-import re
+
+import jmespath
 
 
 def deprecated(message=""):
-    """ Define a deprecated decorator without dependencies on 3rd party libraries
+    """
+    Define a deprecated decorator without dependencies on 3rd party libraries
 
     Note there is a 3rd party library called `deprecated` that provides this feature but goal is to only have
     dependencies on packages already used in the Databricks runtime
     """
 
     # create closure around function that follows use of the decorator
 
@@ -268,30 +273,31 @@
         else:
             revised_lines.append(line)
 
     return '\n'.join(revised_lines)
 
 
 def split_list_matching_condition(lst, cond):
-    """ Split a list on elements that match a condition
+    """
+    Split a list on elements that match a condition
 
     This will find all matches of a specific condition in the list and split the list into sub lists around the
     element that matches this condition.
 
     It will handle multiple matches performing splits on each match.
 
     For example, the following code will produce the results below:
 
     x = ['id', 'city_name', 'id', 'city_id', 'city_pop', 'id', 'city_id', 'city_pop','city_id', 'city_pop','id']
     splitListOnCondition(x, lambda el: el == 'id')
 
 
-    result:
+    Result:
     `[['id'], ['city_name'], ['id'], ['city_id', 'city_pop'],
-     ['id'], ['city_id', 'city_pop', 'city_id', 'city_pop'], ['id']]`
+      ['id'], ['city_id', 'city_pop', 'city_id', 'city_pop'], ['id']]`
 
     :arg lst: list of items to perform condition matches against
     :arg cond: lambda function or function taking single argument and returning True or False
     :returns: list of sublists
     """
     retval = []
 
@@ -317,7 +323,40 @@
             retval.append(lst[ix:ix + 1])
             retval.extend(split_list_matching_condition(lst[ix + 1:], cond))
         else:
             retval = [lst]
 
     # filter out empty lists
     return [el for el in retval if el != []]
+
+
+def json_value_from_path(searchPath, jsonData, defaultValue):
+    """ Get JSON value from JSON data referenced by searchPath
+
+    searchPath should be a JSON path as supported by the `jmespath` package
+    (see https://jmespath.org/)
+
+    :param searchPath: A `jmespath` compatible JSON search path
+    :param jsonData: The json data to search (string representation of the JSON data)
+    :param defaultValue: The default value to be returned if the value was not found
+    :return: Returns the json value if present, otherwise returns the default value
+    """
+    assert searchPath is not None and len(searchPath) > 0, "search path cannot be empty"
+    assert jsonData is not None and len(jsonData) > 0, "JSON data cannot be empty"
+
+    jsonDict = json.loads(jsonData)
+
+    jsonValue = jmespath.search(searchPath, jsonDict)
+
+    if jsonValue is not None:
+        return jsonValue
+
+    return defaultValue
+
+
+def system_time_millis():
+    """ return system time as milliseconds since start of epoch
+
+    :return: system time millis as long
+    """
+    curr_time = round(time.time() / 1000)
+    return curr_time
```

### Comparing `dbldatagen-0.3.4.post2/dbldatagen.egg-info/PKG-INFO` & `dbldatagen-0.3.5/dbldatagen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.4.post2
+Version: 0.3.5
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post2/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.5/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4.post2/dbldatagen.egg-info/SOURCES.txt` & `dbldatagen-0.3.5/dbldatagen.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 dbldatagen/column_spec_options.py
 dbldatagen/data_analyzer.py
 dbldatagen/data_generator.py
 dbldatagen/datagen_constants.py
 dbldatagen/datarange.py
 dbldatagen/daterange.py
 dbldatagen/function_builder.py
+dbldatagen/html_utils.py
 dbldatagen/nrange.py
 dbldatagen/schema_parser.py
 dbldatagen/spark_singleton.py
 dbldatagen/text_generator_plugins.py
 dbldatagen/text_generators.py
 dbldatagen/utils.py
 dbldatagen.egg-info/PKG-INFO
```

### Comparing `dbldatagen-0.3.4.post2/setup.py` & `dbldatagen-0.3.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     The Databricks Labs Data Generator can generate realistic synthetic data sets at scale for testing, 
     benchmarking, environment validation and other purposes.
     """
 
 setuptools.setup(
     name="dbldatagen",
-    version="0.3.4post2",
+    version="0.3.5",
     author="Ronan Stokes, Databricks",
     description="Databricks Labs -  PySpark Synthetic Data Generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/databrickslabs/data-generator",
     project_urls={
         "Databricks Labs": "https://www.databricks.com/learn/labs",
```

