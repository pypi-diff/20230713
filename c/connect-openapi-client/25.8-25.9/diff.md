# Comparing `tmp/connect-openapi-client-25.8.tar.gz` & `tmp/connect-openapi-client-25.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect-openapi-client-25.8.tar", max compression
+gzip compressed data, was "connect-openapi-client-25.9.tar", max compression
```

## Comparing `connect-openapi-client-25.8.tar` & `connect-openapi-client-25.9.tar`

### file list

```diff
@@ -1,29 +1,36 @@
--rw-r--r--   0        0        0    11357 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/LICENSE
--rw-r--r--   0        0        0     1869 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/README.md
--rw-r--r--   0        0        0      298 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/cnct/__init__.py
--rw-r--r--   0        0        0      183 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/cnct/rql.py
--rw-r--r--   0        0        0      373 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/__init__.py
--rw-r--r--   0        0        0      310 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/constants.py
--rw-r--r--   0        0        0        0 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/contrib/__init__.py
--rw-r--r--   0        0        0      242 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/contrib/locust/__init__.py
--rw-r--r--   0        0        0     1641 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/contrib/locust/user.py
--rw-r--r--   0        0        0     1100 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/exceptions.py
--rw-r--r--   0        0        0     6212 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/fluent.py
--rw-r--r--   0        0        0     6907 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/help_formatter.py
--rw-r--r--   0        0        0     1655 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/logger.py
--rw-r--r--   0        0        0     6040 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/mixins.py
--rw-r--r--   0        0        0      471 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/models/__init__.py
--rw-r--r--   0        0        0    12633 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/models/base.py
--rw-r--r--   0        0        0      191 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/models/exceptions.py
--rw-r--r--   0        0        0     5175 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/models/iterators.py
--rw-r--r--   0        0        0    13052 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/models/mixins.py
--rw-r--r--   0        0        0    14635 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/models/resourceset.py
--rw-r--r--   0        0        0     6410 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/openapi.py
--rw-r--r--   0        0        0      189 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/rql/__init__.py
--rw-r--r--   0        0        0     8124 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/rql/base.py
--rw-r--r--   0        0        0     1992 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/rql/utils.py
--rw-r--r--   0        0        0     1246 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/utils.py
--rw-r--r--   0        0        0      386 2022-08-10 15:52:45.948430 connect-openapi-client-25.8/connect/client/version.py
--rw-r--r--   0        0        0     2466 2022-08-10 15:54:42.314667 connect-openapi-client-25.8/pyproject.toml
--rw-r--r--   0        0        0     2780 2022-08-10 15:54:43.263842 connect-openapi-client-25.8/setup.py
--rw-r--r--   0        0        0     3152 2022-08-10 15:54:43.264274 connect-openapi-client-25.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/LICENSE
+-rw-r--r--   0        0        0     1869 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/README.md
+-rw-r--r--   0        0        0      298 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/cnct/__init__.py
+-rw-r--r--   0        0        0      183 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/cnct/rql.py
+-rw-r--r--   0        0        0      373 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/__init__.py
+-rw-r--r--   0        0        0      310 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/constants.py
+-rw-r--r--   0        0        0        0 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/contrib/__init__.py
+-rw-r--r--   0        0        0      242 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/contrib/locust/__init__.py
+-rw-r--r--   0        0        0     1641 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/contrib/locust/user.py
+-rw-r--r--   0        0        0     1100 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/exceptions.py
+-rw-r--r--   0        0        0     6723 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/fluent.py
+-rw-r--r--   0        0        0     6907 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/help_formatter.py
+-rw-r--r--   0        0        0     1655 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/logger.py
+-rw-r--r--   0        0        0     6040 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/mixins.py
+-rw-r--r--   0        0        0      471 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/__init__.py
+-rw-r--r--   0        0        0    12633 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/base.py
+-rw-r--r--   0        0        0      191 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/exceptions.py
+-rw-r--r--   0        0        0     5175 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/iterators.py
+-rw-r--r--   0        0        0    13052 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/mixins.py
+-rw-r--r--   0        0        0    14635 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/models/resourceset.py
+-rw-r--r--   0        0        0     6410 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/openapi.py
+-rw-r--r--   0        0        0      189 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/rql/__init__.py
+-rw-r--r--   0        0        0     8124 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/rql/base.py
+-rw-r--r--   0        0        0     1992 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/rql/utils.py
+-rw-r--r--   0        0        0      239 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/testing/__init__.py
+-rw-r--r--   0        0        0      825 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/testing/fixtures.py
+-rw-r--r--   0        0        0     4043 2022-09-22 13:23:17.484889 connect-openapi-client-25.9/connect/client/testing/fluent.py
+-rw-r--r--   0        0        0      268 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/testing/models/__init__.py
+-rw-r--r--   0        0        0     1051 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/testing/models/base.py
+-rw-r--r--   0        0        0     3751 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/testing/models/mixins.py
+-rw-r--r--   0        0        0     5084 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/testing/models/resourceset.py
+-rw-r--r--   0        0        0     1246 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/utils.py
+-rw-r--r--   0        0        0      401 2022-09-22 13:23:17.488887 connect-openapi-client-25.9/connect/client/version.py
+-rw-r--r--   0        0        0     2499 2022-09-22 13:24:58.460051 connect-openapi-client-25.9/pyproject.toml
+-rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 connect-openapi-client-25.9/setup.py
+-rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 connect-openapi-client-25.9/PKG-INFO
```

### Comparing `connect-openapi-client-25.8/LICENSE` & `connect-openapi-client-25.9/LICENSE`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/README.md` & `connect-openapi-client-25.9/README.md`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/contrib/locust/user.py` & `connect-openapi-client-25.9/connect/client/contrib/locust/user.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/exceptions.py` & `connect-openapi-client-25.9/connect/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/fluent.py` & `connect-openapi-client-25.9/connect/client/fluent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #
 # This file is part of the Ingram Micro CloudBlue Connect Python OpenAPI Client.
 #
 # Copyright (c) 2021 Ingram Micro. All Rights Reserved.
 #
