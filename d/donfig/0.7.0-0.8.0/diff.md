# Comparing `tmp/donfig-0.7.0.tar.gz` & `tmp/donfig-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donfig-0.7.0.tar", last modified: Sat Feb  5 03:10:32 2022, max compression
+gzip compressed data, was "donfig-0.8.0.tar", last modified: Thu Jul 13 13:29:35 2023, max compression
```

## Comparing `donfig-0.7.0.tar` & `donfig-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-05 03:10:32.637977 donfig-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-02-05 03:10:31.000000 donfig-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-02-05 03:10:31.000000 donfig-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5569 2022-02-05 03:10:32.637977 donfig-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3950 2022-02-05 03:10:31.000000 donfig-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-05 03:10:32.637977 donfig-0.7.0/donfig/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-02-05 03:10:31.000000 donfig-0.7.0/donfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3403 2022-02-05 03:10:31.000000 donfig-0.7.0/donfig/_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)    19705 2022-02-05 03:10:31.000000 donfig-0.7.0/donfig/config_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-05 03:10:32.637977 donfig-0.7.0/donfig/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-05 03:10:31.000000 donfig-0.7.0/donfig/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15661 2022-02-05 03:10:31.000000 donfig-0.7.0/donfig/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2022-02-05 03:10:31.000000 donfig-0.7.0/donfig/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-02-05 03:10:31.000000 donfig-0.7.0/donfig/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-02-05 03:10:32.637977 donfig-0.7.0/donfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-05 03:10:32.637977 donfig-0.7.0/donfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5569 2022-02-05 03:10:32.000000 donfig-0.7.0/donfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-02-05 03:10:32.000000 donfig-0.7.0/donfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-05 03:10:32.000000 donfig-0.7.0/donfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-05 03:10:32.000000 donfig-0.7.0/donfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-05 03:10:32.000000 donfig-0.7.0/donfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-05 03:10:32.000000 donfig-0.7.0/donfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-02-05 03:10:32.637977 donfig-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-02-05 03:10:31.000000 donfig-0.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68571 2022-02-05 03:10:31.000000 donfig-0.7.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:29:35.322126 donfig-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-13 13:29:27.000000 donfig-0.8.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-13 13:29:27.000000 donfig-0.8.0/DASK_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-13 13:29:27.000000 donfig-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 13:29:27.000000 donfig-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-13 13:29:35.322126 donfig-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-13 13:29:27.000000 donfig-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:29:35.322126 donfig-0.8.0/donfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-13 13:29:27.000000 donfig-0.8.0/donfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-13 13:29:27.000000 donfig-0.8.0/donfig/_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24644 2023-07-13 13:29:27.000000 donfig-0.8.0/donfig/config_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-13 13:29:27.000000 donfig-0.8.0/donfig/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 13:29:35.322126 donfig-0.8.0/donfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:29:35.322126 donfig-0.8.0/donfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-13 13:29:27.000000 donfig-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 13:29:35.322126 donfig-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-13 13:29:27.000000 donfig-0.8.0/setup.py
```

### Comparing `donfig-0.7.0/LICENSE.txt` & `donfig-0.8.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 Donfig Developers
+Copyright (c) 2018- Donfig Developers
 Copyright (c) 2014-2018, Anaconda, Inc. and contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `donfig-0.7.0/README.rst` & `donfig-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `donfig-0.7.0/donfig/_lock.py` & `donfig-0.8.0/donfig/_lock.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Config syncronization locks ported from upstream dask.
+"""Config synchronization locks ported from upstream dask.
 
 Originally part of Dask and stored in the dask/utils.py module. This module
 should be considered private and should not be imported directly by users.
 There are no guarantees that this module will exist in the future.
 
 """
 
