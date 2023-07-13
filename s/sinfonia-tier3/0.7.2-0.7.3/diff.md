# Comparing `tmp/sinfonia_tier3-0.7.2.tar.gz` & `tmp/sinfonia_tier3-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinfonia_tier3-0.7.2.tar", max compression
+gzip compressed data, was "sinfonia_tier3-0.7.3.tar", max compression
```

## Comparing `sinfonia_tier3-0.7.2.tar` & `sinfonia_tier3-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1088 2022-11-02 13:08:28.772076 sinfonia_tier3-0.7.2/LICENSE
-drwxr-xr-x   0        0        0        0 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/LICENSES/
--rw-r--r--   0        0        0      643 2022-11-02 13:08:28.772076 sinfonia_tier3-0.7.2/LICENSES/0BSD.txt
--rw-r--r--   0        0        0     1593 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/LICENSES/CC-PDDC.txt
--rw-r--r--   0        0        0     1078 2022-11-02 13:08:28.772076 sinfonia_tier3-0.7.2/LICENSES/MIT.txt
--rw-r--r--   0        0        0     3424 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/README.md
--rw-r--r--   0        0        0     2520 2023-03-15 18:28:14.364707 sinfonia_tier3-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      274 2023-03-15 18:28:14.364707 sinfonia_tier3-0.7.2/src/sinfonia_tier3/__init__.py
--rw-r--r--   0        0        0      272 2023-02-27 18:16:53.273696 sinfonia_tier3-0.7.2/src/sinfonia_tier3/__main__.py
--rw-r--r--   0        0        0     3367 2023-03-15 18:22:08.862338 sinfonia_tier3-0.7.2/src/sinfonia_tier3/cli.py
--rw-r--r--   0        0        0     3768 2023-02-27 18:43:06.110692 sinfonia_tier3-0.7.2/src/sinfonia_tier3/cloudlet_deployment.py
--rw-r--r--   0        0        0     2494 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/src/sinfonia_tier3/key_cache.py
--rw-r--r--   0        0        0     4005 2023-02-28 13:57:11.580542 sinfonia_tier3-0.7.2/src/sinfonia_tier3/local_deployment.py
--rw-r--r--   0        0        0     2659 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/src/sinfonia_tier3/netns_helper.py
--rw-r--r--   0        0        0     4299 2022-11-02 13:08:28.776077 sinfonia_tier3-0.7.2/src/sinfonia_tier3/openapi/sinfonia_tier2.yaml
--rw-r--r--   0        0        0        0 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/src/sinfonia_tier3/py.typed
--rw-r--r--   0        0        0     2235 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/src/sinfonia_tier3/root_helper.py
--rw-r--r--   0        0        0        0 2022-11-02 13:08:28.776077 sinfonia_tier3-0.7.2/tests/__init__.py
--rw-r--r--   0        0        0      215 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/tests/conftest.py
--rw-r--r--   0        0        0     2280 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/tests/test_app.py
--rw-r--r--   0        0        0     1537 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/tests/test_key_cache.py
--rw-r--r--   0        0        0      676 2023-02-27 18:16:27.764963 sinfonia_tier3-0.7.2/tests/test_openapi.py
--rw-r--r--   0        0        0     4710 1970-01-01 00:00:00.000000 sinfonia_tier3-0.7.2/setup.py
--rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 sinfonia_tier3-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2022-11-02 13:08:28.772076 sinfonia_tier3-0.7.3/LICENSE
+drwxr-xr-x   0        0        0        0 2022-11-08 18:58:31.716947 sinfonia_tier3-0.7.3/LICENSES/
+-rw-r--r--   0        0        0      643 2022-11-02 13:08:28.772076 sinfonia_tier3-0.7.3/LICENSES/0BSD.txt
+-rw-r--r--   0        0        0     1593 2022-11-08 18:58:31.716947 sinfonia_tier3-0.7.3/LICENSES/CC-PDDC.txt
+-rw-r--r--   0        0        0     1078 2022-11-02 13:08:28.772076 sinfonia_tier3-0.7.3/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3424 2022-12-21 14:08:50.710432 sinfonia_tier3-0.7.3/README.md
+-rw-r--r--   0        0        0     2374 2023-07-13 02:11:53.811735 sinfonia_tier3-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      274 2023-07-13 02:11:53.811735 sinfonia_tier3-0.7.3/src/sinfonia_tier3/__init__.py
+-rw-r--r--   0        0        0      272 2023-07-12 21:35:52.577394 sinfonia_tier3-0.7.3/src/sinfonia_tier3/__main__.py
+-rw-r--r--   0        0        0     3367 2023-07-12 21:35:52.577394 sinfonia_tier3-0.7.3/src/sinfonia_tier3/cli.py
+-rw-r--r--   0        0        0     3844 2023-07-13 02:04:08.046009 sinfonia_tier3-0.7.3/src/sinfonia_tier3/cloudlet_deployment.py
+-rw-r--r--   0        0        0     2494 2022-12-21 14:08:50.714433 sinfonia_tier3-0.7.3/src/sinfonia_tier3/key_cache.py
+-rw-r--r--   0        0        0     4005 2023-07-12 21:35:52.577394 sinfonia_tier3-0.7.3/src/sinfonia_tier3/local_deployment.py
+-rw-r--r--   0        0        0     2659 2022-12-12 13:51:22.010233 sinfonia_tier3-0.7.3/src/sinfonia_tier3/netns_helper.py
+-rw-r--r--   0        0        0     4299 2022-11-02 13:08:28.776077 sinfonia_tier3-0.7.3/src/sinfonia_tier3/openapi/sinfonia_tier2.yaml
+-rw-r--r--   0        0        0        0 2022-11-09 16:02:11.911572 sinfonia_tier3-0.7.3/src/sinfonia_tier3/py.typed
+-rw-r--r--   0        0        0     2235 2022-12-21 14:08:50.714433 sinfonia_tier3-0.7.3/src/sinfonia_tier3/root_helper.py
+-rw-r--r--   0        0        0        0 2022-11-02 13:08:28.776077 sinfonia_tier3-0.7.3/tests/__init__.py
+-rw-r--r--   0        0        0      215 2022-11-09 16:02:11.911572 sinfonia_tier3-0.7.3/tests/conftest.py
+-rw-r--r--   0        0        0     2280 2022-11-09 16:02:11.911572 sinfonia_tier3-0.7.3/tests/test_app.py
+-rw-r--r--   0        0        0     1537 2022-11-09 16:02:11.911572 sinfonia_tier3-0.7.3/tests/test_key_cache.py
+-rw-r--r--   0        0        0      669 2023-07-12 21:50:59.424152 sinfonia_tier3-0.7.3/tests/test_openapi.py
+-rw-r--r--   0        0        0     4710 1970-01-01 00:00:00.000000 sinfonia_tier3-0.7.3/setup.py
+-rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 sinfonia_tier3-0.7.3/PKG-INFO
```

### Comparing `sinfonia_tier3-0.7.2/LICENSE` & `sinfonia_tier3-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/LICENSES/0BSD.txt` & `sinfonia_tier3-0.7.3/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/LICENSES/CC-PDDC.txt` & `sinfonia_tier3-0.7.3/LICENSES/CC-PDDC.txt`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/LICENSES/MIT.txt` & `sinfonia_tier3-0.7.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/README.md` & `sinfonia_tier3-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/pyproject.toml` & `sinfonia_tier3-0.7.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2021-2023 Carnegie Mellon University
 # SPDX-License-Identifier: 0BSD
 
 [tool.poetry]
 name = "sinfonia-tier3"
-version = "0.7.2"
+version = "0.7.3"
 description = "Tier 3 component of the Sinfonia system"
 authors = [
     "Carnegie Mellon University <satya+group@cs.cmu.edu>",
     "Jan Harkes <jaharkes@cs.cmu.edu>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -25,15 +25,15 @@
     {path = "tests", format="sdist"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 attrs = ">=22.1.0"
 importlib-resources = "^5.0"
-openapi-core = "^0.14.2"
+openapi-core = "^0.17.2"
 pyroute2 = "^0.7.3"
 pyyaml = "^6.0"
 requests = "^2.28.1"
 xdg = "^5.1.1"
 yarl = "^1.7.2"
 typing-extensions = "^4.4.0"
 wireguard-tools = "^0.4.1"
@@ -88,24 +88,17 @@
 # pytest decorators are not typed
 module = "tests.*"
 disallow_untyped_decorators = false
 
 [[tool.mypy.overrides]]
 # ignore missing type hints errors from untyped modules
 module = [
-    "openapi_core.*",
     "pyroute2.*",
 ]
 ignore_missing_imports = true
 
-[tool.pytest.ini_options]
-filterwarnings = [
-    "error",
-    "ignore:Subclassing validator classes:DeprecationWarning",
-]
-
 [tool.poe]
 include = "tasks.toml"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sinfonia_tier3-0.7.2/src/sinfonia_tier3/cli.py` & `sinfonia_tier3-0.7.3/src/sinfonia_tier3/cli.py`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/src/sinfonia_tier3/cloudlet_deployment.py` & `sinfonia_tier3-0.7.3/src/sinfonia_tier3/cloudlet_deployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 # Copyright (c) 2021-2022 Carnegie Mellon University
 #
 # SPDX-License-Identifier: MIT
 #
 
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, cast
 from uuid import UUID
 
 import importlib_resources
 import requests
 import yaml
 from attrs import define
