# Comparing `tmp/opsgeniecli-0.1.8.tar.gz` & `tmp/opsgeniecli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsgeniecli-0.1.8.tar", last modified: Thu Jul 13 09:42:28 2023, max compression
+gzip compressed data, was "opsgeniecli-0.1.9.tar", last modified: Thu Jul 13 10:55:18 2023, max compression
```

## Comparing `opsgeniecli-0.1.8.tar` & `opsgeniecli-0.1.9.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 09:42:28.758680 opsgeniecli-0.1.8/
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)        5 2023-07-13 08:51:11.000000 opsgeniecli-0.1.8/.VERSION
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)      171 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/AUTHORS.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     1277 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/CONTRIBUTING.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     8927 2023-07-13 08:51:25.000000 opsgeniecli-0.1.8/HISTORY.rst
--rw-r--r--   0 yhoorneman   (502) staff       (20)     1063 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/LICENSE
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)      396 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/MANIFEST.in
--rw-r--r--   0 yhoorneman   (502) staff       (20)    16425 2023-07-13 09:42:28.759365 opsgeniecli-0.1.8/PKG-INFO
--rw-r--r--   0 yhoorneman   (502) staff       (20)      635 2023-07-13 09:14:58.000000 opsgeniecli-0.1.8/Pipfile
--rw-r--r--   0 yhoorneman   (502) staff       (20)    78894 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/Pipfile.lock
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     2272 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/README.rst
--rw-r--r--   0 yhoorneman   (502) staff       (20)      901 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/USAGE.rst
--rw-r--r--   0 yhoorneman   (502) staff       (20)      588 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/dev-requirements.txt
-drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 09:42:28.628066 opsgeniecli-0.1.8/docs/
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     6782 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/Makefile
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)       28 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/authors.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     8936 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/conf.py
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)       33 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/contributing.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)       28 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/history.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)      507 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/index.rst
--rw-r--r--   0 yhoorneman   (502) staff       (20)       33 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/installation.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)       27 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/readme.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)       26 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/docs/usage.rst
-drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 09:42:28.710056 opsgeniecli-0.1.8/opsgeniecli/
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)        5 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/.VERSION
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)      171 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/AUTHORS.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     1277 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/CONTRIBUTING.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     8927 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/HISTORY.rst
--rw-r--r--   0 yhoorneman   (502) staff       (20)     1063 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/LICENSE
--rw-r--r--   0 yhoorneman   (502) staff       (20)      635 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/Pipfile
--rw-r--r--   0 yhoorneman   (502) staff       (20)    78894 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/Pipfile.lock
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     2272 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/README.rst
--rw-r--r--   0 yhoorneman   (502) staff       (20)      901 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/USAGE.rst
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     1811 2023-03-21 13:56:18.000000 opsgeniecli-0.1.8/opsgeniecli/__init__.py
--rw-r--r--   0 yhoorneman   (502) staff       (20)     2212 2023-03-21 13:56:18.000000 opsgeniecli-0.1.8/opsgeniecli/_version.py
-drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 09:42:28.752220 opsgeniecli-0.1.8/opsgeniecli/conf/
--rw-r--r--   0 yhoorneman   (502) staff       (20)      814 2023-03-21 13:56:18.000000 opsgeniecli-0.1.8/opsgeniecli/conf/logging.json-example
--rw-r--r--   0 yhoorneman   (502) staff       (20)      588 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/dev-requirements.txt
--rw-r--r--   0 yhoorneman   (502) staff       (20)     4999 2023-03-21 13:57:25.000000 opsgeniecli-0.1.8/opsgeniecli/opsgenie_cli_test.py
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)    95022 2023-03-21 13:57:25.000000 opsgeniecli-0.1.8/opsgeniecli/opsgeniecli.py
--rw-r--r--   0 yhoorneman   (502) staff       (20)     1725 2023-03-21 13:56:18.000000 opsgeniecli-0.1.8/opsgeniecli/opsgeniecliexceptions.py
--rw-r--r--   0 yhoorneman   (502) staff       (20)      475 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/opsgeniecli/requirements.txt
-drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 09:42:28.749048 opsgeniecli-0.1.8/opsgeniecli.egg-info/
--rw-r--r--   0 yhoorneman   (502) staff       (20)    16425 2023-07-13 09:42:28.000000 opsgeniecli-0.1.8/opsgeniecli.egg-info/PKG-INFO
--rw-r--r--   0 yhoorneman   (502) staff       (20)     1044 2023-07-13 09:42:28.000000 opsgeniecli-0.1.8/opsgeniecli.egg-info/SOURCES.txt
--rw-r--r--   0 yhoorneman   (502) staff       (20)        1 2023-07-13 09:42:28.000000 opsgeniecli-0.1.8/opsgeniecli.egg-info/dependency_links.txt
--rw-r--r--   0 yhoorneman   (502) staff       (20)       62 2023-07-13 09:42:28.000000 opsgeniecli-0.1.8/opsgeniecli.egg-info/entry_points.txt
--rw-r--r--   0 yhoorneman   (502) staff       (20)        1 2023-03-21 14:14:07.000000 opsgeniecli-0.1.8/opsgeniecli.egg-info/not-zip-safe
--rw-r--r--   0 yhoorneman   (502) staff       (20)      142 2023-07-13 09:42:28.000000 opsgeniecli-0.1.8/opsgeniecli.egg-info/requires.txt
--rw-r--r--   0 yhoorneman   (502) staff       (20)       12 2023-07-13 09:42:28.000000 opsgeniecli-0.1.8/opsgeniecli.egg-info/top_level.txt
--rw-r--r--   0 yhoorneman   (502) staff       (20)      475 2023-07-13 09:42:27.000000 opsgeniecli-0.1.8/requirements.txt
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)      151 2023-07-13 09:42:28.768872 opsgeniecli-0.1.8/setup.cfg
--rwxr-xr-x   0 yhoorneman   (502) staff       (20)     2278 2023-07-13 09:31:05.000000 opsgeniecli-0.1.8/setup.py
-drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 09:42:28.754214 opsgeniecli-0.1.8/tests/
--rw-r--r--   0 yhoorneman   (502) staff       (20)     2257 2023-03-21 13:56:17.000000 opsgeniecli-0.1.8/tests/test_opsgeniecli.py
+drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 10:55:18.753859 opsgeniecli-0.1.9/
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)        5 2023-07-13 10:53:41.000000 opsgeniecli-0.1.9/.VERSION
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)      171 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/AUTHORS.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     1277 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/CONTRIBUTING.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     8924 2023-07-13 10:53:44.000000 opsgeniecli-0.1.9/HISTORY.rst
+-rw-r--r--   0 yhoorneman   (502) staff       (20)     1063 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/LICENSE
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)      396 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/MANIFEST.in
+-rw-r--r--   0 yhoorneman   (502) staff       (20)    11727 2023-07-13 10:55:18.754349 opsgeniecli-0.1.9/PKG-INFO
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      664 2023-07-13 10:52:11.000000 opsgeniecli-0.1.9/Pipfile
+-rw-r--r--   0 yhoorneman   (502) staff       (20)    80148 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/Pipfile.lock
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     2272 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/README.rst
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      901 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/USAGE.rst
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      588 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/dev-requirements.txt
+drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 10:55:18.644217 opsgeniecli-0.1.9/docs/
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     6782 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/Makefile
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)       28 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/authors.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     8936 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/conf.py
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)       33 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/contributing.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)       28 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/history.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)      507 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/index.rst
+-rw-r--r--   0 yhoorneman   (502) staff       (20)       33 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/installation.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)       27 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/readme.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)       26 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/docs/usage.rst
+drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 10:55:18.718577 opsgeniecli-0.1.9/opsgeniecli/
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)        5 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/.VERSION
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)      171 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/AUTHORS.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     1277 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/CONTRIBUTING.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     8924 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/HISTORY.rst
+-rw-r--r--   0 yhoorneman   (502) staff       (20)     1063 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/LICENSE
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      664 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/Pipfile
+-rw-r--r--   0 yhoorneman   (502) staff       (20)    80148 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/Pipfile.lock
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     2272 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/README.rst
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      901 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/USAGE.rst
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     1811 2023-03-21 13:56:18.000000 opsgeniecli-0.1.9/opsgeniecli/__init__.py
+-rw-r--r--   0 yhoorneman   (502) staff       (20)     2212 2023-03-21 13:56:18.000000 opsgeniecli-0.1.9/opsgeniecli/_version.py
+drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 10:55:18.746370 opsgeniecli-0.1.9/opsgeniecli/conf/
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      814 2023-03-21 13:56:18.000000 opsgeniecli-0.1.9/opsgeniecli/conf/logging.json-example
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      588 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/dev-requirements.txt
+-rw-r--r--   0 yhoorneman   (502) staff       (20)     4999 2023-07-13 10:46:14.000000 opsgeniecli-0.1.9/opsgeniecli/opsgenie_cli_test.py
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)    94961 2023-07-13 10:46:14.000000 opsgeniecli-0.1.9/opsgeniecli/opsgeniecli.py
+-rw-r--r--   0 yhoorneman   (502) staff       (20)     1725 2023-03-21 13:56:18.000000 opsgeniecli-0.1.9/opsgeniecli/opsgeniecliexceptions.py
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      496 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/opsgeniecli/requirements.txt
+drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 10:55:18.743189 opsgeniecli-0.1.9/opsgeniecli.egg-info/
+-rw-r--r--   0 yhoorneman   (502) staff       (20)    11727 2023-07-13 10:55:18.000000 opsgeniecli-0.1.9/opsgeniecli.egg-info/PKG-INFO
+-rw-r--r--   0 yhoorneman   (502) staff       (20)     1006 2023-07-13 10:55:18.000000 opsgeniecli-0.1.9/opsgeniecli.egg-info/SOURCES.txt
+-rw-r--r--   0 yhoorneman   (502) staff       (20)        1 2023-07-13 10:55:18.000000 opsgeniecli-0.1.9/opsgeniecli.egg-info/dependency_links.txt
+-rw-r--r--   0 yhoorneman   (502) staff       (20)        1 2023-03-21 14:14:07.000000 opsgeniecli-0.1.9/opsgeniecli.egg-info/not-zip-safe
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      163 2023-07-13 10:55:18.000000 opsgeniecli-0.1.9/opsgeniecli.egg-info/requires.txt
+-rw-r--r--   0 yhoorneman   (502) staff       (20)       12 2023-07-13 10:55:18.000000 opsgeniecli-0.1.9/opsgeniecli.egg-info/top_level.txt
+-rw-r--r--   0 yhoorneman   (502) staff       (20)      496 2023-07-13 10:55:17.000000 opsgeniecli-0.1.9/requirements.txt
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)      151 2023-07-13 10:55:18.769539 opsgeniecli-0.1.9/setup.cfg
+-rwxr-xr-x   0 yhoorneman   (502) staff       (20)     2277 2023-07-13 10:46:14.000000 opsgeniecli-0.1.9/setup.py
+drwxr-xr-x   0 yhoorneman   (502) staff       (20)        0 2023-07-13 10:55:18.751803 opsgeniecli-0.1.9/tests/
+-rw-r--r--   0 yhoorneman   (502) staff       (20)     2257 2023-03-21 13:56:17.000000 opsgeniecli-0.1.9/tests/test_opsgeniecli.py
```

### Comparing `opsgeniecli-0.1.8/CONTRIBUTING.rst` & `opsgeniecli-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/HISTORY.rst` & `opsgeniecli-0.1.9/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -506,14 +506,14 @@
 
 * click escaped the query input, which it shouldnt, thus its removed to allow teams with spaces
 
 
 0.1.7 (13-07-2023)
 ------------------
 
