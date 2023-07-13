# Comparing `tmp/aacrgenie-9.0.0.tar.gz` & `tmp/aacrgenie-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aacrgenie-9.0.0.tar", last modified: Tue May 19 07:22:36 2020, max compression
+gzip compressed data, was "dist/aacrgenie-9.0.1.tar", last modified: Tue May 19 07:27:53 2020, max compression
```

## Comparing `aacrgenie-9.0.0.tar` & `aacrgenie-9.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-19 07:22:36.423233 aacrgenie-9.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4369 2020-05-19 07:22:36.423233 aacrgenie-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3392 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-19 07:22:36.419233 aacrgenie-9.0.0/aacrgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4369 2020-05-19 07:22:36.000000 aacrgenie-9.0.0/aacrgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      978 2020-05-19 07:22:36.000000 aacrgenie-9.0.0/aacrgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-19 07:22:36.000000 aacrgenie-9.0.0/aacrgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2020-05-19 07:22:36.000000 aacrgenie-9.0.0/aacrgenie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-19 07:22:36.000000 aacrgenie-9.0.0/aacrgenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       81 2020-05-19 07:22:36.000000 aacrgenie-9.0.0/aacrgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-05-19 07:22:36.000000 aacrgenie-9.0.0/aacrgenie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-19 07:22:36.419233 aacrgenie-9.0.0/bin/
--rw-r--r--   0 runner    (1001) docker     (116)    13782 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/bin/database_to_staging.py
--rw-r--r--   0 runner    (1001) docker     (116)     6926 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/bin/input_to_database.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-19 07:22:36.423233 aacrgenie-9.0.0/genie/
--rw-r--r--   0 runner    (1001) docker     (116)      602 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4177 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12289 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/assay.py
--rw-r--r--   0 runner    (1001) docker     (116)    24921 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/bed.py
--rw-r--r--   0 runner    (1001) docker     (116)      378 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/bedSP.py
--rw-r--r--   0 runner    (1001) docker     (116)      117 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/cbs.py
--rw-r--r--   0 runner    (1001) docker     (116)    30660 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/clinical.py
--rw-r--r--   0 runner    (1001) docker     (116)     2843 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/clinicalSP.py
--rw-r--r--   0 runner    (1001) docker     (116)     7309 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/cna.py
--rw-r--r--   0 runner    (1001) docker     (116)      676 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    23931 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/consortium_to_public.py
--rw-r--r--   0 runner    (1001) docker     (116)     9144 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/create_case_lists.py
--rw-r--r--   0 runner    (1001) docker     (116)    32005 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/dashboard_table_updater.py
--rw-r--r--   0 runner    (1001) docker     (116)    65496 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/database_to_staging.py
--rw-r--r--   0 runner    (1001) docker     (116)     5605 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/example_filetype_format.py
--rw-r--r--   0 runner    (1001) docker     (116)     6397 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/fusions.py
--rw-r--r--   0 runner    (1001) docker     (116)    33478 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/input_to_database.py
--rw-r--r--   0 runner    (1001) docker     (116)    14465 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/maf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1495 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/mafSP.py
--rw-r--r--   0 runner    (1001) docker     (116)     2938 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/mutationsInCis.py
--rw-r--r--   0 runner    (1001) docker     (116)     3444 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/patientCounts.py
--rw-r--r--   0 runner    (1001) docker     (116)      212 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/patientRetraction.py
--rw-r--r--   0 runner    (1001) docker     (116)    32948 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/process_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1893 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/sampleRetraction.py
--rw-r--r--   0 runner    (1001) docker     (116)     2527 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/seg.py
--rw-r--r--   0 runner    (1001) docker     (116)     2811 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/toRetract.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    10031 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/validate.py
--rw-r--r--   0 runner    (1001) docker     (116)    10698 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/vcf.py
--rw-r--r--   0 runner    (1001) docker     (116)     4989 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/vitalStatus.py
--rw-r--r--   0 runner    (1001) docker     (116)      570 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/workflow.py
--rw-r--r--   0 runner    (1001) docker     (116)     1928 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/genie/write_invalid_reasons.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-05-19 07:22:36.423233 aacrgenie-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1168 2020-05-19 07:22:22.000000 aacrgenie-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-19 07:27:53.518545 aacrgenie-9.0.1/
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     4430 2020-05-19 07:27:53.518545 aacrgenie-9.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3453 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-19 07:27:53.514545 aacrgenie-9.0.1/aacrgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4430 2020-05-19 07:27:53.000000 aacrgenie-9.0.1/aacrgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      978 2020-05-19 07:27:53.000000 aacrgenie-9.0.1/aacrgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-19 07:27:53.000000 aacrgenie-9.0.1/aacrgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2020-05-19 07:27:53.000000 aacrgenie-9.0.1/aacrgenie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-19 07:27:53.000000 aacrgenie-9.0.1/aacrgenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2020-05-19 07:27:53.000000 aacrgenie-9.0.1/aacrgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-05-19 07:27:53.000000 aacrgenie-9.0.1/aacrgenie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-19 07:27:53.514545 aacrgenie-9.0.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (116)    13782 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/bin/database_to_staging.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6926 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/bin/input_to_database.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-19 07:27:53.518545 aacrgenie-9.0.1/genie/
+-rw-r--r--   0 runner    (1001) docker     (116)      602 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4177 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12289 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/assay.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24921 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/bed.py
+-rw-r--r--   0 runner    (1001) docker     (116)      378 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/bedSP.py
+-rw-r--r--   0 runner    (1001) docker     (116)      117 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/cbs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30660 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/clinical.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2843 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/clinicalSP.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7309 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/cna.py
+-rw-r--r--   0 runner    (1001) docker     (116)      676 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23931 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/consortium_to_public.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9144 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/create_case_lists.py
+-rw-r--r--   0 runner    (1001) docker     (116)    32005 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/dashboard_table_updater.py
+-rw-r--r--   0 runner    (1001) docker     (116)    65496 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/database_to_staging.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5605 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/example_filetype_format.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6397 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/fusions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    33478 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/input_to_database.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14465 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/maf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1495 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/mafSP.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2938 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/mutationsInCis.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3444 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/patientCounts.py
+-rw-r--r--   0 runner    (1001) docker     (116)      212 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/patientRetraction.py
+-rw-r--r--   0 runner    (1001) docker     (116)    32948 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/process_functions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1893 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/sampleRetraction.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2527 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/seg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2811 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/toRetract.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    10031 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/validate.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10698 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/vcf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4989 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/vitalStatus.py
+-rw-r--r--   0 runner    (1001) docker     (116)      570 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1928 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/genie/write_invalid_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-05-19 07:27:53.518545 aacrgenie-9.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1168 2020-05-19 07:27:46.000000 aacrgenie-9.0.1/setup.py
```

### Comparing `aacrgenie-9.0.0/PKG-INFO` & `aacrgenie-9.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aacrgenie
-Version: 9.0.0
+Version: 9.0.1
 Summary: Processing and validation for GENIE
 Home-page: https://github.com/Sage-Bionetworks/Genie
 Author: Thomas Yu
 Author-email: thomas.yu@sagebionetworks.org
 License: MIT
