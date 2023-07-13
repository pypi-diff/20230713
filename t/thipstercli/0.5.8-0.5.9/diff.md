# Comparing `tmp/thipstercli-0.5.8.tar.gz` & `tmp/thipstercli-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.5.8.tar", last modified: Tue Jun 27 13:16:59 2023, max compression
+gzip compressed data, was "thipstercli-0.5.9.tar", last modified: Wed Jul 12 09:15:24 2023, max compression
```

## Comparing `thipstercli-0.5.8.tar` & `thipstercli-0.5.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:16:59.283970 thipstercli-0.5.8/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-27 13:16:55.000000 thipstercli-0.5.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-27 13:16:59.283970 thipstercli-0.5.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-27 13:16:55.000000 thipstercli-0.5.8/README.md
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-27 13:16:55.000000 thipstercli-0.5.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 13:16:59.283970 thipstercli-0.5.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-27 13:16:55.000000 thipstercli-0.5.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:16:59.279970 thipstercli-0.5.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 13:16:55.000000 thipstercli-0.5.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-06-27 13:16:55.000000 thipstercli-0.5.8/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-27 13:16:55.000000 thipstercli-0.5.8/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-27 13:16:55.000000 thipstercli-0.5.8/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-27 13:16:55.000000 thipstercli-0.5.8/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-06-27 13:16:55.000000 thipstercli-0.5.8/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-27 13:16:55.000000 thipstercli-0.5.8/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:16:59.279970 thipstercli-0.5.8/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:16:59.283970 thipstercli-0.5.8/thipstercli/commands/
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     8194 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/commands/info.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/commands/providers.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/commands/repository.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-27 13:16:55.000000 thipstercli-0.5.8/thipstercli/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:16:59.279970 thipstercli-0.5.8/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-27 13:16:59.000000 thipstercli-0.5.8/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-27 13:16:59.000000 thipstercli-0.5.8/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 13:16:59.000000 thipstercli-0.5.8/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-27 13:16:59.000000 thipstercli-0.5.8/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      284 2023-06-27 13:16:59.000000 thipstercli-0.5.8/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-27 13:16:59.000000 thipstercli-0.5.8/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:24.001062 thipstercli-0.5.9/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-07-12 09:15:19.000000 thipstercli-0.5.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-07-12 09:15:24.001062 thipstercli-0.5.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-07-12 09:15:19.000000 thipstercli-0.5.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-07-12 09:15:19.000000 thipstercli-0.5.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 09:15:24.001062 thipstercli-0.5.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-07-12 09:15:20.000000 thipstercli-0.5.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:23.997063 thipstercli-0.5.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 09:15:19.000000 thipstercli-0.5.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-07-12 09:15:19.000000 thipstercli-0.5.9/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-07-12 09:15:19.000000 thipstercli-0.5.9/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-12 09:15:19.000000 thipstercli-0.5.9/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-07-12 09:15:19.000000 thipstercli-0.5.9/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-07-12 09:15:19.000000 thipstercli-0.5.9/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-12 09:15:19.000000 thipstercli-0.5.9/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:23.997063 thipstercli-0.5.9/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:24.001062 thipstercli-0.5.9/thipstercli/commands/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8194 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/commands/info.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/commands/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/commands/repository.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-07-12 09:15:19.000000 thipstercli-0.5.9/thipstercli/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:23.997063 thipstercli-0.5.9/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-07-12 09:15:23.000000 thipstercli-0.5.9/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-12 09:15:23.000000 thipstercli-0.5.9/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:15:23.000000 thipstercli-0.5.9/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-12 09:15:23.000000 thipstercli-0.5.9/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-07-12 09:15:23.000000 thipstercli-0.5.9/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-12 09:15:23.000000 thipstercli-0.5.9/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.5.8/LICENSE` & `thipstercli-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/PKG-INFO` & `thipstercli-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.5.8
+Version: 0.5.9
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: doc
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # THipster CLI
 
 CLI tool to interact and use [THipster](https://github.com/THipster/THipster), build with [Typer](https://typer.tiangolo.com/).
 
 THipster is a tool dedicated to simplifying the ordeal associated with writing Terraform files.
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.5.8 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.5.9 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
-Provides-Extra: doc Provides-Extra: test Provides-Extra: dev License-File:
+Provides-Extra: doc Provides-Extra: dev Provides-Extra: test License-File:
 LICENSE # THipster CLI CLI tool to interact and use [THipster](https://
 github.com/THipster/THipster), build with [Typer](https://typer.tiangolo.com/).
 THipster is a tool dedicated to simplifying the ordeal associated with writing
 Terraform files. It allows users to write infrastructure as code in a
 simplified format, using either YAML (with JINJA) or the dedicated Thipster
 DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
 create Terraform files and apply them to the chosen provider.
```

### Comparing `thipstercli-0.5.8/README.md` & `thipstercli-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/pyproject.toml` & `thipstercli-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/setup.py` & `thipstercli-0.5.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.5.8'
+__version__ = '0.5.9'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.5.8/tests/conftest.py` & `thipstercli-0.5.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/tests/test_cli.py` & `thipstercli-0.5.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/tests/test_config.py` & `thipstercli-0.5.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/tests/test_info.py` & `thipstercli-0.5.9/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/tests/test_providers.py` & `thipstercli-0.5.9/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/tests/test_repository.py` & `thipstercli-0.5.9/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli/cli.py` & `thipstercli-0.5.9/thipstercli/cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli/commands/config.py` & `thipstercli-0.5.9/thipstercli/commands/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli/commands/info.py` & `thipstercli-0.5.9/thipstercli/commands/info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli/commands/providers.py` & `thipstercli-0.5.9/thipstercli/commands/providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli/commands/repository.py` & `thipstercli-0.5.9/thipstercli/commands/repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli/config.py` & `thipstercli-0.5.9/thipstercli/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli/display.py` & `thipstercli-0.5.9/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli/helpers.py` & `thipstercli-0.5.9/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.8/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.5.9/thipstercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.5.8
+Version: 0.5.9
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: doc
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # THipster CLI
 
 CLI tool to interact and use [THipster](https://github.com/THipster/THipster), build with [Typer](https://typer.tiangolo.com/).
 
 THipster is a tool dedicated to simplifying the ordeal associated with writing Terraform files.
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.5.8 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.5.9 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
-Provides-Extra: doc Provides-Extra: test Provides-Extra: dev License-File:
+Provides-Extra: doc Provides-Extra: dev Provides-Extra: test License-File:
 LICENSE # THipster CLI CLI tool to interact and use [THipster](https://
 github.com/THipster/THipster), build with [Typer](https://typer.tiangolo.com/).
 THipster is a tool dedicated to simplifying the ordeal associated with writing
 Terraform files. It allows users to write infrastructure as code in a
 simplified format, using either YAML (with JINJA) or the dedicated Thipster
 DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
 create Terraform files and apply them to the chosen provider.
```

### Comparing `thipstercli-0.5.8/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.5.9/thipstercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

