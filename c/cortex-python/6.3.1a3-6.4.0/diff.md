# Comparing `tmp/cortex-python-6.3.1a3.tar.gz` & `tmp/cortex-python-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex-python-6.3.1a3.tar", last modified: Wed May  3 15:18:28 2023, max compression
+gzip compressed data, was "cortex-python-6.4.0.tar", last modified: Thu Jul 13 17:40:31 2023, max compression
```

## Comparing `cortex-python-6.3.1a3.tar` & `cortex-python-6.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/
--rw-r--r--   0 root         (0) root         (0)      533 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11368 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4623 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3938 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/cortex/
--rw-r--r--   0 root         (0) root         (0)      877 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/__init__.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/__version__.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/auth.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/camel.py
--rw-r--r--   0 root         (0) root         (0)    27147 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/client.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/connection.py
--rw-r--r--   0 root         (0) root         (0)      684 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/constant.py
--rw-r--r--   0 root         (0) root         (0)     9662 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/content.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/env.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/cortex/experiment/
--rw-r--r--   0 root         (0) root         (0)      675 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7794 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/experiment/local.py
--rw-r--r--   0 root         (0) root         (0)    10770 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/experiment/model.py
--rw-r--r--   0 root         (0) root         (0)    37404 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/experiment/remote.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/message.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/model.py
--rw-r--r--   0 root         (0) root         (0)    10071 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/properties.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/secrets.py
--rw-r--r--   0 root         (0) root         (0)    11705 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/serviceconnector.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/session.py
--rw-r--r--   0 root         (0) root         (0)     8521 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/skill.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/timer.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/types.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/utils.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/cortex_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4623 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2175 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/test/
--rw-r--r--   0 root         (0) root         (0)      590 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/test/unit/
--rw-r--r--   0 root         (0) root         (0)      590 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/authenticationclient_test.py
--rw-r--r--   0 root         (0) root         (0)     4371 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/connectionclient_test.py
--rw-r--r--   0 root         (0) root         (0)     9014 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/cortex_test.py
--rw-r--r--   0 root         (0) root         (0)     5216 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/environment_config_test.py
--rw-r--r--   0 root         (0) root         (0)     6809 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/experiment_test.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/fixtures.py
--rw-r--r--   0 root         (0) root         (0)     8807 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/run_test.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/serviceconnector_test.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/sessionclient_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.683555 cortex-python-6.4.0/
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-13 17:37:47.000000 cortex-python-6.4.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    11368 2023-07-13 17:37:47.000000 cortex-python-6.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-13 17:37:47.000000 cortex-python-6.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-07-13 17:40:31.683555 cortex-python-6.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-07-13 17:37:47.000000 cortex-python-6.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.679555 cortex-python-6.4.0/cortex/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/camel.py
+-rw-r--r--   0 root         (0) root         (0)    27238 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/client.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/connection.py
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/constant.py
+-rw-r--r--   0 root         (0) root         (0)     9669 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/content.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/env.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.679555 cortex-python-6.4.0/cortex/experiment/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/experiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7794 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/experiment/local.py
+-rw-r--r--   0 root         (0) root         (0)    10770 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/experiment/model.py
+-rw-r--r--   0 root         (0) root         (0)    37474 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/experiment/remote.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/message.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/model.py
+-rw-r--r--   0 root         (0) root         (0)    10071 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/properties.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/secrets.py
+-rw-r--r--   0 root         (0) root         (0)    11705 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/serviceconnector.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/session.py
+-rw-r--r--   0 root         (0) root         (0)     8521 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/skill.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/timer.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/types.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.679555 cortex-python-6.4.0/cortex_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 17:40:31.683555 cortex-python-6.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-07-13 17:37:47.000000 cortex-python-6.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.679555 cortex-python-6.4.0/test/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.683555 cortex-python-6.4.0/test/unit/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/authenticationclient_test.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/connectionclient_test.py
+-rw-r--r--   0 root         (0) root         (0)     9029 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/cortex_test.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/environment_config_test.py
+-rw-r--r--   0 root         (0) root         (0)     6424 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/experiment_test.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     8439 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/run_test.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/serviceconnector_test.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/sessionclient_test.py
```

### Comparing `cortex-python-6.3.1a3/LICENSE` & `cortex-python-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/PKG-INFO` & `cortex-python-6.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.3.1a3
+Version: 6.4.0
 Summary: Python module for the CognitiveScale Cortex Cognitive Platform
 Home-page: https://github.com/CognitiveScale/cortex-python
 Author: CognitiveScale
 Author-email: support@cognitivescale.com
 License: Apache 2.0
 Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
 Project-URL: Source, https://github.com/CognitiveScale/cortex-python
