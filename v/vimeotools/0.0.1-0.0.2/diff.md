# Comparing `tmp/vimeotools-0.0.1.tar.gz` & `tmp/vimeotools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vimeotools-0.0.1.tar", last modified: Sat Jul  8 17:09:32 2023, max compression
+gzip compressed data, was "dist/vimeotools-0.0.2.tar", last modified: Thu Jul 13 14:07:37 2023, max compression
```

## Comparing `vimeotools-0.0.1.tar` & `vimeotools-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-08 17:09:32.694799 vimeotools-0.0.1/
--rw-r--r--   0 georg      (502) staff       (20)     2292 2023-07-08 17:09:32.694994 vimeotools-0.0.1/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)     1229 2023-07-08 16:58:08.000000 vimeotools-0.0.1/README.md
--rw-r--r--   0 georg      (502) staff       (20)      806 2023-07-08 17:09:32.695659 vimeotools-0.0.1/setup.cfg
--rw-r--r--   0 georg      (502) staff       (20)       69 2023-07-07 15:14:58.000000 vimeotools-0.0.1/setup.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-08 17:09:32.683733 vimeotools-0.0.1/src/
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-08 17:09:32.691798 vimeotools-0.0.1/src/vimeotools/
--rw-r--r--   0 georg      (502) staff       (20)      335 2023-07-07 15:14:58.000000 vimeotools-0.0.1/src/vimeotools/__init__.py
--rw-r--r--   0 georg      (502) staff       (20)    17555 2023-07-08 06:46:19.000000 vimeotools-0.0.1/src/vimeotools/vimeo_base.py
--rw-r--r--   0 georg      (502) staff       (20)     1553 2023-07-08 10:11:11.000000 vimeotools-0.0.1/src/vimeotools/vimeo_connection.py
--rw-r--r--   0 georg      (502) staff       (20)    19279 2023-07-08 06:49:12.000000 vimeotools-0.0.1/src/vimeotools/vimeo_constants.py
--rw-r--r--   0 georg      (502) staff       (20)    30913 2023-07-08 10:50:09.000000 vimeotools-0.0.1/src/vimeotools/vimeo_data.py
--rw-r--r--   0 georg      (502) staff       (20)     8403 2023-07-08 06:49:53.000000 vimeotools-0.0.1/src/vimeotools/vimeo_folder.py
--rw-r--r--   0 georg      (502) staff       (20)    10807 2023-07-08 06:47:19.000000 vimeotools-0.0.1/src/vimeotools/vimeo_showcase.py
--rw-r--r--   0 georg      (502) staff       (20)     8046 2023-07-07 15:14:58.000000 vimeotools-0.0.1/src/vimeotools/vimeo_video.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-08 17:09:32.694431 vimeotools-0.0.1/src/vimeotools.egg-info/
--rw-r--r--   0 georg      (502) staff       (20)     2292 2023-07-08 17:09:31.000000 vimeotools-0.0.1/src/vimeotools.egg-info/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)      465 2023-07-08 17:09:32.000000 vimeotools-0.0.1/src/vimeotools.egg-info/SOURCES.txt
--rw-r--r--   0 georg      (502) staff       (20)        1 2023-07-08 17:09:32.000000 vimeotools-0.0.1/src/vimeotools.egg-info/dependency_links.txt
--rw-r--r--   0 georg      (502) staff       (20)        8 2023-07-08 17:09:32.000000 vimeotools-0.0.1/src/vimeotools.egg-info/requires.txt
--rw-r--r--   0 georg      (502) staff       (20)       11 2023-07-08 17:09:32.000000 vimeotools-0.0.1/src/vimeotools.egg-info/top_level.txt
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 14:07:37.437346 vimeotools-0.0.2/
+-rw-r--r--   0 georg      (502) staff       (20)     3050 2023-07-13 14:07:37.437548 vimeotools-0.0.2/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)     1229 2023-07-08 16:58:08.000000 vimeotools-0.0.2/README.md
+-rw-r--r--   0 georg      (502) staff       (20)      806 2023-07-13 14:07:37.438348 vimeotools-0.0.2/setup.cfg
+-rw-r--r--   0 georg      (502) staff       (20)       69 2023-07-07 15:14:58.000000 vimeotools-0.0.2/setup.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 14:07:37.426527 vimeotools-0.0.2/src/
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 14:07:37.434193 vimeotools-0.0.2/src/vimeotools/
+-rw-r--r--   0 georg      (502) staff       (20)      335 2023-07-07 15:14:58.000000 vimeotools-0.0.2/src/vimeotools/__init__.py
+-rw-r--r--   0 georg      (502) staff       (20)    14614 2023-07-13 10:51:12.000000 vimeotools-0.0.2/src/vimeotools/vimeo_base.py
+-rw-r--r--   0 georg      (502) staff       (20)     1597 2023-07-13 04:27:52.000000 vimeotools-0.0.2/src/vimeotools/vimeo_connection.py
+-rw-r--r--   0 georg      (502) staff       (20)    19344 2023-07-13 09:54:51.000000 vimeotools-0.0.2/src/vimeotools/vimeo_constants.py
+-rw-r--r--   0 georg      (502) staff       (20)    34427 2023-07-13 13:25:48.000000 vimeotools-0.0.2/src/vimeotools/vimeo_data.py
+-rw-r--r--   0 georg      (502) staff       (20)     8799 2023-07-13 04:42:19.000000 vimeotools-0.0.2/src/vimeotools/vimeo_folder.py
+-rw-r--r--   0 georg      (502) staff       (20)    11723 2023-07-13 10:56:05.000000 vimeotools-0.0.2/src/vimeotools/vimeo_showcase.py
+-rw-r--r--   0 georg      (502) staff       (20)    12553 2023-07-13 05:54:15.000000 vimeotools-0.0.2/src/vimeotools/vimeo_video.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 14:07:37.436973 vimeotools-0.0.2/src/vimeotools.egg-info/
+-rw-r--r--   0 georg      (502) staff       (20)     3050 2023-07-13 14:07:36.000000 vimeotools-0.0.2/src/vimeotools.egg-info/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)      465 2023-07-13 14:07:37.000000 vimeotools-0.0.2/src/vimeotools.egg-info/SOURCES.txt
+-rw-r--r--   0 georg      (502) staff       (20)        1 2023-07-13 14:07:36.000000 vimeotools-0.0.2/src/vimeotools.egg-info/dependency_links.txt
+-rw-r--r--   0 georg      (502) staff       (20)        8 2023-07-13 14:07:37.000000 vimeotools-0.0.2/src/vimeotools.egg-info/requires.txt
+-rw-r--r--   0 georg      (502) staff       (20)       11 2023-07-13 14:07:37.000000 vimeotools-0.0.2/src/vimeotools.egg-info/top_level.txt
```

### Comparing `vimeotools-0.0.1/PKG-INFO` & `vimeotools-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vimeotools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tools for Vimeo
 Home-page: https://github.com/georgpfolz/vimeotools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/georgpfolz/vimeotools/issues
 Project-URL: Documentation, https://georgpfolz.github.io/vimeotools
