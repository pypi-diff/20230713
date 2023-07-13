# Comparing `tmp/voicemeeter_compact-1.9.0.tar.gz` & `tmp/voicemeeter_compact-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_compact-1.9.0.tar", max compression
+gzip compressed data, was "voicemeeter_compact-1.9.1.tar", max compression
```

## Comparing `voicemeeter_compact-1.9.0.tar` & `voicemeeter_compact-1.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter_compact-1.9.0/LICENSE
--rw-r--r--   0        0        0      730 2023-07-10 19:52:01.330626 voicemeeter_compact-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     6125 2023-07-10 03:18:55.019093 voicemeeter_compact-1.9.0/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter_compact-1.9.0/vmcompact/__init__.py
--rw-r--r--   0        0        0     6246 2023-07-11 07:31:35.433343 voicemeeter_compact-1.9.0/vmcompact/app.py
--rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter_compact-1.9.0/vmcompact/banner.py
--rw-r--r--   0        0        0    23962 2023-07-10 23:26:02.030414 voicemeeter_compact-1.9.0/vmcompact/builders.py
--rw-r--r--   0        0        0    11135 2023-07-10 23:59:51.207793 voicemeeter_compact-1.9.0/vmcompact/channels.py
--rw-r--r--   0        0        0     9852 2023-07-10 23:14:22.369555 voicemeeter_compact-1.9.0/vmcompact/config.py
--rw-r--r--   0        0        0     2835 2023-07-07 21:51:19.065698 voicemeeter_compact-1.9.0/vmcompact/configurations.py
--rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter_compact-1.9.0/vmcompact/data.py
--rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter_compact-1.9.0/vmcompact/errors.py
--rw-r--r--   0        0        0     9178 2023-07-10 23:25:00.326724 voicemeeter_compact-1.9.0/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter_compact-1.9.0/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    16901 2023-07-10 22:04:53.242069 voicemeeter_compact-1.9.0/vmcompact/menu.py
--rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter_compact-1.9.0/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter_compact-1.9.0/vmcompact/subject.py
--rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 voicemeeter_compact-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter_compact-1.9.1/LICENSE
+-rw-r--r--   0        0        0      730 2023-07-13 00:28:29.352025 voicemeeter_compact-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6125 2023-07-10 03:18:55.019093 voicemeeter_compact-1.9.1/README.md
+-rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter_compact-1.9.1/vmcompact/__init__.py
+-rw-r--r--   0        0        0     6247 2023-07-13 00:20:26.988130 voicemeeter_compact-1.9.1/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter_compact-1.9.1/vmcompact/banner.py
+-rw-r--r--   0        0        0    23962 2023-07-10 23:26:02.030414 voicemeeter_compact-1.9.1/vmcompact/builders.py
+-rw-r--r--   0        0        0    11135 2023-07-10 23:59:51.207793 voicemeeter_compact-1.9.1/vmcompact/channels.py
+-rw-r--r--   0        0        0     9852 2023-07-10 23:14:22.369555 voicemeeter_compact-1.9.1/vmcompact/config.py
+-rw-r--r--   0        0        0     2835 2023-07-07 21:51:19.065698 voicemeeter_compact-1.9.1/vmcompact/configurations.py
+-rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter_compact-1.9.1/vmcompact/data.py
+-rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter_compact-1.9.1/vmcompact/errors.py
+-rw-r--r--   0        0        0     9178 2023-07-10 23:25:00.326724 voicemeeter_compact-1.9.1/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter_compact-1.9.1/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    16901 2023-07-10 22:04:53.242069 voicemeeter_compact-1.9.1/vmcompact/menu.py
+-rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter_compact-1.9.1/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter_compact-1.9.1/vmcompact/subject.py
+-rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 voicemeeter_compact-1.9.1/PKG-INFO
```

### Comparing `voicemeeter_compact-1.9.0/LICENSE` & `voicemeeter_compact-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/pyproject.toml` & `voicemeeter_compact-1.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.9.0"
+version = "1.9.1"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
 packages = [{ include = "vmcompact" }]
 include = ["vmcompact/img/cat.ico"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sv-ttk = "^2.5.1"
 tomli = { version = "^2.0.1", python = "<3.11" }
-voicemeeter-api = "^2.1.2"
-vban-cmd = "^2.2.0"
+voicemeeter-api = "^2.3.2"
+vban-cmd = "^2.3.2"
 
 [tool.poetry.dev-dependencies]
 black = { version = "^22.6.0", allow-prereleases = true }
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `voicemeeter_compact-1.9.0/README.md` & `voicemeeter_compact-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/app.py` & `voicemeeter_compact-1.9.1/vmcompact/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         _base_values.run_update = True
         if self._vmr.gui.launched_by_api:
             self.on_pdirty()
 
     def healthcheck_step(self):
         if not _base_values.vban_connected:
             try:
-                self._vmr.pdirty
+                self._vmr.version
             except voicemeeterlib.error.CAPIError:
                 resp = messagebox.askyesno(message="Restart Voicemeeter GUI?")
                 if resp:
                     self.logger.debug(
                         "healthcheck failed, rebuilding the app after GUI restart."
                     )
                     self._vmr.end_thread()
```

### Comparing `voicemeeter_compact-1.9.0/vmcompact/banner.py` & `voicemeeter_compact-1.9.1/vmcompact/banner.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/builders.py` & `voicemeeter_compact-1.9.1/vmcompact/builders.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/channels.py` & `voicemeeter_compact-1.9.1/vmcompact/channels.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/config.py` & `voicemeeter_compact-1.9.1/vmcompact/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/configurations.py` & `voicemeeter_compact-1.9.1/vmcompact/configurations.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/data.py` & `voicemeeter_compact-1.9.1/vmcompact/data.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/gainlayer.py` & `voicemeeter_compact-1.9.1/vmcompact/gainlayer.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/img/cat.ico` & `voicemeeter_compact-1.9.1/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/menu.py` & `voicemeeter_compact-1.9.1/vmcompact/menu.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/navigation.py` & `voicemeeter_compact-1.9.1/vmcompact/navigation.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/vmcompact/subject.py` & `voicemeeter_compact-1.9.1/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.0/PKG-INFO` & `voicemeeter_compact-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.9.0
+Version: 1.9.1
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sv-ttk (>=2.5.1,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
-Requires-Dist: vban-cmd (>=2.2.0,<3.0.0)
-Requires-Dist: voicemeeter-api (>=2.1.2,<3.0.0)
+Requires-Dist: vban-cmd (>=2.3.2,<3.0.0)
+Requires-Dist: voicemeeter-api (>=2.3.2,<3.0.0)
 Project-URL: Repository, https://github.com/onyx-and-iris/voicemeeter-compact
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![OS: Windows](https://img.shields.io/badge/os-windows-red)
```