-from openapi_core import create_spec
+from openapi_core import Spec, unmarshal_response
 from openapi_core.contrib.requests import (
     RequestsOpenAPIRequest,
     RequestsOpenAPIResponse,
 )
-from openapi_core.validation.response.validators import ResponseValidator
 from wireguard_tools import WireguardConfig, WireguardKey
 from yarl import URL
 
 from .key_cache import KeyCacheEntry
 
 
 @define
@@ -110,24 +109,28 @@
     # load openapi specification to validate the response
     spec_text = (
         importlib_resources.files("sinfonia_tier3.openapi")
         .joinpath("sinfonia_tier2.yaml")
         .read_text()
     )
     spec_dict = yaml.safe_load(spec_text)
-    spec = create_spec(spec_dict)
+    spec = Spec.create(spec_dict)
 
     # create request/response wrappers for validation
     openapi_request = RequestsOpenAPIRequest(response.request)
     openapi_response = RequestsOpenAPIResponse(response)
 
-    # validate the response
-    validator = ResponseValidator(
-        spec, custom_formatters={"wireguard_public_key": WireguardKeyFormatter()}
+    # validate and unpack the response
+    extra_validators = dict(wireguard_public_Key=WireguardKeyFormatter())
+    result = unmarshal_response(
+        openapi_request,
+        openapi_response,
+        spec=spec,
+        extra_format_validators=extra_validators,
     )
-    result = validator.validate(openapi_request, openapi_response)
-    result.raise_for_errors()
 
+    # validation should have failed if this is None, I think
+    assert result.data is not None
     return [
         CloudletDeployment.from_dict(deployment_keys.private_key, deployment)
-        for deployment in result.data
+        for deployment in cast(Any, result.data)
     ]
```

### Comparing `sinfonia_tier3-0.7.2/src/sinfonia_tier3/key_cache.py` & `sinfonia_tier3-0.7.3/src/sinfonia_tier3/key_cache.py`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/src/sinfonia_tier3/local_deployment.py` & `sinfonia_tier3-0.7.3/src/sinfonia_tier3/local_deployment.py`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/src/sinfonia_tier3/netns_helper.py` & `sinfonia_tier3-0.7.3/src/sinfonia_tier3/netns_helper.py`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/src/sinfonia_tier3/openapi/sinfonia_tier2.yaml` & `sinfonia_tier3-0.7.3/src/sinfonia_tier3/openapi/sinfonia_tier2.yaml`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/src/sinfonia_tier3/root_helper.py` & `sinfonia_tier3-0.7.3/src/sinfonia_tier3/root_helper.py`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/tests/test_app.py` & `sinfonia_tier3-0.7.3/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/tests/test_key_cache.py` & `sinfonia_tier3-0.7.3/tests/test_key_cache.py`

 * *Files identical despite different names*

### Comparing `sinfonia_tier3-0.7.2/tests/test_openapi.py` & `sinfonia_tier3-0.7.3/tests/test_openapi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright (c) 2022 Carnegie Mellon University
 # SPDX-License-Identifier: MIT
 
 from pathlib import Path
 
 import pytest
 import yaml
-from openapi_core import create_spec
+from openapi_core import Spec
 
 
 class TestOpenApiSpecs:
     @pytest.fixture(scope="class")
     def specification_dir(self) -> Path:
         return Path(__file__).parents[1] / "src" / "sinfonia_tier3" / "openapi"
 
     @pytest.mark.filterwarnings("ignore::DeprecationWarning")
     def test_tier2_spec(self, specification_dir: Path) -> None:
         spec_yaml = specification_dir.joinpath("sinfonia_tier2.yaml").read_text()
         spec_dict = yaml.safe_load(spec_yaml)
-        spec = create_spec(spec_dict)
+        spec = Spec.create(spec_dict)
         assert spec is not None
```

### Comparing `sinfonia_tier3-0.7.2/setup.py` & `sinfonia_tier3-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 package_data = \
 {'': ['*'], 'sinfonia_tier3': ['openapi/*']}
 
 install_requires = \
 ['attrs>=22.1.0',
  'importlib-resources>=5.0,<6.0',
- 'openapi-core>=0.14.2,<0.15.0',
+ 'openapi-core>=0.17.2,<0.18.0',
  'pyroute2>=0.7.3,<0.8.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'typing-extensions>=4.4.0,<5.0.0',
  'wireguard-tools>=0.4.1,<0.5.0',
  'wireguard4netns>=0.1.3,<0.2.0',
  'xdg>=5.1.1,<6.0.0',
  'yarl>=1.7.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['sinfonia-tier3 = sinfonia_tier3.cli:main']}
 
 setup_kwargs = {
     'name': 'sinfonia-tier3',
-    'version': '0.7.2',
+    'version': '0.7.3',
     'description': 'Tier 3 component of the Sinfonia system',
     'long_description': "# Sinfonia\n\nManages discovery of nearby cloudlets and deployment of backends for\nedge-native applications.\n\nThe framework is a 3 tiered system. Tier 1 is located in the cloud and tracks\navailability of the Tier 2 instances running on the edge of the network\n(cloudlets) where backends can be deployed. Tier 3 is the client application\nthat mediates the discovery and deployment process for edge-native\napplications.\n\nThis repository implements an example Tier3 client which can be used both as a\ncommand-line application and as a Python library.\n\n\n## Installation\n\nYou probably don't need to install this directly, most of the time it should\nget installed as a dependency of whichever edge-native application is using\nthe Sinfonia framework to discover nearby cloudlets.\n\nBut if you want to run the standalone command-line application, you can install\nthis with installable with `pipx install sinfonia-tier3` or\n`pip install [--user] sinfonia-tier3`.\n\n\n## Usage\n\nThe `sinfonia-tier3` application would normally be called by any edge-native\napplication that uses the Sinfonia framework to deploy its application specific\nbackend on a nearby cloudlet.\n\nThe information needed by the application are the URL of a Tier1 instance\nand the UUID identifying the required backend. The remainder of the arguments\nconsist of the actual frontend application and arguments that will be launched\nin an seperate network namespace connecting back to the deployed backend.\n\n    $ sinfonia-tier3 <tier1-url> <uuid> <frontend-app> <args...>\n\nAn example application with UUID:00000000-0000-0000-0000-000000000000 (or the\nconvenient alias 'helloworld') starts an nginx server that will be accessible\nwith the hostname 'helloworld'.\n\n    $ sinfonia-tier3 https://tier1.server.url/ helloworld /bin/sh\n    sinfonia$ curl -v http://helloworld/\n    ...\n    sinfonia$ exit\n\nWhen the frontend application exits, the network namespace and WireGuard tunnel\nare cleaned up. Any resources on the cloudlet will be automatically released\nonce the Sinfonia-tier2 instance notices the VPN tunnel has been idle.\n\n\n## Installation from this source repository\n\nYou need a recent version of `poetry`\n\n    $ pip install --user pipx\n    $ ~/.local/bin/pipx ensurepath\n    ... possibly restart shell to pick up the right PATH\n    $ pipx install poetry\n\nAnd then use poetry to install the necessary dependencies,\n\n    $ git clone https://github.com/cmusatyalab/sinfonia-tier3.git\n    $ cd sinfonia-tier3\n    $ poetry install\n    $ poetry run sinfonia-tier3 ...\n    ... or\n    $ poetry shell\n    (env)$ sinfonia-tier3 ...\n\n\n## Why do we need a sudo password when deploying\n\nActually you should not need a password if `wireguard4netns` works correctly\nBut if for some reason it fails to create the tuntap device and launch\nwireguard-go, the code will fall back on the older `sudo` implementation.\n\nThe older `sudo` implementation uses the in-kernel Wireguard implementation and\nneeds root access to create and configure the WireGuard device and endpoint.\nAll of the code running as root is contained in\n[src/sinfonia_tier3/root_helper.py](https://github.com/cmusatyalab/sinfonia-tier3/blob/main/src/sinfonia_tier3/root_helper.py)\n\nIt runs the equivalent of the following.\n\n```sh\n    ip link add wg-tunnel type wireguard\n    wg set wg-tunnel private-key <private-key> peer <public-key> endpoint ...\n    ip link set dev wg-tunnel netns <application network namespace>\n```\n",
     'author': 'Carnegie Mellon University',
     'author_email': 'satya+group@cs.cmu.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cmusatyalab/sinfonia-tier3',
```

### Comparing `sinfonia_tier3-0.7.2/PKG-INFO` & `sinfonia_tier3-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinfonia-tier3
-Version: 0.7.2
+Version: 0.7.3
 Summary: Tier 3 component of the Sinfonia system
 Home-page: https://github.com/cmusatyalab/sinfonia-tier3
 License: MIT
 Author: Carnegie Mellon University
 Author-email: satya+group@cs.cmu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22.1.0)
 Requires-Dist: importlib-resources (>=5.0,<6.0)
-Requires-Dist: openapi-core (>=0.14.2,<0.15.0)
+Requires-Dist: openapi-core (>=0.17.2,<0.18.0)
 Requires-Dist: pyroute2 (>=0.7.3,<0.8.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: wireguard-tools (>=0.4.1,<0.5.0)
 Requires-Dist: wireguard4netns (>=0.1.3,<0.2.0)
 Requires-Dist: xdg (>=5.1.1,<6.0.0)
```