@@ -40,13 +40,22 @@
 
 You can also opt to create or set an object in live mode, so everytime a property is queried, the appropriate request is made on Vimeo first.
 
 ## documentation
 The (Sphinx) documentation is very crude (created with autodoc) currently and will be improved in subsequent versions.
 
 # History
+## 0.0.2 (2023-07-12)
+- VimeoData gets the methods **save** and **load**, to save or load data as json or pickle. 
+- the **__init__** of VimeoVideo, VimeoShowcase, VimeoFolder gets a parameter **data**, where the data can be passed when the object is created, so no request is needed.
+- Objects have a new attribute **temp_data** (dictionary) where you can store data relevant to your runing program directly on the object.
+- The **VimeoData** object can be added to **VimeoVideo**, **VimeoShowcase** and **VimeoFolder** instances. So the data object can be updated if there is a change in one of those insetances.
+- using **pathlib** (instead of os.path): all filepath parameters accept Path objects.
+
+Still no unit tests, this is still very much in beta!
+
 ## 0.0.1 (2023-07-07)
 This is the first version. It provides the **VimeoConnection**, **VimeoData**, **Video** and **VimeoShowcase** and **VimeoFolder** classes.
 
 The package is still very much in beta, as many of the possible methods of this classes are not implemented yet and other classes (e.g. for Groups or Portfolios) shall be implemented later. It is also not well tested at the moment. Use it at your own risk!
```

### Comparing `vimeotools-0.0.1/README.md` & `vimeotools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.1/setup.cfg` & `vimeotools-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vimeotools
-version = 0.0.1
+version = 0.0.2
 author = Georg Pfolz
 author_email = georg.pfolz@invesy.at
 description = Tools for Vimeo
 long_description = file: README.md,HISTORY.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE.txt
```

### Comparing `vimeotools-0.0.1/src/vimeotools/vimeo_base.py` & `vimeotools-0.0.2/src/vimeotools/vimeo_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,42 @@
 """
 
 from typing import TYPE_CHECKING, Dict, Optional, List, Union, Any, Literal
 import json
 from vimeo_constants import (
     GETTER_STR,
     SETTER_STR,
-    PROPERTIES_BASE
+    PROPERTIES_BASE,
+    RETURNING_MAP,
+    WHAT_MAP
 )
 if TYPE_CHECKING:
     from vimeo_folder import VimeoFolder
     from vimeo_connection import VimeoConnection
+    from vimeo_data import VimeoData
+
+def transform_returning(
+    returning: str
+) -> str:
+    returning = returning.lower()
+
+    try:
+        return RETURNING_MAP[returning]
+    except KeyError:
+        raise ValueError(f'Unknown value for returning: {returning}')
+
+def transform_what(
+    what: str
+) -> str:
+    what = what.lower()
+
+    try:
+        return WHAT_MAP[what]
+    except KeyError:
+        raise ValueError(f'Unknown value for what: {what}')
 
 def nested_value(
     data: Dict[str, Any],
     path: Union[List[str], str]
 ) -> Any:
     """
     Get a nested value from a dictionary using a list of keys as the path.
@@ -144,15 +167,15 @@
     def get_parent_folder_data(
         self,
         keys: Optional[List[str]] = None,
         refresh: bool = False
     ) -> Dict[str, Any]:
         if not refresh and self._parent:
             return self._parent.get_data(refresh=False)
-            
+        
         folder_data = self.get_data(refresh=refresh).get('parent_folder', {}) # type: ignore
 
         if not keys:
             return folder_data
         else:
             return {k: folder_data[k] for k in keys if k in folder_data}
     
@@ -227,39 +250,57 @@
     def uri(self) -> str:
         return self._uri
     
     @property
     def code(self) -> str:
         return self._code
     
+    @property
+    def temp_data(self) -> Dict[str, Any]:
+        return self._temp_data
+    
+    @temp_data.setter
+    def temp_data(self, value: Dict[str, Any]) -> None:
+        self._temp_data = value
+
     for key, val in PROPERTIES_BASE.items():
         exec(GETTER_STR.format(prop=key))
         if val['type'] == 'str' and val.get('setable'):
             key = val.get('set_key', key)
             exec(SETTER_STR.format(prop=key))
 
     def __init__(
         self,
         connection: 'VimeoConnection',
         code_or_uri: Optional[str] = None,
-        live: bool = False  # live mode
+        live: bool = False,  # live mode
+        data: Optional[Dict[str, Any]] = None,
+        data_object: Optional['VimeoData'] = None
     ):
         self.connection = connection
         self.client = connection.client
         self._live = live