-* Testing installation with pipx
+* Using absolute imports
 
 
-0.1.8 (13-07-2023)
+0.1.9 (13-07-2023)
 ------------------
 
-* Testing with pipx
+* Using absolute imports
```

### Comparing `opsgeniecli-0.1.8/LICENSE` & `opsgeniecli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/Pipfile` & `opsgeniecli-0.1.9/Pipfile`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 prospector = ">=1.8,<2.0"
 coverage = ">=7,<8.0"
 nose = ">=1.3,<2.0"
 nose-htmloutput = ">=0.1,<1.0"
 tox = ">=4.0<5.0"
 betamax = ">=0.8,<1.0"
 betamax-serializers = "~=0.2,<1.0"
-semver = ">=3.0"
+semver = "==2.13.0"
 gitwrapperlib = ">=1.0,<2.0"
+twine = ">=4.0,<5.0"
 coloredlogs = ">=15.0,<16.0"
 emoji = ">=2.0,<3.0"
 toml = ">=0.1,<1.0"
-twine = "*"
 
 [packages]
 coloredlogs = "~=15.0.1"
 click = "~=7.1.2"
 click-completion = "~=0.5.2"
-opsgenielib = "~=0.0.36"
+opsgenielib = "==0.0.36"
 pendulum = "~=2.1.2"
 prettytable = "~=3.2.0"
 pytz = "*"
 requests = "*"
+setuptools = "*"
```

