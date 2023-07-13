# Comparing `tmp/jinja2_humanize_extension-0.2.2.tar.gz` & `tmp/jinja2_humanize_extension-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_humanize_extension-0.2.2.tar", last modified: Tue Oct 11 13:40:19 2022, max compression
+gzip compressed data, was "jinja2_humanize_extension-0.3.0.tar", last modified: Thu Jul 13 14:11:45 2023, max compression
```

## Comparing `jinja2_humanize_extension-0.2.2.tar` & `jinja2_humanize_extension-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:40:19.863038 jinja2_humanize_extension-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:40:19.863038 jinja2_humanize_extension-0.2.2/.metwork-framework/
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-10-11 13:40:10.000000 jinja2_humanize_extension-0.2.2/.metwork-framework/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-10-11 13:40:10.000000 jinja2_humanize_extension-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-11 13:40:10.000000 jinja2_humanize_extension-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-10-11 13:40:19.863038 jinja2_humanize_extension-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2466 2022-10-11 13:40:10.000000 jinja2_humanize_extension-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:40:19.863038 jinja2_humanize_extension-0.2.2/jinja2_humanize_extension/
--rw-r--r--   0 runner    (1001) docker     (121)     2533 2022-10-11 13:40:10.000000 jinja2_humanize_extension-0.2.2/jinja2_humanize_extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:40:19.863038 jinja2_humanize_extension-0.2.2/jinja2_humanize_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-10-11 13:40:19.000000 jinja2_humanize_extension-0.2.2/jinja2_humanize_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-10-11 13:40:19.000000 jinja2_humanize_extension-0.2.2/jinja2_humanize_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 13:40:19.000000 jinja2_humanize_extension-0.2.2/jinja2_humanize_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-11 13:40:19.000000 jinja2_humanize_extension-0.2.2/jinja2_humanize_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-11 13:40:19.000000 jinja2_humanize_extension-0.2.2/jinja2_humanize_extension.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-11 13:40:10.000000 jinja2_humanize_extension-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-11 13:40:19.863038 jinja2_humanize_extension-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-10-11 13:40:18.000000 jinja2_humanize_extension-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:11:45.450951 jinja2_humanize_extension-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-13 14:11:37.000000 jinja2_humanize_extension-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 14:11:37.000000 jinja2_humanize_extension-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-13 14:11:45.450951 jinja2_humanize_extension-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-13 14:11:37.000000 jinja2_humanize_extension-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:11:45.446951 jinja2_humanize_extension-0.3.0/jinja2_humanize_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-13 14:11:37.000000 jinja2_humanize_extension-0.3.0/jinja2_humanize_extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:11:45.450951 jinja2_humanize_extension-0.3.0/jinja2_humanize_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-13 14:11:45.000000 jinja2_humanize_extension-0.3.0/jinja2_humanize_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-13 14:11:45.000000 jinja2_humanize_extension-0.3.0/jinja2_humanize_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:11:45.000000 jinja2_humanize_extension-0.3.0/jinja2_humanize_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 14:11:45.000000 jinja2_humanize_extension-0.3.0/jinja2_humanize_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 14:11:45.000000 jinja2_humanize_extension-0.3.0/jinja2_humanize_extension.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 14:11:37.000000 jinja2_humanize_extension-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:11:45.450951 jinja2_humanize_extension-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-13 14:11:44.000000 jinja2_humanize_extension-0.3.0/setup.py
```

### Comparing `jinja2_humanize_extension-0.2.2/LICENSE` & `jinja2_humanize_extension-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_humanize_extension-0.2.2/PKG-INFO` & `jinja2_humanize_extension-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-Metadata-Version: 2.1
-Name: jinja2_humanize_extension
-Version: 0.2.2
-Summary: a jinja2 extension to use humanize library inside jinja2 templates
-Home-page: https://github.com/metwork-framework/jinja2_humanize_extension
-Author: Fabien MARTY
-Author-email: fabien.marty@gmail.com
-License: BSD
-Keywords: jinja2 extension
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# jinja2_humanize_extension
+
+[//]: # (automatically generated from https://github.com/metwork-framework/github_organization_management/blob/master/common_files/README.md)
+
+**Status (master branch)**
+
+
+
+[![GitHub CI](https://github.com/metwork-framework/jinja2_humanize_extension/workflows/CI/badge.svg?branch=master)](https://github.com/metwork-framework/jinja2_humanize_extension/actions?query=workflow%3ACI+branch%3Amaster)
+[![Maintenance](https://raw.githubusercontent.com/metwork-framework/resources/master/badges/maintained.svg)](https://github.com/metwork-framework/resources/blob/master/badges/maintained.svg)
+
+
+
 
 ## What is it ?
 
 This is a [jinja2](http://jinja.pocoo.org/) extension to use [humanize](https://python-humanize.readthedocs.io/) library inside jinja2 templates.
 
 ## Syntax
 
 The generic syntax is `{{ 'VALUE'|humanize_{humanize_fn}([humanize_fn_args]) }}`.
 
 Following [humanize](https://python-humanize.readthedocs.io/) functions are currently mapped:
 
 - `naturalsize`
-- `abs_timedelta`
-- `date_and_delta`
+- `_abs_timedelta` (deprecated with humanize >= 4.0, we keep it for compatibility)
+- `_date_and_delta` (deprecated with humanize >= 4.0, we keep it for compatibility)
 - `naturaldate`
 - `naturalday`
 - `naturaldelta`
 - `naturaltime`
 - `precisedelta`
 - `humanize_intword`
 
@@ -65,7 +62,30 @@
 env = Environment(extensions=["jinja2_humanize_extension.HumanizeExtension"])
 
 template = env.from_string("The file size is : {{ 30000000|humanize_naturalsize() }}")
 result = template.render()
 
 # [...]
 ```
+
+
+
+
+
+
+## Contributing guide
+
+See [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
+
+
+## Code of Conduct
+
+See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) file.
+
+
+
+## Sponsors
+
+*(If you are officially paid to work on MetWork Framework, please contact us to add your company logo here!)*
+
+[![logo](https://raw.githubusercontent.com/metwork-framework/resources/master/sponsors/meteofrance-small.jpeg)](http://www.meteofrance.com)
```

### Comparing `jinja2_humanize_extension-0.2.2/README.md` & `jinja2_humanize_extension-0.3.0/jinja2_humanize_extension.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: jinja2-humanize-extension
+Version: 0.3.0
+Summary: a jinja2 extension to use humanize library inside jinja2 templates
+Home-page: https://github.com/metwork-framework/jinja2_humanize_extension
+Author: Fabien MARTY
+Author-email: fabien.marty@gmail.com
+License: BSD
+Keywords: jinja2 extension
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # jinja2_humanize_extension
 
 [//]: # (automatically generated from https://github.com/metwork-framework/github_organization_management/blob/master/common_files/README.md)
 
 **Status (master branch)**
 
 
@@ -19,16 +36,16 @@
 ## Syntax
 
 The generic syntax is `{{ 'VALUE'|humanize_{humanize_fn}([humanize_fn_args]) }}`.
 
 Following [humanize](https://python-humanize.readthedocs.io/) functions are currently mapped:
 
 - `naturalsize`
-- `abs_timedelta`
-- `date_and_delta`
+- `_abs_timedelta` (deprecated with humanize >= 4.0, we keep it for compatibility)
+- `_date_and_delta` (deprecated with humanize >= 4.0, we keep it for compatibility)
 - `naturaldate`
 - `naturalday`
 - `naturaldelta`
 - `naturaltime`
 - `precisedelta`
 - `humanize_intword`
```

### Comparing `jinja2_humanize_extension-0.2.2/jinja2_humanize_extension/__init__.py` & `jinja2_humanize_extension-0.3.0/jinja2_humanize_extension/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from jinja2.ext import Extension
 from humanize import naturalsize
 
 from humanize.time import (
-    abs_timedelta,
-    date_and_delta,
+    _abs_timedelta,
+    _date_and_delta,
     naturaldate,
     naturalday,
     naturaldelta,
     naturaltime,
     precisedelta,
 )
 from humanize.number import intword
@@ -17,47 +17,45 @@
     from jinja2 import pass_eval_context as eval_context
 except ImportError:
     from jinja2 import evalcontextfilter as eval_context
 
 
 @eval_context
 def humanize_abs_timedelta(eval_ctx, delta):
-    return abs_timedelta(delta)
+    return _abs_timedelta(delta)
 
 
 @eval_context
 def humanize_intword(eval_ctx, value, format="%.1f"):
     return intword(value, format=format)
 
 
 @eval_context
 def humanize_naturalsize(eval_ctx, value, binary=False, gnu=False, format="%.1f"):
     return naturalsize(value, binary=binary, gnu=gnu, format=format)
 
 
 @eval_context
 def humanize_date_and_delta(eval_ctx, value, *args):
-    return date_and_delta(value, *args)
+    return _date_and_delta(value, *args)
 
 
 @eval_context
 def humanize_naturaldate(eval_ctx, value):
     return naturaldate(value)
 
 
 @eval_context
 def humanize_naturalday(eval_ctx, value):
     return naturalday(value)
 
 
 @eval_context
-def humanize_naturaldelta(
-    eval_ctx, value, months=True, minimum_unit="seconds", when=None
-):
-    return naturaldelta(value, months=months, minimum_unit=minimum_unit, when=when)
+def humanize_naturaldelta(eval_ctx, value, months=True, minimum_unit="seconds"):
+    return naturaldelta(value, months=months, minimum_unit=minimum_unit)
 
 
 @eval_context
 def humanize_naturaltime(
     eval_ctx, value, future=False, months=True, minimum_unit="seconds", when=None
 ):
     return naturaltime(
```

### Comparing `jinja2_humanize_extension-0.2.2/jinja2_humanize_extension.egg-info/PKG-INFO` & `jinja2_humanize_extension-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 Metadata-Version: 2.1
-Name: jinja2-humanize-extension
-Version: 0.2.2
+Name: jinja2_humanize_extension
+Version: 0.3.0
 Summary: a jinja2 extension to use humanize library inside jinja2 templates
 Home-page: https://github.com/metwork-framework/jinja2_humanize_extension
 Author: Fabien MARTY
 Author-email: fabien.marty@gmail.com
 License: BSD
 Keywords: jinja2 extension
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# jinja2_humanize_extension
+
+[//]: # (automatically generated from https://github.com/metwork-framework/github_organization_management/blob/master/common_files/README.md)
+
+**Status (master branch)**
+
+
+
+[![GitHub CI](https://github.com/metwork-framework/jinja2_humanize_extension/workflows/CI/badge.svg?branch=master)](https://github.com/metwork-framework/jinja2_humanize_extension/actions?query=workflow%3ACI+branch%3Amaster)
+[![Maintenance](https://raw.githubusercontent.com/metwork-framework/resources/master/badges/maintained.svg)](https://github.com/metwork-framework/resources/blob/master/badges/maintained.svg)
+
+
+
+
 ## What is it ?
 
 This is a [jinja2](http://jinja.pocoo.org/) extension to use [humanize](https://python-humanize.readthedocs.io/) library inside jinja2 templates.
 
 ## Syntax
 
 The generic syntax is `{{ 'VALUE'|humanize_{humanize_fn}([humanize_fn_args]) }}`.
 
 Following [humanize](https://python-humanize.readthedocs.io/) functions are currently mapped:
 
 - `naturalsize`
-- `abs_timedelta`
-- `date_and_delta`
+- `_abs_timedelta` (deprecated with humanize >= 4.0, we keep it for compatibility)
+- `_date_and_delta` (deprecated with humanize >= 4.0, we keep it for compatibility)
 - `naturaldate`
 - `naturalday`
 - `naturaldelta`
 - `naturaltime`
 - `precisedelta`
 - `humanize_intword`
 
@@ -65,7 +79,30 @@
 env = Environment(extensions=["jinja2_humanize_extension.HumanizeExtension"])
 
 template = env.from_string("The file size is : {{ 30000000|humanize_naturalsize() }}")
 result = template.render()
 
 # [...]
 ```
+
+
+
+
+
+
+## Contributing guide
+
+See [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
+
+
+## Code of Conduct
+
+See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) file.
+
+
+
+## Sponsors
+
+*(If you are officially paid to work on MetWork Framework, please contact us to add your company logo here!)*
+
+[![logo](https://raw.githubusercontent.com/metwork-framework/resources/master/sponsors/meteofrance-small.jpeg)](http://www.meteofrance.com)
```

### Comparing `jinja2_humanize_extension-0.2.2/setup.py` & `jinja2_humanize_extension-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as reqs:
     install_requires = [
         line for line in reqs.read().split('\n')
         if (line and not line.startswith('--')) and (";" not in line)]
 
-with open(".metwork-framework/README.md") as f:
+with open("README.md") as f:
     long_description = f.read().replace("{% raw %}", "").replace("{% endraw %}", "")
 
 setup(
     author="Fabien MARTY",
     author_email="fabien.marty@gmail.com",
     name="jinja2_humanize_extension",
-    version="0.2.2",
+    version="0.3.0",
     license="BSD",
     packages=find_packages(),
     install_requires=install_requires,
     python_requires='>=3.0',
     description="a jinja2 extension to use humanize library inside jinja2 templates",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