+        self._temp_data = {}  # temporary data storage for the object
+        data_object = data_object
+
+        if data_object and not data:
+            data = data_object._data
+
+        if data:
+            self._data = data
+        else:
+            self._data = None  # initialize data as hidden attribute: method get_data() has to be used
 
         if code_or_uri:
             if '/' in code_or_uri:  # assume it's a uri
                 self._uri = code_or_uri
                 self._code = code_or_uri.split('/')[-1]
             else:  # assume it's a code
                 self._code = code_or_uri
                 self._uri = f'{self.BASE_URI}/{code_or_uri}'
-
-        self._data = None  # initialize data as hidden attribute: method get_data() has to be used
     
     def _keys_is_allowed_to_set(
         self,
         key: str
     ) -> bool:
         key = key.split(' ')[0]  # some keys can include a number after the key name
         allowed_keys = [key.split(' ')[0] for key in self.allowed_keys_to_set] # type: ignore (in child class)
@@ -371,14 +412,26 @@
         return self.get_property(
             property='user'
         )
     
     def get_user_link(self) -> str:
         return self.get_user_data()['link']
     
+    @property
+    def user_uri(self) -> str:
+        return self.get_user_data()['uri']
+    
+    @property
+    def user_id(self) -> str:
+        return self.user_uri.split('/')[-1]
+
+    @property
+    def user_name(self) -> str:
+        return self.get_user_data()['name']
+
     def get_user_uri(self) -> str:
         return self.get_user_data()['uri']
 
     def get_user_name(
         self
     ) -> str:
         return self.get_user_data()['name']
@@ -443,182 +496,35 @@
         self._data = data
 
 
 class VimeoItem(VimeoBaseItem):  # videos and showcases
     """
     An abstract class to represent a Vimeo Item. This is the base of the
     Video and Showcase classes.
-
-    One key method is get_data(), which not only returns the item's data
-    but also stores it in the object for future use. If the refresh parameter
-    is not set to True, the data will not be fetched again from the API in
-    subsequent calls to get_data().
     """
 
     def __init__(
         self,
         connection: 'VimeoConnection',
-        code_or_uri: str
+        code_or_uri: str,
+        data: Optional[Dict[str, Any]] = None,
+        data_object: Optional['VimeoData'] = None
     ):
         """
         Initialize the VimeoItem object.
 
         :param code_or_uri: str
         :param client: vimeo.VimeoClient, or a Vimeo instance's 
                        (from this module) client attribute
         """
         super().__init__(
             connection=connection,
-            code_or_uri=code_or_uri
-        )
-
-    def add_tag(
-        self,
-        tag: str,
-        refresh: bool = False
-    ):
-        self.add_tags(
-            tags=tag,
-            refresh=refresh
-        )
-
-    def add_tags(
-        self,
-        tags: Union[str, List[str]],
-        refresh: bool = False
-    ):
-        """
-        Add tags to the video.
-        :param tags: str or list of str
-        :param refresh: bool
-        :return: None
-        """
-        if isinstance(tags, str):
-            tags = [tags]
-        
-        tags = self.get_tags(refresh=refresh) + tags # type: ignore
-
-        self.set_tags(
-            tags=tags
+            code_or_uri=code_or_uri,
+            data=data,
+            data_object=data_object
         )
 
     def get_description(
         self,
         refresh: bool = False
     ) -> str:
         return self.get_property('description', refresh=refresh)
-
-    def get_tags(
-        self,
-        returning: Literal[
-            'dict',
-            'list',
-            'json',
-            'names',
-            'name',
-            'uris',
-            'uri',
-            'tags',
-            'tag',
-            'canonical'
-        ] = 'dict',
-        refresh: bool = False
-    ) -> Union[List[str], str]:
-        tags = self.get_property('tags', refresh=refresh)
-
-        # not sure why data has not always the same structure
-        if isinstance(tags, dict):
-            tags = tags['data']
-
-        if returning == 'dict':
-            return tags
-        elif returning == 'list':
-            return tags['data']
-        elif returning == 'json':
-            return json.dumps(tags)
-        else:
-            if returning.endswith('s'):
-                returning = returning[:-1] # type: ignore
-            return [tag[returning] for tag in tags]
-
-    def remove_tag(
-        self,
-        tag: str
-    ):
-        """
-        Remove a tag from the video.
-        :param tag: str
-        :return: None
-
-        This method uses the delete method of the Vimeo API.
-        """
-        response = self.client.delete(
-            f'{self.uri}/tags/{tag}'
-        )
-        assert response.status_code == 204, f'Error: {response.status_code}'
-        self._data['tags'] = response.text.json()['tags']  # type: ignore
-
-    def remove_tags(
-        self,
-        tags: Union[str, List[str]],
-        refresh: bool = False
-    ):
-        """
-        Remove tags from the video.
-        :param tags: str or list of str
-        :param refresh: bool
-        :return: None
-
-        This method uses the put method of the Vimeo API.
-        """
-        if isinstance(tags, str):
-            tags = [tags]
-        
-        tags_list = [{'name': tag} for tag in self.get_tags(refresh=refresh) if tag not in tags]
-        
-        response = self.client.put(
-            f'{self.uri}/tags',
-            data=tags_list
-        )
-        assert response.status_code == 200, f'Error: {response.status_code}'
-        self._data['tags'] = tags  # type: ignore
-
-    def set_description(self, value: str):
-        self.set_property(
-            key='description',
-            value=value
-        )
-
-    def set_tags(
-        self,
-        tags: Union[str, List[str], List[Dict[str, str]]]
-    ):
-        set_tags = []
-        for tag in tags:
-            if isinstance(tag, str):
-                set_tags.append({'name': tag})
-            if isinstance(tag, dict):
-                set_tags.append({'name': tag['name']})
-
-        uri = f'{self.uri}/tags'
-        
-        tags_list = [tag for tag in set_tags]
-        response = self.client.put(
-            uri,
-            data=tags_list
-        )
-        if response.status_code == 400:
-            raise Exception((
-                '400: Bad Request,'
-                "either the request body wasn't supplied,"
-                'or a parameter is invalid, '
-                "The request body doesn't contain a JSON-encoded list of tags. "
-                f'You supplied: {tags_list}'
-            ))
-        elif response.status_code == 403:
-            raise Exception((
-                '403: Forbidden, you are not allowed to add tags to this video.'
-                'You may not have the permission or the total number of tags exceeds the limit (20). '
-                f'You supplied: {tags_list}'
-            ))
-        assert response.status_code == 200, f'Error: {response.status_code}'
-        self._data['tags'] = response.json()  # type: ignore
```

### Comparing `vimeotools-0.0.1/src/vimeotools/vimeo_connection.py` & `vimeotools-0.0.2/src/vimeotools/vimeo_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 from the vimeo package and the base URI, which is used to build the
 request URIs.
 """
 
 from typing import TYPE_CHECKING, Dict, Optional, List, Any, Union, Literal
 import vimeo
 import json
+from pathlib import Path
     
 
 class VimeoConnection:
 
     def __init__(
         self,
-        config_file: Optional[str] = 'vimeo_config.json',
+        config_file: Optional[Union[str, Path]] = Path('vimeo_config.json'),
         token: Optional[str] = None,
         key: Optional[str] = None,
         secret: Optional[str] = None
     ):
         """
         Initialize the Vimeo client.