@@ -57,15 +57,15 @@
 
     This is useful for consistently protecting resources on a per-process
     level.
 
     The creation of locks is itself not threadsafe.
     """
 
-    _locks = WeakValueDictionary()
+    _locks: WeakValueDictionary = WeakValueDictionary()
 
     def __init__(self, token=None):
         self.token = token or str(uuid.uuid4())
         if self.token in SerializableLock._locks:
             self.lock = SerializableLock._locks[self.token]
         else:
             self.lock = Lock()
```

### Comparing `donfig-0.7.0/donfig/config_obj.py` & `donfig-0.8.0/donfig/config_obj.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+from __future__ import annotations
+
 import ast
+import base64
+import contextlib
+import json
 import os
 import pprint
 import site
 import sys
-from collections.abc import Mapping
+import warnings
+from collections.abc import Mapping, Sequence
 from contextlib import nullcontext
 from copy import deepcopy
+from typing import Any, Literal, MutableMapping
 
-from ._lock import SerializableLock
-
-try:
-    import yaml
-except ImportError:
-    yaml = None
+import yaml
 
+from ._lock import SerializableLock
 
 no_default = "__no_default__"
 
 
-def canonical_name(k, config):
+def canonical_name(k: str, config: Mapping[str, Any]) -> str:
     """Return the canonical name for a key.
 
     Handles user choice of '-' or '_' conventions by standardizing on whichever
     version was set first. If a key already exists in either hyphen or
     underscore form, the existing version is the canonical name. If neither
     version exists the original key is used as is.
     """
@@ -59,59 +62,82 @@
 
     if altk in config:
         return altk
 
     return k
 
 
-def update(old, new, priority="new"):
+def update(
+    old: MutableMapping[str, Any],
+    new: Mapping[str, Any],
+    priority: Literal["old", "new", "new-defaults"] = "new",
+    defaults: Mapping | None = None,
+) -> Mapping[str, Any]:
     """Update a nested dictionary with values from another
 
     This is like dict.update except that it smoothly merges nested values
 
     This operates in-place and modifies old
 
     Parameters
     ----------
-    priority: string {'old', 'new'}
+    priority: string {'old', 'new', 'new-defaults'}
         If new (default) then the new dictionary has preference.
         Otherwise the old dictionary does.
+        If 'new-defaults', a mapping should be given of the current defaults.
+        Only if a value in ``old`` matches the current default, it will be
+        updated with ``new``.
 
     Examples
     --------
     >>> a = {'x': 1, 'y': {'a': 2}}
     >>> b = {'x': 2, 'y': {'b': 3}}
     >>> update(a, b)  # doctest: +SKIP
     {'x': 2, 'y': {'a': 2, 'b': 3}}
 
     >>> a = {'x': 1, 'y': {'a': 2}}
     >>> b = {'x': 2, 'y': {'b': 3}}
     >>> update(a, b, priority='old')  # doctest: +SKIP
     {'x': 1, 'y': {'a': 2, 'b': 3}}
 
+    >>> d = {'x': 0, 'y': {'a': 2}}
+    >>> a = {'x': 1, 'y': {'a': 2}}
+    >>> b = {'x': 2, 'y': {'a': 3, 'b': 3}}
+    >>> update(a, b, priority='new-defaults', defaults=d)  # doctest: +SKIP
+    {'x': 1, 'y': {'a': 3, 'b': 3}}
+
     See Also
     --------
     donfig.config_obj.merge
 
     """
     for k, v in new.items():
         k = canonical_name(k, old)
 
         if isinstance(v, Mapping):
             if k not in old or old[k] is None:
                 old[k] = {}
-            update(old[k], v, priority=priority)
+            update(
+                old[k],
+                v,
+                priority=priority,
+                defaults=defaults.get(k) if defaults else None,
+            )
         else:
-            if priority == "new" or k not in old:
+            if (
+                priority == "new"
+                or k not in old
+                or (priority == "new-defaults" and defaults and k in defaults and defaults[k] == old[k])
+            ):
                 old[k] = v
 
     return old
 
 
-def merge(*dicts):
+def merge(*dicts: Mapping) -> dict:
     """Update a sequence of nested dictionaries
 
     This prefers the values in the latter dictionaries to those in the former
 
     Examples
     --------
     >>> a = {'x': 1, 'y': {'a': 2}}
