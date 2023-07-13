# Comparing `tmp/olive2022-0.1.6.tar.gz` & `tmp/olive2022-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olive2022-0.1.6.tar", max compression
+gzip compressed data, was "olive2022-0.1.7.tar", max compression
```

## Comparing `olive2022-0.1.6.tar` & `olive2022-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1083 2022-10-27 01:45:26.035428 olive2022-0.1.6/LICENSE
--rw-r--r--   0        0        0     3806 2022-12-18 05:57:38.045549 olive2022-0.1.6/README.md
--rw-r--r--   0        0        0     1867 2022-12-19 16:45:02.556636 olive2022-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    14505 2022-12-19 16:45:02.556636 olive2022-0.1.6/src/olive2022.py
--rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 olive2022-0.1.6/setup.py
--rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 olive2022-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-10-27 01:45:26.035428 olive2022-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3806 2022-11-30 14:42:51.676977 olive2022-0.1.7/README.md
+-rw-r--r--   0        0        0     1867 2023-07-13 04:02:56.235123 olive2022-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    14505 2023-07-13 04:02:56.235123 olive2022-0.1.7/src/olive2022.py
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 olive2022-0.1.7/setup.py
+-rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 olive2022-0.1.7/PKG-INFO
```

### Comparing `olive2022-0.1.6/LICENSE` & `olive2022-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `olive2022-0.1.6/README.md` & `olive2022-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `olive2022-0.1.6/pyproject.toml` & `olive2022-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2022 Carnegie Mellon University
 # SPDX-License-Identifier: 0BSD
 
 [tool.poetry]
 name = "olive2022"
