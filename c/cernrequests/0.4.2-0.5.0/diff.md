# Comparing `tmp/cernrequests-0.4.2.tar.gz` & `tmp/cernrequests-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cernrequests-0.4.2.tar", last modified: Wed Jul  5 10:27:28 2023, max compression
+gzip compressed data, was "cernrequests-0.5.0.tar", last modified: Thu Jul 13 15:01:50 2023, max compression
```

## Comparing `cernrequests-0.4.2.tar` & `cernrequests-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-05 10:27:28.063117 cernrequests-0.4.2/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     7651 2023-05-23 15:59:26.000000 cernrequests-0.4.2/LICENSE
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6994 2023-07-05 10:27:28.063117 cernrequests-0.4.2/PKG-INFO
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6618 2023-07-04 14:11:37.000000 cernrequests-0.4.2/README.md
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-05 10:27:28.059117 cernrequests-0.4.2/cernrequests/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      558 2023-07-04 15:19:33.000000 cernrequests-0.4.2/cernrequests/__init__.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    14605 2023-06-30 14:11:06.000000 cernrequests-0.4.2/cernrequests/cern-cacert.pem
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2718 2023-06-30 14:11:19.000000 cernrequests-0.4.2/cernrequests/certs.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2479 2023-07-04 14:06:53.000000 cernrequests-0.4.2/cernrequests/cookies.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2327 2023-07-04 14:18:04.000000 cernrequests-0.4.2/cernrequests/core.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1475 2023-07-04 10:48:19.000000 cernrequests-0.4.2/cernrequests/token.py
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-05 10:27:28.063117 cernrequests-0.4.2/cernrequests.egg-info/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6994 2023-07-05 10:27:28.000000 cernrequests-0.4.2/cernrequests.egg-info/PKG-INFO
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      399 2023-07-05 10:27:28.000000 cernrequests-0.4.2/cernrequests.egg-info/SOURCES.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2023-07-05 10:27:28.000000 cernrequests-0.4.2/cernrequests.egg-info/dependency_links.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       36 2023-07-05 10:27:28.000000 cernrequests-0.4.2/cernrequests.egg-info/requires.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       13 2023-07-05 10:27:28.000000 cernrequests-0.4.2/cernrequests.egg-info/top_level.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2023-07-05 10:27:28.063117 cernrequests-0.4.2/setup.cfg
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1842 2023-07-05 10:27:21.000000 cernrequests-0.4.2/setup.py
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-05 10:27:28.063117 cernrequests-0.4.2/tests/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1335 2023-06-30 14:14:27.000000 cernrequests-0.4.2/tests/test_cernrequests.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1531 2023-07-04 10:48:19.000000 cernrequests-0.4.2/tests/test_real_data.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-13 15:01:50.496666 cernrequests-0.5.0/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     7651 2023-05-23 15:59:26.000000 cernrequests-0.5.0/LICENSE
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     8537 2023-07-13 15:01:50.492666 cernrequests-0.5.0/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     8161 2023-07-13 15:01:30.000000 cernrequests-0.5.0/README.md
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-13 15:01:50.492666 cernrequests-0.5.0/cernrequests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      558 2023-07-13 13:59:14.000000 cernrequests-0.5.0/cernrequests/__init__.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    14605 2023-06-30 14:11:06.000000 cernrequests-0.5.0/cernrequests/cern-cacert.pem
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2718 2023-06-30 14:11:19.000000 cernrequests-0.5.0/cernrequests/certs.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2479 2023-07-04 14:06:53.000000 cernrequests-0.5.0/cernrequests/cookies.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2347 2023-07-10 12:48:33.000000 cernrequests-0.5.0/cernrequests/core.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1464 2023-07-13 13:16:58.000000 cernrequests-0.5.0/cernrequests/token.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-13 15:01:50.492666 cernrequests-0.5.0/cernrequests.egg-info/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     8537 2023-07-13 15:01:50.000000 cernrequests-0.5.0/cernrequests.egg-info/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      399 2023-07-13 15:01:50.000000 cernrequests-0.5.0/cernrequests.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2023-07-13 15:01:50.000000 cernrequests-0.5.0/cernrequests.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       36 2023-07-13 15:01:50.000000 cernrequests-0.5.0/cernrequests.egg-info/requires.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       13 2023-07-13 15:01:50.000000 cernrequests-0.5.0/cernrequests.egg-info/top_level.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2023-07-13 15:01:50.496666 cernrequests-0.5.0/setup.cfg
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1690 2023-07-05 10:30:36.000000 cernrequests-0.5.0/setup.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-13 15:01:50.492666 cernrequests-0.5.0/tests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1336 2023-07-13 13:16:24.000000 cernrequests-0.5.0/tests/test_cernrequests.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2282 2023-07-13 13:21:15.000000 cernrequests-0.5.0/tests/test_real_data.py
```

### Comparing `cernrequests-0.4.2/LICENSE` & `cernrequests-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.2/PKG-INFO` & `cernrequests-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-Metadata-Version: 2.1
-Name: cernrequests
-Version: 0.4.2
-Home-page: https://github.com/CMSTrackerDPG/cernrequests
-Author: Peter Stein
-Author-email: peter.stein@cern.ch
-Maintainer: CMS DQM team
-Maintainer-email: cms-dqm-coreTeam@cern.ch
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://travis-ci.com/CMSTrackerDPG/cernrequests.svg?branch=master)](https://travis-ci.com/CMSTrackerDPG/cernrequests)
+![Functional tests](https://github.com/CMSTrackerDPG/cernrequests/actions/workflows/test_package.yaml/badge.svg)
 [![](https://img.shields.io/pypi/v/cernrequests.svg)](https://pypi.org/project/cernrequests/)
 
 
 # CERN Requests
 
 
 Enables using [`requests`]("https://github.com/requests/requests") without having to configure the CERN Root certificates or getting an API access token manually.
 
 Inspired by [`certifi`](https://github.com/certifi/python-certifi), [`requests-kerberos`](https://github.com/requests/requests-kerberos), [`cern-sso-python`](https://github.com/cerndb/cern-sso-python) and [`api-access-examples`](https://gitlab.cern.ch/authzsvc/docs/api-access-examples/-/tree/master/python).
 
 The Root certificate bundle is copied from the [linuxsoft cern page](http://linuxsoft.cern.ch/cern/centos/7/cern/x86_64/repoview/CERN-CA-certs.html) and can also be created manually by downloading the CERN Grid Certification Authority files from [cafiles.cern.ch/cafiles](https://cafiles.cern.ch/cafiles/).
 
 ## Installation
 
-Requires ```Python 2.7``` or ```Python 3.4+```
+> **Warning**
+> We are no longer supporting Python 2.7.
+
+Requires Python 3.6+.
 
 ```bash
 pip install cernrequests
 ```
 
 ## Prerequisites
 
@@ -110,17 +101,25 @@
 ```
 > **Note**
 > The `target_audience` depends on the SSO registration name of the _target_ application. E.g.
 > if you want to access the development instance of Run Registry, `target_audience` should be 
 > `dev-cmsrunregistry-sso-proxy`. 
 > In case of doubt, communicate with the app's developers directly. 
 
+The `get_with_token` method also accepts an `api_token` argument, in case you want to reuse an already issued and non-expired one that you got from [`get_api_token`](#get_api_token).
+
 ##### `get_api_token`
 
 This is a method that needs a `target_application` parameter and will try and get an API token, using the `SSO_CLIENT_ID` and `SSO_CLIENT_SECRET` provided as environment variables. 
+
+A `tuple` is returned: `api_token` (`str`) and the `expiration_datetime` (`datetime`).
+
+> **Note**
+> The `expiration_datetime` is not used internally, so it's returned
+> to the user, if they need to check when the token expires. 
 #### Alternative usage
 
 If you want to use ```requests``` directly without the CERN wrapper you can get the exact same functionality by doing:
 
 ```python
 import requests
 from cernrequests import certs
@@ -161,21 +160,43 @@
 cernrequests.get(url, cert=(cert,key))
 ```
 
 This way you can even use custom names such as ```cert.pem``` and ```key.pem```
 
 ## Testing
 
+### Locally
+
 ```bash
 python -m venv venv
 source venv/bin/activate
+pip install -e .
 pip install -r testing-requirements.txt
 pytest
 ```
 
+### GitHub actions
+
+To run the tests on GitHub, we have uploaded a set of `userkey.pem` and `usercert.pem` files, encrypted with GPG. Those are decrypted, using a secret and then used normally. 
+
+See [`the yaml file`](.github/workflows/test_package.yaml) for more details.
+
+> **Note**
+> If the actions are failing, make sure that the Grid Certificates are still valid. You may need to recreate them. For instructions, see [here](https://web.archive.org/web/20230713134837/https://docs.github.com/en/actions/security-guides/encrypted-secrets#storing-large-secrets). Create new grid certificates, encrypt them with a password and replace `tests/usercert.pem.gpg` and `tests/userkey.pem.gpg`. You will also need to update the `GPG_ENC_PASSWORD` secret with the password you used to encrypt them.
+
+## [Package developers] Updating the package on PyPI
+
+```bash
+python3 -m pip install --upgrade pip build twine
+python3 -m build
+python3 -m twine upload --skip-existing --repository pypi dist/*
+```
+Instructions from [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
+
+
 ## FAQ
 
 ### I'm getting `certificate verify failed`! What should I do?
 
 The `cernrequests/cern-cacerts.pem` file has expired, and will need to be updated by the library maintainer. 
 
 1. ```bash
@@ -198,8 +219,8 @@
 
 - http://docs.python-requests.org/en/master/
 - https://certifi.io/en/latest/
 - https://github.com/cerndb/cern-sso-python
 - https://linux.web.cern.ch/linux/docs/cernssocookie.shtml
 - http://linuxsoft.cern.ch/cern/centos/7/cern/x86_64/repoview/CERN-CA-certs.html
 - https://ca.cern.ch/ca/
-- https://auth.docs.cern.ch
+- https://auth.docs.cern.ch
```

### Comparing `cernrequests-0.4.2/README.md` & `cernrequests-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,38 @@
-[![Build Status](https://travis-ci.com/CMSTrackerDPG/cernrequests.svg?branch=master)](https://travis-ci.com/CMSTrackerDPG/cernrequests)
+Metadata-Version: 2.1
+Name: cernrequests
+Version: 0.5.0
+Home-page: https://github.com/CMSTrackerDPG/cernrequests
+Author: Peter Stein
+Author-email: peter.stein@cern.ch
+Maintainer: CMS DQM team
+Maintainer-email: cms-dqm-coreTeam@cern.ch
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Functional tests](https://github.com/CMSTrackerDPG/cernrequests/actions/workflows/test_package.yaml/badge.svg)
 [![](https://img.shields.io/pypi/v/cernrequests.svg)](https://pypi.org/project/cernrequests/)
 
 
 # CERN Requests
 
 
 Enables using [`requests`]("https://github.com/requests/requests") without having to configure the CERN Root certificates or getting an API access token manually.
 
 Inspired by [`certifi`](https://github.com/certifi/python-certifi), [`requests-kerberos`](https://github.com/requests/requests-kerberos), [`cern-sso-python`](https://github.com/cerndb/cern-sso-python) and [`api-access-examples`](https://gitlab.cern.ch/authzsvc/docs/api-access-examples/-/tree/master/python).
 
 The Root certificate bundle is copied from the [linuxsoft cern page](http://linuxsoft.cern.ch/cern/centos/7/cern/x86_64/repoview/CERN-CA-certs.html) and can also be created manually by downloading the CERN Grid Certification Authority files from [cafiles.cern.ch/cafiles](https://cafiles.cern.ch/cafiles/).
 
 ## Installation
 
-Requires ```Python 2.7``` or ```Python 3.4+```
+> **Warning**
+> We are no longer supporting Python 2.7.
+
+Requires Python 3.6+.
 
 ```bash
 pip install cernrequests
 ```
 
 ## Prerequisites
 
@@ -98,17 +113,25 @@
 ```
 > **Note**
 > The `target_audience` depends on the SSO registration name of the _target_ application. E.g.
 > if you want to access the development instance of Run Registry, `target_audience` should be 
 > `dev-cmsrunregistry-sso-proxy`. 
 > In case of doubt, communicate with the app's developers directly. 
 
+The `get_with_token` method also accepts an `api_token` argument, in case you want to reuse an already issued and non-expired one that you got from [`get_api_token`](#get_api_token).
+
 ##### `get_api_token`
 
 This is a method that needs a `target_application` parameter and will try and get an API token, using the `SSO_CLIENT_ID` and `SSO_CLIENT_SECRET` provided as environment variables. 
+
+A `tuple` is returned: `api_token` (`str`) and the `expiration_datetime` (`datetime`).
+
+> **Note**
+> The `expiration_datetime` is not used internally, so it's returned
+> to the user, if they need to check when the token expires. 
 #### Alternative usage
 
 If you want to use ```requests``` directly without the CERN wrapper you can get the exact same functionality by doing:
 
 ```python
 import requests
 from cernrequests import certs
@@ -149,21 +172,43 @@
 cernrequests.get(url, cert=(cert,key))
 ```
 
 This way you can even use custom names such as ```cert.pem``` and ```key.pem```
 
 ## Testing
 
+### Locally
+
 ```bash
 python -m venv venv
 source venv/bin/activate
+pip install -e .
 pip install -r testing-requirements.txt
 pytest
 ```
 
+### GitHub actions
+
+To run the tests on GitHub, we have uploaded a set of `userkey.pem` and `usercert.pem` files, encrypted with GPG. Those are decrypted, using a secret and then used normally. 
+
+See [`the yaml file`](.github/workflows/test_package.yaml) for more details.
+
+> **Note**
+> If the actions are failing, make sure that the Grid Certificates are still valid. You may need to recreate them. For instructions, see [here](https://web.archive.org/web/20230713134837/https://docs.github.com/en/actions/security-guides/encrypted-secrets#storing-large-secrets). Create new grid certificates, encrypt them with a password and replace `tests/usercert.pem.gpg` and `tests/userkey.pem.gpg`. You will also need to update the `GPG_ENC_PASSWORD` secret with the password you used to encrypt them.
+
+## [Package developers] Updating the package on PyPI
+
+```bash
+python3 -m pip install --upgrade pip build twine
+python3 -m build
+python3 -m twine upload --skip-existing --repository pypi dist/*
+```
+Instructions from [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
+
+
 ## FAQ
 
 ### I'm getting `certificate verify failed`! What should I do?
 
 The `cernrequests/cern-cacerts.pem` file has expired, and will need to be updated by the library maintainer. 
 
 1. ```bash
@@ -186,8 +231,8 @@
 
 - http://docs.python-requests.org/en/master/
 - https://certifi.io/en/latest/
 - https://github.com/cerndb/cern-sso-python
 - https://linux.web.cern.ch/linux/docs/cernssocookie.shtml
 - http://linuxsoft.cern.ch/cern/centos/7/cern/x86_64/repoview/CERN-CA-certs.html
 - https://ca.cern.ch/ca/
-- https://auth.docs.cern.ch
+- https://auth.docs.cern.ch
```

### Comparing `cernrequests-0.4.2/cernrequests/__init__.py` & `cernrequests-0.5.0/cernrequests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
-# © Copyright 2018 CERN
+# © Copyright 2023 CERN
 #
 # This software is distributed under the terms of the GNU Lesser General Public
 # Licence version 3 (LGPL Version 3), copied verbatim in the file “LICENSE”
 #
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 
 from .core import get, get_with_token
 from .token import get_api_token
 from .cookies import get_sso_cookies
```

### Comparing `cernrequests-0.4.2/cernrequests/cern-cacert.pem` & `cernrequests-0.5.0/cernrequests/cern-cacert.pem`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.2/cernrequests/certs.py` & `cernrequests-0.5.0/cernrequests/certs.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.2/cernrequests/cookies.py` & `cernrequests-0.5.0/cernrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.2/cernrequests/core.py` & `cernrequests-0.5.0/cernrequests/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     is behind CERN SSO. It's working with the ""new"" (2023/06) SSO.
 
     Accepts two arguments:
     - target_application (str): The name of the target application
         You want the token for. This is the name that the target application
         has used to register in the CERN SSO Application. Contact the
         target application's developers
-    - api_token (str): If provided, it's used to
+    - api_token (str): If not provided, a new one will be requested.
     """
     if "target_application" not in kwargs:
         raise Exception("You must specify the target_application")
     target_application = kwargs.pop("target_application")
     client_id = os.environ.get("SSO_CLIENT_ID")
     client_secret = os.environ.get("SSO_CLIENT_SECRET")
     if "api_token" in kwargs:
```

### Comparing `cernrequests-0.4.2/cernrequests/token.py` & `cernrequests-0.5.0/cernrequests/token.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 API Token getter, based on
 https://gitlab.cern.ch/authzsvc/docs/api-access-examples/-/blob/master/python/api_token.py
 """
 
 import logging
 import datetime
 import requests
-import jwt
 
 DEFAULT_SERVER = "auth.cern.ch"
 DEFAULT_REALM = "cern"
 DEFAULT_REALM_PREFIX = "auth/realms/{}"
 DEFAULT_TOKEN_ENDPOINT = "api-access/token"
```

### Comparing `cernrequests-0.4.2/cernrequests.egg-info/PKG-INFO` & `cernrequests-0.5.0/cernrequests.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: cernrequests
-Version: 0.4.2
+Version: 0.5.0
 Home-page: https://github.com/CMSTrackerDPG/cernrequests
 Author: Peter Stein
 Author-email: peter.stein@cern.ch
 Maintainer: CMS DQM team
 Maintainer-email: cms-dqm-coreTeam@cern.ch
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://travis-ci.com/CMSTrackerDPG/cernrequests.svg?branch=master)](https://travis-ci.com/CMSTrackerDPG/cernrequests)
+![Functional tests](https://github.com/CMSTrackerDPG/cernrequests/actions/workflows/test_package.yaml/badge.svg)
 [![](https://img.shields.io/pypi/v/cernrequests.svg)](https://pypi.org/project/cernrequests/)
 
 
 # CERN Requests
 
 
 Enables using [`requests`]("https://github.com/requests/requests") without having to configure the CERN Root certificates or getting an API access token manually.
 
 Inspired by [`certifi`](https://github.com/certifi/python-certifi), [`requests-kerberos`](https://github.com/requests/requests-kerberos), [`cern-sso-python`](https://github.com/cerndb/cern-sso-python) and [`api-access-examples`](https://gitlab.cern.ch/authzsvc/docs/api-access-examples/-/tree/master/python).
 
 The Root certificate bundle is copied from the [linuxsoft cern page](http://linuxsoft.cern.ch/cern/centos/7/cern/x86_64/repoview/CERN-CA-certs.html) and can also be created manually by downloading the CERN Grid Certification Authority files from [cafiles.cern.ch/cafiles](https://cafiles.cern.ch/cafiles/).
 
 ## Installation
 
-Requires ```Python 2.7``` or ```Python 3.4+```
+> **Warning**
+> We are no longer supporting Python 2.7.
+
+Requires Python 3.6+.
 
 ```bash
 pip install cernrequests
 ```
 
 ## Prerequisites
 
@@ -110,17 +113,25 @@
 ```
 > **Note**
 > The `target_audience` depends on the SSO registration name of the _target_ application. E.g.
 > if you want to access the development instance of Run Registry, `target_audience` should be 
 > `dev-cmsrunregistry-sso-proxy`. 
 > In case of doubt, communicate with the app's developers directly. 
 
+The `get_with_token` method also accepts an `api_token` argument, in case you want to reuse an already issued and non-expired one that you got from [`get_api_token`](#get_api_token).
+
 ##### `get_api_token`
 
 This is a method that needs a `target_application` parameter and will try and get an API token, using the `SSO_CLIENT_ID` and `SSO_CLIENT_SECRET` provided as environment variables. 
+
+A `tuple` is returned: `api_token` (`str`) and the `expiration_datetime` (`datetime`).
+
+> **Note**
+> The `expiration_datetime` is not used internally, so it's returned
+> to the user, if they need to check when the token expires. 
 #### Alternative usage
 
 If you want to use ```requests``` directly without the CERN wrapper you can get the exact same functionality by doing:
 
 ```python
 import requests
 from cernrequests import certs
@@ -161,21 +172,43 @@
 cernrequests.get(url, cert=(cert,key))
 ```
 
 This way you can even use custom names such as ```cert.pem``` and ```key.pem```
 
 ## Testing
 
+### Locally
+
 ```bash
 python -m venv venv
 source venv/bin/activate
+pip install -e .
 pip install -r testing-requirements.txt
 pytest
 ```
 
+### GitHub actions
+
+To run the tests on GitHub, we have uploaded a set of `userkey.pem` and `usercert.pem` files, encrypted with GPG. Those are decrypted, using a secret and then used normally. 
+
+See [`the yaml file`](.github/workflows/test_package.yaml) for more details.
+
+> **Note**
+> If the actions are failing, make sure that the Grid Certificates are still valid. You may need to recreate them. For instructions, see [here](https://web.archive.org/web/20230713134837/https://docs.github.com/en/actions/security-guides/encrypted-secrets#storing-large-secrets). Create new grid certificates, encrypt them with a password and replace `tests/usercert.pem.gpg` and `tests/userkey.pem.gpg`. You will also need to update the `GPG_ENC_PASSWORD` secret with the password you used to encrypt them.
+
+## [Package developers] Updating the package on PyPI
+
+```bash
+python3 -m pip install --upgrade pip build twine
+python3 -m build
+python3 -m twine upload --skip-existing --repository pypi dist/*
+```
+Instructions from [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
+
+
 ## FAQ
 
 ### I'm getting `certificate verify failed`! What should I do?
 
 The `cernrequests/cern-cacerts.pem` file has expired, and will need to be updated by the library maintainer. 
 
 1. ```bash
```

### Comparing `cernrequests-0.4.2/setup.py` & `cernrequests-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,14 @@
     version_file = read(*file_paths)
     version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
     if version_match:
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
 
 
-from os import listdir
-from os.path import isfile, join
-
-onlyfiles = [f for f in listdir(here) if isfile(join(here, f))]
-
-print("!!!!!!!!!", onlyfiles)
 with open(os.path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="cernrequests",
     version=find_version("cernrequests", "__init__.py"),
     long_description=long_description,
```

### Comparing `cernrequests-0.4.2/tests/test_cernrequests.py` & `cernrequests-0.5.0/tests/test_cernrequests.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # This software is distributed under the terms of the GNU Lesser General Public
 # Licence version 3 (LGPL Version 3), copied verbatim in the file “LICENSE”
 #
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
+
 import json
 import pytest
 import cernrequests
 from cernrequests.certs import where, default_user_certificate_paths
 
 
 def test_cernrequests():
```

### Comparing `cernrequests-0.4.2/tests/test_real_data.py` & `cernrequests-0.5.0/tests/test_real_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,46 +8,71 @@
 #
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
 import os
 import json
-import requests
-
+from datetime import datetime
 import cernrequests
-from cernrequests import certs
-from cernrequests.cookies import get_sso_cookies
-from cernrequests.core import get, get_with_token
+
+RR_URL = "https://cmsrunregistry-qa.web.cern.ch/api/get_all_dataset_names_of_run/357756"
 
 
-def test_dqmgui():
+def test_get_with_certs():
     """
-    The DQM GUI does not require cookies, but does require Grid User Certificates
+    The DQM GUI does not require token authentication, but does require Grid User Certificates
     :return:
     """
     url = "https://cmsweb.cern.ch/dqm/offline/jsonfairy/archive/321012/StreamExpress/Run2018D-Express-v1/DQMIO/"
     expected = json.loads('{"hist": "unsupported type"}')
 
     assert expected == cernrequests.get(url).json()
 
 
-def test_rr():
+def test_get_with_token():
+    """
+    Test to check that not having a token at hand and using get_with_token
+    works.
+
+    RunRegistry requires token authentication.
+    """
+
+    # TODO: Update this URL when new SSO is deployed for production RR
+
+    response = cernrequests.get_with_token(
+        RR_URL, target_application="cmsrunregistry-sso-proxy"
+    ).json()
+    expected = [
+        "/Express/Collisions2022/DQM",
+        "/Express/Commissioning2022/DQM",
+        "online",
+        "/PromptReco/Collisions2022/DQM",
+    ]
+
+    assert expected == response
+
+
+def test_get_api_token_and_get_with_token():
     """
-    RunRegistry requires cookies
+    Test that gets a token and then uses it, to verify its reusability.
     """
 
-    url = (
-        "https://dev-cmsrunregistry.web.cern.ch/api/get_all_dataset_names_of_run/357756"
+    token, expires = cernrequests.get_api_token(
+        client_id=os.environ.get("SSO_CLIENT_ID"),
+        client_secret=os.environ.get("SSO_CLIENT_SECRET"),
+        target_application="cmsrunregistry-sso-proxy",
     )
-    response = get_with_token(
-        url, target_application="dev-cmsrunregistry-sso-proxy"
+    assert token
+    assert expires > datetime.now()
+
+    response = cernrequests.get_with_token(
+        url=RR_URL, target_application="cmsrunregistry-sso-proxy", api_token=token
     ).json()
     expected = [
-        # TODO: Uncomment this when new SSO is deployed for production RR
-        # "/Express/Collisions2022/DQM",
-        # "/Express/Commissioning2022/DQM",
+        "/Express/Collisions2022/DQM",
+        "/Express/Commissioning2022/DQM",
         "online",
-        # "/PromptReco/Collisions2022/DQM",
+        "/PromptReco/Collisions2022/DQM",
     ]
 
     assert expected == response
```