@@ -120,21 +146,21 @@
     {'x': 1, 'y': {'a': 2, 'b': 3}}
 
     See Also
     --------
     donfig.config_obj.update
 
     """
-    result = {}
+    result: dict = {}
     for d in dicts:
         update(result, d)
     return result
 
 
-def collect_yaml(paths):
+def collect_yaml(paths: Sequence[str]) -> list[dict]:
     """Collect configuration from yaml files
 
     This searches through a list of paths, expands to find all yaml or json
     files, and then parses each file.
 
     """
     # Find all paths
@@ -143,67 +169,87 @@
         if os.path.exists(path):
             if os.path.isdir(path):
                 try:
                     file_paths.extend(
                         sorted(
                             os.path.join(path, p)
                             for p in os.listdir(path)
-                            if os.path.splitext(p)[1].lower()
-                            in (".json", ".yaml", ".yml")
+                            if os.path.splitext(p)[1].lower() in (".json", ".yaml", ".yml")
                         )
                     )
                 except OSError:
                     # Ignore permission errors
                     pass
             else:
                 file_paths.append(path)
 
     configs = []
 
     # Parse yaml files
     for path in file_paths:
-        try:
-            with open(path) as f:
-                data = yaml.safe_load(f.read()) or {}
-                configs.append(data)
-        except OSError:
-            # Ignore permission errors
-            pass
+        config = _load_config_file(path)
+        if config is not None:
+            configs.append(config)
 
     return configs
 
 
-def collect_env(prefix, env=None):
+def _load_config_file(path: str) -> dict | None:
+    try:
+        with open(path) as f:
+            config = yaml.safe_load(f.read())
+    except OSError:
+        # Ignore permission errors
+        return None
+    except Exception as exc:
+        raise ValueError(f"A config file at {path!r} is malformed, original error " f"message:\n\n{exc}") from None
+    if config is not None and not isinstance(config, dict):
+        raise ValueError(
+            f"A config file at {path!r} is malformed - config files must have "
+            f"a dict as the top level object, got a {type(config).__name__} instead"
+        )
+    return config
+
+
+def collect_env(
+    prefix: str, env: Mapping[str, str] | None = None, deprecations: MutableMapping[str, str | None] | None = None
+) -> dict:
     """Collect config from environment variables
 
     This grabs environment variables of the form "DASK_FOO__BAR_BAZ=123" and
     turns these into config variables of the form ``{"foo": {"bar-baz": 123}}``
     It transforms the key and value in the following way:
 
     -  Lower-cases the key text
     -  Treats ``__`` (double-underscore) as nested access
     -  Calls ``ast.literal_eval`` on the value
 
     """
     if env is None:
         env = os.environ
-    d = {}
+
+    serial_env = f"{prefix}_INTERNAL_INHERIT_CONFIG"
+    if serial_env in env:
+        d = deserialize(env[serial_env])
+    else:
+        d = {}
+
     prefix_len = len(prefix)
     for name, value in env.items():
         if name.startswith(prefix):
             varname = name[prefix_len:].lower().replace("__", ".")
             try:
                 d[varname] = ast.literal_eval(value)
             except (SyntaxError, ValueError):
                 d[varname] = value
 
-    result = {}
+    result: dict = {}
     # fake thread lock to use set functionality
     lock = nullcontext()
-    ConfigSet(result, lock, d)
+    ConfigSet(result, lock, deprecations or {}, d)
     return result
 
 
 class ConfigSet:
     """Temporarily set configuration values within a context manager
 
     Note, this class should be used directly from the `Config`
@@ -219,25 +265,61 @@
     See Also
     --------
     donfig.Config.set
     donfig.Config.get
 
     """
 
-    def __init__(self, config, lock, arg=None, **kwargs):
+    def __init__(
+        self,
+        config: MutableMapping,
+        lock: SerializableLock | contextlib.AbstractContextManager,
+        deprecations: MutableMapping[str, str | None],
+        arg: Mapping | None = None,
+        **kwargs,
+    ):
         with lock:
             self.config = config
-            self._record = []
+            self.deprecations = deprecations
+            self._record: list[tuple[str, tuple, Any]] = []
 
             if arg is not None:
                 for key, value in arg.items():
+                    key = self._check_deprecations(key)
                     self._assign(key.split("."), value, config)
             if kwargs:
                 for key, value in kwargs.items():
-                    self._assign(key.split("__"), value, config)
+                    key = key.replace("__", ".")
+                    key = self._check_deprecations(key)
+                    self._assign(key.split("."), value, config)
+
+    def _check_deprecations(self, key: str):
+        """Check if the provided value has been renamed or removed.
+
+        Parameters
+        ----------
+        key : str
+            The configuration key to check
+
+        Returns
+        -------
+        new: str
+            The proper key, whether the original (if no deprecation) or the aliased
+            value
+
+        """
+        if key in self.deprecations:
+            new = self.deprecations[key]
+            if new:
+                warnings.warn(f"Configuration key {key!r} has been deprecated. " f"Please use {new!r} instead")
+                return new
+            else:
+                raise ValueError(f"Configuration value {key!r} has been removed")
+        else:
+            return key
 
     def __enter__(self):
         return self.config
 
     def __exit__(self, type, value, traceback):
         for op, path, value in reversed(self._record):
             d = self.config
@@ -250,26 +332,33 @@
                     try:
                         d = d[key]
                     except KeyError:
                         break
                 else:
                     d.pop(path[-1], None)
 
-    def _assign(self, keys, value, d, path=(), record=True):
+    def _assign(
+        self,
+        keys: Sequence[str],
+        value: Any,
+        d: MutableMapping,
+        path: tuple[str, ...] = (),
+        record: bool = True,
+    ) -> None:
         """Assign value into a nested configuration dictionary
 
         Parameters
         ----------
         keys : Sequence[str]
             The nested path of keys to assign the value, similar to toolz.put_in
         value: object
         d : dict
             The part of the nested dictionary into which we want to assign the
             value