### Comparing `opsgeniecli-0.1.8/Pipfile.lock` & `opsgeniecli-0.1.9/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9759920634920635%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'1d9772272072558c34d9016a1e1878da996e978b457b53b1ff6ac6ccf8f09103'}}",*

 * * "'default'": "{'opsgenielib': {'hashes': "*

 * *              "['sha256:1d07530b00d478ad5f8e944b7f17dbf23bbd7e11ea81d30941de1f87741f7dbb', "*

 * *              "'sha256:96099d6866d65c0c02bf1411e74b662c0c6f5a459194e3bd94f3155b53067f20'], "*

 * *              "'version': '==0.0.36'}, 'pytz': {'hashes': "*

 * *              "['sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0', "*

 * *           […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1c11fe10dc5940076cd3b759861b80ba90b1a67d9ae8bf6f548186595dcd955d"
+            "sha256": "1d9772272072558c34d9016a1e1878da996e978b457b53b1ff6ac6ccf8f09103"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
@@ -204,19 +204,19 @@
                 "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.1.3"
         },
         "opsgenielib": {
             "hashes": [
-                "sha256:67663ef70b225ab33f4bc8007823a579cf19fcee8015abedb7788d3598afb16d",
-                "sha256:e03fec18ab690a2097dfe984eb95d7a036b4672496c2b5593f63e0b54b449c53"
+                "sha256:1d07530b00d478ad5f8e944b7f17dbf23bbd7e11ea81d30941de1f87741f7dbb",
+                "sha256:96099d6866d65c0c02bf1411e74b662c0c6f5a459194e3bd94f3155b53067f20"
             ],
             "index": "pypi",
-            "version": "==0.0.41"
+            "version": "==0.0.36"
         },
         "pendulum": {
             "hashes": [
                 "sha256:0731f0c661a3cb779d398803655494893c9f581f6488048b3fb629c2342b5394",
                 "sha256:1245cd0075a3c6d889f581f6325dd8404aca5884dea7223a5566c38aab94642b",
                 "sha256:29c40a6f2942376185728c9a0347d7c0f07905638c83007e1d262781f1e6953a",
                 "sha256:2d1619a721df661e506eff8db8614016f0720ac171fe80dda1333ee44e684087",
@@ -255,19 +255,19 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pytz": {
             "hashes": [
-                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
-                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
+                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
+                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
             ],
             "index": "pypi",
-            "version": "==2023.3"
+            "version": "==2022.7.1"
         },
         "pytzdata": {
             "hashes": [
                 "sha256:3efa13b335a00a8de1d345ae41ec78dd11c9f8807f522d39850f2dd828681540",
                 "sha256:e1e14750bcf95016381e4d472bad004eef710f2d6417240904070b3d6654485f"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -277,14 +277,22 @@
             "hashes": [
                 "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
                 "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
             ],
             "index": "pypi",
             "version": "==2.28.2"
         },
+        "setuptools": {
+            "hashes": [
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
+            ],
+            "index": "pypi",
+            "version": "==68.0.0"
+        },
         "shellingham": {
             "hashes": [
                 "sha256:368bf8c00754fd4f55afb7bbb86e272df77e4dc76ac29dbcbb81a59e9fc15744",
                 "sha256:823bc5fb5c34d60f285b624e7264f4dda254bc803a3774a147bf99c0e3004a28"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.5.0.post1"
@@ -656,15 +664,17 @@
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
                 "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
-                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
+                "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743",
+                "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==6.8.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
@@ -879,21 +889,29 @@
             "hashes": [
                 "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
                 "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.2.0"
         },
+        "poetry-semver": {
+            "hashes": [
+                "sha256:4e6349bd7231cc657f0e1930f7b204e87e33dfd63eef5cac869363969515083a",
+                "sha256:d809b612aa27b39bf2d0fc9d31b4f4809b0e972646c5f19cfa46c725b7638810"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==0.1.0"
+        },
         "prospector": {
             "hashes": [
-                "sha256:3bfe103c28bb821cca84926ca31357fbfd32405e4bf8c34ca2e55885684557e4",
-                "sha256:cc8f09e79bdd32247edddf05b666940e88ad96338a84f5717b1e8c0678337821"
+                "sha256:599f31516f857d785058773875e9358702ad653e65461e8cad44134d8ee17b1f",
+                "sha256:c24011019e48b54745dc0f5d3d25e9d6b19750129996c134253c2f1eed9d45ac"
             ],
             "index": "pypi",
-            "version": "==1.10.2"
+            "version": "==1.9.0"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
@@ -1034,55 +1052,59 @@
                 "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.0.0"
         },
         "requirements-detector": {
             "hashes": [
-                "sha256:3642cd7a5b261d79536c36bb7ecacf2adabd902d2e0e42bfb2ba82515da10501",
-                "sha256:d7c60493bf166da3dd59de0e6cb25765e0e32a1931aeae92614034e5786d0bd0"
+                "sha256:246bd23867c12061eadb346a6fe2e616f0b64e681936154a76c494a27cda3ea8",
+                "sha256:9af62db621c95e0176fed029079924e648de22cd0bb4189c441b9376942faab1"
             ],
             "markers": "python_version >= '3.7' and python_version < '4.0'",
-            "version": "==1.2.2"
+            "version": "==1.1.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
                 "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:91954fe80cfb7985727a467ca98a7618e5dd15178cc2da10f553b36a93859001",
+                "sha256:a104f37270bf677148d8acb07d33be1569eeee87e2d1beb286a4e9113caf6f2f",
                 "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.4.2"
         },
         "semver": {
             "hashes": [
-                "sha256:2a23844ba1647362c7490fe3995a86e097bb590d16f0f32dfc383008f19e4cdf",
-                "sha256:9ec78c5447883c67b97f98c3b6212796708191d22e4ad30f4570f840171cbce1"
+                "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4",
+                "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"
             ],
             "index": "pypi",
-            "version": "==3.0.1"
+            "version": "==2.13.0"
         },
         "setoptconf-tmp": {
             "hashes": [
                 "sha256:76035d5cd1593d38b9056ae12d460eca3aaa34ad05c315b69145e138ba80a745",
                 "sha256:e0480addd11347ba52f762f3c4d8afa3e10ad0affbc53e3ffddc0ca5f27d5778"
             ],
             "version": "==0.3.1"
         },
         "sh": {
             "hashes": [
                 "sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5",
-                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60"
+                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60",
+                "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
+                "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
             ],
             "markers": "sys_platform != 'win32'",
             "version": "==2.0.4"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
```

### Comparing `opsgeniecli-0.1.8/README.rst` & `opsgeniecli-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/USAGE.rst` & `opsgeniecli-0.1.9/USAGE.rst`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/dev-requirements.txt` & `opsgeniecli-0.1.9/dev-requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # This file is created and managed automatically by the template and it is left
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
 sphinx>=6.2.1
 sphinx-rtd-theme>=1.2.2
-prospector>=1.10.2
+prospector>=1.9.0
 coverage>=7.2.7
 nose>=1.3.7
 nose-htmloutput>=0.6.0
 tox>=4.6.4
 betamax>=0.8.1
 betamax-serializers~=0.2.1
-semver>=3.0.1
+semver==2.13.0
 gitwrapperlib>=1.0.3
+twine>=4.0.2
 coloredlogs>=15.0.1
 emoji>=2.6.0
-toml>=0.10.2
-twine~=4.0.2
+toml>=0.10.2
```

### Comparing `opsgeniecli-0.1.8/docs/Makefile` & `opsgeniecli-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/docs/conf.py` & `opsgeniecli-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli/CONTRIBUTING.rst` & `opsgeniecli-0.1.9/opsgeniecli/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli/HISTORY.rst` & `opsgeniecli-0.1.9/opsgeniecli/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -506,14 +506,14 @@
 
 * click escaped the query input, which it shouldnt, thus its removed to allow teams with spaces
 
 
 0.1.7 (13-07-2023)
 ------------------
 
-* Testing installation with pipx
+* Using absolute imports
 
 
-0.1.8 (13-07-2023)
+0.1.9 (13-07-2023)
 ------------------
 
-* Testing with pipx
+* Using absolute imports
```

### Comparing `opsgeniecli-0.1.8/opsgeniecli/LICENSE` & `opsgeniecli-0.1.9/opsgeniecli/LICENSE`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli/Pipfile` & `opsgeniecli-0.1.9/opsgeniecli/Pipfile`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 prospector = ">=1.8,<2.0"
 coverage = ">=7,<8.0"
 nose = ">=1.3,<2.0"
 nose-htmloutput = ">=0.1,<1.0"
 tox = ">=4.0<5.0"
 betamax = ">=0.8,<1.0"
 betamax-serializers = "~=0.2,<1.0"
-semver = ">=3.0"
+semver = "==2.13.0"
 gitwrapperlib = ">=1.0,<2.0"
+twine = ">=4.0,<5.0"
 coloredlogs = ">=15.0,<16.0"
 emoji = ">=2.0,<3.0"
 toml = ">=0.1,<1.0"
-twine = "*"
 
 [packages]
 coloredlogs = "~=15.0.1"
 click = "~=7.1.2"
 click-completion = "~=0.5.2"
-opsgenielib = "~=0.0.36"
+opsgenielib = "==0.0.36"
 pendulum = "~=2.1.2"
 prettytable = "~=3.2.0"
 pytz = "*"
 requests = "*"
+setuptools = "*"
```

### Comparing `opsgeniecli-0.1.8/opsgeniecli/Pipfile.lock` & `opsgeniecli-0.1.9/opsgeniecli/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9759920634920635%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'1d9772272072558c34d9016a1e1878da996e978b457b53b1ff6ac6ccf8f09103'}}",*

 * * "'default'": "{'opsgenielib': {'hashes': "*

 * *              "['sha256:1d07530b00d478ad5f8e944b7f17dbf23bbd7e11ea81d30941de1f87741f7dbb', "*

 * *              "'sha256:96099d6866d65c0c02bf1411e74b662c0c6f5a459194e3bd94f3155b53067f20'], "*

 * *              "'version': '==0.0.36'}, 'pytz': {'hashes': "*

 * *              "['sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0', "*

 * *           […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1c11fe10dc5940076cd3b759861b80ba90b1a67d9ae8bf6f548186595dcd955d"
+            "sha256": "1d9772272072558c34d9016a1e1878da996e978b457b53b1ff6ac6ccf8f09103"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
@@ -204,19 +204,19 @@
                 "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.1.3"
         },
         "opsgenielib": {
             "hashes": [
-                "sha256:67663ef70b225ab33f4bc8007823a579cf19fcee8015abedb7788d3598afb16d",
-                "sha256:e03fec18ab690a2097dfe984eb95d7a036b4672496c2b5593f63e0b54b449c53"
+                "sha256:1d07530b00d478ad5f8e944b7f17dbf23bbd7e11ea81d30941de1f87741f7dbb",
+                "sha256:96099d6866d65c0c02bf1411e74b662c0c6f5a459194e3bd94f3155b53067f20"
             ],
             "index": "pypi",
-            "version": "==0.0.41"
+            "version": "==0.0.36"
         },
         "pendulum": {
             "hashes": [
                 "sha256:0731f0c661a3cb779d398803655494893c9f581f6488048b3fb629c2342b5394",
                 "sha256:1245cd0075a3c6d889f581f6325dd8404aca5884dea7223a5566c38aab94642b",
                 "sha256:29c40a6f2942376185728c9a0347d7c0f07905638c83007e1d262781f1e6953a",
                 "sha256:2d1619a721df661e506eff8db8614016f0720ac171fe80dda1333ee44e684087",
@@ -255,19 +255,19 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pytz": {
             "hashes": [
-                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
-                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
+                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
+                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
             ],
             "index": "pypi",
-            "version": "==2023.3"
+            "version": "==2022.7.1"
         },
         "pytzdata": {
             "hashes": [
                 "sha256:3efa13b335a00a8de1d345ae41ec78dd11c9f8807f522d39850f2dd828681540",
                 "sha256:e1e14750bcf95016381e4d472bad004eef710f2d6417240904070b3d6654485f"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -277,14 +277,22 @@
             "hashes": [
                 "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
                 "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
             ],
             "index": "pypi",
             "version": "==2.28.2"
         },
+        "setuptools": {
+            "hashes": [
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
+            ],
+            "index": "pypi",
+            "version": "==68.0.0"
+        },
         "shellingham": {
             "hashes": [
                 "sha256:368bf8c00754fd4f55afb7bbb86e272df77e4dc76ac29dbcbb81a59e9fc15744",
                 "sha256:823bc5fb5c34d60f285b624e7264f4dda254bc803a3774a147bf99c0e3004a28"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.5.0.post1"
@@ -656,15 +664,17 @@
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
                 "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
-                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
+                "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743",
+                "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==6.8.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
@@ -879,21 +889,29 @@
             "hashes": [
                 "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
                 "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.2.0"
         },
+        "poetry-semver": {
+            "hashes": [
+                "sha256:4e6349bd7231cc657f0e1930f7b204e87e33dfd63eef5cac869363969515083a",
+                "sha256:d809b612aa27b39bf2d0fc9d31b4f4809b0e972646c5f19cfa46c725b7638810"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==0.1.0"
+        },
         "prospector": {
             "hashes": [
-                "sha256:3bfe103c28bb821cca84926ca31357fbfd32405e4bf8c34ca2e55885684557e4",
-                "sha256:cc8f09e79bdd32247edddf05b666940e88ad96338a84f5717b1e8c0678337821"
+                "sha256:599f31516f857d785058773875e9358702ad653e65461e8cad44134d8ee17b1f",
+                "sha256:c24011019e48b54745dc0f5d3d25e9d6b19750129996c134253c2f1eed9d45ac"
             ],
             "index": "pypi",
-            "version": "==1.10.2"
+            "version": "==1.9.0"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
@@ -1034,55 +1052,59 @@
                 "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.0.0"
         },
         "requirements-detector": {
             "hashes": [
-                "sha256:3642cd7a5b261d79536c36bb7ecacf2adabd902d2e0e42bfb2ba82515da10501",
-                "sha256:d7c60493bf166da3dd59de0e6cb25765e0e32a1931aeae92614034e5786d0bd0"
+                "sha256:246bd23867c12061eadb346a6fe2e616f0b64e681936154a76c494a27cda3ea8",
+                "sha256:9af62db621c95e0176fed029079924e648de22cd0bb4189c441b9376942faab1"
             ],
             "markers": "python_version >= '3.7' and python_version < '4.0'",
-            "version": "==1.2.2"
+            "version": "==1.1.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
                 "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:91954fe80cfb7985727a467ca98a7618e5dd15178cc2da10f553b36a93859001",
+                "sha256:a104f37270bf677148d8acb07d33be1569eeee87e2d1beb286a4e9113caf6f2f",
                 "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.4.2"
         },
         "semver": {
             "hashes": [
-                "sha256:2a23844ba1647362c7490fe3995a86e097bb590d16f0f32dfc383008f19e4cdf",
-                "sha256:9ec78c5447883c67b97f98c3b6212796708191d22e4ad30f4570f840171cbce1"
+                "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4",
+                "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"
             ],
             "index": "pypi",
-            "version": "==3.0.1"
+            "version": "==2.13.0"
         },
         "setoptconf-tmp": {
             "hashes": [
                 "sha256:76035d5cd1593d38b9056ae12d460eca3aaa34ad05c315b69145e138ba80a745",
                 "sha256:e0480addd11347ba52f762f3c4d8afa3e10ad0affbc53e3ffddc0ca5f27d5778"
             ],
             "version": "==0.3.1"
         },
         "sh": {
             "hashes": [
                 "sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5",
-                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60"
+                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60",
+                "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
+                "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
             ],
             "markers": "sys_platform != 'win32'",
             "version": "==2.0.4"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
```

### Comparing `opsgeniecli-0.1.8/opsgeniecli/README.rst` & `opsgeniecli-0.1.9/opsgeniecli/README.rst`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli/USAGE.rst` & `opsgeniecli-0.1.9/opsgeniecli/USAGE.rst`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli/__init__.py` & `opsgeniecli-0.1.9/opsgeniecli/__init__.py`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli/_version.py` & `opsgeniecli-0.1.9/opsgeniecli/_version.py`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli/conf/logging.json-example` & `opsgeniecli-0.1.9/opsgeniecli/conf/logging.json-example`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli/dev-requirements.txt` & `opsgeniecli-0.1.9/opsgeniecli/dev-requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # This file is created and managed automatically by the template and it is left
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
 sphinx>=6.2.1
 sphinx-rtd-theme>=1.2.2
-prospector>=1.10.2
+prospector>=1.9.0
 coverage>=7.2.7
 nose>=1.3.7
 nose-htmloutput>=0.6.0
 tox>=4.6.4
 betamax>=0.8.1
 betamax-serializers~=0.2.1
-semver>=3.0.1
+semver==2.13.0
 gitwrapperlib>=1.0.3
+twine>=4.0.2
 coloredlogs>=15.0.1
 emoji>=2.6.0
-toml>=0.10.2
-twine~=4.0.2
+toml>=0.10.2
```

### Comparing `opsgeniecli-0.1.8/opsgeniecli/opsgenie_cli_test.py` & `opsgeniecli-0.1.9/opsgeniecli/opsgenie_cli_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 
-from opsgenielib import Opsgenie
-import json
+from opsgenielib.opsgenielib import Opsgenie
 from opsgenielib.opsgenielibexceptions import InvalidApiKey
 
 
 try:
     opsgenie = Opsgenie('3244807b-413f-4228-99f7-5dc2252d69d6')
 except InvalidApiKey:
     raise SystemExit('I am sorry to say that the provided api key is invalid.')
```

### Comparing `opsgeniecli-0.1.8/opsgeniecli/opsgeniecli.py` & `opsgeniecli-0.1.9/opsgeniecli/opsgeniecli.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,32 +27,29 @@
 """
 Main code for opsgeniecli
 
 .. _Google Python Style Guide:
     http://google.github.io/styleguide/pyguide.html
 
 """
-from datetime import timedelta
-from datetime import datetime
 from operator import itemgetter
 import pendulum
 import urllib.parse
 import urllib.request
 import os
 import collections
 import pathlib
 import random
 import sys
 import re
 import json
 import requests
 from prettytable import PrettyTable
 import click
-import pytz
-from opsgenielib import Opsgenie, InvalidApiKey
+from opsgenielib.opsgenielib import Opsgenie, InvalidApiKey
 
 __author__ = '''Yorick Hoorneman <yhoorneman@gmail.com>'''
 __docformat__ = '''google'''
 __date__ = '''26-02-2019'''
 __copyright__ = '''Copyright 2019, Yorick Hoorneman'''
 __credits__ = ["Yorick Hoorneman"]
 __license__ = '''MIT'''
```

### Comparing `opsgeniecli-0.1.8/opsgeniecli/opsgeniecliexceptions.py` & `opsgeniecli-0.1.9/opsgeniecli/opsgeniecliexceptions.py`

 * *Files identical despite different names*

### Comparing `opsgeniecli-0.1.8/opsgeniecli.egg-info/SOURCES.txt` & `opsgeniecli-0.1.9/opsgeniecli.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -36,13 +36,12 @@
 opsgeniecli/opsgenie_cli_test.py
 opsgeniecli/opsgeniecli.py
 opsgeniecli/opsgeniecliexceptions.py
 opsgeniecli/requirements.txt
 opsgeniecli.egg-info/PKG-INFO
 opsgeniecli.egg-info/SOURCES.txt
 opsgeniecli.egg-info/dependency_links.txt
-opsgeniecli.egg-info/entry_points.txt
 opsgeniecli.egg-info/not-zip-safe
 opsgeniecli.egg-info/requires.txt
 opsgeniecli.egg-info/top_level.txt
 opsgeniecli/conf/logging.json-example
 tests/test_opsgeniecli.py
```

### Comparing `opsgeniecli-0.1.8/setup.py` & `opsgeniecli-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     license='MIT',
     zip_safe=False,
     keywords='''opsgeniecli ''',
     entry_points = {
                    'console_scripts': [
                        # enable this to automatically generate a script in /usr/local/bin called myscript that points to your
                        #  opsgeniecli.opsgeniecli:main method
-                       'opsgeniecli = opsgeniecli.opsgeniecli:main'
+                       # 'myscript = opsgeniecli.opsgeniecli:main'
                    ]},
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.7',
```

### Comparing `opsgeniecli-0.1.8/tests/test_opsgeniecli.py` & `opsgeniecli-0.1.9/tests/test_opsgeniecli.py`

 * *Files identical despite different names*