+import contextvars
 import threading
 from json.decoder import JSONDecodeError
 
 from connect.client.constants import CONNECT_ENDPOINT_URL, CONNECT_SPECS_URL
 from connect.client.mixins import AsyncClientMixin, SyncClientMixin
 from connect.client.models import AsyncCollection, AsyncNS, Collection, NS
 from connect.client.utils import get_headers
@@ -70,20 +71,28 @@
         self.max_retries = max_retries
         self._use_specs = use_specs
         self._validate_using_specs = validate_using_specs
         self.specs_location = specs_location or CONNECT_SPECS_URL
         self.specs = None
         if self._use_specs:
             self.specs = OpenAPISpecs(self.specs_location)
-        self.response = None
+        self._response = None
         self.logger = logger
         self._help_formatter = DefaultFormatter(self.specs)
         self.timeout = timeout
         self.resourceset_append = resourceset_append
 
+    @property
+    def response(self):
+        return self._response
+
+    @response.setter
+    def response(self, value):
+        self._response = value
+
     def __getattr__(self, name):
         """
         Returns a collection object called ``name``.
 
         :param name: The name of the collection to retrieve.
         :type name: str
         :return: a collection called ``name``.
@@ -165,21 +174,34 @@
                 error = self.response.json()
                 if 'error_code' in error and 'errors' in error:
                     return error
             except JSONDecodeError:
                 pass
 
 
-class ConnectClient(_ConnectClientBase, SyncClientMixin):
+class ConnectClient(_ConnectClientBase, threading.local, SyncClientMixin):
     def _get_collection_class(self):
         return Collection
 
     def _get_namespace_class(self):
         return NS
 
 
 class AsyncConnectClient(_ConnectClientBase, AsyncClientMixin):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._response = contextvars.ContextVar('response', default=None)
+
+    @property
+    def response(self):
+        return self._response.get()
+
+    @response.setter
+    def response(self, value):
+        self._response.set(value)
+
     def _get_collection_class(self):
         return AsyncCollection
 
     def _get_namespace_class(self):
         return AsyncNS
```

### Comparing `connect-openapi-client-25.8/connect/client/help_formatter.py` & `connect-openapi-client-25.9/connect/client/help_formatter.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/logger.py` & `connect-openapi-client-25.9/connect/client/logger.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/mixins.py` & `connect-openapi-client-25.9/connect/client/mixins.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/models/base.py` & `connect-openapi-client-25.9/connect/client/models/base.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/models/iterators.py` & `connect-openapi-client-25.9/connect/client/models/iterators.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/models/mixins.py` & `connect-openapi-client-25.9/connect/client/models/mixins.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/models/resourceset.py` & `connect-openapi-client-25.9/connect/client/models/resourceset.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/openapi.py` & `connect-openapi-client-25.9/connect/client/openapi.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/rql/base.py` & `connect-openapi-client-25.9/connect/client/rql/base.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/rql/utils.py` & `connect-openapi-client-25.9/connect/client/rql/utils.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/connect/client/utils.py` & `connect-openapi-client-25.9/connect/client/utils.py`

 * *Files identical despite different names*

### Comparing `connect-openapi-client-25.8/pyproject.toml` & `connect-openapi-client-25.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-openapi-client"
-version = "25.8"
+version = "25.9"
 description = "Connect Python OpenAPI Client"
 authors = ["CloudBlue"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
     { include = "cnct" }
 ]
@@ -38,39 +38,39 @@
 python = ">=3.7,<4"
 connect-markdown-renderer = "^2"
 PyYAML = ">=5.3.1"
 requests = ">=2.23"
 inflect = ">=4.1"
 httpx = ">=0.23"
 asgiref = "^3.3.4"
+responses = "^0.12.0"
+pytest-httpx = ">=0.20"
+importlib-metadata = { version = "^4.12.0", python = ">=3.7,<3.8" }
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
 pytest-cov = "^2.10.1"
 pytest-mock = "^3.3.1"
 coverage = {extras = ["toml"], version = "^5.3"}
-Sphinx = "^3.2.1"
-sphinx-rtd-theme = "^0.5.0"
-sphinx-copybutton = "^0.3.0"
-setuptools-scm = "^4.1.2"
-setuptools = "^50.3.2"
-twine = "^3.2.0"
-wheel = "^0.35.1"
-responses = "^0.12.0"
 flake8 = "~3.8"
 flake8-bugbear = "~20"
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "~2.0"
 flake8-future-import = "~0.4"
 flake8-import-order = "~0.18"
 flake8-broken-line = "~0.3"
-sphinx-markdown-builder = "^0.5.4"
 pytest-asyncio = "^0.15.1"
-pytest-httpx = ">=0.20"
 mock = { version = "^4.0.3", markers = "python_version < '3.8'" }
+mkdocs = "^1.3.1"
+mkdocs-material = "^8.5.3"
+mkautodoc = "^0.2.0"
+
+[tool.poetry.plugins.pytest11]
+"pytest_connect_client" = "connect.client.testing.fixtures"
+
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>=42"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "tests"
```

### Comparing `connect-openapi-client-25.8/setup.py` & `connect-openapi-client-25.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,38 +4,50 @@
 packages = \
 ['cnct',
  'connect',
  'connect.client',
  'connect.client.contrib',
  'connect.client.contrib.locust',
  'connect.client.models',
- 'connect.client.rql']
+ 'connect.client.rql',
+ 'connect.client.testing',
+ 'connect.client.testing.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=5.3.1',
  'asgiref>=3.3.4,<4.0.0',
  'connect-markdown-renderer>=2,<3',
  'httpx>=0.23',
  'inflect>=4.1',
- 'requests>=2.23']
+ 'pytest-httpx>=0.20',
+ 'requests>=2.23',
+ 'responses>=0.12.0,<0.13.0']
+
+extras_require = \
+{':python_version >= "3.7" and python_version < "3.8"': ['importlib-metadata>=4.12.0,<5.0.0']}
+
+entry_points = \
+{'pytest11': ['pytest_connect_client = connect.client.testing.fixtures']}
 
 setup_kwargs = {
     'name': 'connect-openapi-client',
-    'version': '25.8',
+    'version': '25.9',
     'description': 'Connect Python OpenAPI Client',
     'long_description': '# Connect Python OpenAPI Client\n\n![pyversions](https://img.shields.io/pypi/pyversions/connect-openapi-client.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-openapi-client.svg)](https://pypi.org/project/connect-openapi-client/) [![Build Status](https://github.com/cloudblue/connect-python-openapi-client/workflows/Build%20Connect%20Python%20OpenAPI%20Client/badge.svg)](https://github.com/cloudblue/connect-python-openapi-client/actions) [![codecov](https://codecov.io/gh/cloudblue/connect-python-openapi-client/branch/master/graph/badge.svg)](https://codecov.io/gh/cloudblue/connect-python-openapi-client) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-open-api-client&metric=alert_status)](https://sonarcloud.io/dashboard?id=connect-open-api-client)\n\n\n\n\n## Introduction\n\n`Connect Python OpenAPI Client` is the simple, concise, powerful and REPL-friendly CloudBlue Connect API client.\n\nIt has been designed following the [fluent interface design pattern](https://en.wikipedia.org/wiki/Fluent_interface).\n\nDue to its REPL-friendly nature, using the CloudBlue Connect OpenAPI specifications it allows developers to learn and\nplay with the CloudBlue Connect API using a python REPL like [jupyter](https://jupyter.org/) or [ipython](https://ipython.org/).\n\n\n## Install\n\n`Connect Python OpenAPI Client` requires python 3.7 or later.\n\n\n`Connect Python OpenAPI Client` can be installed from [pypi.org](https://pypi.org/project/connect-openapi-client/) using pip:\n\n```\n$ pip install connect-openapi-client\n```\n\n\n## Documentation\n\n[`Connect Python OpenAPI Client` documentation](https://connect-openapi-client.readthedocs.io/en/latest/) is hosted on the _Read the Docs_ service.\n\n\n## License\n\n``Connect Python OpenAPI Client`` is released under the [Apache License Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).\n',
     'author': 'CloudBlue',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://connect.cloudblue.com',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
+    'entry_points': entry_points,
     'python_requires': '>=3.7,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `connect-openapi-client-25.8/PKG-INFO` & `connect-openapi-client-25.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: connect-openapi-client
-Version: 25.8
+Version: 25.9
 Summary: Connect Python OpenAPI Client
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Keywords: fulfillment,api,client,openapi,utility,connect,cloudblue
 Author: CloudBlue
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=5.3.1)
 Requires-Dist: asgiref (>=3.3.4,<4.0.0)
 Requires-Dist: connect-markdown-renderer (>=2,<3)
 Requires-Dist: httpx (>=0.23)
+Requires-Dist: importlib-metadata (>=4.12.0,<5.0.0); python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: inflect (>=4.1)
+Requires-Dist: pytest-httpx (>=0.20)
 Requires-Dist: requests (>=2.23)
+Requires-Dist: responses (>=0.12.0,<0.13.0)
 Project-URL: Documentation, https://connect-openapi-client.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/cloudblue/connect-python-openapi-client
 Description-Content-Type: text/markdown
 
 # Connect Python OpenAPI Client
 
 ![pyversions](https://img.shields.io/pypi/pyversions/connect-openapi-client.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-openapi-client.svg)](https://pypi.org/project/connect-openapi-client/) [![Build Status](https://github.com/cloudblue/connect-python-openapi-client/workflows/Build%20Connect%20Python%20OpenAPI%20Client/badge.svg)](https://github.com/cloudblue/connect-python-openapi-client/actions) [![codecov](https://codecov.io/gh/cloudblue/connect-python-openapi-client/branch/master/graph/badge.svg)](https://codecov.io/gh/cloudblue/connect-python-openapi-client) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-open-api-client&metric=alert_status)](https://sonarcloud.io/dashboard?id=connect-open-api-client)
```