-        path : List[str]
+        path : tuple[str], optional
             Used internally to hold the path of old values
         record : bool, optional
             Whether this operation needs to be recorded to allow for rollback.
 
         """
         key = canonical_name(keys[0], d)
         path = path + (key,)
@@ -321,21 +410,22 @@
     else:
         return config
 
 
 class Config:
     def __init__(
         self,
-        name,
-        defaults=None,
-        paths=None,
-        env=None,
-        env_var=None,
-        root_env_var=None,
-        env_prefix=None,
+        name: str,
+        defaults: list[Mapping[str, Any]] | None = None,
+        paths: list[str] | None = None,
+        env: Mapping[str, str] | None = None,
+        env_var: str | None = None,
+        root_env_var: str | None = None,
+        env_prefix: str | None = None,
+        deprecations: Mapping[str, str | None] | None = None,
     ):
         if root_env_var is None:
             root_env_var = f"{name.upper()}_ROOT_CONFIG"
         if paths is None:
             paths = [
                 os.getenv(root_env_var, f"/etc/{name}"),
                 os.path.join(sys.prefix, "etc", name),
@@ -350,25 +440,29 @@
         if env_var is None:
             env_var = f"{name.upper()}_CONFIG"
         if env_var in os.environ:
             main_path = os.environ[env_var]
             paths.append(main_path)
         else:
             main_path = os.path.join(os.path.expanduser("~"), ".config", name)
+        if deprecations is None:
+            deprecations = {}
 
         # Remove duplicate paths while preserving ordering
         paths = list(reversed(list(dict.fromkeys(reversed(paths)))))
 
         self.name = name
         self.env_prefix = env_prefix
         self.env = env
         self.main_path = main_path
         self.paths = paths
         self.defaults = defaults or []
-        self.config = {}
+        self.deprecations = deprecations
+
+        self.config: MutableMapping[str, Any] = {}
         self.config_lock = SerializableLock()
         self.refresh()
 
     def __contains__(self, item):
         try:
             self[item]
             return True
@@ -377,24 +471,24 @@
 
     def __getitem__(self, item):
         return self.get(item)
 
     def pprint(self, **kwargs):
         return pprint.pprint(self.config, **kwargs)
 
-    def collect(self, paths=None, env=None):
+    def collect(self, paths: list[str] | None = None, env: Mapping[str, str] | None = None) -> dict:
         """Collect configuration from paths and environment variables
 
         Parameters
         ----------
-        paths : List[str]
+        paths : list[str]
             A list of paths to search for yaml config files. Defaults to the
             paths passed when creating this object.
 
-        env : dict
+        env : Mapping[str, str]
             The system environment variables to search through. Defaults to
             the environment dictionary passed when creating this object.
 
         Returns
         -------
         config: dict
 
@@ -412,15 +506,15 @@
         if yaml:
             configs.extend(collect_yaml(paths=paths))
 
         configs.append(collect_env(self.env_prefix, env=env))
 
         return merge(*configs)
 
-    def refresh(self, **kwargs):
+    def refresh(self, **kwargs) -> None:
         """Update configuration by re-reading yaml files and env variables.
 
         This goes through the following stages:
 
         1.  Clearing out all old configuration
         2.  Updating from the stored defaults from downstream libraries
             (see update_defaults)
@@ -440,15 +534,15 @@
         self.clear()
 
         for d in self.defaults:
             update(self.config, d, priority="old")
 
         update(self.config, self.collect(**kwargs))
 
-    def get(self, key, default=no_default):
+    def get(self, key: str, default: Any = no_default) -> Any:
         """Get elements from global config
 
         Use '.' for nested access
 
         Examples
         --------
         >>> from donfig import Config
@@ -476,26 +570,28 @@
             except (TypeError, IndexError, KeyError):
                 if default is not no_default:
                     return default
                 else:
                     raise
         return result
 