```

### Comparing `vimeotools-0.0.1/src/vimeotools/vimeo_constants.py` & `vimeotools-0.0.2/src/vimeotools/vimeo_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     return self.get_data()['{prop}']
 """
 
 SETTER_STR = """
 @{prop}.setter
 def {prop}(self, value: str):
     self._data['{prop}'] = value
-    self._set_key('{prop}', value)
+    self.set_property('{set_key}', value)
 """
 
 # properties that are common to VimeoVideo, VimeoShowcase, VimeoFolder
 
 PROPERTIES_BASE = {
     'name': {'type': str, 'setable': True},
     'created_time': {'type': str},
@@ -216,14 +216,15 @@
     'hide_nav',  #  	    Boolean	Whether to hide Vimeo navigation when displaying the showcase.
     'hide_upcoming',  #     Boolean	Whether to include the upcoming live event in the showcase.
     'layout',  #    	    String	The type of layout for presenting the showcase.
                     #           grid - The videos appear in a grid.
                     #           player - The videos appear in the player.
                     #           name	String	The name of the showcase.
                     #           password	String	The showcase's password. This field is required only when privacy is password.
+    'name',  #      	    String	The name of the showcase.
     'privacy',  #    	    String	The privacy level of the showcase.
                     #           anybody - Anyone can access the showcase, either on Vimeo or through an embed.
                     #           embed_only - The showcase doesn't appear on Vimeo, but it can be embedded on other sites.
                     #           nobody - No one can access the showcase, including the authenticated user.
                     #           password - Only people with the password can access the showcase.
                     #           team - Only members of the authenticated user's team can access the showcase.
                     #           unlisted - The showcase can't be accessed if the URL omits its unlisted hash.
```

### Comparing `vimeotools-0.0.1/src/vimeotools/vimeo_data.py` & `vimeotools-0.0.2/src/vimeotools/vimeo_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,48 +4,60 @@
 Vimeo Tools VimeoData
 =====================
 
 This module contains the class VimeoData, which is used to display
 information about a Vimeo account and its videos, folders and albums.
 """
 from typing import TYPE_CHECKING, Dict, Optional, List, Union, Any, Literal
+from pathlib import Path
 import json
+import pickle
 from vimeo_constants import (
-    MIN_KEYS,
-    RETURNING_MAP,
-    WHAT_MAP
+    MIN_KEYS
+)
+from vimeo_base import (
+    get_lines,
+    nested_value,
+    transform_returning,
+    transform_what
 )
-from vimeo_base import get_lines, nested_value
 from vimeo_connection import VimeoConnection
 from vimeo_video import VimeoVideo
 from vimeo_folder import VimeoFolder
 from vimeo_showcase import VimeoShowcase
 
 class VimeoData:
 
     def __init__(
         self,
         connection: VimeoConnection,
+        data_file: Optional[str] = None
     ):
         """
         Class for displaying information about a Vimeo account:
         - Account data
         - Videos
         - Folders
         - Showcases (Albums)
         """
         self.connection = connection
         self.client = connection.client
         self.uri = connection.uri
 
-        # initialize
-        self._account_data = None
-        self._videos_data = None
-        self._folders_data = None
-        self._albums_data = None
+        if data_file:
+            self.load(
+                file=data_file
+            )
+        else:
+            # initialize
+            self._account_data = None
+            self._videos_data = None
+            self._folders_data = None
+            self._albums_data = None
+        
         self._videos = None
         self._folders = None
         self._albums = None
 
     def info(
         self
     ) -> str:
