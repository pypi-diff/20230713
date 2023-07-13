# Comparing `tmp/pangeo-forge-cordex-0.3.2.tar.gz` & `tmp/pangeo-forge-cordex-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.3.2.tar", last modified: Mon Jun  5 11:45:04 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.3.3.tar", last modified: Thu Jul 13 20:14:31 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.3.2.tar` & `pangeo-forge-cordex-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.517220 pangeo-forge-cordex-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 11:45:04.000000 pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-05 11:45:04.525220 pangeo-forge-cordex-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:45:04.521220 pangeo-forge-cordex-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-05 11:44:53.000000 pangeo-forge-cordex-0.3.2/tests/test_recipe_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.575570 pangeo-forge-cordex-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.579570 pangeo-forge-cordex-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.579570 pangeo-forge-cordex-0.3.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.579570 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.3.2/.github/workflows/ci.yaml` & `pangeo-forge-cordex-0.3.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.3.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/.gitignore` & `pangeo-forge-cordex-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/LICENSE` & `pangeo-forge-cordex-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/PKG-INFO` & `pangeo-forge-cordex-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.3.2
+Version: 0.3.3
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/catalog.py` & `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/catalog.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/esgf_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import ssl
 
 import requests
 
 from .utils import combine_response, parse_dataset_response, sort_files_by_dataset_id
 
+host = "https://esgf-data.dkrz.de/esg-search/search"
+
 
 def logon(host=None):
     from pyesgf.logon import LogonManager
 
     if host is None:
         host = "esgf-data.dkrz.de"
     lm = LogonManager(verify=True)
@@ -35,19 +37,21 @@
     sslcontext = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH)
     sslcontext.load_verify_locations(capath=lm.esgf_certs_dir)
     sslcontext.load_cert_chain(lm.esgf_credentials)
     return sslcontext
 
 
 def request(
-    url="https://esgf-node.llnl.gov/esg-search/search",
+    url=None,
     project="CORDEX",
     type="File",
     **search,
 ):
+    if url is None:
+        url = host
     version = search.get("version", None)
     if type == "File" and version:
         # this does not work for File searches since version denotes here rcm_version
         del search["version"]
     elif version and version.startswith("v"):
         search["version"] = version[1:]
     params = dict(project=project, type=type, format="application/solr+json", limit=500)
```

### Comparing `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 # 'cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas'
 known_projects = [
     "CORDEX",  # Usual Cordex datasets from CMIP5 downscaling
     "CORDEX-Reklies",  # This is Downscaling from Reklies project
     "CORDEX-Adjust",  # Bias adjusted output
     "CORDEX-ESD",  # Statistical downscaling
+    "CORDEX-FPSCONV",  # FPS convection
 ]
 
 
 cordex_template = "project.product.domain.institute.driving_model.experiment.ensemble.rcm_name.rcm_version.time_frequency.variable.version"
 cordex_adjust_template = "project.product.domain.institute.driving_model.experiment.ensemble.rcm_name.bias_adjustment.time_frequency.variable.version"
 
 base_params = {
@@ -62,15 +63,15 @@
 
 def facets_from_iid(iid, project=None):
     """Translates iid string to facet dict according to project naming scheme"""
     if project is None:
         # take project id from first iid entry by default
         project = project_from_iid(iid)
     iid = f"{project}." + ".".join(iid.split(".")[1:])
-    iid_name_template = id_templates[project]
+    iid_name_template = id_templates.get(project, cordex_template)
     # this does not work yet with CORDEX project
     # template = get_dataset_id_template(project)
     # facet_names = facets_from_template(template)
     facets = {}
     for name, value in zip(iid_name_template.split("."), iid.split(".")):
         if value != "*":
             facets[name] = value
@@ -105,15 +106,15 @@
 
 def request_project_facets(project, url=None):
     template = get_dataset_id_template(project, url)
     return facets_from_template(template)
 
 
 def request_from_facets(url, project, type="Dataset", **facets):
-    params = request_params[project].copy()
+    params = request_params.get(project, cordex_params).copy()
     params.update(facets)
     params["project"] = project
     params["type"] = type
     return requests.get(url=url, params=params)
 
 
 def instance_ids_from_request(json_dict):
```

### Comparing `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/recipe.py` & `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/recipe.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex/utils.py` & `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/PKG-INFO` & `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.3.2
+Version: 0.3.3
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.3.2/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/setup.cfg` & `pangeo-forge-cordex-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/tests/test_parsing.py` & `pangeo-forge-cordex-0.3.3/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.2/tests/test_recipe_creation.py` & `pangeo-forge-cordex-0.3.3/tests/test_recipe_creation.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import xarray as xr
 from pangeo_forge_recipes.patterns import pattern_from_file_sequence
 from pangeo_forge_recipes.recipes import XarrayZarrRecipe
 
 from pangeo_forge_cordex import logon, recipe_inputs_from_iids
 
 iids = [
-    # "cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas.v20140620",
+    "cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas.v20140620",
     "cordex.output.EUR-11.GERICS.ECMWF-ERAINT.evaluation.r1i1p1.REMO2015.v1.mon.tas.v20180813",
 ]
 
 
 @pytest.mark.parametrize("iid", iids)
 def test_recipe_inputs(iid):
     sslcontext = logon()
```