-version = "0.1.6"
+version = "0.1.7"
 description = "Edge-native virtual desktop application"
 authors = [
     "Carnegie Mellon University <satya+group@cs.cmu.edu>",
     "Jan Harkes <jaharkes@cs.cmu.edu>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -21,15 +21,15 @@
 packages = [
     { include = "olive2022.py", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyyaml = "^6.0"
-sinfonia-tier3 = "^0.6.2"
+sinfonia-tier3 = "^0.7.0"
 tqdm = "^4.64.1"
 xdg = "^5.1.1"
 yarl = "^1.8.1"
 
 [tool.poetry.scripts]
 olive2022 = "olive2022:main"
```

### Comparing `olive2022-0.1.6/src/olive2022.py` & `olive2022-0.1.7/src/olive2022.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # SPDX-License-Identifier: MIT
 #
 """
 Launch an Olive Archive virtual machine on a Sinfonia-Tier2 cloudlet and
 connect over the Sinfonia-created wireguard tunnel with a vnc client.
 """
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 import argparse
 import os
 import socket
 import subprocess
 import sys
 import uuid
```

### Comparing `olive2022-0.1.6/setup.py` & `olive2022-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 package_dir = \
 {'': 'src'}
 
 modules = \
 ['olive2022']
 install_requires = \
 ['pyyaml>=6.0,<7.0',
- 'sinfonia-tier3>=0.6.2,<0.7.0',
+ 'sinfonia-tier3>=0.7.0,<0.8.0',
  'tqdm>=4.64.1,<5.0.0',
  'xdg>=5.1.1,<6.0.0',
  'yarl>=1.8.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['olive2022 = olive2022:main']}
 
 setup_kwargs = {
     'name': 'olive2022',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Edge-native virtual desktop application',
     'long_description': "# Olive 2022\n\nEdge-native virtual desktop application that uses the\n[Sinfonia](https://github.com/cmusatyalab/sinfonia) framework to discover a\nnearby cloudlet to run the virtual machine.\n\nVirtual machine images from [Olivearchive](https://olivearchive.org) are\nconverted from their original vmnetx package format to a containerDisk\nthat can be executed with KubeVirt. The containerDisk images can be pushed into\na private Docker registry.\n\n\n## Installation\n\nOlive2022 depends on an available VNC client. I've found that virt-viewer from\nlibvirt generally does a good job. On a Debian/Ubuntu system this can be\ninstalled with.\n\n```\nsudo apt install virt-viewer\n```\n\nIt is best to manage the installation of olive2022 in a separate virtualenv with\n[pipx](https://pypa.github.io/pipx/installation/).\n\n```\npython3 -m pip install --user pipx\npython3 -m pipx ensurepath\n```\n\nOnce these dependencies are in place, installation should be fairly\nstraightforward, even specifying a python version should only be necessary if\nthe system default happens to be older than Python-3.7.\n\n```\npipx install olive2022\n```\n\nIf installation fails at any point, there are various troubleshooting tips at\nthe end of this document.\n\n\n## Usage\n\n`olive2022 install` creates a .desktop file to declare a handler for\nvmnetx+https URLs.\n\nWhen you then 'Launch' a virtual machine from the Olivearchive website, the\nhandler will execute `olive2022 launch` with the VMNetX URL for the virtual\nmachine image.\n\n\n## Internals\n\n`olive2022 launch` hashes the VMNetX URL to a Sinfonia UUID, and uses\n`sinfonia-tier3` to request the relevant backend to be started on a nearby\ncloudlet. When deployment has started, `sinfonia-tier3` will create a local\nwireguard tunnel endpoint and runs `olive2022 stage2` which waits for the\ndeployment to complete by probing if the VNC endpoint has become accessible.\nIt will then try to run remote-viewer (from the virt-viewer package),\ngvncviewer, or vncviewer.\n\n\n## Converting VMNetX packages\n\n`olive2022 convert` will take a VMNetX URL, download the vmnetx format package\nfile and convert it to a containerDisk image and associated Sinfonia recipe.\nThe Docker registry to push the containerDisk image to can be set with the\n`OLIVE2022_REGISTRY` environment variable. If it is a private repository, the\nnecessary pull credentials to add to the recipe can be specified with\n`OLIVE2022_CREDENTIALS=<username>:<access_token>`.\n\n\n## Installation troubleshooting\n\n#### `/usr/bin/python3: No module named pip`\n\nPip is not installed on your system. On Debian/Ubuntu systems, to reduce the\nchance of interfering with packaged Python modules, the default Python\ninstallation does not install pip and even disables the `python3 -m ensurepip`\nway of installing a recent version of the pip package manager. You have to\ninstall the python3-pip and python3-venv packages.\n\n```\nsudo apt install python3-pip python3-venv\n```\n\n#### `pipx: command not found`\n\n`python3 -m pipx ensurepath` is only able to fix the PATH environment for\nsome (mostly bourne-like) shells. If you are using bash/sh/fish/zsh it may be\nsufficient to restart your terminal to pick up the new path.\n\nWith csh/tcsh you will probably have to add the following to your `.login` or\n`.cshrc` files and/or run `rehash` to pick up any new binaries.\n\n```\nset path = ( $path $HOME/.local/bin )\n```\n\n#### `ERROR: Could not find a version that satisfies the requirement olive2022 (from versions: none)`\n\nBecause Olive2022 depends on Python-3.7 or newer, installation fails with this\nerror when the default Python interpreter is older. On Ubuntu 18.04 you can\ninstall a newer Python interpreter and explicitly specify it as an alternate\ninterpreter version when installing with pipx.\n\n```\nsudo apt install python3.8\npipx install --python python3.8 olive2022\n```\n",
     'author': 'Carnegie Mellon University',
     'author_email': 'satya+group@cs.cmu.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cmusatyalab/olive2022',
```

### Comparing `olive2022-0.1.6/PKG-INFO` & `olive2022-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olive2022
-Version: 0.1.6
+Version: 0.1.7
 Summary: Edge-native virtual desktop application
 Home-page: https://github.com/cmusatyalab/olive2022
 License: MIT
 Author: Carnegie Mellon University
 Author-email: satya+group@cs.cmu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: sinfonia-tier3 (>=0.6.2,<0.7.0)
+Requires-Dist: sinfonia-tier3 (>=0.7.0,<0.8.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: xdg (>=5.1.1,<6.0.0)
 Requires-Dist: yarl (>=1.8.1,<2.0.0)
 Project-URL: Repository, https://github.com/cmusatyalab/olive2022
 Description-Content-Type: text/markdown
 
 # Olive 2022
```

