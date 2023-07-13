# Comparing `tmp/fuo-ytmusic-0.2.1.tar.gz` & `tmp/fuo-ytmusic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo-ytmusic-0.2.1.tar", last modified: Thu Jul 13 15:47:24 2023, max compression
+gzip compressed data, was "fuo-ytmusic-0.2.2.tar", last modified: Thu Jul 13 15:50:59 2023, max compression
```

## Comparing `fuo-ytmusic-0.2.1.tar` & `fuo-ytmusic-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:47:24.601179 fuo-ytmusic-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 15:47:24.601179 fuo-ytmusic-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:47:24.597178 fuo-ytmusic-0.2.1/fuo_ytmusic/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:47:24.601179 fuo-ytmusic-0.2.1/fuo_ytmusic/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18244 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/page_explore_qml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/page_fav.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/page_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:47:24.601179 fuo-ytmusic-0.2.1/fuo_ytmusic/qml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:47:24.601179 fuo-ytmusic-0.2.1/fuo_ytmusic/qml/dummydata/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/qml/dummydata/explore_backend.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/qml/page_explore.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/qml/uploader.qml
--rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/timeparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/fuo_ytmusic/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:47:24.597178 fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 15:47:24.000000 fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-13 15:47:24.000000 fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:47:24.000000 fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 15:47:24.000000 fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 15:47:24.000000 fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 15:47:24.000000 fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 15:47:24.601179 fuo-ytmusic-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 15:47:23.000000 fuo-ytmusic-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:50:59.194598 fuo-ytmusic-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 15:50:59.194598 fuo-ytmusic-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:50:59.190597 fuo-ytmusic-0.2.2/fuo_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:50:59.194598 fuo-ytmusic-0.2.2/fuo_ytmusic/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18244 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/page_explore_qml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/page_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:50:59.194598 fuo-ytmusic-0.2.2/fuo_ytmusic/qml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:50:59.194598 fuo-ytmusic-0.2.2/fuo_ytmusic/qml/dummydata/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/qml/dummydata/explore_backend.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/qml/page_explore.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/qml/uploader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/timeparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/fuo_ytmusic/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:50:59.194598 fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 15:50:58.000000 fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-13 15:50:59.000000 fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:50:58.000000 fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 15:50:58.000000 fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 15:50:58.000000 fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 15:50:58.000000 fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 15:50:59.194598 fuo-ytmusic-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 15:50:57.000000 fuo-ytmusic-0.2.2/setup.py
```

### Comparing `fuo-ytmusic-0.2.1/LICENSE.txt` & `fuo-ytmusic-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/PKG-INFO` & `fuo-ytmusic-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fuo-ytmusic
-Version: 0.2.1
+Version: 0.2.2
 Summary: feeluown Youtube Music plugin
 Home-page: https://github.com/feeluown/feeluown-ytmusic
 Author: Bruce Zhang
 Author-email: zttt183525594@gmail.com
 License: UNKNOWN
 Description: # YouTube Music plugin for FeelUOwn player
```

### Comparing `fuo-ytmusic-0.2.1/README.md` & `fuo-ytmusic-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
 - [x] Get song detail by id
 - [ ] Add/remove song from a playlist
 - [ ] Upload songs to cloud
 - [ ] Discovering page
 
 ## Changelog
 
-- v0.2.1 (2023-07-13)
+- v0.2.2 (2023-07-13)
   - fix can't get song media properly
 
 ## License
 
 This project is licensed under the [GPLv3](LICENSE.txt).
```

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/__init__.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from feeluown.app import App
 
 __alias__ = 'ytmusic'
-__version__ = '0.2.0'
+__version__ = '0.2.2'
 __desc__ = 'YouTube Music plugin'
 
 
 ui_mgr = None
 
 
 def init_config(config):
```

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/assets/icon.svg` & `fuo-ytmusic-0.2.2/fuo_ytmusic/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/models.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/models.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/page_explore_qml.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/page_explore_qml.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/page_fav.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/page_fav.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/page_more.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/page_more.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/patch.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/patch.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/provider.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/provider.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/qml/dummydata/explore_backend.qml` & `fuo-ytmusic-0.2.2/fuo_ytmusic/qml/dummydata/explore_backend.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/qml/page_explore.qml` & `fuo-ytmusic-0.2.2/fuo_ytmusic/qml/page_explore.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/qml/uploader.qml` & `fuo-ytmusic-0.2.2/fuo_ytmusic/qml/uploader.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/service.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/service.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/timeparse.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/timeparse.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic/ui.py` & `fuo-ytmusic-0.2.2/fuo_ytmusic/ui.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/PKG-INFO` & `fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fuo-ytmusic
-Version: 0.2.1
+Version: 0.2.2
 Summary: feeluown Youtube Music plugin
 Home-page: https://github.com/feeluown/feeluown-ytmusic
 Author: Bruce Zhang
 Author-email: zttt183525594@gmail.com
 License: UNKNOWN
 Description: # YouTube Music plugin for FeelUOwn player
```

### Comparing `fuo-ytmusic-0.2.1/fuo_ytmusic.egg-info/SOURCES.txt` & `fuo-ytmusic-0.2.2/fuo_ytmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.1/pyproject.toml` & `fuo-ytmusic-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fuo-ytmusic"
-version = "0.2.0"
+version = "0.2.2"
 description = "feeluown Youtube Music plugin"
 authors = ["Bruce Zhang <zttt183525594@gmail.com>"]
 keywords = ["feeluown", "ytmusic", "youtube"]
 homepage = "https://github.com/feeluown/feeluown-ytmusic"
 readme = "README.md"
 include = ["fuo_ytmusic/assets/*.svg", "fuo_ytmusic/qml/*.qml"]
```

### Comparing `fuo-ytmusic-0.2.1/setup.py` & `fuo-ytmusic-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['cachetools', 'feeluown>=3.7.13', 'pydantic', 'pytube', 'ytmusicapi']
 
 entry_points = \
 {'fuo.plugins_v1': ['ytmusic = fuo_ytmusic']}
 
 setup_kwargs = {
     'name': 'fuo-ytmusic',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'feeluown Youtube Music plugin',
     'long_description': "# YouTube Music plugin for FeelUOwn player\n\n## Prerequisites\n\nInstall [FeelUOwn](https://github.com/feeluown/FeelUOwn) before installing this plugin.\nSees: [Documentation](https://feeluown.readthedocs.io/)\n\n## Installation\n\n```shell\npip install fuo-ytmusic  # Lastest stable release\npip install https://github.com/feeluown/feeluown-ytmusic.git  # master branch\npoetry install  # Local development\n```\n\n## Configuration\n\n### Proxies\n\n```python\n# In ~/.fuorc\nconfig.deffield('YTM_HTTP_PROXY', type_=str, default='', desc='YouTube Music 代理设置')\nconfig.YTM_HTTP_PROXY='127.0.0.1:10809'\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please create a new issue first to discuss what you'd like to change.\n\nPlease make sure to compatible with [FeelUOwn](https://github.com/feeluown/FeelUOwn) lastest stable release.\n\n## License\n\nThis project is licensed under the [GPLv3](LICENSE.txt).\n",
     'author': 'Bruce Zhang',
     'author_email': 'zttt183525594@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/feeluown/feeluown-ytmusic',
```

