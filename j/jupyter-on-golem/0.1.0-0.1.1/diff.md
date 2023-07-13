# Comparing `tmp/jupyter_on_golem-0.1.0.tar.gz` & `tmp/jupyter_on_golem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_on_golem-0.1.0.tar", max compression
+gzip compressed data, was "jupyter_on_golem-0.1.1.tar", max compression
```

## Comparing `jupyter_on_golem-0.1.0.tar` & `jupyter_on_golem-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0       73 2023-05-24 08:24:51.150637 jupyter_on_golem-0.1.0/jupyter_on_golem/__init__.py
--rw-r--r--   0        0        0     1283 2023-07-05 09:18:35.387766 jupyter_on_golem-0.1.0/jupyter_on_golem/__main__.py
--rw-r--r--   0        0        0    24404 2023-07-03 11:43:53.685452 jupyter_on_golem-0.1.0/jupyter_on_golem/golem.py
--rw-r--r--   0        0        0     2597 2023-07-03 11:05:36.616651 jupyter_on_golem-0.1.0/jupyter_on_golem/golem_kernel.py
--rw-r--r--   0        0        0      782 2023-06-26 09:19:12.479783 jupyter_on_golem-0.1.0/jupyter_on_golem/manifest.json
--rw-r--r--   0        0        0     3700 2023-07-03 11:12:57.770603 jupyter_on_golem-0.1.0/jupyter_on_golem/remote_python.py
--rw-r--r--   0        0        0      733 2023-07-05 09:11:25.855757 jupyter_on_golem-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 jupyter_on_golem-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-13 11:20:06.802724 jupyter_on_golem-0.1.1/LICENSE
+-rw-r--r--   0        0        0    13422 2023-07-13 11:20:06.802724 jupyter_on_golem-0.1.1/README.md
+-rw-r--r--   0        0        0       73 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/__init__.py
+-rw-r--r--   0        0        0     1283 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/__main__.py
+-rw-r--r--   0        0        0    24503 2023-07-13 11:23:56.850117 jupyter_on_golem-0.1.1/jupyter_on_golem/golem.py
+-rw-r--r--   0        0        0     2597 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/golem_kernel.py
+-rw-r--r--   0        0        0      782 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/manifest.json
+-rw-r--r--   0        0        0     3700 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/remote_python.py
+-rw-r--r--   0        0        0      754 2023-07-13 11:25:02.465957 jupyter_on_golem-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    14498 1970-01-01 00:00:00.000000 jupyter_on_golem-0.1.1/PKG-INFO
```

### Comparing `jupyter_on_golem-0.1.0/jupyter_on_golem/__main__.py` & `jupyter_on_golem-0.1.1/jupyter_on_golem/__main__.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.0/jupyter_on_golem/golem.py` & `jupyter_on_golem-0.1.1/jupyter_on_golem/golem.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,28 +42,29 @@
 '''
 
 HELP_TEMPLATE = '''\
      _                   _                             ____       _                
     | |_   _ _ __  _   _| |_ ___ _ __    ___  _ __    / ___| ___ | | ___ _ __ ___  
  _  | | | | | '_ \| | | | __/ _ \ '__|  / _ \| '_ \  | |  _ / _ \| |/ _ \ '_ ` _ \ 
 | |_| | |_| | |_) | |_| | ||  __/ |    | (_) | | | | | |_| | (_) | |  __/ | | | | |
- \___/ \__,_| .__/ \__, |\__\___|_|     \___/|_| |_|  \____|\___/|_|\___|_| |_| |_| version: 0.1.0
+ \___/ \__,_| .__/ \__, |\__\___|_|     \___/|_| |_|  \____|\___/|_|\___|_| |_| |_| version: 0.1.1
             |_|    |___/                                                           
 
 Easy to use tool to run Your Jupyter Notebooks on the Golem Network!
 
 COMMANDS:    
     %status		Shows current status of Jupyter on Golem
     %fund		Requests for testnet funds, e.g. '%fund goerli'
     %budget		Allocates GLM tokens for payments, e.g. '%budget goerli 2'. Available networks: goerli, polygon, mainnet.
     %connect		Looks for Provider which meets with defined criteria [mem|cores|disk], e.g. '%connect mem>1'				
     %disconnect 	Disconnects from the currently active Provider
     %download	 	Downloads file from Provider's ./workdir folder to local machine, e.g. '%download dataset.csv'
     %upload		Uploads file from local machine into Provider's ./workdir folder, e.g. '%upload results.csv'
-    %help		Shows this message
+    %help		Shows this message    
+    %pip install    Installs PyPI package on the Provider's host, e.g. "%pip install colorama"
 
 '''
 
 PROVIDER_TEMPLATE = '''\
 Connected to {provider_name} [{provider_id}]
     RAM: {ram} GB
     DISK: {disk} GB
```

### Comparing `jupyter_on_golem-0.1.0/jupyter_on_golem/golem_kernel.py` & `jupyter_on_golem-0.1.1/jupyter_on_golem/golem_kernel.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.0/jupyter_on_golem/manifest.json` & `jupyter_on_golem-0.1.1/jupyter_on_golem/manifest.json`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.0/jupyter_on_golem/remote_python.py` & `jupyter_on_golem-0.1.1/jupyter_on_golem/remote_python.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.0/pyproject.toml` & `jupyter_on_golem-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "jupyter-on-golem"
-version = "0.1.0"
+version = "0.1.1"
 description = "Jupyter Python kernel running on Golem network (https://www.golem.network/)"
+readme = "README.md"
 authors = ["GolemFactory <contact.jupyter@golem.network>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Distributed Computing"
```

