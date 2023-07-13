# Comparing `tmp/fabrictestbed-extensions-1.5.1.tar.gz` & `tmp/fabrictestbed-extensions-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.5.1.tar", last modified: Sat Jun 17 10:20:23 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.6.0b1.tar", last modified: Thu Jul 13 19:11:51 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.5.1.tar` & `fabrictestbed-extensions-1.6.0b1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1025 2023-05-11 18:23:24.341681 fabrictestbed-extensions-1.5.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-05-11 18:23:24.341808 fabrictestbed-extensions-1.5.1/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-05-11 18:23:24.341926 fabrictestbed-extensions-1.5.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1806 2023-05-12 13:41:06.568624 fabrictestbed-extensions-1.5.1/.gitignore
--rw-r--r--   0        0        0      666 2023-05-11 18:23:24.342134 fabrictestbed-extensions-1.5.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2897 2023-06-08 17:08:10.775764 fabrictestbed-extensions-1.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-05-11 18:23:24.342656 fabrictestbed-extensions-1.5.1/LICENSE
--rw-r--r--   0        0        0     4054 2023-05-11 18:23:24.342855 fabrictestbed-extensions-1.5.1/README.md
--rw-r--r--   0        0        0      638 2023-05-11 18:23:24.343022 fabrictestbed-extensions-1.5.1/docs/Makefile
--rw-r--r--   0        0        0      799 2023-05-11 18:23:24.343131 fabrictestbed-extensions-1.5.1/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-05-11 18:23:24.343312 fabrictestbed-extensions-1.5.1/docs/source/conf.py
--rw-r--r--   0        0        0     8968 2023-06-12 18:07:22.395922 fabrictestbed-extensions-1.5.1/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-05-11 18:23:24.343613 fabrictestbed-extensions-1.5.1/docs/source/index.rst
--rw-r--r--   0        0        0      147 2023-06-16 15:42:46.821851 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.344271 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-05-11 18:23:24.344572 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-05-11 18:23:24.345052 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-05-11 18:23:24.345347 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-05-11 18:23:24.345570 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-05-11 18:23:24.345738 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    21455 2023-06-14 14:18:40.297506 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    77331 2023-06-15 15:40:37.951763 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5821 2023-06-08 17:08:10.777119 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    26311 2023-06-16 15:44:08.976055 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    40019 2023-06-08 17:08:10.777971 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    96366 2023-06-10 11:36:12.662165 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    38331 2023-06-12 00:52:03.202648 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81762 2023-06-08 17:08:10.780745 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.350075 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2023-05-11 18:23:24.351514 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2023-05-11 18:23:24.351919 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2023-05-11 18:23:24.352243 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.352522 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-05-11 18:23:24.352740 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34389 2023-06-09 15:08:19.572155 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-05-11 18:23:24.353250 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-05-11 18:23:24.353667 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-05-11 18:23:24.353942 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-05-11 18:23:24.354269 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-05-11 18:23:24.354513 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-05-11 18:23:24.354856 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-05-11 18:23:24.355043 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-05-11 18:23:24.355416 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.355793 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-05-11 18:23:24.356170 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-05-11 18:23:24.356417 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-05-11 18:23:24.356653 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1340 2023-06-17 09:55:40.708206 fabrictestbed-extensions-1.5.1/pyproject.toml
--rwxr-xr-x   0        0        0      122 2023-05-11 18:23:24.357218 fabrictestbed-extensions-1.5.1/sphinx.sh
--rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-07-13 19:11:12.627401 fabrictestbed-extensions-1.6.0b1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1727 2023-07-13 19:11:12.627648 fabrictestbed-extensions-1.6.0b1/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-07-13 19:11:12.627776 fabrictestbed-extensions-1.6.0b1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1806 2023-07-13 19:11:12.627899 fabrictestbed-extensions-1.6.0b1/.gitignore
+-rw-r--r--   0        0        0      666 2023-07-13 19:11:12.628010 fabrictestbed-extensions-1.6.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0     3134 2023-07-13 19:11:12.628291 fabrictestbed-extensions-1.6.0b1/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-07-13 19:11:12.628702 fabrictestbed-extensions-1.6.0b1/LICENSE
+-rw-r--r--   0        0        0     4093 2023-07-13 19:11:12.628878 fabrictestbed-extensions-1.6.0b1/README.md
+-rw-r--r--   0        0        0      638 2023-07-13 19:11:12.629133 fabrictestbed-extensions-1.6.0b1/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-07-13 19:11:12.629318 fabrictestbed-extensions-1.6.0b1/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-07-13 19:11:12.629573 fabrictestbed-extensions-1.6.0b1/docs/source/conf.py
+-rw-r--r--   0        0        0     8968 2023-07-13 19:11:12.629746 fabrictestbed-extensions-1.6.0b1/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-07-13 19:11:12.630094 fabrictestbed-extensions-1.6.0b1/docs/source/index.rst
+-rw-r--r--   0        0        0      149 2023-07-13 19:11:46.204422 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.630706 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18043 2023-07-13 19:11:12.630995 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6203 2023-07-13 19:11:12.631560 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68406 2023-07-13 19:11:12.631815 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-07-13 19:11:12.632118 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-07-13 19:11:12.632370 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    21495 2023-07-13 19:11:12.633036 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    77361 2023-07-13 19:11:12.634055 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5822 2023-07-13 19:11:12.634355 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    26310 2023-07-13 19:11:12.634666 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    40016 2023-07-13 19:11:12.635187 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    96387 2023-07-13 19:11:12.635705 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    38529 2023-07-13 19:11:12.636077 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81759 2023-07-13 19:11:12.636971 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.637479 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2023-07-13 19:11:12.639231 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2023-07-13 19:11:12.639596 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2023-07-13 19:11:12.639917 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.640209 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3081 2023-07-13 19:11:12.640528 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-07-13 19:11:12.640718 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8437 2023-07-13 19:11:12.640903 fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1585 2023-07-13 19:11:37.018800 fabrictestbed-extensions-1.6.0b1/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2023-07-13 19:11:12.641373 fabrictestbed-extensions-1.6.0b1/sphinx.sh
+-rw-r--r--   0        0        0    13331 2023-07-13 19:11:12.641937 fabrictestbed-extensions-1.6.0b1/tests/benchmarks/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    20582 2023-07-13 19:11:12.642271 fabrictestbed-extensions-1.6.0b1/tests/benchmarks/link_benchmark.py
+-rw-r--r--   0        0        0    20886 2023-07-13 19:11:12.642664 fabrictestbed-extensions-1.6.0b1/tests/benchmarks/local_network_benchmark.py
+-rw-r--r--   0        0        0    44920 2023-07-13 19:11:12.643280 fabrictestbed-extensions-1.6.0b1/tests/benchmarks/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10017 2023-07-13 19:11:12.643622 fabrictestbed-extensions-1.6.0b1/tests/benchmarks/nvme_benchmark.py
+-rw-r--r--   0        0        0    14764 2023-07-13 19:11:12.643933 fabrictestbed-extensions-1.6.0b1/tests/integration/abc_test.py
+-rw-r--r--   0        0        0    34368 2023-07-13 19:11:12.644201 fabrictestbed-extensions-1.6.0b1/tests/integration/component_tests.py
+-rw-r--r--   0        0        0    10205 2023-07-13 19:11:12.644478 fabrictestbed-extensions-1.6.0b1/tests/integration/hello_fabric.py
+-rw-r--r--   0        0        0        1 2023-07-13 19:11:12.644724 fabrictestbed-extensions-1.6.0b1/tests/unit/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-13 19:11:12.645011 fabrictestbed-extensions-1.6.0b1/tests/unit/data/dummy-token.json
+-rw-r--r--   0        0        0     5095 2023-07-13 19:11:12.645235 fabrictestbed-extensions-1.6.0b1/tests/unit/test_basic.py
+-rw-r--r--   0        0        0      398 2023-07-13 19:11:12.645487 fabrictestbed-extensions-1.6.0b1/tox.ini
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.6.0b1/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.5.1/.github/workflows/build.yml` & `fabrictestbed-extensions-1.6.0b1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.6.0b1/.github/workflows/checks.yml`

 * *Files 22% similar despite different names*

```diff
@@ -34,19 +34,23 @@
           python-version: "3.9"
           cache: 'pip'  # cache pip dependencies
           cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install black