```

### Comparing `cortex-python-6.3.1a3/README.md` & `cortex-python-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/__init__.py` & `cortex-python-6.4.0/cortex/experiment/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .client import Cortex
-from .message import Message
-
-from .__version__ import __title__, __description__, __url__, __version__
-from .__version__ import __author__, __author_email__, __license__
-from .__version__ import __copyright__
-
-__all__ = ["__version__", "Cortex", "Message"]
+from .remote import ExperimentClient, Experiment, RemoteRun
+from .model import Run
```

### Comparing `cortex-python-6.3.1a3/cortex/auth.py` & `cortex-python-6.4.0/cortex/auth.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/camel.py` & `cortex-python-6.4.0/cortex/camel.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/client.py` & `cortex-python-6.4.0/cortex/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,39 +69,39 @@
     """
     API client used to access Connections, Managed Content, Experiments, Secrets, Models, Sessions, Skills and Types in a Fabric cluster. Experiments also have a `local client` (:class:`cortex.experiment.local.LocalExperiment`) for data scientists to work without access to a Fabric cluster.
 
     Create an instance of the Cortex Fabric client. There are a few different ways in which you can instantiate a Client
 
     1. If the user has the Cortex CLI installed and configured to a Fabric environment, AND a default project is set, they can do the following:
 
-    >>> from cortex import Cortex; client = Cortex.client()
+    >>> from cortex.client import Cortex; client = Cortex.client()
 
     2. If the user has the Cortex CLI installed and configured, but a default project is not set:
 
-    >>> from cortex import Cortex; client = Cortex.client(project="some-project")
+    >>> from cortex.client import Cortex; client = Cortex.client(project="some-project")
 
     3. If the user does not have the Cortex CLI installed, or is using the cortex-python package from within a Skill (Daemon) running inside a Fabric cluster, they can simply extract the required parameters from the request object and create a Cortex client like below:
 
     .. code-block::
 
-        from cortex import Cortex
+        from cortex.client import Cortex
 
         @app.post('/invoke')
         def start(req: dict):
             payload = req['payload']
             client = Cortex.client(api_endpoint=req["apiEndpoint"], project=req["projectId"], token=req["token"])
             client.experiments.list_experiments()
             ....
 
     4. If the user does not have the Cortex CLI installed, or is using the cortex-python package from within a **Skill(Job)** running inside a Fabric cluster, they can simply pass the `params` object passed into the Job script and create a Cortex client:
 
     .. code-block:: python
 
         # contents of main.py for a Skill (job)
-        from cortex import Cortex
+        from cortex.client import Cortex
 
         def main(params):
             client = Cortex.from_message(params)
 
         if __name__ == "__main__":
             if len(sys.argv)<2:
                 print("Message/payload argument is required")
@@ -190,15 +190,15 @@
 
         If you want to access experiments for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.experiments_client` instead
 
         .. code-block::
 
             ## use default .experiments client helper
-            from cortex import Cortex
+            from cortex.client import Cortex
             client = Cortex.client()
             client.experiments.list_experiments()
             client.experiments.save_experiment()
             client.experiments.list_runs()
             client.experiments.delete_runs()
 
         Refer to the documentation of :class:`cortex.experiment.ExperimentClient` to learn more about the methods available on the ExperimentClient
@@ -228,15 +228,15 @@
 
         If you want to access connections for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.connections_client` instead
 
         .. code-block::
 
             ## use default .connections client helper
-            from cortex import Cortex
+            from cortex.client import Cortex
             client = Cortex.client()
             client.connections.save_connection
             client.connections.get_connection
 
         Refer to the documentation of :class:`cortex.connection.ConnectionClient` to learn more about the methods available on the ConnectionClient
 
         :returns: An instance of this helper class that enables access to the Fabric Connections API.
@@ -264,15 +264,15 @@
 
         If you want to access managed content for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.content_client` instead
 
         .. code-block::
 
             ## use default .content client helper
-            from cortex import Cortex
+            from cortex.client import Cortex
             client = Cortex.client()
             client.content.list
             client.content.upload
             client.content.exists
             .....
 
         Refer to the documentation of :class:`cortex.content.ManagedContentClient` to learn more about the methods available on the ManagedContentClient
@@ -302,15 +302,15 @@
 
         If you want to access models for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.models_client` instead
 
         .. code-block::
 
             ## use default .models client helper
-            from cortex import Cortex
+            from cortex.client import Cortex
             client = Cortex.client()
             client.models.list_models()
             client.models.get_model()
             client.models.save_model()
             .....
 
         Refer to the documentation of :class:`cortex.model.ModelClient` to learn more about the methods available on the ModelClient
@@ -344,15 +344,15 @@
 
         If you want to access secrets for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.secrets_client` instead
 
         .. code-block::
 
             ## use default .secrets client helper
-            from cortex import Cortex
+            from cortex.client import Cortex
             client = Cortex.client()
             client.models.get_secret()
             client.models.post_secret()
             .....
 
         Refer to the documentation of :class:`cortex.secrets.SecretsClient` to learn more about the methods available on the SecretsClient
 
@@ -381,15 +381,15 @@
 
         If you want to access Skills for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.skills_client` instead
 
         .. code-block::
 
             ## use default .skills client helper
-            from cortex import Cortex
+            from cortex.client import Cortex
             client = Cortex.client()
             client.skills.get_skill()
             client.skills.save_skill()
             client.skills.delete_skill()
             client.skills.get_logs()
             client.skills.deploy()
             client.skills.undeploy()
@@ -422,15 +422,15 @@
 
         If you want to access Sessions for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.sessions_client` instead
 
         .. code-block::
 
             ## use default .sessions client helper
-            from cortex import Cortex
+            from cortex.client import Cortex
             client = Cortex.client()
             client.sessions.start_session()
             client.sessions.get_session_data()
             client.sessions.put_session_data()
             client.sessions.delete_session()
             .....
 
@@ -461,15 +461,15 @@
 
         If you want to access Types for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.types_client` instead
 
         .. code-block::
 
             ## use default .types client helper
-            from cortex import Cortex
+            from cortex.client import Cortex
             client = Cortex.client()
             client.types.get_type()
             client.types.save_type()
             .....
 
         Refer to the documentation of :class:`cortex.types.TypeClient` to learn more about the methods available on the TypeClient
 
@@ -541,15 +541,15 @@
 
             You can also set a default project when configuring your Cortex CLI using `cortex configure --project <your-project>`.
 
             This value will be updated into the `$HOME/.cortex/config` file. If your Cortex config file `$HOME/.cortex/config` does not contain a default `project` set for the profile being used as the default one, you will need to set the project key when instantiating a :class:`cortex.client.Client`.
 
         **Example**
 
-        >>> from cortex import Cortex
+        >>> from cortex.client import Cortex
         >>> cortex = Cortex.client(project='example-project')
 
         :param api_endpoint: The Cortex URL.
         :param api_version: The version of the API to use with this client.
         :param verify_ssl_cert: A boolean to enable/disable SSL validation, or path to a CA_BUNDLE file or directory with certificates of trusted CAs (default: True)
         :param project: Cortex Project that you want to use.
         :param token: (optional) Use JWT token for authenticating requests, will default to settings in ~/.cortex/config if not provided
```

### Comparing `cortex-python-6.3.1a3/cortex/connection.py` & `cortex-python-6.4.0/cortex/connection.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/constant.py` & `cortex-python-6.4.0/cortex/constant.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/content.py` & `cortex-python-6.4.0/cortex/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 log = get_logger(__name__)
 
 
 class ManagedContentClient(_Client):
     """
     A client used to access the `Cortex managed content service (blob store) <https://cognitivescale.github.io/cortex-fabric/docs/manage-data/managed-content>`_. You can find a pre-created instance of this class on every :py:class:`cortex.client.Client` instance via the :py:attr:`Client.content` attribute.
 
-    >>> from cortex import Cortex; client = Cortex.client();
+    >>> from cortex.client import Cortex; client = Cortex.client();
     >>> client.content.list() # list content from the default project configured for the user
 
     """  # pylint: disable=line-too-long
 
     URIs = {"content": "projects/{projectId}/content"}
 
     def upload(
```

### Comparing `cortex-python-6.3.1a3/cortex/env.py` & `cortex-python-6.4.0/cortex/env.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/exceptions.py` & `cortex-python-6.4.0/cortex/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/experiment/__init__.py` & `cortex-python-6.4.0/test/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """
 Copyright 2023 Cognitive Scale, Inc. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
