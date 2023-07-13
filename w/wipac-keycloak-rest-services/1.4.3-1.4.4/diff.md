# Comparing `tmp/wipac-keycloak-rest-services-1.4.3.tar.gz` & `tmp/wipac-keycloak-rest-services-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-keycloak-rest-services-1.4.3.tar", last modified: Wed Jul 12 19:11:10 2023, max compression
+gzip compressed data, was "wipac-keycloak-rest-services-1.4.4.tar", last modified: Thu Jul 13 16:17:42 2023, max compression
```

## Comparing `wipac-keycloak-rest-services-1.4.3.tar` & `wipac-keycloak-rest-services-1.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:11:10.210116 wipac-keycloak-rest-services-1.4.3/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4044 2023-07-12 19:11:10.210116 wipac-keycloak-rest-services-1.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:11:10.210116 wipac-keycloak-rest-services-1.4.3/krs/
--rw-r--r--   0 root         (0) root         (0)      513 2023-07-12 19:11:08.000000 wipac-keycloak-rest-services-1.4.3/krs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20266 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/apps.py
--rw-r--r--   0 root         (0) root         (0)    15733 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/email.py
--rw-r--r--   0 root         (0) root         (0)    10971 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/groups.py
--rw-r--r--   0 root         (0) root         (0)     8766 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/institutions.py
--rw-r--r--   0 root         (0) root         (0)    22784 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/ldap.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/py.typed
--rw-r--r--   0 root         (0) root         (0)     5722 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/token.py
--rw-r--r--   0 root         (0) root         (0)     9213 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/krs/users.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-07-12 19:11:10.210116 wipac-keycloak-rest-services-1.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-12 19:11:07.000000 wipac-keycloak-rest-services-1.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:11:10.210116 wipac-keycloak-rest-services-1.4.3/wipac_keycloak_rest_services.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4044 2023-07-12 19:11:10.000000 wipac-keycloak-rest-services-1.4.3/wipac_keycloak_rest_services.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-12 19:11:10.000000 wipac-keycloak-rest-services-1.4.3/wipac_keycloak_rest_services.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:11:10.000000 wipac-keycloak-rest-services-1.4.3/wipac_keycloak_rest_services.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      200 2023-07-12 19:11:10.000000 wipac-keycloak-rest-services-1.4.3/wipac_keycloak_rest_services.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-12 19:11:10.000000 wipac-keycloak-rest-services-1.4.3/wipac_keycloak_rest_services.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:17:42.708353 wipac-keycloak-rest-services-1.4.4/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-07-13 16:17:42.708353 wipac-keycloak-rest-services-1.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:17:42.704352 wipac-keycloak-rest-services-1.4.4/krs/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20266 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/apps.py
+-rw-r--r--   0 root         (0) root         (0)    15733 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/email.py
+-rw-r--r--   0 root         (0) root         (0)    10971 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/groups.py
+-rw-r--r--   0 root         (0) root         (0)     8766 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/institutions.py
+-rw-r--r--   0 root         (0) root         (0)    22784 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/ldap.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/token.py
+-rw-r--r--   0 root         (0) root         (0)     9213 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/krs/users.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-07-13 16:17:42.708353 wipac-keycloak-rest-services-1.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-13 16:17:39.000000 wipac-keycloak-rest-services-1.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:17:42.708353 wipac-keycloak-rest-services-1.4.4/wipac_keycloak_rest_services.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-07-13 16:17:42.000000 wipac-keycloak-rest-services-1.4.4/wipac_keycloak_rest_services.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-13 16:17:42.000000 wipac-keycloak-rest-services-1.4.4/wipac_keycloak_rest_services.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 16:17:42.000000 wipac-keycloak-rest-services-1.4.4/wipac_keycloak_rest_services.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-13 16:17:42.000000 wipac-keycloak-rest-services-1.4.4/wipac_keycloak_rest_services.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-13 16:17:42.000000 wipac-keycloak-rest-services-1.4.4/wipac_keycloak_rest_services.egg-info/top_level.txt
```

### Comparing `wipac-keycloak-rest-services-1.4.3/LICENSE` & `wipac-keycloak-rest-services-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/PKG-INFO` & `wipac-keycloak-rest-services-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.4.3
+Version: 1.4.4
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_pflghnqn_/tmp5zlt6rsa_TarContainer/0/2", line 93, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_pflghnqn_/tmp5zlt6rsa_TarContainer/0/2", line 93, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.3
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.4
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

### Comparing `wipac-keycloak-rest-services-1.4.3/README.md` & `wipac-keycloak-rest-services-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/__init__.py` & `wipac-keycloak-rest-services-1.4.4/krs/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.4.3"
+__version__ = "1.4.4"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/apps.py` & `wipac-keycloak-rest-services-1.4.4/krs/apps.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/bootstrap.py` & `wipac-keycloak-rest-services-1.4.4/krs/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/email.py` & `wipac-keycloak-rest-services-1.4.4/krs/email.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/groups.py` & `wipac-keycloak-rest-services-1.4.4/krs/groups.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/institutions.py` & `wipac-keycloak-rest-services-1.4.4/krs/institutions.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/ldap.py` & `wipac-keycloak-rest-services-1.4.4/krs/ldap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/rabbitmq.py` & `wipac-keycloak-rest-services-1.4.4/krs/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/token.py` & `wipac-keycloak-rest-services-1.4.4/krs/token.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/krs/users.py` & `wipac-keycloak-rest-services-1.4.4/krs/users.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/setup.cfg` & `wipac-keycloak-rest-services-1.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.3/wipac_keycloak_rest_services.egg-info/PKG-INFO` & `wipac-keycloak-rest-services-1.4.4/wipac_keycloak_rest_services.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.4.3
+Version: 1.4.4
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_pflghnqn_/tmp5zlt6rsa_TarContainer/0/19", line 93, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_pflghnqn_/tmp5zlt6rsa_TarContainer/0/19", line 93, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.3
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.4
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

