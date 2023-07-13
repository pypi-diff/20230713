# Comparing `tmp/fabrictestbed-1.5.1.tar.gz` & `tmp/fabrictestbed-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.5.1.tar", last modified: Sat Jun 17 10:06:29 2023, max compression
+gzip compressed data, was "fabrictestbed-1.6.0b1.tar", last modified: Thu Jul 13 18:48:55 2023, max compression
```

## Comparing `fabrictestbed-1.5.1.tar` & `fabrictestbed-1.6.0b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1806 2023-05-11 17:40:59.099816 fabrictestbed-1.5.1/.gitignore
--rw-r--r--   0        0        0     1071 2023-05-11 17:40:59.100151 fabrictestbed-1.5.1/LICENSE
--rw-r--r--   0        0        0       24 2023-05-11 17:40:59.100302 fabrictestbed-1.5.1/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-05-31 18:44:19.979642 fabrictestbed-1.5.1/README.md
--rw-r--r--   0        0        0       22 2023-06-17 09:55:40.694524 fabrictestbed-1.5.1/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.100987 fabrictestbed-1.5.1/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    18169 2023-05-11 17:40:59.101162 fabrictestbed-1.5.1/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.101319 fabrictestbed-1.5.1/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-05-11 17:40:59.101479 fabrictestbed-1.5.1/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-05-11 17:40:59.101641 fabrictestbed-1.5.1/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    19811 2023-06-08 14:43:40.270937 fabrictestbed-1.5.1/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.101985 fabrictestbed-1.5.1/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.102200 fabrictestbed-1.5.1/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0     1069 2023-06-17 09:55:40.689347 fabrictestbed-1.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.102597 fabrictestbed-1.5.1/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-05-11 17:40:59.102713 fabrictestbed-1.5.1/test/test_cli.py
--rw-r--r--   0        0        0     6530 1970-01-01 00:00:00.000000 fabrictestbed-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b1/.gitignore
+-rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b1/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b1/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b1/README.md
+-rw-r--r--   0        0        0       24 2023-07-13 18:48:14.169461 fabrictestbed-1.6.0b1/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b1/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    18169 2023-07-13 18:40:33.775336 fabrictestbed-1.6.0b1/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b1/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b1/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b1/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    19830 2023-07-13 18:48:14.174657 fabrictestbed-1.6.0b1/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b1/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.776762 fabrictestbed-1.6.0b1/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     1071 2023-07-13 18:48:30.199529 fabrictestbed-1.6.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b1/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b1/test/test_cli.py
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b1/PKG-INFO
```

### Comparing `fabrictestbed-1.5.1/.gitignore` & `fabrictestbed-1.6.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.1/LICENSE` & `fabrictestbed-1.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.1/README.md` & `fabrictestbed-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.1/fabrictestbed/cli/cli.py` & `fabrictestbed-1.6.0b1/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.1/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.6.0b1/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.1/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.6.0b1/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.1/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.6.0b1/fabrictestbed/slice_manager/slice_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import json
 import os
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from typing import Tuple, Union, List, Any, Dict
 
 import paramiko
 from fabric_cf.orchestrator.swagger_client import Sliver, Slice
 from fabric_cf.orchestrator.swagger_client.models import PoaData
 
 from fabrictestbed.slice_editor import ExperimentTopology, AdvertisedTopology, Node, GraphFormat
@@ -96,15 +96,15 @@
         """
         self.__check_initialized()
 
         id_token = self.get_id_token()
         created_at = self.tokens.get(CredmgrProxy.CREATED_AT, None)
 
         created_at_time = datetime.strptime(created_at, CredmgrProxy.TIME_FORMAT)
-        now = datetime.utcnow()
+        now = datetime.now(timezone.utc)
 
         if id_token is None or now - created_at_time >= timedelta(minutes=30):
             return True
 
         return False
 
     def __load_tokens(self):
```

### Comparing `fabrictestbed-1.5.1/fabrictestbed/util/constants.py` & `fabrictestbed-1.6.0b1/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.1/pyproject.toml` & `fabrictestbed-1.6.0b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dynamic = ["version"]
 
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click",
-    "fabric-credmgr-client==1.5.0",
+    "fabric-credmgr-client==1.6.0b2",
     "fabric-orchestrator-client==1.5.1",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.optional-dependencies]
```

### Comparing `fabrictestbed-1.5.1/test/test_cli.py` & `fabrictestbed-1.6.0b1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.1/PKG-INFO` & `fabrictestbed-1.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.5.1
+Version: 1.6.0b1
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
-Requires-Dist: fabric-credmgr-client==1.5.0
+Requires-Dist: fabric-credmgr-client==1.6.0b2
 Requires-Dist: fabric-orchestrator-client==1.5.1
 Requires-Dist: paramiko
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
```