-   https://www.apache.org/licenses/LICENSE-2.0
+  https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
-from .remote import ExperimentClient, Experiment, RemoteRun
-from .model import Run
```

### Comparing `cortex-python-6.3.1a3/cortex/experiment/local.py` & `cortex-python-6.4.0/cortex/experiment/local.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/experiment/model.py` & `cortex-python-6.4.0/cortex/experiment/model.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/experiment/remote.py` & `cortex-python-6.4.0/cortex/experiment/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 log = get_logger(__name__)
 
 
 class ExperimentClient(_Client):
     """
     A client for the `Cortex experiment and model management API <https://cognitivescale.github.io/cortex-fabric/docs/models/experiments>`_. You can find a pre-created instance of this class on every :class:`cortex.client.Client` instance via the :attr:`Client.experiments` attribute.
 
-    >>> from cortex import Cortex; client = Cortex.client();
+    >>> from cortex.client import Cortex; client = Cortex.client();
     >>> client.experiments.list_experiments() # list experiments from the default project configured for the user
     """  # pylint: disable=line-too-long
 
     headers = {"Content-Type": "application/json"}
 
     URIs = {
         "experiments": "projects/{projectId}/experiments",
@@ -63,15 +63,15 @@
             "{experimentName}/runs/{runId}/metrics/{metricId}"
         ),
     }
 
     def list_experiments(self) -> List[Dict]:
         """Returns a list of experiments available on the project configured for the experiment client.
 
-        >>> from cortex import Cortex; cc=Cortex.client()
+        >>> from cortex.client import Cortex; cc=Cortex.client()
         >>> cc.experiments.list_experiments()
         [{'_version': 2, 'name': 'op-gc_dtree_exp', 'title': 'Decision Tree model', 'description': 'Decision Tree model', 'meta': None, 'tags': [], 'modelId': 'op-german-credit', 'updatedAt': '2023-01-24T10:21:01.347Z', 'createdAt': '2023-01-24T10:11:16.445Z'}]
 
         :return: A list containing multiple dictionaries, each corresponding to an experiment and all associated metadata
         :rtype: List[Dict]
         """
         res = self._serviceconnector.request(
@@ -81,15 +81,15 @@
         res_json = res.json()
 
         return res_json.get("experiments", [])
 
     def save_experiment(self, experiment_name: str, model_id=None, **kwargs) -> Dict:
         """Save an experiment with the provided `experiment_name`, and `modelId`. All the fields specified in the `API reference for Cortex Experiments <https://cognitivescale.github.io/cortex-fabric/swagger/index.html#operation/CreateExperiment>`_ (except name and modelId) can be passed in as keyword args to this method
 
-        >>> from cortex import Cortex; cc=Cortex.client()
+        >>> from cortex.client import Cortex; cc=Cortex.client()
         >>> cc.experiments.save_experiment('exp-name', 'juhf')
         {'_version': 1, 'name': 'exp-name', 'tags': [], '_projectId': 'exp-test', 'modelId': 'juhf'}
 
         :param experiment_name: Name to use for the new experiment which is to be saved
         :type experiment_name: str
         :param model_id: _description_, defaults to None
         :type model_id: str, optional
@@ -112,15 +112,15 @@
         )
         raise_for_status_with_detail(res)
         return res.json()
 
     def delete_experiment(self, experiment_name: str) -> bool:
         """Delete an experiment specified by `experiment_name`
 
-        >>> from cortex import Cortex; cc=Cortex.client(project='test')
+        >>> from cortex.client import Cortex; cc=Cortex.client(project='test')
         >>> cc.experiments.delete_experiment('another')
         True
 
         :param experiment_name: Name of the experiment to be deleted
         :type experiment_name: str
         :return: A boolean value indicating the status of the delete operation
         :rtype: bool
@@ -133,15 +133,15 @@
         res_json = res.json()
 
         return res_json.get("success", False)
 
     def get_experiment(self, experiment_name: str) -> Dict:
         """Retrieve all data for the experiment with name `experiment_name`
 
-        >>> from cortex import Cortex; cc=Cortex.client()
+        >>> from cortex.client import Cortex; cc=Cortex.client()
         >>> cc.experiments.get_experiment('ddgc_dtree_exp')
         {'_version': 1, 'name': 'ddgc_dtree_exp', 'title': 'Decision Tree model', 'description': 'Decision Tree model', 'tags': [], '_projectId': 'test', 'modelId': 'german-credit-model'}
 
         :param experiment_name: Name of the experiment to retrieve data from
         :type experiment_name: str
         :return: A dictionary with all metadata about the experiment
         :rtype: Dict
@@ -153,15 +153,15 @@
         raise_for_status_with_detail(res)
 
         return res.json()
 
     def list_runs(self, experiment_name: str) -> List[Dict]:
         """`List all the runs <https://cognitivescale.github.io/cortex-fabric/swagger/index.html#operation/ListRuns>`_ that belong to the specified `experiment_name`
 
-        >>> from cortex import Cortex; cc=Cortex.client()
+        >>> from cortex.client import Cortex; cc=Cortex.client()
         >>> cc.experiments.list_runs('op-gc_dtree_exp')
         [{'_id': '63cfb10ffe65fb07bf8a94b9', '_projectId': 'test', 'runId': 'run_01', 'experimentName': 'op-gc_dtree_exp', 'params': {'category': 'Decision Tree', 'version': 1, 'SourceData': 'Upstream Server Data'}, 'metrics': {'accuracy': 0.68}, 'meta': {'algo': 'DecisionTreeClassifier'}, '_createdAt': '2023-01-24T10:21:03.120Z', '_updatedAt': '2023-01-24T10:21:04.497Z', 'artifacts': {'model': 'experiments/op-gc_dtree_exp/run_01/artifacts/model'}}]
 
         :param experiment_name: Experiment name whose runs are to be listed
         :type experiment_name: str
         :return: A List of dictionaries that contain the information available for each run of that experiment
         :rtype: List[Dict]
@@ -176,15 +176,15 @@
         return res_json.get("runs", [])
 
     def find_runs(
         self, experiment_name: str, filter_obj: Dict, sort: dict = None, limit=25
     ) -> List[Dict]:
         """Similar to :meth:`cortex.experiment.ExperimentClient.list_runs`, but also allows you to filter with a mongo-style query dictionary passed in through `filter_obj`, along with `sort` and `limit` options
 
-        >>> from cortex import Cortex; cc=Cortex.client()
+        >>> from cortex.client import Cortex; cc=Cortex.client()
         >>> cc.experiments.find_runs('op-gc_dtree_exp', filter_obj={"runId": "run_01"})
         [{'_id': '63cfb10ffe65fb07bf8a94b9', '_projectId': 'test', 'runId': 'run_01', 'experimentName': 'op-gc_dtree_exp', 'params': {'category': 'Decision Tree', 'version': 1, 'SourceData': 'Upstream Server Data'}, 'metrics': {'accuracy': 0.68}, 'meta': {'algo': 'DecisionTreeClassifier'}, '_createdAt': '2023-01-24T10:21:03.120Z', '_updatedAt': '2023-01-24T10:21:04.497Z', 'artifacts': {'model': 'experiments/op-gc_dtree_exp/run_01/artifacts/model'}}]
 
         :param experiment_name: Name of the experiment whose runs are to be filtered
         :type experiment_name: str
         :param filter_obj: A mongo style query object. For example. `{"runId": "run_01"}`. Allowed fields which can be set as keys in this dictionary include [runId, _createdAt, startTime, endTime, took, experimentName]
         :type filter_obj: Dict
@@ -215,15 +215,15 @@
     def delete_runs(
         self,
         experiment_name,
         filter_obj: Dict = None,
     ) -> str:
         """Delete runs belonging to the specified `experiment_name` that match the optional `filter_obj` conditions
 
-        >>> from cortex import Cortex; cc=Cortex.client(project='test')
+        >>> from cortex.client import Cortex; cc=Cortex.client(project='test')
         >>> cc.experiments.delete_runs('op-gc_dtree_exp')
         'Runs deleted'
 
         :param experiment_name: Name of the experiment whose runs are to be deleted
         :type experiment_name: str
         :param filter_obj: A mongo style query object. For example. `{"runId": "run_01"}`. Allowed fields which can be set as keys in this dictionary include [runId, _createdAt, startTime, endTime, took, experimentName]
         :type filter_obj: Dict
@@ -246,15 +246,15 @@
         res_json = res.json()
 
         return res_json.get("message")
 
     def create_run(self, experiment_name: str, **kwargs) -> Dict:
         """Creates a run for the specified `experiment_name`. Refer to the `official CreateRun docs <https://cognitivescale.github.io/cortex-fabric/swagger/index.html#operation/CreateRun>`_ for information on other possible `kwargs` this method can accept
 
-        >>> from cortex import Cortex; cc=Cortex.client(project='test')
+        >>> from cortex.client import Cortex; cc=Cortex.client(project='test')
         >>> cc.experiments.create_run('op-gc_dtree_exp')
         {'_projectId': 'test', 'runId': 'ox00gu0', 'experimentName': 'op-gc_dtree_exp', '_id': '63f0f9e809c5267ccb9110ca', '_createdAt': '2023-02-18T16:16:40.405Z', '_updatedAt': '2023-02-18T16:16:40.405Z'}
 
         :raises: :exc:`requests.exceptions.HTTPError`
         :param experiment_name: The experiment to associate with this run.
         :type experiment_name: str
         :return: A dictionary providing a JSON representation of the created run
@@ -275,15 +275,15 @@
         )
         raise_for_status_with_detail(res)
         return res.json()
 
     def get_run(self, experiment_name: str, run_id: str) -> Dict:
         """Get all details available for a `run_id` belonging to an `experiment_name`
 
-        >>> from cortex import Cortex; cc=Cortex.client(project='test')
+        >>> from cortex.client import Cortex; cc=Cortex.client(project='test')
         >>> cc.experiments.get_run('op-gc_dtree_exp', 'ox00gu0')
         {'_id': '63f0f9e809c5267ccb9110ca', '_projectId': 'test', 'runId': 'ox00gu0', 'experimentName': 'op-gc_dtree_exp', '_createdAt': '2023-02-18T16:16:40.405Z', '_updatedAt': '2023-02-18T16:16:40.405Z'}
 
         :raises: :exc:`requests.exceptions.HTTPError`
         :param experiment_name: Name of the experiment whose run is to be retrieved
         :type experiment_name: str
         :param run_id: ID of the Run to be retrieved
```

### Comparing `cortex-python-6.3.1a3/cortex/message.py` & `cortex-python-6.4.0/cortex/message.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/model.py` & `cortex-python-6.4.0/cortex/model.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/properties.py` & `cortex-python-6.4.0/cortex/properties.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/secrets.py` & `cortex-python-6.4.0/cortex/secrets.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/serviceconnector.py` & `cortex-python-6.4.0/cortex/serviceconnector.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/session.py` & `cortex-python-6.4.0/cortex/session.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/skill.py` & `cortex-python-6.4.0/cortex/skill.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/timer.py` & `cortex-python-6.4.0/cortex/timer.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/types.py` & `cortex-python-6.4.0/cortex/types.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/utils.py` & `cortex-python-6.4.0/cortex/utils.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex/viz.py` & `cortex-python-6.4.0/cortex/viz.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/cortex_python.egg-info/PKG-INFO` & `cortex-python-6.4.0/cortex_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.3.1a3
+Version: 6.4.0
 Summary: Python module for the CognitiveScale Cortex Cognitive Platform
 Home-page: https://github.com/CognitiveScale/cortex-python
 Author: CognitiveScale
 Author-email: support@cognitivescale.com
 License: Apache 2.0
 Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
 Project-URL: Source, https://github.com/CognitiveScale/cortex-python
```

### Comparing `cortex-python-6.3.1a3/cortex_python.egg-info/SOURCES.txt` & `cortex-python-6.4.0/cortex_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/setup.py` & `cortex-python-6.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,14 @@
         "cuid>=0.3,<1",
         "dill>=0.2.8.2",
     ],
     extras_require={
         "viz": ["matplotlib>=2.2.2,<3", "seaborn>=0.9.0,<0.10", "pandas"],
         "jupyter": ["ipython>=6.4.0,<7", "maya>=0.5.0", "jinja2"],
     },