@@ -173,56 +185,65 @@
         :param localpath: If it exists, fetches data from local file.
         :param returning:
         - If 'dict', returns the video data as a dict, as provided by Vimeo.
         - If 'list', returns a list of dicts (one dict per video, as in the 'data' key of the Vimeo response)
         - If 'json', returns a json string.
         """
         # set returning to singular
-        returning = self._transform_returning(returning=returning)  # type: ignore
+        returning = transform_returning(returning=returning)  # type: ignore
 
-        data = {}
+        data = {'data': []}
 
         data_stored = self._data_stored(what=what)
         items_stored = self._items_stored(what=what)
-
+        
         if not refresh:
             if returning == 'dict' and data_stored:
                 return data_stored
             elif returning == 'object' and items_stored:
+
                 return items_stored
 
-        # no refresh or first time
-        items_list = []
-        page = 1
+        if not refresh:
+            if what == 'videos' and self._videos_data:
+                data['data'] = self._videos_data.get('data', [])
+            elif what == 'albums' and self._albums_data:
+                data['data'] = self._albums_data.get('data', [])
+            elif what == 'projects' and self._folders_data:
+                data['data'] = self._folders_data.get('data', [])
         
-        while True:
-            response = self.client.get(
-                f'/me/{what}',
-                params={
-                    'page': page,
-                    'per_page': 100
-                }
-            )
-            if response.status_code != 200:
-                raise Exception(f'Error getting {what}: {response.text}')
-            
-            # we don't care if data is overwritten!
-            # this way we end with the last page number
-            # and the items_list is added thereafter anyway
-            data = response.json()
+        if not data.get('data'):
+            # no refresh or first time
+            items_list = []
+            page = 1
+            while True:
+                response = self.client.get(
+                    f'/me/{what}',
+                    params={
+                        'page': page,
+                        'per_page': 100
+                    }
+                )
+                if response.status_code != 200:
+                    raise Exception(f'Error getting {what}: {response.text}')
+                
+                # we don't care if data is overwritten!
+                # this way we end with the last page number
+                # and the items_list is added thereafter anyway
+                data = response.json()
 
-            for item in data['data']:
-                item['code'] = item.get('uri').split('/')[-1]  # add vimeo code to data
+                for item in data['data']:
+                    item['code'] = item.get('uri').split('/')[-1]  # add vimeo code to data
 
-            items_list.extend(data['data'])
-            if data['paging']['next'] is None:
-                break
-            page += 1
+                items_list.extend(data['data'])
+                if data['paging']['next'] is None:
+                    break
+                page += 1
 
-        data['data'] = items_list
+            data['data'] = items_list
 
         # at this point, data must be a dict
         if what == 'videos':
             self._videos_data = data
         elif what == 'albums':
             self._albums_data = data
         elif what == 'projects':
@@ -231,47 +252,53 @@
         if returning == 'dict':
             return data
         elif returning == 'object':
             if what == 'videos':
                 videos = [
                     VimeoVideo(
                         code_or_uri=video['uri'],
-                        conection=self.connection
+                        connection=self.connection,
+                        data_object=self,
+                        data=video
                     )
                     for video
-                    in items_list
+                    in data['data']
                 ]
                 self._videos = videos
                 return videos
             elif what == 'albums':
                 albums = [
                     VimeoShowcase(
                         code_or_uri=album['uri'],
-                        connection=self.connection
+                        connection=self.connection,
+                        data_object=self,
+                        data=album
                     )
                     for album
-                    in items_list
+                    in data['data']
                 ]
                 self._albums = albums
                 return albums
             elif what == 'projects':
                 folders = [
                     VimeoFolder(
                         code_or_uri=folder['uri'],
-                        connection=self.connection
+                        connection=self.connection,
+                        data_object=self,
+                        data=folder
                     )
                     for folder
-                    in items_list
+                    in data['data']
                 ]
                 self._folders = folders
                 return folders
         elif returning in ('code', 'uri'):
-            return [item[returning] for item in items_list]
+            return [item[returning] for item in data['data']]
         elif returning == 'list':
-            return items_list
+            return data['data']
         elif returning == 'json':
             return json.dumps(data, indent=4)
         else:
             # will never happen, we keep it for the return type check
             raise ValueError(f'Unknown returning value: {returning}')
     
     def get_count(
@@ -401,15 +428,15 @@
             List[Dict[str, Any]],
             List[VimeoFolder], str
         ]:
         """
         Get all folders.
         :return: list of VimeoFolder objects
         """
-        returning = self._transform_returning(returning) # type: ignore
+        returning = transform_returning(returning) # type: ignore
 
         return self._get_items(
             what='projects',
             returning=returning, # type: ignore
             refresh=refresh
         ) # type: ignore
 
@@ -527,15 +554,15 @@
                           - 'object', 'objects, 'album' or 'albums': returns a list of VimeoVideo objects
                           - 'dict': returns a dict as provided by the Vimeo API
                           - 'list': returns a list of dict as provided by the Vimeo API in the 'data' key
                           - 'json': returns a json string
         
         Obviously, returning the list of VimeoShowcase objects takes more time than returning the list of dicts.
         """
-        returning = self._transform_returning(returning) # type: ignore
+        returning = transform_returning(returning) # type: ignore
 
         return self._get_items(
             what='albums',
             returning=returning,  # type: ignore
             refresh=refresh
         ) # type: ignore
     
@@ -548,15 +575,15 @@
             'account',
             'all'
         ] = 'all'
     ) -> None:
         """
         Refresh data.
         """
