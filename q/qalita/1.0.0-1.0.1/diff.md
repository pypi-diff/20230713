# Comparing `tmp/qalita-1.0.0.tar.gz` & `tmp/qalita-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalita-1.0.0.tar", max compression
+gzip compressed data, was "qalita-1.0.1.tar", max compression
```

## Comparing `qalita-1.0.0.tar` & `qalita-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    19753 2023-07-13 17:15:31.059605 qalita-1.0.0/LICENSE
--rw-r--r--   0        0        0      370 2023-07-13 17:15:31.060605 qalita-1.0.0/docs/README.md
--rw-r--r--   0        0        0     1134 2023-07-13 17:15:31.566613 qalita-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 17:15:31.083606 qalita-1.0.0/qalita/__init__.py
--rw-r--r--   0        0        0     4662 2023-07-13 17:15:31.060605 qalita-1.0.0/qalita/cli.py
--rw-r--r--   0        0        0        0 2023-07-13 17:15:31.084606 qalita-1.0.0/qalita/commands/__init__.py
--rw-r--r--   0        0        0    17343 2023-07-13 17:15:31.061606 qalita-1.0.0/qalita/commands/agent.py
--rw-r--r--   0        0        0    14244 2023-07-13 17:15:31.061606 qalita-1.0.0/qalita/commands/pack.py
--rw-r--r--   0        0        0     9429 2023-07-13 17:15:31.061606 qalita-1.0.0/qalita/commands/source.py
--rw-r--r--   0        0        0        0 2023-07-13 17:15:31.084606 qalita-1.0.0/qalita/internal/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-13 17:15:31.061606 qalita-1.0.0/qalita/internal/logger.py
--rw-r--r--   0        0        0     2486 2023-07-13 17:15:31.061606 qalita-1.0.0/qalita/internal/utils.py
--rw-r--r--   0        0        0     1408 1970-01-01 00:00:00.000000 qalita-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    19753 2023-07-13 21:38:07.871172 qalita-1.0.1/LICENSE
+-rw-r--r--   0        0        0      416 2023-07-13 21:38:07.871172 qalita-1.0.1/docs/README.md
+-rw-r--r--   0        0        0     1169 2023-07-13 21:38:19.649227 qalita-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 21:38:07.895172 qalita-1.0.1/qalita/__init__.py
+-rw-r--r--   0        0        0     4660 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/cli.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:38:07.895172 qalita-1.0.1/qalita/commands/__init__.py
+-rw-r--r--   0        0        0    18014 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/commands/agent.py
+-rw-r--r--   0        0        0    14225 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/commands/pack.py
+-rw-r--r--   0        0        0     9429 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/commands/source.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:38:07.895172 qalita-1.0.1/qalita/internal/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/internal/logger.py
+-rw-r--r--   0        0        0     2486 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/internal/utils.py
+-rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 qalita-1.0.1/PKG-INFO
```

### Comparing `qalita-1.0.0/LICENSE` & `qalita-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qalita-1.0.0/pyproject.toml` & `qalita-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "qalita"
-version = "1.0.0"
-description = "Qalita Command line Tool"
+version = "1.0.1"
+description = "Qalita Command Line Interface"
 authors = ["Armand LEOPOLD <armand.leopold@qalita.io>"]
 readme = "docs/README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -13,14 +13,16 @@
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Quality Assurance"
 ]
+include = ["version.json"]
+
 
 [tool.poetry.scripts]
 qalita = "qalita.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pylint = "^2.17.4"
```

### Comparing `qalita-1.0.0/qalita/cli.py` & `qalita-1.0.1/qalita/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 # QALITA (c) COPYRIGHT 2023 - ALL RIGHTS RESERVED -
 """
-import click
 import sys
-import yaml
-import toml
+import os
 import json
 import base64
+import yaml
+import click
 
 from qalita.internal.logger import init_logging
 
 logger = init_logging()
 
 
 class CustomContext(click.Context):
@@ -26,15 +26,15 @@
     def save_source_config(self):
         with open("qalita-conf.yaml", "w") as file:
             yaml.dump(self.config, file)
 
     def load_source_config(self):
         try:
             with open("qalita-conf.yaml", "r") as file:
-                return yaml.load(file, Loader=yaml.FullLoader)
+                return yaml.safe_load(file)
         except FileNotFoundError:
             logger.warning("Configuration file not found, creating a new one.")
             self.config = {"version": 1, "sources": []}
             self.save_source_config()
             return self.config
         except Exception as e:
             logger.warning(
@@ -100,40 +100,40 @@
     ----------------------------------------------------------------------------\n\r
     Please, Help us improve our service by reporting any bug by filing a bug report, Thanks ! \n\r
     mail : contact-project+qalita-platform-toolset-cli-bug@incoming.gitlab.com \n\r
     ----------------------------------------------------------------------------"""
     pass
 
 