-    tests_require=["mocket>=3.9.0,<4.0", "pytest>=7.2.1,<8"],
+    tests_require=["requests-mock>=1.10.0", "pytest>=7.2.1,<8"],
     classifiers=[
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3.6",
     ],
 )
```

### Comparing `cortex-python-6.3.1a3/test/__init__.py` & `cortex-python-6.4.0/test/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/test/unit/authenticationclient_test.py` & `cortex-python-6.4.0/test/unit/authenticationclient_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import unittest
-
-from mocket import mocketize
+import requests_mock
 
 from cortex.auth import AuthenticationClient
 from cortex.utils import decode_JWT, verify_JWT
 from .fixtures import mock_pat_config, mock_api_endpoint, register_mock_fabric_info
 
 
+@requests_mock.Mocker()
 class TestAuthenticationClient(unittest.TestCase):
     def setUp(self):
-        register_mock_fabric_info()
-        self.ac = AuthenticationClient()
+        pass
 
-    @mocketize
-    def test_contructor_with_args(self):
+    def test_contructor_with_args(self, m):
         # This client doesn't need parameters, but allow them for backward compat
+        register_mock_fabric_info(m)
         ac = AuthenticationClient(mock_api_endpoint(), 4)
         jwt = ac.fetch_auth_token(mock_pat_config())
 
-    @mocketize
-    def test_fetch_auth_token(self):
+    def test_fetch_auth_token(self, m):
+        register_mock_fabric_info(m)
+        self.ac = AuthenticationClient()
         # setup
         # uri = self.ac.URIs['authenticate'].format(projectId='cogscale')
         # url = self.ac._serviceconnector._construct_url(uri)
         body = mock_pat_config()
         # Entry.single_register(Entry.POST,
         #                       url,
         #                       status = 200,
@@ -46,12 +46,11 @@
         # execute
         # todo mock this call?..
         token = self.ac.fetch_auth_token(body)
         # test
         decodedbody = decode_JWT(token)
         self.assertEqual(body["issuer"], decodedbody[1]["iss"])
 
