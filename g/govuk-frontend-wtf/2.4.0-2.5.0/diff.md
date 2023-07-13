# Comparing `tmp/govuk-frontend-wtf-2.4.0.tar.gz` & `tmp/govuk-frontend-wtf-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk-frontend-wtf-2.4.0.tar", last modified: Tue Apr 25 18:57:58 2023, max compression
+gzip compressed data, was "govuk-frontend-wtf-2.5.0.tar", last modified: Thu Jul 13 14:28:24 2023, max compression
```

## Comparing `govuk-frontend-wtf-2.4.0.tar` & `govuk-frontend-wtf-2.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.580022 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/gov_form_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/button.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/charactercount.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/checkboxes.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/date.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/file-upload.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/input.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/radios.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/textarea.html
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/wtforms_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.584022 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/tests/test_wtf_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:24.054489 govuk-frontend-wtf-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-13 14:28:24.054489 govuk-frontend-wtf-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:24.050489 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/gov_form_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:24.054489 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/charactercount.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/checkboxes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/date.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/file-upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/radios.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/templates/textarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/wtforms_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:24.050489 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-13 14:28:24.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 14:28:24.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:28:24.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 14:28:24.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 14:28:24.000000 govuk-frontend-wtf-2.5.0/govuk_frontend_wtf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 14:28:24.054489 govuk-frontend-wtf-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:24.054489 govuk-frontend-wtf-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-13 14:28:09.000000 govuk-frontend-wtf-2.5.0/tests/test_wtf_widgets.py
```

### Comparing `govuk-frontend-wtf-2.4.0/LICENSE` & `govuk-frontend-wtf-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-2.4.0/PKG-INFO` & `govuk-frontend-wtf-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-wtf
-Version: 2.4.0
+Version: 2.5.0
 Summary: GOV.UK Frontend WTForms Widgets
 Home-page: https://github.com/LandRegistry/govuk-frontend-wtf
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.7.0](https://img.shields.io/badge/govuk--frontend%20version-4.7.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
```

### Comparing `govuk-frontend-wtf-2.4.0/README.md` & `govuk-frontend-wtf-2.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.7.0](https://img.shields.io/badge/govuk--frontend%20version-4.7.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
```

### Comparing `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/gov_form_base.py` & `govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/gov_form_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
             "name": field.name,
             "items": kwargs["items"],
             "hint": {"text": field.description},
         }
 
         # Merge in any extra params passed in from the template layer
         if "params" in kwargs:
-
             # Merge items individually as otherwise the merge will append new ones
             if "items" in kwargs["params"]:
                 for index, item in enumerate(kwargs["params"]["items"]):
                     item = self.merge_params(params["items"][index], item)
 
                 del kwargs["params"]["items"]
```

### Comparing `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/main.py` & `govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/main.py`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/wtforms_widgets.py` & `govuk-frontend-wtf-2.5.0/govuk_frontend_wtf/wtforms_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,13 +319,12 @@
             item = {"text": label, "value": val, "selected": selected}
 
             kwargs["items"].append(item)
 
         return super().__call__(field, **kwargs)
 
     def map_gov_params(self, field, **kwargs):
-
         params = super().map_gov_params(field, **kwargs)
 
         params["items"] = kwargs["items"]
 
         return params
```

### Comparing `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/PKG-INFO` & `govuk-frontend-wtf-2.5.0/govuk_frontend_wtf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-wtf
-Version: 2.4.0
+Version: 2.5.0
 Summary: GOV.UK Frontend WTForms Widgets
 Home-page: https://github.com/LandRegistry/govuk-frontend-wtf
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.7.0](https://img.shields.io/badge/govuk--frontend%20version-4.7.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
```

### Comparing `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/SOURCES.txt` & `govuk-frontend-wtf-2.5.0/govuk_frontend_wtf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-2.4.0/setup.py` & `govuk-frontend-wtf-2.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,39 +9,38 @@
 templates = []
 directories = glob.glob("govuk_frontend_wtf/templates/*.html")
 for directory in directories:
     templates.append(os.path.relpath(os.path.dirname(directory), "govuk_frontend_wtf") + "/*.html")
 
 setuptools.setup(
     name="govuk-frontend-wtf",
-    version="2.4.0",
+    version="2.5.0",
     author="Matt Shaw",
     author_email="matthew.shaw@landregistry.gov.uk",
     description="GOV.UK Frontend WTForms Widgets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LandRegistry/govuk-frontend-wtf",
     packages=setuptools.find_packages(exclude=["tests"]),
     package_data={"govuk_frontend_wtf": templates},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Environment :: Web Environment",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Code Generators",
         "Topic :: Software Development :: User Interfaces",
         "Topic :: Text Processing :: Markup :: HTML",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "deepmerge",
         "flask",
         "flask-wtf",
         "govuk-frontend-jinja>=2.0.0",
         "jinja2",
         "wtforms",
```

### Comparing `govuk-frontend-wtf-2.4.0/tests/test_wtf_widgets.py` & `govuk-frontend-wtf-2.5.0/tests/test_wtf_widgets.py`

 * *Files identical despite different names*