-        what = self._transform_what(what) # type: ignore
+        what = transform_what(what) # type: ignore
 
         if what in ('account', 'all'):
             self._get_account_data(
                 refresh=True
             )
         if what in ('albums', 'all'):
             self._get_items(
@@ -736,15 +763,15 @@
                           - 'item', 'items, 'video' or 'videos': returns a list of VimeoVideo objects
                           - 'dict': returns a dict as provided by the Vimeo API
                           - 'list': returns a list of dict as provided by the Vimeo API in the 'data' key
                           - 'json': returns a json string
         
         Obviously, returning the list of VimeoVideo objects takes more time than returning the list of dicts.
         """
-        returning = self._transform_returning(returning) # type: ignore
+        returning = transform_returning(returning) # type: ignore
 
         return self._get_items(
             what='videos',
             returning=returning,  # type: ignore
             refresh=refresh
         ) # type: ignore
 
@@ -785,15 +812,15 @@
         :param album_code: str
         :param returning: str, default: 'dict'
         :return: list of dict
 
         Example:
         vimeo_client.get_videos_from_album(album='123456', returning='list')
         """
-        returning = self._transform_returning(returning) # type: ignore
+        returning = transform_returning(returning) # type: ignore
 
         try:
             return showcase.get_videos(  # type: ignore
                 returning=returning
             )
         except AttributeError:
             """
@@ -851,15 +878,15 @@
             'code',
             'codes',
             'uri',
             'uris'
         ] = 'objects',
         refresh: bool = False
     ) -> Union[VimeoVideo, List[Dict[str, Any]], List[str], str]:
-        returning = self._transform_returning(returning) # type: ignore
+        returning = transform_returning(returning) # type: ignore
         
         if not refresh and self._videos_data is not None:
             video = [
                 video
                 for video
                 in self._videos_data['data']
                 if tag in video['tags']['tag']
@@ -915,15 +942,15 @@
         mode: str = 'default',
         ignore_keys: List[str] = [],
         show_keys: List[str] = [],
         indent: int = 0,
         refresh: bool = False,
         returning: Literal['str', 'lines'] = 'str'
     ) -> Union[str, List[str]]:
-        what = self._transform_what(what) # type: ignore
+        what = transform_what(what) # type: ignore
 
         data = {}
 
         if what == 'account':
             data = self._get_account_data(
                 returning='dict',
                 refresh=refresh
@@ -959,36 +986,93 @@
         
         return self._print(
             data=data, # type: ignore (impossible that it's not a dict)
             ignore_keys=ignore_keys,
             indent=indent,
             returning=returning
         )
-        
-    def _transform_what(
+    
+    def load(
         self,
-        what: str
-    ) -> str:
-        what = what.lower()
+        file: Union[Path, str] = Path('vimeo_data.json'),
+        format: Optional[Literal['json', 'pickle']] = None,
+        refresh: bool = False
+    ) -> None:
+        if isinstance(file, str):
+            file = Path(file)
 
-        try:
-            return WHAT_MAP[what]
-        except KeyError:
-            raise ValueError(f'Unknown value for what: {what}')
+        if not file.exists():
+            raise FileNotFoundError(f'File not found: {file}')
+        
+        if not format:
+            format = file.suffix[1:]  # type: ignore
 
-    def _transform_returning(
+        if format == 'json':
+            with open(file, 'r') as f:
+                data = json.load(f)
+        elif format == 'pickle':
+            with open(file, 'rb') as f:
+                data = pickle.load(f)
+        else:
+            raise ValueError(f'Unknown format: {format}')
+        
+        if not data:
+            raise ValueError(f'No data in {file}')
+
+        self._data = data
+
+        # redundant!
+        self._account_data = data['account']
+        self._videos_data = data['videos']
+        self._folders_data = data['projects']
+        self._albums_data = data['albums']
+    
+    def save(
         self,
-        returning: str
-    ) -> str:
-        returning = returning.lower()
+        file: Optional[Union[Path, str]] = Path('vimeo_data.json'),
+        format: Optional[Literal['json', 'pickle']] = None,
+        refresh: bool = False
+    ) -> None:
+        if isinstance(file, str):
+            file = Path(file)
+        
+        if not format:
+            format = file.suffix[1:]  # type: ignore
 
-        try:
-            return RETURNING_MAP[returning]
-        except KeyError:
-            raise ValueError(f'Unknown value for returning: {returning}')
+        data_to_save = {
+            'account': self._get_account_data(
+                returning='dict',
+                refresh=refresh
+            ),
+            'videos': self._get_items(
+                what='videos',
+                returning='dict',
+                refresh=refresh
+            ),
+            'albums': self._get_items(
+                what='albums',
+                returning='dict',
+                refresh=refresh
+            ),
+            'projects': self.get_folders(
+                returning='dict',
+                refresh=refresh
+            )
+        }
+
+        print(f'Saving data to {file}...')
+        
+        if format == 'json':
+            with open(file, 'w') as f:
+                json.dump(data_to_save, f, indent=4)
+        elif format == 'pickle':
+            with open(file, 'wb') as f:
+                pickle.dump(data_to_save, f)
+        else:
+            raise ValueError(f'Unknown format: {format}')
 
     def show_account(
         self,
         mode: str = 'default',
         ignore_keys: List[str] = [],
         show_keys: List[str] = [],
         indent: int = 0,
@@ -1057,7 +1141,31 @@
             mode=mode,
             ignore_keys=ignore_keys,
             show_keys=show_keys,
             indent=indent,
             refresh=refresh,
             returning=returning
         )
+
+    def update_data(
+        self,
+        what: Literal['account', 'videos', 'albums', 'projects'],
+        data: Union[Dict[str, Any], List[Dict[str, Any]]]
+    ) -> None:
+        """
+        Update data in the VimeoData object
+        """
+        map_what = {
+            'account': self._account_data,
+            'videos': self._videos_data,
+            'albums': self._albums_data,
+            'projects': self._folders_data
+        }
+
+        if isinstance(data, list):
+            """
+            find the item(s) in the list by uri or code and update them
+            or append them if they don't exist
+            """
+            pass
+        elif isinstance(data, dict):
+            map_what[what] = data
```

### Comparing `vimeotools-0.0.1/src/vimeotools/vimeo_folder.py` & `vimeotools-0.0.2/src/vimeotools/vimeo_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,78 +3,91 @@
 =========================
 Vimeo Tools Folder Module
 =========================
 
 This module contains the class VimeoFolder, which represents a Vimeo folder
 (projects).
 """
-from typing import List, Dict, Optional, Any, Union, Literal
-import vimeo
-import json
+from typing import TYPE_CHECKING, List, Dict, Optional, Any, Union, Literal
 from vimeo_connection import VimeoConnection
 from vimeo_base import VimeoChild, VimeoItem, get_lines
 from vimeo_video import VimeoVideo
 from vimeo_constants import (
-    GETTER_STR,
     PROPERTIES_BASE,
     PROPERTIES_FOLDER
 )
 
+if TYPE_CHECKING:
+    from vimeo_data import VimeoData
+
 class VimeoFolder(VimeoItem, VimeoChild):
 
     BASE_URI = '/me/projects'
     allowed_keys_to_set = ['name']
 
     def __init__(
         self,
         connection: VimeoConnection,
         code_or_uri: Optional[str] = None,
         name: Optional[str] = None,
         description: Optional[str] = None,
+        data: Optional[Dict[str, Any]] = None,
+        data_object: Optional['VimeoData'] = None,
         privacy: Literal['anybody', 'nobody', 'password', 'users'] = 'nobody',
         users: List[str] = [],
         parent_folder: Optional[Union[str, 'VimeoFolder']] = None,
         password: Optional[str] = None,
         sort: Literal['arrange', 'date', 'manual', 'name', 'plays', 'likes', 'comments', 'duration'] = 'date',
         layout: Literal['grid', 'player'] = 'grid',
         theme: Literal['dark', 'standard'] = 'standard'
     ):
         self.connection = connection
         self.client = connection.client
 
+        self._data = None  # type: Optional[Dict[str, Any]]
+        self._parent  = None  # type: Optional[VimeoFolder]
+        self._videos = None  # type: Optional[List[VimeoVideo]]
+        self._videos_data = None  # type: Optional[List[Dict[str, Any]]]
+
+        
         if name and code_or_uri:
             raise ValueError(
                 'Parameters: Either code_or_uri or name must be provided.'
             )
-        elif name:
+
+        if not name and data:
+            name = data.get('name')
+
+        if name:
             self._code = self._create(
                 name=name,
                 description=description,
                 privacy=privacy,
                 users=users,
                 parent_folder=parent_folder,
                 password=password,
                 sort=sort,
                 layout=layout,
                 theme=theme
             )
+        else:
+            raise ValueError(
+                'Parameters: Either code_or_uri or name must be provided.'
+            )
 
         # init the parent class
         super(VimeoItem, self).__init__(
             code_or_uri=code_or_uri or self._code,
-            connection=connection
+            connection=connection,
+            data=data,
+            data_object=data_object
         )
 
         super(VimeoChild, self).__init__() # type: ignore
 
-        self._data = None  # type: Optional[Dict[str, Any]]
-        self._parent  = None  # type: Optional[VimeoFolder]
-        self._videos = None  # type: Optional[List[VimeoVideo]]
-        self._videos_data = None  # type: Optional[List[Dict[str, Any]]]
-
     def __str__(self) -> str:
         ignore_keys = ['user', 'metadata', 'pictures']
         
         lines = [
             f'Object: {VimeoFolder.__repr__(self)}',
         ] + get_lines(key='code', value=self.code, bullet='-', indent=2)
```

### Comparing `vimeotools-0.0.1/src/vimeotools/vimeo_showcase.py` & `vimeotools-0.0.2/src/vimeotools/vimeo_showcase.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,37 +6,43 @@
 
 This module contains the class VimeoShowcase.
 """
 from __future__ import annotations
 from typing import TYPE_CHECKING, Dict, Optional, List, Union, Any, Literal
 import vimeo
 import json
-from vimeo_base import VimeoItem, get_lines
+from vimeo_base import (
+    VimeoItem,
+    get_lines,
+    transform_returning
+)
 from vimeo_constants import (
     GETTER_STR,
     SETTER_STR,
     PROPERTIES_BASE,
     PROPERTIES_SHOWCASE,
     SHOWCASE_ALLOWED_KEYS_TO_SET
 )
 from vimeo_video import VimeoVideo as VimeoVideo_
 
 if TYPE_CHECKING:
     from vimeo_connection import VimeoConnection
+    from vimeo_data import VimeoData
 """
 if TYPE_CHECKING:
     from vimeo_video import VimeoVideo
 """
 
 class VimeoShowcase(VimeoItem):
     """
     A class to represent a Vimeo showcase.
     """
     BASE_URI = '/albums'
     API_URI = '/me/albums'
+    USER_URI = '/users/{user_id}/albums'
     allowed_keys_to_set = SHOWCASE_ALLOWED_KEYS_TO_SET
 
     for key, val in PROPERTIES_SHOWCASE.items():
         exec(GETTER_STR.format(prop=key))
         if val['type'] == 'str' and val.get('setable'):
             set_key = val.get('set_key')
             if set_key is None:
@@ -45,48 +51,62 @@
             exec(SETTER_STR.format(prop=set_key))
 
     def __init__(
         self,
         connection: VimeoConnection,
         code_or_uri: Optional[str] = None,
         name: Optional[str] = None,
+        data: Optional[Dict[str, Any]] = None,
+        data_object: Optional[VimeoData] = None,
+        videos: List[VimeoVideo_] = [],
         creation_data: Optional[Dict[str, Any]] = {},  # for creation, must at least contain 'name'
     ):
         """
         Initialize a Vimeo showcase.
         :param client: Union[vimeo.VimeoClient, Dict[str, str]]
         :param code_or_uri: Optional[str]
         :param creation_data: Optional[Dict[str, Any]]
         """
 
         # init the parent class
         super().__init__(
             code_or_uri=code_or_uri,
-            connection=connection
+            connection=connection,
+            data=data,
+            data_object=data_object
         )
-        self._videos = None
+        self._videos = videos
+
+        if data:  # data provided, no request needed
+            self._data = data
+            return
 
         if name:
             creation_data['name'] = name  # type: ignore
         
         if not code_or_uri and not creation_data:
             raise ValueError('Either code_or_uri or data must be provided.')
         elif code_or_uri and creation_data:
             raise ValueError('Only one of code_or_uri or data must be provided.')
         elif creation_data:
             # create a new showcase
             response = self.client.post(self.API_URI, data=creation_data)
             if response.status_code == 201:  # success in creating a new showcase
                 self._data = response.json()
+                self._uri = self._data['uri']
+                self._code = self._data['uri'].split('/')[-1]
             elif response.status_code == 400:
                 raise ValueError('Invalid data.')
             elif response.status_code == 403:
                 raise PermissionError('You do not have permission to create a showcase.')
             else:
                 raise ValueError(f'Status code {response.status_code}. Unknown error.')
+        
+        for video in videos:
+            self.add_video(video)
     
     def __str__(self) -> str:
         ignore_keys = ['user', 'metadata', 'pictures']
         
         lines = [f'Object: {VimeoShowcase.__repr__(self)}']
         
         for prop, meta in {**PROPERTIES_BASE, **PROPERTIES_SHOWCASE}.items():
@@ -98,17 +118,15 @@
             lines += get_lines(
                 key=prop,
                 value=value,
                 bullet='-',
                 indent=2
             )
         
-        
-
-        videos = self.videos
+        videos = self.videos or []
         lines.append(f'  - {len(videos)} Videos')
         if videos:
             for video in videos:
                 lines.append(f'    - {video.name} ({video.code})') # type: ignore
 
         lines.append(f'  - more keys: ' + ', '.join(ignore_keys))
         return '\n'.join(lines)
@@ -127,27 +145,36 @@
         picture: str
     ):
         """
         Add a thumbnail to the showcase.
         """
         raise NotImplementedError
     
+    @property
+    def videos(
+        self
+    ) -> List[VimeoVideo_]:
+        """
+        Get the videos of the showcase.
+        """
+        return self.get_videos()
+
     def add_video(
         self,
         video: Union[str, VimeoVideo_]  # code or object
     ):
         """
         Add a video to the showcase.
         """
-        try:
-            video = video.get_code() # type: ignore
-        except AttributeError:
-            pass
-            
-        uri = f'{self.API_URI}/{self.code}/videos/{video}'
+        if isinstance(video, VimeoVideo_):
+            video = video.code # type: ignore
+
+        # uri_base = self.USER_URI.format(user_id=self.user_id) 
+        uri = f'{self.BASE_URI}/{self.code}/videos/{video}'
+        print('uri', uri)
         
         response = self.client.put(uri)
         if response.status_code == 204:
             pass
         elif response.status_code == 403:
             raise PermissionError('You do not have permission to add a video to this showcase.')
         elif response.status_code == 404:
@@ -197,33 +224,37 @@
         """
         raise NotImplementedError
     
     def get_videos(
         self,
         refresh: bool = False,
         returning: Literal[
+            'code',
             'codes',
+            'uri',
             'uris',
+            'name',
             'names',
             'dict',
             'list',
+            'object',
             'objects',
             'json'
-        ] = 'objects'
+        ] = 'object'
     ) -> Union[
             Dict[str, Any],
             List[Dict[str, Any]],
             List[VimeoVideo_],
             List[str],
             str
         ]:
         """
         Get the videos of the showcase.
         """