-    @mocketize
-    def test_expired_token(self):
+    def test_expired_token(self, m):
         # Shouldn't fail to validate expired token WITHIN the python lib, this is responsibiltiy of auth proxy...
         exp_token = "eyJhbGciOiJFZERTQSIsImtpZCI6IkhwVy15YTdGU1U3eVYtYWx6eWV3UFBEd1BlRmdya2kwVlFQS2JoNEo0UHciLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJjb3J0ZXgiLCJleHAiOjE2MzAzNDgxOTYsImlhdCI6MTYzMDM0ODE2NiwiaXNzIjoiY29nbml0aXZlc2NhbGUuY29tIiwianRpIjoiU0dkRjVidG1fUXlYcjZhMVRrOU9oZyIsIm5iZiI6MTYzMDM0ODE2Niwic3ViIjoiNzFhOGZhYWMtOWRmYi00MjhkLWE5MGMtMGI1MzQ4MWI4NjY1In0.pB7hvEcIMV1Qt6GTGPGcKbS1zhidPMJ-luV-KBOaHrwgCh2jDOQdve2Sv5RqmNa6Jkk-Bxh-1g4XG8CxGGSqAQ"
         verify_JWT(exp_token)
```

### Comparing `cortex-python-6.3.1a3/test/unit/connectionclient_test.py` & `cortex-python-6.4.0/test/unit/connectionclient_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,108 +11,96 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from io import BytesIO, StringIO
-import json
 import unittest
-
-from mocket.mockhttp import Entry
-from mocket import mocketize
+import requests_mock
 
 from cortex.connection import ConnectionClient
 from cortex.content import ManagedContentClient
-from cortex import Cortex
+from cortex.client import Cortex
 
 from .fixtures import john_doe_token, mock_api_endpoint, mock_project
 
 projectId = mock_project()
 url = mock_api_endpoint()
-TOKEN = john_doe_token()
+TOKEN=''
+with requests_mock.Mocker() as m:
+    TOKEN = john_doe_token(m)
 
 
+@requests_mock.Mocker()
 class TestConnectionClient(unittest.TestCase):
     def setUp(self):
         params = {"token": TOKEN, "projectId": projectId, "apiEndpoint": url}
         self.cc = ConnectionClient(url, token=TOKEN, project=projectId)
         self.mc = ManagedContentClient(url, token=TOKEN, project=projectId)
         self.client = Cortex.from_message(params)
         self.mcFromClient = ManagedContentClient(self.client)
 
-    @mocketize
-    def test_save_connection(self):
+    def test_save_connection(self, m):
         uri = self.cc.URIs["connections"].format(projectId=projectId)
         url = self.cc._serviceconnector._construct_url(uri)
         connection = {"connectionType": "ctype", "name": "cname"}
-        Entry.single_register(Entry.POST, url, status=200, body=json.dumps(connection))
+        m.post(url, status_code=200, json=connection)
         r = self.cc.save_connection(connection=connection)
         self.assertEqual(r, connection)
 
-    @mocketize
-    def test_upload(self):
+    def test_upload(self, m):
         key = "some-key"
         result = {"Key": key}
         uri = self.mc.URIs["content"].format(projectId=projectId)
         local_url = self.mc._serviceconnector._construct_url(uri)
         with BytesIO(b"arbitrary content") as content:
-            Entry.single_register(
-                Entry.POST, local_url, status=200, body=json.dumps(result)
-            )
+            m.post(local_url, status_code=200, json=result)
             res = self.mc.upload(
                 key=key,
                 stream_name="foo",
                 stream=content,
                 content_type="application/octet-stream",
             )
             self.assertEqual(res, result)
 
         with StringIO("arbitrary content") as content:
-            Entry.single_register(
-                Entry.POST, local_url, status=200, body=json.dumps(result)
-            )
+            m.post(local_url, status_code=200, json=result)
             res = self.mc.upload(
                 key=key,
                 stream_name="foo",
                 stream=content,
                 content_type="application/text",
             )
             self.assertEqual(res, result)
 
-    @mocketize
-    def test_uploadStreaming(self):
+    def test_uploadStreaming(self, m):
         key = "some-key"
         result = {"Key": key}
         uri = "{0}/{1}".format(self.mc.URIs["content"].format(projectId=projectId), key)
         local_url = self.mc._serviceconnector._construct_url(uri)
 
         with BytesIO(b"arbitrary content") as content:
-            Entry.single_register(
-                Entry.POST, local_url, status=200, body=json.dumps(result)
-            )
+            m.post(local_url, status_code=200, json=result)
             r = self.mc.upload_streaming(
                 key=key, stream=content, content_type="application/octet-stream"
             )
             self.assertEqual(r, result)
 
-    @mocketize
-    def test_download(self):
+    def test_download(self, m):
         key = "some-key"
         uri = "{0}/{1}".format(self.mc.URIs["content"].format(projectId=projectId), key)
         local_url = self.mc._serviceconnector._construct_url(uri)
         buf = b"arbitrary content"
         with BytesIO(buf) as content:
-            Entry.single_register(Entry.GET, local_url, status=200, body=content)
+            m.get(local_url, status_code=200, body=content)
             r = self.mc.download(key=key)
             self.assertEqual(r.read(), buf)
 
-    @mocketize
-    def test_exists(self):
+    def test_exists(self, m):
         key = "some-key"
         result = {"Key": key}
         uri = "{0}/{1}".format(self.mc.URIs["content"].format(projectId=projectId), key)
         url = self.cc._serviceconnector._construct_url(uri)
-        Entry.single_register(Entry.HEAD, url, status=200, body=json.dumps(result))
-
+        m.head(url, status_code=200, json=result)
         r = self.mc.exists(key=key)
         self.assertTrue(r)
```

### Comparing `cortex-python-6.3.1a3/test/unit/cortex_test.py` & `cortex-python-6.4.0/test/unit/cortex_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,34 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import unittest
 
 from unittest.mock import Mock
-from mocket.mockhttp import Entry
-from mocket import mocketize
 
-from cortex import Cortex
+import requests_mock
+
+from cortex.client import Cortex
 from cortex.message import Message
 import pytest
 from cortex.connection import ConnectionClient, Connection
 from cortex.content import ManagedContentClient
 from cortex.experiment import ExperimentClient, Experiment
 from cortex.model import ModelClient, Model
 from cortex.secrets import SecretsClient, Secret
 from cortex.session import SessionClient, Session
 from cortex.types import TypeClient, Type
 from cortex.skill import SkillClient, Skill
 
 from .fixtures import john_doe_subject, john_doe_token, mock_api_endpoint
 
-token = john_doe_token()
+token =''
+with requests_mock.Mocker() as m:
+    token = john_doe_token(m)
 api_endpoint = mock_api_endpoint()
 api_version = 4
 
 
 class TestCortex(unittest.TestCase):
     def test_client(self):
         account = "unittest"