+          python -m pip install black==23.* isort==5.*
 
       - name: Run "black --check"
         run: |
-          python -m black --check --verbose .
+          python -m black --check .
+
+      - name: Run "isort --check"
+        run: |
+          python -m isort --profile black --check .
 
       # Remind PR authors to update CHANGELOG.md
       - name: Check that Changelog has been updated
         if: github.event_name == 'pull_request' && !contains(github.event.pull_request.labels.*.name, 'no changelog')
         run: |
           # `git diff --exit-code` exits with 1 if there were
           # differences and 0 means no differences. Here we negate
```

### Comparing `fabrictestbed-extensions-1.5.1/.github/workflows/test.yml` & `fabrictestbed-extensions-1.6.0b1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/.gitignore` & `fabrictestbed-extensions-1.6.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/.readthedocs.yaml` & `fabrictestbed-extensions-1.6.0b1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/CHANGELOG.md` & `fabrictestbed-extensions-1.6.0b1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 This is the changelog file for FABRIC testbed extensions.  All notable
 changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [Unreleased]
+
+- Address a crash when querying NUMA properties. (Issue
+  [#191](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/191),
+  PR [#192](https://github.com/fabric-testbed/fabrictestbed-extensions/pull/192))
+
 
 ## [1.4.4] - 2023-05-21
 
 ### Fixed
 
 - Changed some error that were printing to stdout to log instead.
```

### Comparing `fabrictestbed-extensions-1.5.1/LICENSE` & `fabrictestbed-extensions-1.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/README.md` & `fabrictestbed-extensions-1.6.0b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 
 
 ## Contributing to FABlib
 
 Contributions to FABlib are made with GitHub Pull Requests. When you
 submit a pull request, some tests will run against it:
 
-- Code formatting will be checked using [black].  Be sure that your
-  code is formatted with black, using its defaults.
+- Code formatting will be checked using [black] and [isort].  Be sure
+  that your code is formatted with these tools.
 - CHANGELOG.md will be checked for updates.
 - Packages will be built.
 - Unit tests will be run.
 
 You can run tests in your environment, like so, using [pytest]:
 
 ```console
@@ -135,7 +135,8 @@
 
 [flit]: https://flit.pypa.io/en/stable/
 [package uploads]: https://flit.pypa.io/en/latest/upload.html
 
 [build]: https://pypi.org/project/build/
 [pytest]: https://pypi.org/project/pytest/
 [black]: https://pypi.org/project/black/
+[isort]: https://pypi.org/project/isort/
```

### Comparing `fabrictestbed-extensions-1.5.1/docs/Makefile` & `fabrictestbed-extensions-1.6.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/docs/make.bat` & `fabrictestbed-extensions-1.6.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/docs/source/conf.py` & `fabrictestbed-extensions-1.6.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/docs/source/fablib.rst` & `fabrictestbed-extensions-1.6.0b1/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/docs/source/index.rst` & `fabrictestbed-extensions-1.6.0b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 import os
 import traceback
-
 from abc import ABC, abstractmethod
 from typing import List
 
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
 from fabrictestbed.slice_editor import (
-    ExperimentTopology,
     Capacities,
-    ComponentType,
     ComponentCatalog,
+    ComponentType,
+    ExperimentTopology,
 )
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 
 
 class AbcTopologyEditor(ABC):
     EXPERIMENT_STATE_UNSUBMITTED = "unsubmitted"
     EXPERIMENT_STATE_LIVE = "live"
     EXPERIMENT_STATE_ERROR = "error"
     EXPERIMENT_STATE_DELETED = "deleted or error"
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,41 +19,36 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
-import os
-import traceback
-import re
-
 import functools
-
 import importlib.resources as pkg_resources
+import os
+import re
+import traceback
 from typing import List
 
+import ipycytoscape as cy
 from fabrictestbed.slice_editor import (
-    ExperimentTopology,
     Capacities,
-    ComponentType,
+    ComponentCatalog,
     ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
     ServiceType,
-    ComponentCatalog,
 )
-from fabrictestbed.slice_editor import ExperimentTopology, Capacities
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
-
-import ipycytoscape as cy
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 from IPython.display import display
 from ipywidgets import Output
 
-from .abc_topology_editor import AbcTopologyEditor
-
 from .. import images
+from .abc_topology_editor import AbcTopologyEditor
 
 
 class CytoscapeTopologyEditor(AbcTopologyEditor):
     # FABRIC design elements https://fabric-testbed.net/branding/style/
     FABRIC_PRIMARY = "#27aae1"
     FABRIC_PRIMARY_LIGHT = "#cde4ef"
     FABRIC_PRIMARY_DARK = "#078ac1"
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,53 +19,49 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
-import os
-import traceback
-import re
-
 import functools
-
 import importlib.resources as pkg_resources
+import os
+import re
+import traceback
 from typing import List
 
 import ipywidgets as widgets
-from ipywidgets import HTML, Layout
+from fabrictestbed.slice_editor import (
+    Capacities,
+    ComponentCatalog,
+    ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
+    ServiceType,
+)
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 from ipyleaflet import (
+    AntPath,
+    CircleMarker,
+    DrawControl,
+    FullScreenControl,
+    Icon,
+    LayerGroup,
     Map,
     Marker,
     Rectangle,
     WidgetControl,
-    basemaps,
-    Icon,
-    LayerGroup,
     ZoomControl,
-    AntPath,
-    DrawControl,
-    CircleMarker,
-    FullScreenControl,
-)
-from fabrictestbed.slice_editor import (
-    ExperimentTopology,
-    Capacities,
-    ComponentType,
-    ComponentModelType,
-    ServiceType,
-    ComponentCatalog,
+    basemaps,
 )
-from fabrictestbed.slice_editor import ExperimentTopology, Capacities
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
-
-from .abc_topology_editor import AbcTopologyEditor
+from ipywidgets import HTML, Layout
 
 from .. import images
+from .abc_topology_editor import AbcTopologyEditor
 
 
 class GeoTopologyEditor(AbcTopologyEditor):
     # Constants
     # U.S. Default Map Center
     DEFAULT_US_MAP_CENTER = (38.12480976137421, -85.7129)
     DEFAULT_US_MAP_ZOOM = 4.0
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 import os
-
 from abc import ABC
+
 from fabrictestbed.util.constants import Constants
 
 
 class AbcFabLIB(ABC):
     FABRIC_BASTION_USERNAME = "FABRIC_BASTION_USERNAME"
     FABRIC_BASTION_KEY_LOCATION = "FABRIC_BASTION_KEY_LOCATION"
     FABRIC_BASTION_HOST = "FABRIC_BASTION_HOST"
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,46 +19,46 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
-from typing import TYPE_CHECKING
+
 import json
+from typing import TYPE_CHECKING
+
 import jinja2
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabrictestbed_extensions.fablib.node import Node
     from fabrictestbed_extensions.fablib.interface import Interface
     from fabrictestbed_extensions.fablib.interface import Interface
 
-from tabulate import tabulate
-from typing import List
-
 import logging
+from typing import List
 
-from fabrictestbed.slice_editor import ComponentModelType, Labels, Flags
 from fabrictestbed.slice_editor import Component as FimComponent
-from fabrictestbed.slice_editor import UserData
+from fabrictestbed.slice_editor import ComponentModelType, Flags, Labels, UserData
+from tabulate import tabulate
 
 
 class Component:
     component_model_map = {
         "NIC_Basic": ComponentModelType.SharedNIC_ConnectX_6,
         "NIC_ConnectX_6": ComponentModelType.SmartNIC_ConnectX_6,
         "NIC_ConnectX_5": ComponentModelType.SmartNIC_ConnectX_5,
         "NVME_P4510": ComponentModelType.NVME_P4510,
         "GPU_TeslaT4": ComponentModelType.GPU_Tesla_T4,
         "GPU_RTX6000": ComponentModelType.GPU_RTX6000,
         "GPU_A40": ComponentModelType.GPU_A40,
         "GPU_A30": ComponentModelType.GPU_A30,
         "NIC_OpenStack": ComponentModelType.SharedNIC_OpenStack_vNIC,
-        "FPGA_Xilinx_U280": ComponentModelType.FPGA_Xilinx_U280
+        "FPGA_Xilinx_U280": ComponentModelType.FPGA_Xilinx_U280,
     }
 
     def __str__(self):
         """
         Creates a tabulated string describing the properties of the component.
 
         Intended for printing component information.
@@ -120,15 +120,15 @@
             "disk": str(self.get_disk()),
             "units": str(self.get_unit()),
             "pci_address": str(self.get_pci_addr()),
             "model": str(self.get_model()),
             "type": str(self.get_type()),
             "dev": str(self.get_device_name()),
             "node": str(self.get_node().get_name()),
-            "numa": str(self.get_numa_node())
+            "numa": str(self.get_numa_node()),
         }
 
     def generate_template_context(self):
         context = self.toDict()
         context["interfaces"] = []
         # for interface in self.get_interfaces():
         #    context["interfaces"].append(interface.get_name())
@@ -401,16 +401,19 @@
         """
         return self.get_fim_component().details
 
     def get_numa_node(self) -> str:
         """
         Get the Numa Node assigned to the device
         """
-        if self.get_fim_component() is not None:
+        try:
             return self.get_fim_component().get_property(pname="label_allocations").numa
+        except Exception as e:
+            logging.error(f"get_numa_node failed: {e}")
+            return None
 
     def get_disk(self) -> int:
         """
         Gets the amount of disk space on this component.
 
         :return: this component's disk space
         :rtype: int
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/fablib.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,41 +19,38 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
-import os
+
+import json
 import logging
+import os
 import random
 from concurrent.futures import ThreadPoolExecutor
+from ipaddress import IPv4Network, IPv6Network
+from typing import TYPE_CHECKING, Dict, List
 
+import pandas as pd
+from fabrictestbed.util.constants import Constants
 from IPython import get_ipython
-
-from typing import List, Dict
-
-from typing import TYPE_CHECKING
-
 from IPython.core.display_functions import display
-from fabrictestbed.util.constants import Constants
-from fabrictestbed_extensions import __version__ as fablib_version
-import pandas as pd
-from ipaddress import IPv4Network, IPv6Network
 from tabulate import tabulate
-import json
 
+from fabrictestbed_extensions import __version__ as fablib_version
 
 if TYPE_CHECKING:
     from fabric_cf.orchestrator.swagger_client import Slice as OrchestratorSlice
 
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 from fim.user import Node as FimNode
 
-from fabrictestbed_extensions.fablib.resources import Resources, Links, FacilityPorts
+from fabrictestbed_extensions.fablib.resources import FacilityPorts, Links, Resources
 from fabrictestbed_extensions.fablib.slice import Slice
 
 
 class fablib:
     default_fablib_manager = None
 
     @staticmethod
@@ -767,15 +764,15 @@
         if bastion_username is not None:
             self.bastion_username = bastion_username
         if bastion_key_filename is not None:
             self.bastion_key_filename = bastion_key_filename
         if log_level is not None:
             self.set_log_level(log_level)
         if log_file is not None:
-            self.log_level = log_file
+            self.log_file = log_file
         if data_dir is not None:
             self.data_dir = data_dir
 
         self.set_log_file(log_file=self.log_file)
 
         # if self.log_file is not None and self.log_level is not None:
         #    logging.basicConfig(filename=self.log_file, level=self.LOG_LEVELS[self.log_level],
@@ -1058,15 +1055,17 @@
         :type filter_function: lambda
         :return: table in format specified by output parameter
         :param update
         :param pretty_names
         :param force_refresh
         :rtype: Object
         """
-        return self.get_resources(update=update, force_refresh=force_refresh).list_sites(
+        return self.get_resources(
+            update=update, force_refresh=force_refresh
+        ).list_sites(
             output=output,
             fields=fields,
             quiet=quiet,
             filter_function=filter_function,
             pretty_names=pretty_names,
         )
 
@@ -1281,15 +1280,17 @@
         if self.facility_ports is None:
             self.facility_ports = FacilityPorts(self)
         elif update:
             self.facility_ports.update()
 
         return self.facility_ports
 
-    def get_resources(self, update: bool = True, force_refresh:bool = False) -> Resources:
+    def get_resources(
+        self, update: bool = True, force_refresh: bool = False
+    ) -> Resources:
         """
         Get a reference to the resources object. The resources object
         is used to query for available resources and capacities.
 
         :return: the resources object
         :rtype: Resources
         """
@@ -1675,15 +1676,17 @@
                 "Failed to get advertised_topology: {}, {}".format(
                     return_status, topology
                 )
             )
 
         return topology.sites[site]
 
-    def get_available_resources(self, update: bool = False, force_refresh: bool = False) -> Resources:
+    def get_available_resources(
+        self, update: bool = False, force_refresh: bool = False
+    ) -> Resources:
         """
         Get the available resources.
 
         Optionally update the available resources by querying the FABRIC
         services. Otherwise, this method returns the existing information.
 
         :param update:
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
 
-from tabulate import tabulate
 import json
+from typing import TYPE_CHECKING, List
+
 import jinja2
+from fabrictestbed.slice_editor import Capacities, Labels
+from tabulate import tabulate
 
-from fabrictestbed.slice_editor import Labels, Capacities
 from fabrictestbed_extensions.fablib.interface import Interface
 
-from typing import TYPE_CHECKING, List
-
 if TYPE_CHECKING:
-    from fabrictestbed_extensions.fablib.slice import Slice
     from fim.user.interface import Interface as FimInterface
 
+    from fabrictestbed_extensions.fablib.slice import Slice
+
 
 class FacilityPort:
     fim_interface = None
     slice = None
 
     def __init__(self, slice: Slice, fim_interface: FimInterface):
         """
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,25 +21,23 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
 
 import ipaddress
-
-from fabrictestbed.slice_editor import Flags
-from tabulate import tabulate
-from ipaddress import IPv4Address
 import json
-import jinja2
-
 import logging
-
+from ipaddress import IPv4Address
 from typing import TYPE_CHECKING, Any
 
+import jinja2
+from fabrictestbed.slice_editor import Flags
+from tabulate import tabulate
+
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabrictestbed_extensions.fablib.node import Node
     from fabrictestbed_extensions.fablib.network_service import NetworkService
     from fabrictestbed_extensions.fablib.component import Component
 
 from fabrictestbed.slice_editor import UserData
@@ -120,15 +118,15 @@
             "state": "State",
             "error": "Error",
             "ssh_command": "SSH Command",
             "public_ssh_key_file": "Public SSH Key File",
             "private_ssh_key_file": "Private SSH Key File",
             "mode": "Mode",
             "ip_addr": "IP Address",
-            "numa": "Numa Node"
+            "numa": "Numa Node",
         }
 
     def toDict(self, skip=[]):
         """
         Returns the interface attributes as a dictionary
 
         :return: slice attributes as dictionary
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/network_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,40 +21,33 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
 
 import logging
+from typing import TYPE_CHECKING, List, Union
 
 from tabulate import tabulate
-from typing import List, Union
-
-from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabrictestbed_extensions.fablib.interface import Interface
     from fabric_cf.orchestrator.swagger_client import Sliver as OrchestratorSliver
 
-from fabrictestbed.slice_editor import (
-    ServiceType,
-    Labels,
-    Flags,
-    NetworkService as FimNetworkService,
-)
-from fim.slivers.network_service import ServiceType, NSLayer
-
-from fabrictestbed.slice_editor import UserData
-from fabric_cf.orchestrator.orchestrator_proxy import Status
-
-from ipaddress import IPv4Address, IPv6Address, IPv4Network, IPv6Network
 import ipaddress
 import json
+from ipaddress import IPv4Address, IPv4Network, IPv6Address, IPv6Network
+
 import jinja2
+from fabric_cf.orchestrator.orchestrator_proxy import Status
+from fabrictestbed.slice_editor import Flags, Labels
+from fabrictestbed.slice_editor import NetworkService as FimNetworkService
+from fabrictestbed.slice_editor import ServiceType, UserData
+from fim.slivers.network_service import NSLayer, ServiceType
 
 
 class NetworkService:
     network_service_map = {
         "L2Bridge": ServiceType.L2Bridge,
         "L2PTP": ServiceType.L2PTP,
         "L2STS": ServiceType.L2STS,
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,48 +20,44 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
 
+import concurrent.futures
 import ipaddress
 import json
+import logging
+import select
 import threading
 import time
-import paramiko
-import logging
+from concurrent.futures import ThreadPoolExecutor
+from typing import TYPE_CHECKING, Dict, List, Tuple, Union
 
+import jinja2
+import paramiko
 from IPython.core.display_functions import display
-from fabrictestbed_extensions.fablib.network_service import NetworkService
 from tabulate import tabulate
-import select
-import jinja2
-
-from concurrent.futures import ThreadPoolExecutor
-import concurrent.futures
-
 
-from typing import List, Union, Tuple, Dict
-
-from typing import TYPE_CHECKING
+from fabrictestbed_extensions.fablib.network_service import NetworkService
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabric_cf.orchestrator.swagger_client import Sliver as OrchestratorSliver
 
-from fim.slivers.network_service import NSLayer
+from ipaddress import IPv4Address, IPv4Network, IPv6Address, IPv6Network, ip_address
 
-from fabrictestbed.slice_editor import Labels, CapacityHints, ServiceType
-from fabrictestbed.slice_editor import Capacities, UserData
-from ipaddress import ip_address, IPv4Address, IPv6Address, IPv4Network, IPv6Network
+from fabrictestbed.slice_editor import Capacities, CapacityHints, Labels
+from fabrictestbed.slice_editor import Node as FimNode
+from fabrictestbed.slice_editor import ServiceType, UserData
+from fim.slivers.network_service import NSLayer
 
 from fabrictestbed_extensions.fablib.component import Component
 from fabrictestbed_extensions.fablib.interface import Interface
-from fabrictestbed.slice_editor import Node as FimNode
 
 
 class Node:
     default_cores = 2
     default_ram = 8
     default_disk = 10
     default_image = "default_rocky_8"
@@ -1295,16 +1291,18 @@
                     # Credit to Stack Overflow user tintin's post here: https://stackoverflow.com/a/32758464
                     stdout_chunks = []
                     try:
                         stdout_chunks.append(
                             stdout.channel.recv(len(stdout.channel.in_buffer))
                         )
                     except EOFError:
-                        logging.warning('A Paramiko EOFError has occurred, '
-                                        'if this is part of a reboot sequence, it can be ignored')
+                        logging.warning(
+                            "A Paramiko EOFError has occurred, "
+                            "if this is part of a reboot sequence, it can be ignored"
+                        )
                     stderr_chunks = []
 
                     while (
                         not channel.closed
                         or channel.recv_ready()
                         or channel.recv_stderr_ready()
                     ):
@@ -1779,16 +1777,16 @@
         :type remote_directory_path: str
         :param retry: how many times to retry SCP upon failure
         :type retry: int
         :param retry_interval: how often to retry SCP on failure
         :type retry_interval: int
         :raise Exception: if management IP is invalid
         """
-        import tarfile
         import os
+        import tarfile
         import tempfile
 
         logging.debug(
             f"upload node: {self.get_name()}, local_directory_path: {local_directory_path}"
         )
 
         output_filename = local_directory_path.split("/")[-1]
@@ -1879,16 +1877,16 @@
         :type remote_directory_path: str
         :param retry: how many times to retry SCP upon failure
         :type retry: int
         :param retry_interval: how often to retry SCP on failure
         :type retry_interval: int
         :raise Exception: if management IP is invalid
         """
-        import tarfile
         import os
+        import tarfile
 
         logging.debug(
             f"upload node: {self.get_name()}, local_directory_path: {local_directory_path}"
         )
 
         temp_file = "/tmp/unpackingfile.tar.gz"
         self.execute(
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
-import logging
-from tabulate import tabulate
 
-from typing import List, Tuple
 import json
+import logging
+from typing import List, Tuple
 
-from fabrictestbed.slice_editor import AdvertisedTopology
-from fabrictestbed.slice_editor import Capacities
+from fabrictestbed.slice_editor import AdvertisedTopology, Capacities
 from fabrictestbed.slice_manager import Status
-from fim.user import link, interface
+from fim.user import interface, link
+from tabulate import tabulate
 
 
 class Resources:
     site_pretty_names = {
         "name": "Name",
         "state": "State",
         "address": "Address",
@@ -72,14 +71,17 @@
         "rtx6000_allocated": "RTX6000 Allocated",
         "a30_available": "A30 Available",
         "a30_capacity": "A30 Capacity",
         "a30_allocated": "A30 Allocated",
         "a40_available": "A40 Available",
         "a40_capacity": "A40 Capacity",
         "a40_allocated": "A40 Allocated",
+        "fpga_u280_available": "U280 Available",
+        "fpga_u280_capacity": "U280 Capacity",
+        "fpga_u280_allocated": "U280 Allocated",
     }
 
     def __init__(self, fablib_manager, force_refresh: bool = False):
         """
         Constructor
         :return:
         """
@@ -140,15 +142,15 @@
                 "ConnectX-6 (100 Gbps x2 NIC)",
                 "ConnectX-5 (25 Gbps x2 NIC)",
                 "P4510 (NVMe 1TB)",
                 "Tesla T4 (GPU)",
                 "RTX6000 (GPU)",
                 "A30 (GPU)",
                 "A40 (GPU)",
-                "FPGA-Xilinx-U280"
+                "FPGA-Xilinx-U280",
             ],
         )
 
     def show_site(
         self,
         site_name: str,
         output: str = None,
@@ -492,15 +494,17 @@
     def update(self, force_refresh: bool = False):
         """
         Update the available resources by querying the FABRIC services
 
         """
         logging.info(f"Updating available resources")
         return_status, topology = (
-            self.get_fablib_manager().get_slice_manager().resources(force_refresh=force_refresh)
+            self.get_fablib_manager()
+            .get_slice_manager()
+            .resources(force_refresh=force_refresh)
         )
         if return_status != Status.OK:
             raise Exception(
                 "Failed to get advertised_topology: {}, {}".format(
                     return_status, topology
                 )
             )
@@ -624,18 +628,24 @@
             "a30_capacity": self.get_component_capacity(site_name, "GPU-A30"),
             "a30_allocated": self.get_component_capacity(site_name, "GPU-A30")
             - self.get_component_available(site_name, "GPU-A30"),
             "a40_available": self.get_component_available(site_name, "GPU-A40"),
             "a40_capacity": self.get_component_capacity(site_name, "GPU-A40"),
             "a40_allocated": self.get_component_capacity(site_name, "GPU-A40")
             - self.get_component_available(site_name, "GPU-A40"),
-            "fpga_u280_available": self.get_component_available(site_name, "FPGA-Xilinx-U280"),
-            "fpga_u280_capacity": self.get_component_capacity(site_name, "FPGA-Xilinx-U280"),
-            "fpga_u280_allocated": self.get_component_capacity(site_name, "FPGA-Xilinx-U280")
-                             - self.get_component_available(site_name, "FPGA-Xilinx-U280"),
+            "fpga_u280_available": self.get_component_available(
+                site_name, "FPGA-Xilinx-U280"
+            ),
+            "fpga_u280_capacity": self.get_component_capacity(
+                site_name, "FPGA-Xilinx-U280"
+            ),
+            "fpga_u280_allocated": self.get_component_capacity(
+                site_name, "FPGA-Xilinx-U280"
+            )
+            - self.get_component_available(site_name, "FPGA-Xilinx-U280"),
         }
 
     def site_to_dictXXX(self, site):
         site_name = site.name
         return {
             "name": {"pretty_name": "Name", "value": site.name},
             "address": {
@@ -803,15 +813,15 @@
             "fpga_u280_capacity": {
                 "pretty_name": "FPGA U280 Capacity",
                 "value": self.get_component_capacity(site_name, "FPGA-Xilinx-U280"),
             },
             "fpga_u280_allocated": {
                 "pretty_name": "FPGA U280 Allocated",
                 "value": self.get_component_capacity(site_name, "FPGA-Xilinx-U280")
-                         - self.get_component_available(site_name, "FPGA-Xilinx-U280"),
+                - self.get_component_available(site_name, "FPGA-Xilinx-U280"),
             },
         }
 
     def list_sites(
         self,
         output=None,
         fields=None,
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/fablib/slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,51 +19,47 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
-import ipaddress
 
-import time
+import ipaddress
+import json
 import logging
+import time
 from concurrent.futures import ThreadPoolExecutor
-
-import pandas as pd
-import json
-
 from typing import TYPE_CHECKING
 
+import pandas as pd
 from IPython.core.display_functions import display
+
 from fabrictestbed_extensions.fablib.facility_port import FacilityPort
 
 if TYPE_CHECKING:
     from fabric_cf.orchestrator.swagger_client import (
         Slice as OrchestratorSlice,
         Sliver as OrchestratorSliver,
     )
     from fabrictestbed_extensions.fablib.fablib import FablibManager
 
-from tabulate import tabulate
-
-from ipaddress import ip_address, IPv4Address
-
-from typing import List, Union, Dict
-
-from concurrent.futures import ThreadPoolExecutor
 import concurrent.futures
+from concurrent.futures import ThreadPoolExecutor
+from ipaddress import IPv4Address, ip_address
+from typing import Dict, List, Union
 
 from fabrictestbed.slice_editor import ExperimentTopology
-from fabrictestbed.slice_manager import Status, SliceState
+from fabrictestbed.slice_manager import SliceState, Status
+from tabulate import tabulate
 
-from fabrictestbed_extensions.fablib.network_service import NetworkService
-from fabrictestbed_extensions.fablib.node import Node
 from fabrictestbed_extensions.fablib.component import Component
 from fabrictestbed_extensions.fablib.interface import Interface
+from fabrictestbed_extensions.fablib.network_service import NetworkService
+from fabrictestbed_extensions.fablib.node import Node
 
 
 class Slice:
     def __init__(self, fablib_manager: FablibManager, name: str = None):
         """
         Constructor. Sets the default slice state to be callable.
 
@@ -1698,17 +1694,18 @@
         :param interval: how often in seconds to check on slice state
         :type interval: int
         :raises Exception: if the slice state is undesirable, or waiting times out
         :return: the stable slice on the slice manager
         :rtype: SMSlice
         """
 
-        from IPython.display import clear_output
         import time
 
+        from IPython.display import clear_output
+
         logging.debug(f"wait_jupyter: slice {self.get_name()}")
 
         start = time.time()
 
         # if len(self.get_interfaces()) > 0:
         #    hasNetworks = True
         # else:
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.6.0b1/tests/integration/abc_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,21 +19,20 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 import os
-import traceback
 import time
-
+import traceback
 from abc import ABC, abstractmethod
+from ipaddress import IPv4Address, ip_address
 
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
-from ipaddress import ip_address, IPv4Address
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 
 
 class AbcTest(ABC):
     def __init__(self):
         self.slice_manager = SliceManager()
         self.advertised_topology = None
         self.slice = None
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.6.0b1/tests/integration/component_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,53 +19,50 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
+import functools
+import importlib.resources as pkg_resources
 import os
-import traceback
 import re
-
-import functools
 import time
-
-import importlib.resources as pkg_resources
+import traceback
 from typing import List
 
+from abc_test import AbcTest
 from fabrictestbed.slice_editor import (
-    Labels,
-    ExperimentTopology,
     Capacities,
-    ComponentType,
+    ComponentCatalog,
     ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
+    Labels,
     ServiceType,
-    ComponentCatalog,
 )
-from fabrictestbed.slice_editor import ExperimentTopology, Capacities
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 
+from fabrictestbed_extensions import images
 
 from .abc_test import AbcTest
 
-from .. import images
-
 
 class ComponentTest(AbcTest):
     COMPONENT_MODELS = {
         "GPU_Tesla_T4": ComponentModelType.GPU_Tesla_T4,
         "GPU_RTX6000": ComponentModelType.GPU_RTX6000,
         "GPU_A30": ComponentModelType.GPU_A30,
         "GPU_A40": ComponentModelType.GPU_A40,
         "SharedNIC_ConnectX_6": ComponentModelType.SharedNIC_ConnectX_6,
         "SmartNIC_ConnectX_6": ComponentModelType.SmartNIC_ConnectX_6,
         "SmartNIC_ConnectX_5": ComponentModelType.SmartNIC_ConnectX_5,
         "NVME_P4510": ComponentModelType.NVME_P4510,
-        "FPGA_Xilinx_U280": ComponentModelType.FPGA_Xilinx_U280
+        "FPGA_Xilinx_U280": ComponentModelType.FPGA_Xilinx_U280,
     }
 
     def __init__(self):
         """
         Constructor
         :return:
         """
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.6.0b1/tests/benchmarks/gpu_tesla_t4_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,40 +19,35 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
+import functools
+import importlib.resources as pkg_resources
 import os
-import traceback
 import re
-
-import functools
 import time
-
-import importlib.resources as pkg_resources
+import traceback
 from typing import List
 
 from fabrictestbed.slice_editor import (
-    Labels,
-    ExperimentTopology,
     Capacities,
-    ComponentType,
+    ComponentCatalog,
     ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
+    Labels,
     ServiceType,
-    ComponentCatalog,
 )
-from fabrictestbed.slice_editor import ExperimentTopology, Capacities
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
-
-
-from .abc_test import AbcTest
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 
-from .. import images
+from fabrictestbed_extensions import images
+from tests.integration.abc_test import AbcTest
 
 
 class GPUTeslaT4Benchmark(AbcTest):
     def __init__(self):
         """
         Constructor
         :return:
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.6.0b1/tests/integration/hello_fabric.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,41 +19,38 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
+import functools
+import importlib.resources as pkg_resources
 import os
-import traceback
 import re
-
-import functools
 import time
-
-import importlib.resources as pkg_resources
+import traceback
 from typing import List
 
+from abc_test import AbcTest
 from fabrictestbed.slice_editor import (
-    Labels,
-    ExperimentTopology,
     Capacities,
-    ComponentType,
+    ComponentCatalog,
     ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
+    Labels,
     ServiceType,
-    ComponentCatalog,
 )
-from fabrictestbed.slice_editor import ExperimentTopology, Capacities
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 
+from fabrictestbed_extensions import images
 
 from .abc_test import AbcTest
 
-from .. import images
-
 
 class HelloFABRIC(AbcTest):
     def __init__(self):
         """
         Constructor
         :return:
         """
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.6.0b1/tests/benchmarks/link_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,39 +19,35 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
+import importlib.resources as pkg_resources
+import json
 import os
-import traceback
 import re
-import json
-import paramiko
 import time
-
-import importlib.resources as pkg_resources
+import traceback
 from typing import List
 
+import paramiko
 from fabrictestbed.slice_editor import (
-    ExperimentTopology,
     Capacities,
-    ComponentType,
+    ComponentCatalog,
     ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
     ServiceType,
-    ComponentCatalog,
 )
-from fabrictestbed.slice_editor import ExperimentTopology, Capacities
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 from fabrictestbed.util.constants import Constants
 
-from .abc_test import AbcTest
-
-from .. import images
+from tests.integration.abc_test import AbcTest
 
 
 class LinkBenchmark(AbcTest):
     def __init__(self):
         """
         Constructor
         :return:
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.6.0b1/tests/benchmarks/local_network_benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,39 +19,36 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
+import importlib.resources as pkg_resources
+import json
 import os
-import traceback
 import re
-import json
-import paramiko
 import time
-
-import importlib.resources as pkg_resources
+import traceback
 from typing import List
 
+import paramiko
 from fabrictestbed.slice_editor import (
-    ExperimentTopology,
     Capacities,
-    ComponentType,
+    ComponentCatalog,
     ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
     ServiceType,
-    ComponentCatalog,
 )
-from fabrictestbed.slice_editor import ExperimentTopology, Capacities
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 from fabrictestbed.util.constants import Constants
 
-from .abc_test import AbcTest
-
-from .. import images
+from fabrictestbed_extensions import images
+from tests.integration.abc_test import AbcTest
 
 
 class LinkBenchmark(AbcTest):
     def __init__(self):
         """
         Constructor
         :return:
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.6.0b1/tests/benchmarks/network_benchmark_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-import os
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
+import importlib.resources as pkg_resources
 import json
+import os
+import re
+import time
+from typing import List
+
+import paramiko
 from fabrictestbed.slice_editor import (
-    ExperimentTopology,
     Capacities,
-    ComponentType,
     ComponentModelType,
-    ServiceType,
+    ComponentType,
+    ExperimentTopology,
     Labels,
+    ServiceType,
 )
-import time
-import paramiko
-import re
-
-import importlib.resources as pkg_resources
-from typing import List
-
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 from fabrictestbed.util.constants import Constants
 
-from .abc_test import AbcTest
-
-from .. import images
+from fabrictestbed_extensions import images
+from tests.integration.abc_test import AbcTest
 
 
 class NetworkBencharks(AbcTest):
     def __init__(self):
         """
         Constructor
         :return:
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.6.0b1/tests/benchmarks/nvme_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,40 +19,35 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
+import functools
+import importlib.resources as pkg_resources
 import os
-import traceback
 import re
-
-import functools
 import time
-
-import importlib.resources as pkg_resources
+import traceback
 from typing import List
 
 from fabrictestbed.slice_editor import (
-    Labels,
-    ExperimentTopology,
     Capacities,
-    ComponentType,
+    ComponentCatalog,
     ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
+    Labels,
     ServiceType,
-    ComponentCatalog,
 )
-from fabrictestbed.slice_editor import ExperimentTopology, Capacities
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
-
-
-from .abc_test import AbcTest
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 
-from .. import images
+from fabrictestbed_extensions import images
+from tests.integration.abc_test import AbcTest
 
 
 class NVMEBenchmark(AbcTest):
     def __init__(self):
         """
         Constructor
         :return:
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.6.0b1/tests/unit/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,29 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 import os
-import traceback
 import time
-
+import traceback
 from abc import ABC, abstractmethod
 from typing import List
 
 from fabric_cf.orchestrator.orchestrator_proxy import SliceState
-from fabrictestbed.slice_manager import SliceManager, Status, SliceState
 from fabrictestbed.slice_editor import (
-    ExperimentTopology,
     Capacities,
-    ComponentType,
+    ComponentCatalog,
     ComponentModelType,
+    ComponentType,
+    ExperimentTopology,
     ServiceType,
-    ComponentCatalog,
 )
+from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 from fabrictestbed.util.constants import Constants
 
 
 class AbcUtils(ABC):
     bastion_username = os.environ["FABRIC_BASTION_USERNAME"]
 
     bastion_public_addr = os.environ["FABRIC_BASTION_HOST"]
```

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.6.0b1/fabrictestbed_extensions/utils/slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 
 
 import time
 
-from fabrictestbed.slice_manager import Status, SliceState
+from fabrictestbed.slice_manager import SliceState, Status
+
 from .abc_utils import AbcUtils
 
 
 class SliceUtils(AbcUtils):
     def __init__(self):
         """
         Constructor
```

### Comparing `fabrictestbed-extensions-1.5.1/pyproject.toml` & `fabrictestbed-extensions-1.6.0b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "ipycytoscape",
     "ipywidgets",
     "ipyleaflet",
     "ipycytoscape",
     "tabulate",
-    "fabrictestbed==1.5.1",
+    "fabrictestbed==1.6.0b1",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
     "ipython>=8.12.0"
     ]
 
@@ -39,12 +39,24 @@
 Homepage = "https://fabric-testbed.net/"
 Sources = "https://github.com/fabric-testbed/fabrictestbed-extensions"
 Documentation = "https://fabric-fablib.readthedocs.io/"
 ChangeLog = "https://github.com/fabric-testbed/fabrictestbed-extensions/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 doc = ["sphinx", "furo"]
-test = ["pytest", "coverage[toml]"]
+test = [
+    "black==23.*",
+    "isort==5.*",
+    "pytest",
+    "coverage[toml]"
+    ]
 
 [tool.coverage.run]
 branch = true
 omit = [ "fabrictestbed_extensions/tests/*" ]
+
+[tool.black]
+src_paths = ["fabrictestbed_extensions", "docs/source/conf.py", "tests"]
+
+[tool.isort]
+profile = "black"
+src_paths = ["fabrictestbed_extensions", "docs/source/conf.py", "tests"]
```

### Comparing `fabrictestbed-extensions-1.5.1/PKG-INFO` & `fabrictestbed-extensions-1.6.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.5.1
+Version: 1.6.0b1
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ipycytoscape
 Requires-Dist: ipywidgets
 Requires-Dist: ipyleaflet
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
-Requires-Dist: fabrictestbed==1.5.1
+Requires-Dist: fabrictestbed==1.6.0b1
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: ipython>=8.12.0
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
+Requires-Dist: black==23.* ; extra == "test"
+Requires-Dist: isort==5.* ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: ChangeLog, https://github.com/fabric-testbed/fabrictestbed-extensions/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://fabric-fablib.readthedocs.io/
 Project-URL: Homepage, https://fabric-testbed.net/
 Project-URL: Sources, https://github.com/fabric-testbed/fabrictestbed-extensions
 Provides-Extra: doc
@@ -88,16 +90,16 @@
 
 
 ## Contributing to FABlib
 
 Contributions to FABlib are made with GitHub Pull Requests. When you
 submit a pull request, some tests will run against it:
 
-- Code formatting will be checked using [black].  Be sure that your
-  code is formatted with black, using its defaults.
+- Code formatting will be checked using [black] and [isort].  Be sure
+  that your code is formatted with these tools.
 - CHANGELOG.md will be checked for updates.
 - Packages will be built.
 - Unit tests will be run.
 
 You can run tests in your environment, like so, using [pytest]:
 
 ```console
@@ -167,8 +169,9 @@
 
 [flit]: https://flit.pypa.io/en/stable/
 [package uploads]: https://flit.pypa.io/en/latest/upload.html
 
 [build]: https://pypi.org/project/build/
 [pytest]: https://pypi.org/project/pytest/
 [black]: https://pypi.org/project/black/
+[isort]: https://pypi.org/project/isort/
```

