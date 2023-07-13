# Comparing `tmp/Leonardo-Ai-SDK-1.6.1.tar.gz` & `tmp/Leonardo-Ai-SDK-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-1.6.1.tar", last modified: Wed Jul 12 00:25:36 2023, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-1.7.0.tar", last modified: Thu Jul 13 00:25:21 2023, max compression
```

## Comparing `Leonardo-Ai-SDK-1.6.1.tar` & `Leonardo-Ai-SDK-1.7.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:25:36.133340 Leonardo-Ai-SDK-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-12 00:25:36.133340 Leonardo-Ai-SDK-1.6.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3505 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 00:25:36.133340 Leonardo-Ai-SDK-1.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:25:36.125340 Leonardo-Ai-SDK-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:25:36.125340 Leonardo-Ai-SDK-1.6.1/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-12 00:25:36.000000 Leonardo-Ai-SDK-1.6.1/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-12 00:25:36.000000 Leonardo-Ai-SDK-1.6.1/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:25:36.000000 Leonardo-Ai-SDK-1.6.1/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-12 00:25:36.000000 Leonardo-Ai-SDK-1.6.1/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 00:25:36.000000 Leonardo-Ai-SDK-1.6.1/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:25:36.129340 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8343 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6385 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/generation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/initimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4716 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:25:36.129340 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:25:36.129340 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/createdataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7314 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/creategeneration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3867 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/createmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/createvariationupscale.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1764 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7835 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8100 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getmodelbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getuserself.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getvariationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2397 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2440 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/uploadinitimage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:25:36.133340 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/controlnet_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/custom_model_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/job_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/sd_generation_style.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/sd_versions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/strength.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/variation_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:25:36.133340 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3363 2023-07-12 00:25:21.000000 Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.528750 Leonardo-Ai-SDK-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-13 00:25:21.528750 Leonardo-Ai-SDK-1.7.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3505 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:25:21.528750 Leonardo-Ai-SDK-1.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.516750 Leonardo-Ai-SDK-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.520750 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.520750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8343 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6385 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/generation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/initimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4716 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.520750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.524750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createdataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7310 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/creategeneration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3867 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1764 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7835 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8100 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getuserself.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2397 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2440 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploadinitimage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.524750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/controlnet_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/custom_model_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/job_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/sd_versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/strength.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/variation_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.524750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3363 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-1.6.1/LICENSE.md` & `Leonardo-Ai-SDK-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/PKG-INFO` & `Leonardo-Ai-SDK-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 1.6.1
+Version: 1.7.0
 Summary: Leonardo Ai Python Client SDK
 Home-page: UNKNOWN
 Author: Leonardo-Ai
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `Leonardo-Ai-SDK-1.6.1/README.md` & `Leonardo-Ai-SDK-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/setup.py` & `Leonardo-Ai-SDK-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="Leonardo-Ai-SDK",
-    version="1.6.1",
+    version="1.7.0",
     author="Leonardo-Ai",
     description="Leonardo Ai Python Client SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `Leonardo-Ai-SDK-1.6.1/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 1.6.1
+Version: 1.7.0
 Summary: Leonardo Ai Python Client SDK
 Home-page: UNKNOWN
 Author: Leonardo-Ai
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `Leonardo-Ai-SDK-1.6.1/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/generation.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/initimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/model.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     r"""The ID of an existing image to use in image2image."""
     init_image_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('init_image_id'), 'exclude': lambda f: f is None }})
     r"""The ID of an Init Image to use in image2image."""
     init_strength: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('init_strength'), 'exclude': lambda f: f is None }})
     r"""How strongly the generated images should reflect the original image in image2image. Must be a float between 0.1 and 0.9."""
     model_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is None }})
     r"""The model ID used for the image generation. If not provided uses sd_version to determine the version of Stable Diffusion to use.
-    
+
     _Leonardo Creative_: 6bef9f1b-29cb-40c7-b9df-32b51c1f67d3
     _Leonardo Select_: cd2b2a15-9760-4174-a5ff-4d2925057376
     _Leonardo Signature_: 291be633-cb24-434f-898f-e662799936ad
     """
     negative_prompt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('negative_prompt'), 'exclude': lambda f: f is None }})
     r"""The negative prompt used for the image generation"""
     num_images: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_images'), 'exclude': lambda f: f is None }})
```

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '1.6.1'
-    gen_version: str = '2.61.4'
+    sdk_version: str = '1.7.0'
+    gen_version: str = '2.62.1'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.6.1/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