```

### Comparing `cortex-python-6.3.1a3/test/unit/environment_config_test.py` & `cortex-python-6.4.0/test/unit/environment_config_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a3/test/unit/experiment_test.py` & `cortex-python-6.4.0/test/unit/experiment_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,110 +14,99 @@
 limitations under the License.
 """
 
 import unittest
 import json
 import os
 
-from cortex import Cortex
+import requests_mock
+
+from cortex.client import Cortex
 from cortex.experiment import ExperimentClient, Experiment
 
-from mocket.mockhttp import Entry
-from mocket import mocketize
 from .fixtures import mock_api_endpoint, mock_project
 from .fixtures import john_doe_token
 
 import dill
 
-TOKEN = john_doe_token()
+TOKEN=''
+with requests_mock.Mocker() as m:
+    TOKEN = john_doe_token(m)
 projectId = mock_project()
 url = mock_api_endpoint()
 params = {"token": TOKEN, "projectId": projectId, "apiEndpoint": url}
 
 
+@requests_mock.Mocker()
 class TestExperiment(unittest.TestCase):
     """
     Test experiment checks experiment functionality
     """
 
     # values for testing experiments
     EXP_NAME = "unittest-exp"
 
     def setUp(self):
         self.cortex = Cortex.from_message(params)
         self.expc = ExperimentClient(self.cortex)
         self.local = Cortex.local()
         self.local_tmp = Cortex.local("/tmp/cortex")
 
-    @mocketize
-    def test_get_remote_experiment(self):
+    def test_get_remote_experiment(self, m):
         uri = self.cortex.experiments.URIs["experiment"].format(
             experimentName=self.EXP_NAME, projectId=projectId
         )
         local_url = self.cortex.experiments._serviceconnector._construct_url(uri)
         returns = {"name": self.EXP_NAME}
-        Entry.single_register(
-            Entry.GET, local_url, status=200, body=json.dumps(returns)
-        )
+        m.get(local_url, status_code=200, json=returns)
 
         exp = self.cortex.experiments.get_experiment(self.EXP_NAME)
         self.assertNotEqual(exp, None)
 
-    @mocketize
-    def test_list_remote_experiments(self):
+    def test_list_remote_experiments(self, m):
         uri = self.cortex.experiments.URIs["experiments"].format(projectId=projectId)
         local_url = self.cortex.experiments._serviceconnector._construct_url(uri)
         returns = {"experiments": [{"name": self.EXP_NAME}]}
-        Entry.single_register(
-            Entry.GET, local_url, status=200, body=json.dumps(returns)
-        )
+        m.get(local_url, status_code=200, json=returns)
         exps = self.cortex.experiments.list_experiments()
 
         self.assertNotEqual(exps, None)
         self.assertIsInstance(exps, list)
 
-    @mocketize
-    def test_make_remote_experiment(self):
+    def test_make_remote_experiment(self, m):
         uri = self.cortex.experiments.URIs["experiments"].format(projectId=projectId)
         local_url = self.cortex.experiments._serviceconnector._construct_url(uri)
         returns = {"name": self.EXP_NAME}
-        Entry.single_register(
-            Entry.POST, local_url, status=200, body=json.dumps(returns)
-        )
+        m.post(local_url, status_code=200, json=returns)
         exp = Experiment(
             document=self.cortex.experiments.save_experiment(self.EXP_NAME),
             client=self.cortex.experiments,
         )
         self.assertNotEqual(exp, None)
         self.assertIsInstance(exp, Experiment)
 
-    @mocketize
-    def test_make_local_experiment(self):
+    def test_make_local_experiment(self, m):
         uri = ExperimentClient.URIs["experiment"].format(
             experimentName=self.EXP_NAME, projectId=projectId
         )
         returns = {"name": self.EXP_NAME}
-        Entry.single_register(Entry.GET, uri, status=200, body=json.dumps(returns))
+        m.get(uri, status_code=200, json=returns)
         exp = self.local.experiment(self.EXP_NAME)
         self.assertNotEqual(exp, None)
 
-    @mocketize
-    def test_make_local_experiment_custom_basedir(self):
+    def test_make_local_experiment_custom_basedir(self, m):
         exp = self.local_tmp.experiment(self.EXP_NAME)
         self.assertNotEqual(exp, None)
         self.assertTrue(os.path.isdir(f"/tmp/cortex/local/experiments/{self.EXP_NAME}"))
 
-    @mocketize
-    def test_remote_load_artifact(self):
+    def test_remote_load_artifact(self, m):
         uri = self.cortex.experiments.URIs["experiments"].format(projectId=projectId)
         local_url = self.expc._serviceconnector._construct_url(uri)
         returns = {"name": self.EXP_NAME}
-        Entry.single_register(
-            Entry.POST, local_url, status=200, body=json.dumps(returns)
-        )
+        m.post(local_url, status_code=200, json=returns)
 
         exp = Experiment(
             document=self.cortex.experiments.save_experiment(
                 experiment_name=self.EXP_NAME
             ),
             client=self.cortex.experiments,
         )
@@ -126,40 +115,34 @@
         # register mock for creating a run
         uri = ExperimentClient.URIs["runs"].format(
             projectId=projectId, experimentName=self.EXP_NAME
         )
         local_url = self.expc._serviceconnector._construct_url(uri)
         run_id = "000001"
         returns = {"runId": run_id}
-        Entry.single_register(
-            Entry.POST, local_url, status=200, body=json.dumps(returns)
-        )
-
+        m.post(local_url, status_code=200, json=returns)
         run = exp.start_run()
         # make an artifact
         my_dictionary = {"a_thing": 1, "another_thing": 2}
 
         # get the artifact & test if it is what is expected
         # register mock for loading an artifact
         uri = ExperimentClient.URIs["artifact"].format(
             experimentName=self.EXP_NAME,
             runId=run_id,
             artifactId="my_dictionary",
             projectId=projectId,
         )
         local_url = self.expc._serviceconnector._construct_url(uri)
-
-        Entry.single_register(
-            Entry.GET, local_url, status=200, body=dill.dumps(my_dictionary)
-        )
+        m.get(local_url, status_code=200, content=dill.dumps(my_dictionary))
 
         result = exp.load_artifact(run, "my_dictionary")
         self.assertEqual(result, my_dictionary)
 
-    def test_save_multiple_local_experiments(self):
+    def test_save_multiple_local_experiments(self, m):
         exp = self.local.experiment(self.EXP_NAME)
         exp.reset()
         run_a = self.make_run(exp)
         run_b = self.make_run(exp)
 
         self.assertTrue(len(exp.runs()) == 2)
 
@@ -169,15 +152,15 @@
 
         # Are runs gone after reset and retrival?
         exp.reset()
 
         exp = self.local.experiment(self.EXP_NAME)
         self.assertTrue(len(exp.runs()) == 0)
 
-    def test_reset_works_in_context(self):
+    def test_reset_works_in_context(self, m):
         exp = self.local.experiment(self.EXP_NAME)
         exp.reset()
         exp.set_meta("style", "supervised")
         exp.set_meta("function", "regression")
         test_artifact = {"model": {}}
         with exp.start_run() as run:
             run.log_artifact("test", test_artifact)
```

### Comparing `cortex-python-6.3.1a3/test/unit/fixtures.py` & `cortex-python-6.4.0/test/unit/fixtures.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 """
 functions for mocking connection to cortex for testing 
 """
 
 import json
 
-from mocket import mocketize
-
 from cortex.utils import generate_token
 from datetime import datetime
 import calendar
-from mocket.mockhttp import Entry
 
 
-@mocketize
-def john_doe_token():
-    register_mock_fabric_info()
+def john_doe_token(mock):
+    register_mock_fabric_info(mock)
     return generate_token(mock_pat_config())
 
 
-def register_mock_fabric_info(base_url=None):
+def register_mock_fabric_info(mock, base_url=None):
     """_summary_
 
     :param url: _description_, defaults to None
     :type url: _type_, optional
     """
     url = None
     if base_url is None:
         url = build_mock_url("info")
     else:
         url = f"{base_url}/fabric/v4/info"
-    Entry.single_register("GET", url, status=200, body=json.dumps(fabric_info_resp()))
+    mock.get(url, status_code=200, json=fabric_info_resp())
 
 
 def fabric_info_resp() -> dict:
     """Mock Fabric info response
 
     :return: dict with fabric info response
     :rtype: dict