-        print('get_videos')
+        returning = transform_returning(returning)
         
         if not refresh and self._videos:
             return self._videos
         
         uri = f'{self.API_URI}/{self.code}/videos'
         response = self.client.get(uri)
 
@@ -242,26 +273,26 @@
             
             self._videos = videos
 
             if returning == 'dict':
                 return videos
             elif returning == 'list':
                 return videos['data'] # type: ignore
-            elif returning == 'objects':
+            elif returning == 'object':
                 return [
                     VimeoVideo_(
                         connection=self.connection,
                         code_or_uri=video['uri']
                     ) for video in videos
                 ]
             elif returning == 'json':
                 return json.dumps(videos)
-            elif returning == 'codes':
+            elif returning == 'code':
                 return [video['uri'].split('/')[-1] for video in videos]
-            elif returning in ('uris', 'names'):
+            elif returning in ('uri', 'name'):
                 return [video[returning[:-1]] for video in videos]
             else:
                 raise ValueError(f'Invalid value {returning} for returning.')
             
         elif response.status_code == 404:
             raise ValueError('The showcase does not exist.')  # should not happen
```

### Comparing `vimeotools-0.0.1/src/vimeotools.egg-info/PKG-INFO` & `vimeotools-0.0.2/src/vimeotools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vimeotools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tools for Vimeo
 Home-page: https://github.com/georgpfolz/vimeotools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/georgpfolz/vimeotools/issues
 Project-URL: Documentation, https://georgpfolz.github.io/vimeotools