-Description: ![genie banner](genie_banner.png)
+Description: ![genie banner](https://raw.githubusercontent.com/Sage-Bionetworks/Genie/master/genie_banner.png)
         
         # AACR Project GENIE
         
         [![Docker Automated](https://img.shields.io/docker/automated/sagebionetworks/genie.svg)](https://hub.docker.com/r/sagebionetworks/genie) ![Docker Build](https://img.shields.io/docker/build/sagebionetworks/genie.svg)
         
         
         ## Introduction
@@ -23,15 +23,15 @@
         - Python 3.6 or higher
         - Synapse [command-line client](http://python-docs.synapse.org/CommandLineClient.html) (`pip install synapseclient`)
         - Python [pandas](http://pandas.pydata.org/) (`pip install pandas`)
         - [bedtools](https://bedtools.readthedocs.io/en/latest/content/installation.html)
         
         ## File Validator
         ```
-        pip install synapsegenie
+        pip install aacrgenie
         genie -v
         ```
         
         This will install all the necessary components for you to run the validator locally on all of your files, including the Synapse client.  Please view the help to see how to run to validator.  
         ```
         genie validate -h
         genie validate data_clinical_supp_SAGE.txt SAGE
```

### Comparing `aacrgenie-9.0.0/README.md` & `aacrgenie-9.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![genie banner](genie_banner.png)
+![genie banner](https://raw.githubusercontent.com/Sage-Bionetworks/Genie/master/genie_banner.png)
 
 # AACR Project GENIE
 
 [![Docker Automated](https://img.shields.io/docker/automated/sagebionetworks/genie.svg)](https://hub.docker.com/r/sagebionetworks/genie) ![Docker Build](https://img.shields.io/docker/build/sagebionetworks/genie.svg)
 
 
 ## Introduction
@@ -15,15 +15,15 @@
 - Python 3.6 or higher
 - Synapse [command-line client](http://python-docs.synapse.org/CommandLineClient.html) (`pip install synapseclient`)
 - Python [pandas](http://pandas.pydata.org/) (`pip install pandas`)
 - [bedtools](https://bedtools.readthedocs.io/en/latest/content/installation.html)
 
 ## File Validator
 ```
-pip install synapsegenie
+pip install aacrgenie
 genie -v
 ```
 
 This will install all the necessary components for you to run the validator locally on all of your files, including the Synapse client.  Please view the help to see how to run to validator.  
 ```
 genie validate -h
 genie validate data_clinical_supp_SAGE.txt SAGE
```

### Comparing `aacrgenie-9.0.0/aacrgenie.egg-info/PKG-INFO` & `aacrgenie-9.0.1/aacrgenie.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aacrgenie
-Version: 9.0.0
+Version: 9.0.1
 Summary: Processing and validation for GENIE
 Home-page: https://github.com/Sage-Bionetworks/Genie
 Author: Thomas Yu
 Author-email: thomas.yu@sagebionetworks.org
 License: MIT
-Description: ![genie banner](genie_banner.png)
+Description: ![genie banner](https://raw.githubusercontent.com/Sage-Bionetworks/Genie/master/genie_banner.png)
         
         # AACR Project GENIE
         
         [![Docker Automated](https://img.shields.io/docker/automated/sagebionetworks/genie.svg)](https://hub.docker.com/r/sagebionetworks/genie) ![Docker Build](https://img.shields.io/docker/build/sagebionetworks/genie.svg)
         
         
         ## Introduction
@@ -23,15 +23,15 @@
         - Python 3.6 or higher
         - Synapse [command-line client](http://python-docs.synapse.org/CommandLineClient.html) (`pip install synapseclient`)
         - Python [pandas](http://pandas.pydata.org/) (`pip install pandas`)
         - [bedtools](https://bedtools.readthedocs.io/en/latest/content/installation.html)
         
         ## File Validator
         ```
-        pip install synapsegenie
+        pip install aacrgenie
         genie -v
         ```
         
         This will install all the necessary components for you to run the validator locally on all of your files, including the Synapse client.  Please view the help to see how to run to validator.  
         ```
         genie validate -h
         genie validate data_clinical_supp_SAGE.txt SAGE
```

### Comparing `aacrgenie-9.0.0/aacrgenie.egg-info/SOURCES.txt` & `aacrgenie-9.0.1/aacrgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/bin/database_to_staging.py` & `aacrgenie-9.0.1/bin/database_to_staging.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/bin/input_to_database.py` & `aacrgenie-9.0.1/bin/input_to_database.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/__init__.py` & `aacrgenie-9.0.1/genie/__init__.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/__main__.py` & `aacrgenie-9.0.1/genie/__main__.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/assay.py` & `aacrgenie-9.0.1/genie/assay.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/bed.py` & `aacrgenie-9.0.1/genie/bed.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/clinical.py` & `aacrgenie-9.0.1/genie/clinical.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/clinicalSP.py` & `aacrgenie-9.0.1/genie/clinicalSP.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/cna.py` & `aacrgenie-9.0.1/genie/cna.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/config.py` & `aacrgenie-9.0.1/genie/config.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/consortium_to_public.py` & `aacrgenie-9.0.1/genie/consortium_to_public.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/create_case_lists.py` & `aacrgenie-9.0.1/genie/create_case_lists.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/dashboard_table_updater.py` & `aacrgenie-9.0.1/genie/dashboard_table_updater.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/database_to_staging.py` & `aacrgenie-9.0.1/genie/database_to_staging.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/example_filetype_format.py` & `aacrgenie-9.0.1/genie/example_filetype_format.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/fusions.py` & `aacrgenie-9.0.1/genie/fusions.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/input_to_database.py` & `aacrgenie-9.0.1/genie/input_to_database.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/maf.py` & `aacrgenie-9.0.1/genie/maf.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/mafSP.py` & `aacrgenie-9.0.1/genie/mafSP.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/mutationsInCis.py` & `aacrgenie-9.0.1/genie/mutationsInCis.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/patientCounts.py` & `aacrgenie-9.0.1/genie/patientCounts.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/process_functions.py` & `aacrgenie-9.0.1/genie/process_functions.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/sampleRetraction.py` & `aacrgenie-9.0.1/genie/sampleRetraction.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/seg.py` & `aacrgenie-9.0.1/genie/seg.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/toRetract.py` & `aacrgenie-9.0.1/genie/toRetract.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/validate.py` & `aacrgenie-9.0.1/genie/validate.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/vcf.py` & `aacrgenie-9.0.1/genie/vcf.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/vitalStatus.py` & `aacrgenie-9.0.1/genie/vitalStatus.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/workflow.py` & `aacrgenie-9.0.1/genie/workflow.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/genie/write_invalid_reasons.py` & `aacrgenie-9.0.1/genie/write_invalid_reasons.py`

 * *Files identical despite different names*

### Comparing `aacrgenie-9.0.0/setup.py` & `aacrgenie-9.0.1/setup.py`

 * *Files identical despite different names*

