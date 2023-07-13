# Comparing `tmp/pbs_installer-2023.7.13.tar.gz` & `tmp/pbs_installer-2023.7.13.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbs_installer-2023.7.13.tar", last modified: Thu Jul 13 12:41:57 2023, max compression
+gzip compressed data, was "pbs_installer-2023.7.13.post0.tar", last modified: Thu Jul 13 13:04:04 2023, max compression
```

## Comparing `pbs_installer-2023.7.13.tar` & `pbs_installer-2023.7.13.post0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1059 2023-07-13 11:33:35.913905 pbs_installer-2023.7.13/LICENSE
--rw-r--r--   0        0        0      235 2023-07-13 11:33:38.258222 pbs_installer-2023.7.13/README.md
--rw-r--r--   0        0        0      839 2023-07-13 12:41:57.439610 pbs_installer-2023.7.13/pyproject.toml
--rw-r--r--   0        0        0      196 2023-07-13 12:22:31.756305 pbs_installer-2023.7.13/src/pbs_installer/__init__.py
--rw-r--r--   0        0        0      450 2023-07-13 11:46:16.941376 pbs_installer-2023.7.13/src/pbs_installer/__main__.py
--rw-r--r--   0        0        0     3606 2023-07-13 12:34:02.158785 pbs_installer-2023.7.13/src/pbs_installer/_install.py
--rw-r--r--   0        0        0     1613 2023-07-13 12:35:17.597283 pbs_installer-2023.7.13/src/pbs_installer/_utils.py
--rw-r--r--   0        0        0    65314 2023-07-13 12:41:30.584590 pbs_installer-2023.7.13/src/pbs_installer/_versions.py
--rw-r--r--   0        0        0        0 2023-07-13 08:54:47.350150 pbs_installer-2023.7.13/tests/__init__.py
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 pbs_installer-2023.7.13/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/LICENSE
+-rw-r--r--   0        0        0      331 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/README.md
+-rw-r--r--   0        0        0      889 2023-07-13 13:04:04.543616 pbs_installer-2023.7.13.post0/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/src/pbs_installer/__init__.py
+-rw-r--r--   0        0        0      450 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/src/pbs_installer/__main__.py
+-rw-r--r--   0        0        0     3762 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/src/pbs_installer/_install.py
+-rw-r--r--   0        0        0     1613 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/src/pbs_installer/_utils.py
+-rw-r--r--   0        0        0    65314 2023-07-13 13:03:50.303558 pbs_installer-2023.7.13.post0/src/pbs_installer/_versions.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:03:50.303558 pbs_installer-2023.7.13.post0/tests/__init__.py
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 pbs_installer-2023.7.13.post0/PKG-INFO
```

### Comparing `pbs_installer-2023.7.13/LICENSE` & `pbs_installer-2023.7.13.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbs_installer-2023.7.13/pyproject.toml` & `pbs_installer-2023.7.13.post0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 ]
 dependencies = [
     "zstandard>=0.21.0",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 dynamic = []
-version = "2023.7.13"
+version = "2023.7.13.post0"
 
 [project.license]
 text = "MIT"
 
+[project.optional-dependencies]
+full = [
+    "requests>=2.24.0",
+]
+
 [project.scripts]
 pbs-install = "pbs_installer.__main__:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "requests>=2.31.0",
     "black>=23.3.0",
 ]
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.scripts.update]
```

### Comparing `pbs_installer-2023.7.13/src/pbs_installer/_install.py` & `pbs_installer-2023.7.13.post0/src/pbs_installer/_install.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 import hashlib
 import logging
 import os
 import tempfile
 from typing import TYPE_CHECKING
 from urllib.parse import unquote
 
-import requests
-
 from ._utils import PythonVersion, get_arch_platform, unpack_tar
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
+    import requests
     from _typeshed import StrPath
 
 THIS_ARCH, THIS_PLATFORM = get_arch_platform()
 
 
 def _get_headers() -> dict[str, str] | None:
     TOKEN = os.getenv("GITHUB_TOKEN")
@@ -53,14 +52,19 @@
         return None
     return resp.text.strip()
 
 
 def download(url: str, destination: StrPath, session: requests.Session | None = None) -> str:
     logger.debug("Downloading url %s to %s", url, destination)
     filename = unquote(url.rsplit("/")[-1])
+    try:
+        import requests
+    except ModuleNotFoundError:
+        raise RuntimeError("You must install requests to use this function") from None
+
     if session is None:
         session = requests.Session()
 
     hasher = hashlib.sha256()
     checksum = _read_sha256(url, session)
 
     with open(destination, "wb") as f:
```

### Comparing `pbs_installer-2023.7.13/src/pbs_installer/_utils.py` & `pbs_installer-2023.7.13.post0/src/pbs_installer/_utils.py`

 * *Files identical despite different names*

### Comparing `pbs_installer-2023.7.13/src/pbs_installer/_versions.py` & `pbs_installer-2023.7.13.post0/src/pbs_installer/_versions.py`

 * *Files identical despite different names*