@@ -40,13 +40,22 @@
 
 You can also opt to create or set an object in live mode, so everytime a property is queried, the appropriate request is made on Vimeo first.
 
 ## documentation
 The (Sphinx) documentation is very crude (created with autodoc) currently and will be improved in subsequent versions.
 
 # History
+## 0.0.2 (2023-07-12)
+- VimeoData gets the methods **save** and **load**, to save or load data as json or pickle. 
+- the **__init__** of VimeoVideo, VimeoShowcase, VimeoFolder gets a parameter **data**, where the data can be passed when the object is created, so no request is needed.
+- Objects have a new attribute **temp_data** (dictionary) where you can store data relevant to your runing program directly on the object.
+- The **VimeoData** object can be added to **VimeoVideo**, **VimeoShowcase** and **VimeoFolder** instances. So the data object can be updated if there is a change in one of those insetances.
+- using **pathlib** (instead of os.path): all filepath parameters accept Path objects.
+
+Still no unit tests, this is still very much in beta!
+
 ## 0.0.1 (2023-07-07)
 This is the first version. It provides the **VimeoConnection**, **VimeoData**, **Video** and **VimeoShowcase** and **VimeoFolder** classes.
 
 The package is still very much in beta, as many of the possible methods of this classes are not implemented yet and other classes (e.g. for Groups or Portfolios) shall be implemented later. It is also not well tested at the moment. Use it at your own risk!
```