-    def update_defaults(self, new):
+    def update_defaults(self, new: Mapping) -> None:
         """Add a new set of defaults to the configuration
 
         It does two things:
 
         1.  Add the defaults to a collection to be used by refresh() later
-        2.  Updates the config with the new configuration
-            prioritizing older values over newer ones
+        2.  Updates the global config with the new configuration.
+            Old values are prioritized over new ones, unless the current value
+            is the old default, in which case it's updated to the new default.
 
         """
+        current_defaults = merge(*self.defaults)
         self.defaults.append(new)
-        update(self.config, new, priority="old")
+        update(self.config, new, priority="new-defaults", defaults=current_defaults)
 
     def to_dict(self):
         """Return dictionary copy of configuration.
 
         .. warning::
 
             This will copy all keys and values. This includes values that
@@ -521,23 +617,23 @@
         """Update the internal configuration dictionary with `new`.
 
         See :func:`~donfig.config_obj.update` for more information.
 
         """
         self.config = update(self.config, new, priority=priority)
 
-    def expand_environment_variables(self):
+    def expand_environment_variables(self) -> None:
         """Expand any environment variables in this configuration in-place.
 
         See :func:`~donfig.config_obj.expand_environment_variables` for more information.
 
         """
         self.config = expand_environment_variables(self.config)
 
-    def rename(self, aliases):
+    def rename(self, aliases: Mapping) -> None:
         """Rename old keys to new keys
 
         This helps migrate older configuration versions over time
 
         """
         old = []
         new = {}
@@ -585,17 +681,17 @@
         >>> config.set(foo__bar=123)  # doctest: +SKIP
 
         See Also
         --------
         donfig.Config.get
 
         """
-        return ConfigSet(self.config, self.config_lock, arg=arg, **kwargs)
+        return ConfigSet(self.config, self.config_lock, self.deprecations, arg=arg, **kwargs)
 
-    def ensure_file(self, source, destination=None, comment=True):
+    def ensure_file(self, source: str, destination: str | None = None, comment: bool = True) -> None:
         """Copy file to default location if it does not already exist
 
         This tries to move a default configuration file to a default location if
         if does not already exist.  It also comments out that file by default.
 
         This is to be used by downstream modules that may
         have default configuration files that they wish to include in the default
@@ -632,23 +728,67 @@
                 # a race condition where a process can be busy creating the
                 # destination while another process reads an empty config file.
                 tmp = "%s.tmp.%d" % (destination, os.getpid())
                 with open(source) as f:
                     lines = list(f)
 
                 if comment:
-                    lines = [
-                        "# " + line
-                        if line.strip() and not line.startswith("#")
-                        else line
-                        for line in lines
-                    ]
+                    lines = ["# " + line if line.strip() and not line.startswith("#") else line for line in lines]
 
                 with open(tmp, "w") as f:
                     f.write("".join(lines))
 
                 try:
                     os.rename(tmp, destination)
                 except OSError:
                     os.remove(tmp)
         except OSError:
             pass
+
+    def serialize(self) -> str:
+        """Serialize conifg data into a string.
+
+        See :func:`serialize` for more information.
+
+        """
+        return serialize(self.config)
+
+
+def serialize(data: Any) -> str:
+    """Serialize config data into a string.
+
+    Typically used to pass config via the ``MYPKG_INTERNAL_INHERIT_CONFIG`` environment variable.
+
+    Parameters
+    ----------
+    data: json-serializable object
+        The data to serialize
+
+    Returns
+    -------
+    serialized_data: str
+        The serialized data as a string
+
+    """
+    return base64.urlsafe_b64encode(json.dumps(data).encode()).decode()
+
+
+def deserialize(data: str) -> Any:
+    """De-serialize config data into the original object.
+
+    Typically used when receiving config via the
+    ``MYPKG_INTERNAL_INHERIT_CONFIG`` environment variable. This is
+    automatically called when a :class:`Config` is created and environment
+    variables are loaded.
+
+    Parameters
+    ----------
+    data: str
+        String serialized by :func:`donfig.serialize`
+
+    Returns
+    -------
+    deserialized_data: obj
+        The de-serialized data
+
+    """
+    return json.loads(base64.urlsafe_b64decode(data.encode()).decode())
```

### Comparing `donfig-0.7.0/donfig/utils.py` & `donfig-0.8.0/donfig/utils.py`

 * *Files identical despite different names*

