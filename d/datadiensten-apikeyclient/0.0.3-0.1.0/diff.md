# Comparing `tmp/datadiensten-apikeyclient-0.0.3.tar.gz` & `tmp/datadiensten-apikeyclient-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadiensten-apikeyclient-0.0.3.tar", last modified: Tue Jul 11 15:01:22 2023, max compression
+gzip compressed data, was "datadiensten-apikeyclient-0.1.0.tar", last modified: Thu Jul 13 05:48:33 2023, max compression
```

## Comparing `datadiensten-apikeyclient-0.0.3.tar` & `datadiensten-apikeyclient-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/
--rw-rw-r--   0 jan       (1000) jan       (1000)      196 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)      619 2023-07-11 15:00:21.000000 datadiensten-apikeyclient-0.0.3/pyproject.toml
--rw-rw-r--   0 jan       (1000) jan       (1000)       38 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/setup.cfg
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/src/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/src/apikeyclient/
--rw-rw-r--   0 jan       (1000) jan       (1000)     3042 2023-06-30 07:23:15.000000 datadiensten-apikeyclient-0.0.3/src/apikeyclient/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-11 15:01:22.462980 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/
--rw-rw-r--   0 jan       (1000) jan       (1000)      196 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)      307 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/SOURCES.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/dependency_links.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       66 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/requires.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       13 2023-07-11 15:01:22.000000 datadiensten-apikeyclient-0.0.3/src/datadiensten_apikeyclient.egg-info/top_level.txt
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-13 05:48:33.862722 datadiensten-apikeyclient-0.1.0/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      196 2023-07-13 05:48:33.858722 datadiensten-apikeyclient-0.1.0/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)      965 2023-07-12 18:04:46.000000 datadiensten-apikeyclient-0.1.0/README.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)      619 2023-07-12 18:04:46.000000 datadiensten-apikeyclient-0.1.0/pyproject.toml
+-rw-rw-r--   0 jan       (1000) jan       (1000)       38 2023-07-13 05:48:33.862722 datadiensten-apikeyclient-0.1.0/setup.cfg
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-13 05:48:33.858722 datadiensten-apikeyclient-0.1.0/src/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-13 05:48:33.858722 datadiensten-apikeyclient-0.1.0/src/apikeyclient/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4476 2023-07-13 05:45:24.000000 datadiensten-apikeyclient-0.1.0/src/apikeyclient/__init__.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-07-13 05:48:33.858722 datadiensten-apikeyclient-0.1.0/src/datadiensten_apikeyclient.egg-info/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      196 2023-07-13 05:48:33.000000 datadiensten-apikeyclient-0.1.0/src/datadiensten_apikeyclient.egg-info/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)      317 2023-07-13 05:48:33.000000 datadiensten-apikeyclient-0.1.0/src/datadiensten_apikeyclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2023-07-13 05:48:33.000000 datadiensten-apikeyclient-0.1.0/src/datadiensten_apikeyclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       66 2023-07-13 05:48:33.000000 datadiensten-apikeyclient-0.1.0/src/datadiensten_apikeyclient.egg-info/requires.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       13 2023-07-13 05:48:33.000000 datadiensten-apikeyclient-0.1.0/src/datadiensten_apikeyclient.egg-info/top_level.txt
```

### Comparing `datadiensten-apikeyclient-0.0.3/pyproject.toml` & `datadiensten-apikeyclient-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "datadiensten-apikeyclient"
-version = "0.0.3"
+version = "0.1.0"
 description = "Client for Datadiensten apikeyserv"
-dependencies = ['pause>=0.3', 'requests', 'PyJWT[crypto]==2.4.0', 'build']
+dependencies = ['pause>=0.3', 'requests', 'PyJWT[crypto]==2.6.0', 'build']
 
 [project.optional-dependencies]  
 dev= [
     'build', 
     'twine'
 ]
```

