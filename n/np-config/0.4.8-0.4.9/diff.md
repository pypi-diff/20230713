# Comparing `tmp/np_config-0.4.8.tar.gz` & `tmp/np_config-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_config-0.4.8.tar", max compression
+gzip compressed data, was "np_config-0.4.9.tar", max compression
```

## Comparing `np_config-0.4.8.tar` & `np_config-0.4.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1824 2023-02-09 02:08:20.863014 np_config-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      650 2022-12-22 09:21:53.778110 np_config-0.4.8/README.md
--rw-r--r--   0        0        0      305 2023-02-03 20:46:13.855762 np_config-0.4.8/src/np_config/__init__.py
--rw-r--r--   0        0        0    14619 2023-02-09 02:07:50.362965 np_config-0.4.8/src/np_config/np_config.py
--rw-r--r--   0        0        0     7588 2023-02-08 23:42:41.768999 np_config-0.4.8/src/np_config/rigs.py
--rw-r--r--   0        0        0     5363 2023-02-09 00:56:07.428030 np_config-0.4.8/src/np_config/utils.py
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 np_config-0.4.8/setup.py
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 np_config-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1824 2023-02-11 18:05:16.510389 np_config-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      650 2022-12-22 09:21:53.778110 np_config-0.4.9/README.md
+-rw-r--r--   0        0        0      305 2023-02-03 20:46:13.855762 np_config-0.4.9/src/np_config/__init__.py
+-rw-r--r--   0        0        0    14545 2023-02-11 18:04:44.500832 np_config-0.4.9/src/np_config/np_config.py
+-rw-r--r--   0        0        0     7549 2023-02-11 18:02:39.878136 np_config-0.4.9/src/np_config/rigs.py
+-rw-r--r--   0        0        0     5363 2023-02-09 00:56:07.428030 np_config-0.4.9/src/np_config/utils.py
+-rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 np_config-0.4.9/setup.py
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 np_config-0.4.9/PKG-INFO
```

### Comparing `np_config-0.4.8/pyproject.toml` & `np_config-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "np_config"
 
 [tool.poetry]
 name = "np_config"
-version = "0.4.8"
+version = "0.4.9"
 description = "Zookeeper configs with local backup, repackaging code from AIBS mpeconfig."
 authors = [
     "Ben Hardcastle <ben.hardcastle@alleninstitute.org>",
     "Ross Hytnen <rossh@alleninstitute.org>", 
     "Ben Sutton <ben.sutton@alleninstitute.org>",
 ]
 maintainers = ["Ben Hardcastle <ben.hardcastle@alleninstitute.org>"]
```

### Comparing `np_config-0.4.8/README.md` & `np_config-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `np_config-0.4.8/src/np_config/np_config.py` & `np_config-0.4.9/src/np_config/np_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 import appdirs
 import yaml
 from kazoo.client import KazooClient
 
 # TODO use local backup for ZK if server unavailable
 
 logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
-logger.setLevel(logging.DEBUG)
 
 # preserve order of keys in dict
 yaml.add_representer(
     dict,
     lambda self, data: yaml.representer.SafeRepresenter.represent_dict(
         self, data.items()
     ),
```

### Comparing `np_config-0.4.8/src/np_config/rigs.py` & `np_config-0.4.9/src/np_config/rigs.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,16 @@
 import os
 import pathlib
 import re
 from typing import Any, Hashable, Optional
 
 import requests
 
-if __name__ == "__main__":
-    import utils
-
-    import np_config
-else:
-    from . import np_config, utils
+import np_config.np_config as np_config
+import np_config.utils as utils
 
 logger = logging.getLogger(__name__)
 
 # all mpe computers --------------------------------------------------------------------
 
 SERVER = "http://mpe-computers/v2.0"
```

### Comparing `np_config-0.4.8/src/np_config/utils.py` & `np_config-0.4.9/src/np_config/utils.py`

 * *Files identical despite different names*

### Comparing `np_config-0.4.8/setup.py` & `np_config-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'typing-extensions']
 
 extras_require = \
 {'dev': ['pip-tools', 'isort', 'mypy', 'black', 'pytest', 'poetry']}
 
 setup_kwargs = {
     'name': 'np-config',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'Zookeeper configs with local backup, repackaging code from AIBS mpeconfig.',
     'long_description': "**For use on internal Allen Institute network**\n\n- fetch configs from ZooKeeper or .yaml/.json file via their path:\n```python\ntest_config: dict = np_config.fetch(\n    '/projects/np_logging_test/defaults/logging'\n)\n```\n\n- the Mindscope ZooKeeper server is at `eng-mindscope:2181`\n- configs can be added via ZooNavigator webview:\n  [http://eng-mindscope:8081](http://eng-mindscope:8081)\n- or more conveniently, via an extension for VSCode such as [gaoliang.visual-zookeeper](https://marketplace.visualstudio.com/items?itemName=gaoliang.visual-zookeeper)\n\n- configs are cached locally: if the ZooKeeper server is unavailable, the local copy will be used",
     'author': 'Ben Hardcastle',
     'author_email': 'ben.hardcastle@alleninstitute.org',
     'maintainer': 'Ben Hardcastle',
     'maintainer_email': 'ben.hardcastle@alleninstitute.org',
     'url': 'None',
```

### Comparing `np_config-0.4.8/PKG-INFO` & `np_config-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-config
-Version: 0.4.8
+Version: 0.4.9
 Summary: Zookeeper configs with local backup, repackaging code from AIBS mpeconfig.
 Author: Ben Hardcastle
 Author-email: ben.hardcastle@alleninstitute.org
 Maintainer: Ben Hardcastle
 Maintainer-email: ben.hardcastle@alleninstitute.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