@@ -85,24 +81,14 @@
 def mock_project():
     """
     the project for mocking
     """
     return "cogscale"
 
 
-def register_entry(verb, url, body: dict):
-    print("Registering mock for", verb, url)
-    Entry.single_register(verb, url, status=200, body=json.dumps(body))
-
-
-def register_entry_from_path(verb, url, path: str):
-    with open(path) as fh:
-        register_entry(verb, url, json.load(fh))
-
-
 def mock_pat_config():
     """
     Return a PAt config to allow test and create new JWTs
     :return: PAT config
     """
     return {
         "jwk": {
```

### Comparing `cortex-python-6.3.1a3/test/unit/run_test.py` & `cortex-python-6.4.0/test/unit/run_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,76 +11,75 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import unittest
-import json
 
 import dill
-from mocket.mockhttp import Entry
-from mocket import mocketize
+import requests_mock
 
 from pytest import raises
 from requests.exceptions import HTTPError
 
-from cortex import Cortex
+from cortex.client import Cortex
 from cortex.experiment import ExperimentClient, RemoteRun, Experiment
 from .fixtures import build_mock_url, mock_api_endpoint, mock_project, john_doe_token
 
 PROJECT = mock_project()
-TOKEN = john_doe_token()
+TOKEN='';
+with requests_mock.Mocker() as m:
+    TOKEN = john_doe_token(m)
+
 url = mock_api_endpoint()
 
 
+@requests_mock.Mocker()
 class TestRun(unittest.TestCase):
     """
     Test experiment checks experiment functionality
     """
 
     RUN_EXP_NAME = "unittest-exp"
     RUN_ID = "000001"
 
-    def setUp(self):
-        params = {"token": TOKEN, "projectId": PROJECT, "apiEndpoint": url}
-        self.local = Cortex.local()
-        self.cortex = Cortex.from_message(params)
-
+    def registerMocks(self, m):
         # register mock for getting an experiment from the client
         uri = ExperimentClient.URIs["experiment"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT
         )
         returns = {"name": self.RUN_EXP_NAME}
-        Entry.single_register(
-            Entry.GET, build_mock_url(uri), status=200, body=json.dumps(returns)
-        )
-
+        m.get(build_mock_url(uri), status_code=200, json=returns)
         # register mock for creating a run
         uri = ExperimentClient.URIs["runs"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT
         )
 
         returns = {"runId": self.RUN_ID}
-        Entry.single_register(
-            Entry.POST, build_mock_url(uri), status=200, body=json.dumps(returns)
-        )
+        m.post(build_mock_url(uri), status_code=200, json=returns)
 
-    @mocketize
-    def test_make_remote_run(self):
+    def setUp(self):
+        params = {"token": TOKEN, "projectId": PROJECT, "apiEndpoint": url}
+        self.local = Cortex.local()
+        self.cortex = Cortex.from_message(params)
+
+
+    def test_make_remote_run(self, m):
+        self.registerMocks(m);
         exp = Experiment(
             document=self.cortex.experiments.get_experiment(self.RUN_EXP_NAME),
             client=self.cortex.experiments,
         )
         r = exp.start_run()
 
         self.assertIsInstance(r, RemoteRun)
 
-    @mocketize
-    def test_get_run(self):
+    def test_get_run(self, m):
+        self.registerMocks(m);
         exp = Experiment(
             document=self.cortex.experiments.get_experiment(self.RUN_EXP_NAME),
             client=self.cortex.experiments,
         )
 
         uri = self.cortex.experiments.URIs["run"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT, runId=self.RUN_ID
@@ -100,41 +99,37 @@
             "_createdAt": "2023-01-24T10:21:03.120Z",
             "_updatedAt": "2023-01-24T10:21:04.497Z",
             "artifacts": {
                 "model": "experiments/praj-op-gc_dtree_exp/run_01/artifacts/model"
             },
         }
 
-        Entry.single_register(
-            Entry.GET, build_mock_url(uri), status=200, body=json.dumps(returns)
-        )
-
+        m.get(build_mock_url(uri), status_code=200, json=returns)
         ret = self.cortex.experiments.get_run(self.RUN_EXP_NAME, self.RUN_ID)
         self.assertEqual(returns, ret)
 
-    @mocketize
-    def test_get_run_failed(self):
+    def test_get_run_failed(self, m):
+        self.registerMocks(m);
         exp = Experiment(
             document=self.cortex.experiments.get_experiment(self.RUN_EXP_NAME),
             client=self.cortex.experiments,
         )
 
         uri = self.cortex.experiments.URIs["run"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT, runId=self.RUN_ID
         )
         returns = "error"
 
-        Entry.single_register(
-            Entry.GET, build_mock_url(uri), status=404, body=json.dumps(returns)
-        )
+        m.get(build_mock_url(uri), status_code=404, json=returns)
+
         with raises(HTTPError) as ex:
             ret = self.cortex.experiments.get_run(self.RUN_EXP_NAME, self.RUN_ID)
 
-    @mocketize
-    def test_run_get_artifact(self):
+    def test_run_get_artifact(self, m):
+        self.registerMocks(m);
         exp = Experiment(
             document=self.cortex.experiments.get_experiment(self.RUN_EXP_NAME),
             client=self.cortex.experiments,
         )
         r = exp.start_run()
 
         test_artifact = {"a": 0.7071, "b": 1.4142, "c": 2.718}
@@ -143,23 +138,20 @@
         # register mock for loading an artifact
         uri = ExperimentClient.URIs["artifact"].format(
             experimentName=self.RUN_EXP_NAME,
             runId=self.RUN_ID,
             artifactId="artifact",
             projectId=PROJECT,
         )
-        Entry.single_register(
-            Entry.GET, build_mock_url(uri), status=200, body=dill.dumps(test_artifact)
-        )
+        m.get(build_mock_url(uri), status_code=200, content=dill.dumps(test_artifact))
         result = r.get_artifact("artifact")
 
         self.assertEqual(test_artifact, result)
 
-    @mocketize
-    def test_list_runs(self):
+    def test_list_runs(self, m):
         uri = self.cortex.experiments.URIs["runs"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT
         )
         local_url = self.cortex.experiments._serviceconnector._construct_url(uri)
         returns = {
             "runs": {
                 "_id": "63cfb10ffe65fb07bf8a94b9",
@@ -177,76 +169,65 @@
                 "_updatedAt": "2023-01-24T10:21:04.497Z",
                 "artifacts": {
                     "model": "experiments/praj-op-gc_dtree_exp/run_01/artifacts/model"
                 },
             }
         }
 
-        Entry.single_register(
-            Entry.GET, local_url, status=200, body=json.dumps(returns)
-        )
-
+        m.get(build_mock_url(uri), status_code=200, json=returns)
         runs = self.cortex.experiments.list_runs(experiment_name=self.RUN_EXP_NAME)
 
         self.assertNotEqual(runs, None)
 
-    @mocketize
-    def test_update_run(self):
+    def test_update_run(self, m):
         uri = self.cortex.experiments.URIs["run"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT, runId=self.RUN_ID
         )
         local_url = self.cortex.experiments._serviceconnector._construct_url(uri)
 
         body = {"success": True}
-        Entry.single_register(Entry.PUT, local_url, status=200, body=json.dumps(body))
+        m.put(build_mock_url(uri), status_code=200, json=body)
 
         ret = self.cortex.experiments.update_run(
             experiment_name=self.RUN_EXP_NAME, run_id=self.RUN_ID, meta={"blah": 1}
         )
         self.assertEqual(ret, True)
 
-    @mocketize
-    def test_update_run_failed(self):
+    def test_update_run_failed(self, m):
         uri = self.cortex.experiments.URIs["run"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT, runId=self.RUN_ID
         )
         local_url = self.cortex.experiments._serviceconnector._construct_url(uri)
 
         body = {"success": False}
-        Entry.single_register(Entry.PUT, local_url, status=200, body=json.dumps(body))
+        m.put(local_url, status_code=200, json=body)
         with raises(Exception) as ex:
             ret = self.cortex.experiments.update_run(
                 experiment_name=self.RUN_EXP_NAME, run_id=self.RUN_ID, meta={"blah": 1}
             )
 
-    @mocketize
-    def test_delete_run(self):
+    def test_delete_run(self, m):
         uri = self.cortex.experiments.URIs["run"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT, runId=self.RUN_ID
         )
         local_url = self.cortex.experiments._serviceconnector._construct_url(uri)
 
         body = {"success": True}
-        Entry.single_register(
-            Entry.DELETE, local_url, status=200, body=json.dumps(body)
-        )
+        m.delete(local_url, status_code=200, json=body)
 
         ret = self.cortex.experiments.delete_run(
             experiment_name=self.RUN_EXP_NAME, run_id=self.RUN_ID
         )
         self.assertTrue(ret)
 
-    @mocketize
-    def test_delete_run_failed(self):
+    def test_delete_run_failed(self, m):
         uri = self.cortex.experiments.URIs["run"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT, runId=self.RUN_ID
         )
         local_url = self.cortex.experiments._serviceconnector._construct_url(uri)
 
-        body = {"success": False}
-        Entry.single_register(
-            Entry.DELETE, local_url, status=200, body=json.dumps(body)
-        )
+        body = {"success": False} # TODO validate should this be a 200 ?
+        m.delete(local_url, status_code=200, json=body)
         with raises(Exception) as ex:
             self.cortex.experiments.delete_run(
                 experiment_name=self.RUN_EXP_NAME, run_id=self.RUN_ID
             )
```

### Comparing `cortex-python-6.3.1a3/test/unit/sessionclient_test.py` & `cortex-python-6.4.0/test/unit/sessionclient_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,90 +10,85 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import json
 import unittest
 import uuid
-from mocket.mockhttp import Entry
-from mocket import mocketize
+import requests_mock
 
 from cortex.session import SessionClient
-from cortex import Cortex
+from cortex.client import Cortex
 
 from .fixtures import john_doe_token, mock_api_endpoint, mock_project
 
 projectId = mock_project()
 url = mock_api_endpoint()
-TOKEN = john_doe_token()
 
+TOKEN=''
+with requests_mock.Mocker() as m:
+    TOKEN = john_doe_token(m)
 
+
+@requests_mock.Mocker()
 class TestSessionClient(unittest.TestCase):
     def setUp(self):
         params = {"token": TOKEN, "projectId": projectId, "apiEndpoint": url}
         self.client = SessionClient(Cortex.from_message(params))
         self.session_id = str(uuid.uuid4())
 
-    def register_entry(self, verb, uri, body):
+    def register_entry(self, m, verb, uri, body):
         url = self.client._serviceconnector._construct_url(uri)
-        Entry.single_register(verb, url, status=200, body=json.dumps(body))
-
+        m.register_uri(verb, url, status_code=200, json=body)
+    
     # Sessions #
-
-    @mocketize
-    def test_start_sessions(self):
+    def test_start_sessions(self, m):
         uri = self.client.URIs["start"].format(projectId=projectId)
         returns = {"sessionId": self.session_id}
-        self.register_entry(Entry.POST, uri, returns)
-
+        self.register_entry(m, 'POST', uri, returns)
         r = self.client.start_session(100, "test")
         self.assertEqual(r, self.session_id)
 
-    @mocketize
-    def test_get_all(self):
+    def test_get_all(self, m):
         uri = self.client.URIs["get"].format(
             sessionId=self.session_id, projectId=projectId
         )
         returns = {"state": {"key1": "value1"}}
-        self.register_entry(Entry.GET, uri, returns)
+        self.register_entry(m, 'GET', uri, returns)
 
         r = self.client.get_session_data(self.session_id, None)
         self.assertEqual(r, returns["state"])
 
-    @mocketize
-    def test_get_by_key(self):
+    def test_get_by_key(self, m):
         uri = (
             self.client.URIs["get"].format(
                 sessionId=self.session_id, projectId=projectId
             )
             + "?key=key1"
         )
         returns = {"state": {"key1": "value1"}}
-        self.register_entry(Entry.GET, uri, returns)
+        self.register_entry(m, 'GET', uri, returns)
 
         r = self.client.get_session_data(self.session_id, "key1")
         self.assertEqual(r, returns["state"])
 
-    @mocketize
-    def test_put(self):
+    def test_put(self, m):
         uri = self.client.URIs["put"].format(
             sessionId=self.session_id, projectId=projectId
         )
         returns = {}
-        self.register_entry(Entry.POST, uri, returns)
+        self.register_entry(m, 'POST', uri, returns)
 
         r = self.client.put_session_data(self.session_id, {})
         self.assertEqual(r, returns)
 
-    @mocketize
-    def test_delete(self):
+    def test_delete(self, m):
         uri = self.client.URIs["delete"].format(
             sessionId=self.session_id, projectId=projectId
         )
         returns = {}
-        self.register_entry(Entry.DELETE, uri, returns)
+        self.register_entry(m, 'DELETE', uri, returns)
 
         r = self.client.delete_session(self.session_id)
         self.assertEqual(r, returns)
```