-def fetch_package_version(path_to_pyproject="pyproject.toml"):
+def fetch_package_version(filename):
     """
-    Fetches the package version from a pyproject.toml file.
-
-    Args:
-    path_to_pyproject (str): The path to the pyproject.toml file.
-
-    Returns:
-    str: The version of the package.
+    Fetch the version from the package.
     """
-    with open(path_to_pyproject, "r") as f:
-        pyproject_toml = toml.load(f)
+    # Open the file
+    with open(filename, 'r') as f:
+        data = json.load(f)
 
-    return pyproject_toml.get("tool", {}).get("poetry", {}).get("version", None)
+    # Retrieve the version
+    version = data.get('version', 'Version not found')
 
+    return version
 
 @cli.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @pass_config
 def version(config):
     """
     Display the version of the cli
     """
     logger.info("------------- QALITA CLI Version -------------")
-    version = fetch_package_version("pyproject.toml")
-    logger.info(f"Version : {version}")
 
+    # Assuming that your json file is named 'version.json' and located in the same directory as this file
+    file_path = os.path.join(os.path.dirname(__file__), 'version.json')
+    version = fetch_package_version(file_path)
+
+    logger.info(f"Version : {version}")
 
 from qalita.commands import agent, source, pack
 
 # Add pack command group to cli
 cli.add_command(pack.pack)
 cli.add_command(agent.agent)
 cli.add_command(source.source)
```

### Comparing `qalita-1.0.0/qalita/commands/agent.py` & `qalita-1.0.1/qalita/commands/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,18 +446,31 @@
     # Copy the downloaded pack to the temp folder
     copy2(pack_file_path, temp_folder_name)
 
     # Uncompress the pack
     with tarfile.open(
         os.path.join(temp_folder_name, pack_file_path.split("/")[-1]), "r:gz"
     ) as tar:
-        tar.extractall(path=temp_folder_name)
-
-    # Delete the compressed pack
-    os.remove(os.path.join(temp_folder_name, pack_file_path.split("/")[-1]))
+        # Validate members
+        safe_members = []
+        for member in tar.getmembers():
+            # Skip if not a file
+            if not member.isfile():
+                continue
+            # Check for path traversal attack
+            if member.name.startswith(('/', '..')):
+                logger.warning(f'Skipping potentially dangerous tar file member {member.name}')
+                continue
+            safe_members.append(member)
+        # Assert that all members are safe
+        assert all(not member.name.startswith(('/', '..')) for member in safe_members), "Unsafe tar file member detected"
+        # Extract safe members
+        tar.extractall(path=temp_folder_name, members=safe_members)
+        # Delete the compressed pack
+        os.remove(os.path.join(temp_folder_name, pack_file_path.split("/")[-1]))
 
     # Load the source configuration
     source_conf = config.load_source_config()
 
     # Find the matching source_id
     matching_sources = [
         s for s in source_conf["sources"] if str(s.get("id")) == str(source_id)
```

### Comparing `qalita-1.0.0/qalita/commands/pack.py` & `qalita-1.0.1/qalita/commands/pack.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     source_dir = (
         f"./{name}_pack"  # Assuming the directory is in the current working directory
     )
     make_tarfile(output_filename, source_dir)
 
     # Send the tar.gz file to the server
     with open(f"./{name}_pack/properties.yaml", "r") as file:
-        pack_properties = yaml.load(file, Loader=yaml.FullLoader)
+        pack_properties = yaml.safe_load(file)
 
     api_url = agent_conf["context"]["local"]["url"]
     registry_id = agent_conf["registries"]["id"]
     pack_name = pack_properties["name"]
     pack_version = pack_properties["version"]
     pack_description = pack_properties["description"]
     user_id = agent_conf["user"]["id"]
```

### Comparing `qalita-1.0.0/qalita/commands/source.py` & `qalita-1.0.1/qalita/commands/source.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.0/qalita/internal/logger.py` & `qalita-1.0.1/qalita/internal/logger.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.0/qalita/internal/utils.py` & `qalita-1.0.1/qalita/internal/utils.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.0/PKG-INFO` & `qalita-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qalita
-Version: 1.0.0
-Summary: Qalita Command line Tool
+Version: 1.0.1
+Summary: Qalita Command Line Interface
 Author: Armand LEOPOLD
 Author-email: armand.leopold@qalita.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -23,14 +23,16 @@
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # QALITA Command Line Interface
 
+![logo](https://app.prod.qalita.io/logo.svg)
+
 ## Installation
 
 `pip install qalita`
 
 ## Usage
 
 ```bash
```

