# Comparing `tmp/vimeotools-0.0.2.tar.gz` & `tmp/vimeotools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vimeotools-0.0.2.tar", last modified: Thu Jul 13 14:07:37 2023, max compression
+gzip compressed data, was "dist/vimeotools-0.0.3.tar", last modified: Thu Jul 13 18:40:32 2023, max compression
```

## Comparing `vimeotools-0.0.2.tar` & `vimeotools-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 14:07:37.437346 vimeotools-0.0.2/
--rw-r--r--   0 georg      (502) staff       (20)     3050 2023-07-13 14:07:37.437548 vimeotools-0.0.2/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)     1229 2023-07-08 16:58:08.000000 vimeotools-0.0.2/README.md
--rw-r--r--   0 georg      (502) staff       (20)      806 2023-07-13 14:07:37.438348 vimeotools-0.0.2/setup.cfg
--rw-r--r--   0 georg      (502) staff       (20)       69 2023-07-07 15:14:58.000000 vimeotools-0.0.2/setup.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 14:07:37.426527 vimeotools-0.0.2/src/
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 14:07:37.434193 vimeotools-0.0.2/src/vimeotools/
--rw-r--r--   0 georg      (502) staff       (20)      335 2023-07-07 15:14:58.000000 vimeotools-0.0.2/src/vimeotools/__init__.py
--rw-r--r--   0 georg      (502) staff       (20)    14614 2023-07-13 10:51:12.000000 vimeotools-0.0.2/src/vimeotools/vimeo_base.py
--rw-r--r--   0 georg      (502) staff       (20)     1597 2023-07-13 04:27:52.000000 vimeotools-0.0.2/src/vimeotools/vimeo_connection.py
--rw-r--r--   0 georg      (502) staff       (20)    19344 2023-07-13 09:54:51.000000 vimeotools-0.0.2/src/vimeotools/vimeo_constants.py
--rw-r--r--   0 georg      (502) staff       (20)    34427 2023-07-13 13:25:48.000000 vimeotools-0.0.2/src/vimeotools/vimeo_data.py
--rw-r--r--   0 georg      (502) staff       (20)     8799 2023-07-13 04:42:19.000000 vimeotools-0.0.2/src/vimeotools/vimeo_folder.py
--rw-r--r--   0 georg      (502) staff       (20)    11723 2023-07-13 10:56:05.000000 vimeotools-0.0.2/src/vimeotools/vimeo_showcase.py
--rw-r--r--   0 georg      (502) staff       (20)    12553 2023-07-13 05:54:15.000000 vimeotools-0.0.2/src/vimeotools/vimeo_video.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 14:07:37.436973 vimeotools-0.0.2/src/vimeotools.egg-info/
--rw-r--r--   0 georg      (502) staff       (20)     3050 2023-07-13 14:07:36.000000 vimeotools-0.0.2/src/vimeotools.egg-info/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)      465 2023-07-13 14:07:37.000000 vimeotools-0.0.2/src/vimeotools.egg-info/SOURCES.txt
--rw-r--r--   0 georg      (502) staff       (20)        1 2023-07-13 14:07:36.000000 vimeotools-0.0.2/src/vimeotools.egg-info/dependency_links.txt
--rw-r--r--   0 georg      (502) staff       (20)        8 2023-07-13 14:07:37.000000 vimeotools-0.0.2/src/vimeotools.egg-info/requires.txt
--rw-r--r--   0 georg      (502) staff       (20)       11 2023-07-13 14:07:37.000000 vimeotools-0.0.2/src/vimeotools.egg-info/top_level.txt
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 18:40:32.549229 vimeotools-0.0.3/
+-rw-r--r--   0 georg      (502) staff       (20)     3268 2023-07-13 18:40:32.549522 vimeotools-0.0.3/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)     1229 2023-07-08 16:58:08.000000 vimeotools-0.0.3/README.md
+-rw-r--r--   0 georg      (502) staff       (20)      806 2023-07-13 18:40:32.550680 vimeotools-0.0.3/setup.cfg
+-rw-r--r--   0 georg      (502) staff       (20)       69 2023-07-07 15:14:58.000000 vimeotools-0.0.3/setup.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 18:40:32.536781 vimeotools-0.0.3/src/
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 18:40:32.544996 vimeotools-0.0.3/src/vimeotools/
+-rw-r--r--   0 georg      (502) staff       (20)      335 2023-07-07 15:14:58.000000 vimeotools-0.0.3/src/vimeotools/__init__.py
+-rw-r--r--   0 georg      (502) staff       (20)    14614 2023-07-13 10:51:12.000000 vimeotools-0.0.3/src/vimeotools/vimeo_base.py
+-rw-r--r--   0 georg      (502) staff       (20)     1597 2023-07-13 04:27:52.000000 vimeotools-0.0.3/src/vimeotools/vimeo_connection.py
+-rw-r--r--   0 georg      (502) staff       (20)    19344 2023-07-13 09:54:51.000000 vimeotools-0.0.3/src/vimeotools/vimeo_constants.py
+-rw-r--r--   0 georg      (502) staff       (20)    34543 2023-07-13 18:33:41.000000 vimeotools-0.0.3/src/vimeotools/vimeo_data.py
+-rw-r--r--   0 georg      (502) staff       (20)     9041 2023-07-13 18:15:06.000000 vimeotools-0.0.3/src/vimeotools/vimeo_folder.py
+-rw-r--r--   0 georg      (502) staff       (20)    11963 2023-07-13 18:25:06.000000 vimeotools-0.0.3/src/vimeotools/vimeo_showcase.py
+-rw-r--r--   0 georg      (502) staff       (20)    12553 2023-07-13 05:54:15.000000 vimeotools-0.0.3/src/vimeotools/vimeo_video.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 18:40:32.548613 vimeotools-0.0.3/src/vimeotools.egg-info/
+-rw-r--r--   0 georg      (502) staff       (20)     3268 2023-07-13 18:40:31.000000 vimeotools-0.0.3/src/vimeotools.egg-info/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)      465 2023-07-13 18:40:32.000000 vimeotools-0.0.3/src/vimeotools.egg-info/SOURCES.txt
+-rw-r--r--   0 georg      (502) staff       (20)        1 2023-07-13 18:40:31.000000 vimeotools-0.0.3/src/vimeotools.egg-info/dependency_links.txt
+-rw-r--r--   0 georg      (502) staff       (20)        8 2023-07-13 18:40:32.000000 vimeotools-0.0.3/src/vimeotools.egg-info/requires.txt
+-rw-r--r--   0 georg      (502) staff       (20)       11 2023-07-13 18:40:32.000000 vimeotools-0.0.3/src/vimeotools.egg-info/top_level.txt
```

### Comparing `vimeotools-0.0.2/PKG-INFO` & `vimeotools-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vimeotools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for Vimeo
 Home-page: https://github.com/georgpfolz/vimeotools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/georgpfolz/vimeotools/issues
 Project-URL: Documentation, https://georgpfolz.github.io/vimeotools
@@ -40,19 +40,26 @@
 
 You can also opt to create or set an object in live mode, so everytime a property is queried, the appropriate request is made on Vimeo first.
 
 ## documentation
 The (Sphinx) documentation is very crude (created with autodoc) currently and will be improved in subsequent versions.
 
 # History
+## 0.0.3 (2023-07-13)
+- **VimeoShocase** und **VimeoFolder**: property **nb_videos**
+- **VimeoData** changed property names
+	- video_count -> nb_videos
+	- showcases_count -> nb_showcases
+	- folders_count -> nb_folders
+
 ## 0.0.2 (2023-07-12)
 - VimeoData gets the methods **save** and **load**, to save or load data as json or pickle. 
 - the **__init__** of VimeoVideo, VimeoShowcase, VimeoFolder gets a parameter **data**, where the data can be passed when the object is created, so no request is needed.
 - Objects have a new attribute **temp_data** (dictionary) where you can store data relevant to your runing program directly on the object.
-- The **VimeoData** object can be added to **VimeoVideo**, **VimeoShowcase** and **VimeoFolder** instances. So the data object can be updated if there is a change in one of those insetances.
+- The **VimeoData** object can be added to **VimeoVideo**, **VimeoShowcase** and **VimeoFolder** instances. So the data object can be updated if there is a change in one of those instances.
 - using **pathlib** (instead of os.path): all filepath parameters accept Path objects.
 
 Still no unit tests, this is still very much in beta!
 
 ## 0.0.1 (2023-07-07)
 This is the first version. It provides the **VimeoConnection**, **VimeoData**, **Video** and **VimeoShowcase** and **VimeoFolder** classes.
```

### Comparing `vimeotools-0.0.2/README.md` & `vimeotools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.2/setup.cfg` & `vimeotools-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vimeotools
-version = 0.0.2
+version = 0.0.3
 author = Georg Pfolz
 author_email = georg.pfolz@invesy.at
 description = Tools for Vimeo
 long_description = file: README.md,HISTORY.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE.txt
```

### Comparing `vimeotools-0.0.2/src/vimeotools/vimeo_base.py` & `vimeotools-0.0.3/src/vimeotools/vimeo_base.py`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.2/src/vimeotools/vimeo_connection.py` & `vimeotools-0.0.3/src/vimeotools/vimeo_connection.py`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.2/src/vimeotools/vimeo_constants.py` & `vimeotools-0.0.3/src/vimeotools/vimeo_constants.py`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.2/src/vimeotools/vimeo_data.py` & `vimeotools-0.0.3/src/vimeotools/vimeo_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,57 +53,14 @@
             self._videos_data = None
             self._folders_data = None
             self._albums_data = None
         
         self._videos = None
         self._folders = None
         self._albums = None
-
-    def info(
-        self
-    ) -> str:
-        """
-        Return a string with information about the account and
-        informations about the videos, folders and albums.
-
-        Be warned that this method will make a lot of requests to the
-        Vimeo API, so it may take a while to complete.
-
-        :return: str
-        """
-        lines = [
-            f'Object: {VimeoConnection.__repr__(self)}',
-            f'  - Account:'
-        ]
-        lines += self.show_account(
-            mode='minimal',
-            indent=4,
-            returning='lines'
-        )
-        lines += self.show_videos(
-            mode='minimal',
-            indent=4,
-            returning='lines'
-        )
-        lines += self.show_folders(
-            mode='minimal',
-            indent=4,
-            returning='lines'
-        )
-        lines += self.show_showcases(
-            mode='minimal',
-            indent=4,
-            returning='lines'
-        )
-
-        lines.append(f'  - {self.get_count(what="videos")} Videos')
-        lines.append(f'  - {self.get_count(what="projects")} Folders')
-        lines.append(f'  - {self.get_count(what="albums")} Showcases')
-
-        return '\n'.join(lines)
     
     def _print(
             self,
             data: Dict[str, Any],
             ignore_keys: List[str] = [],
             indent: int = 0,
             returning: Literal['str', 'lines'] = 'str'
@@ -134,15 +91,47 @@
     ) -> Optional[Dict[str, Any]]:
         if what == 'videos' and self._videos_data:
             return self._videos_data
         elif what == 'albums' and self._albums_data:
             return self._albums_data
         elif what == 'projects' and self._folders_data:
             return self._folders_data
-    
+
+    def _get_account_data(
+        self,
+        returning: Literal['dict', 'json'] = 'dict',
+        keys: Optional[List[str]] = None,
+        refresh: bool = False
+    ) -> Union[dict, str]:
+        """
+        Get account infos.
+        :return: dict
+        """
+        if not refresh and self._account_data:
+            data = self._account_data
+        else:
+            uri = self.uri
+            response = self.client.get(uri)
+            assert response.status_code == 200, f'Error: {response.status_code}'
+            data = response.json()
+            data['code'] = data.get('uri').split('/')[-1]  # add vimeo code to data
+            self._account_data = data
+
+        if returning == 'json':
+            return json.dumps(data, indent=4)
+        else:  # returning == 'dict'
+            if keys:
+                return {
+                    key: data[key]
+                    for key
+                    in keys
+                }
+            else:
+                return data      
+
     def _items_stored(
         self,
         what: Literal['videos', 'albums', 'projects']
     ) -> Optional[
             Union[
                 List[VimeoVideo],
                 List[VimeoShowcase],
@@ -296,44 +285,82 @@
         elif returning == 'list':
             return data['data']
         elif returning == 'json':
             return json.dumps(data, indent=4)
         else:
             # will never happen, we keep it for the return type check
             raise ValueError(f'Unknown returning value: {returning}')
-    
-    def get_count(
-        self,
-        what: Literal['videos', 'albums', 'projects'],
-        refresh: bool = False
-    ) -> int:
-        """
-        Get the number of items (videos or albums).
-        :param what: What to fetch. Either 'videos' or 'albums' (=='showcases').
-        """
-        if not refresh:
-            if what == 'videos' and self._videos_data:
-                return self._videos_data['total']
-            elif what == 'albums' and self._albums_data:
-                return self._albums_data['total']
-            elif what == 'projects' and self._folders_data:
-                return self._folders_data['total']
 
-        response = self.client.get(
-            f'/me/{what}',
-            params={
-                'page': 1,
-                'per_page': 1
-            }
-        )
-        if response.status_code != 200:
-            raise Exception(f'Error getting {what}: {response.text}')
+    def _show_data(
+        self,
+        what: Literal[
+            'videos',
+            'video',
+            'album',
+            'albums',
+            'showcase',
+            'showcases',
+            'folder',
+            'folders',
+            'project',
+            'projects',
+            'account'
+        ],
+        mode: str = 'default',
+        ignore_keys: List[str] = [],
+        show_keys: List[str] = [],
+        indent: int = 0,
+        refresh: bool = False,
+        returning: Literal['str', 'lines'] = 'str'
+    ) -> Union[str, List[str]]:
+        what = transform_what(what) # type: ignore
 
-        return response.json()['total']
+        data = {}
 
+        if what == 'account':
+            data = self._get_account_data(
+                returning='dict',
+                refresh=refresh
+            )
+        elif what in ('videos', 'albums'):
+            data = self._get_items(
+                what=what,  # type: ignore (-> transform_what)
+                returning='dict',
+                refresh=refresh
+            )
+        elif what == 'projects':
+            data = self.get_folders(
+                returning='dict',
+                refresh=refresh
+            )
+        else:
+            raise ValueError(f'Unknown value for what: {what}')
+        
+        if show_keys:
+            ignore_keys = [
+                key
+                for key
+                in data.keys() # type: ignore (impossible that it's not a dict)
+                if key not in show_keys
+            ]
+        elif not ignore_keys:  # use mode only if no ignore_keys and no show_keys
+            if mode == 'default':
+                ignore_keys = ['pictures', 'metadata']
+            elif mode == 'minimal':
+                ignore_keys += MIN_KEYS[what]
+            elif mode == 'max':
+                ignore_keys = []
+        
+        return self._print(
+            data=data, # type: ignore (impossible that it's not a dict)
+            ignore_keys=ignore_keys,
+            indent=indent,
+            returning=returning
+        )
+    
     @property
     def account(
         self
     ) -> dict:
         """
         Get account infos.
         :return: dict
@@ -360,56 +387,42 @@
         Get account infos.
         :return: str (json)
         """
         return self._get_account_data(
             returning='json'
         ) # type: ignore
 
-    def _get_account_data(
+    def get_count(
         self,
-        returning: Literal['dict', 'json'] = 'dict',
-        keys: Optional[List[str]] = None,
+        what: Literal['videos', 'albums', 'projects'],
         refresh: bool = False
-    ) -> Union[dict, str]:
-        """
-        Get account infos.
-        :return: dict
-        """
-        if not refresh and self._account_data:
-            data = self._account_data
-        else:
-            uri = self.uri
-            response = self.client.get(uri)
-            assert response.status_code == 200, f'Error: {response.status_code}'
-            data = response.json()
-            data['code'] = data.get('uri').split('/')[-1]  # add vimeo code to data
-            self._account_data = data
-
-        if returning == 'json':
-            return json.dumps(data, indent=4)
-        else:  # returning == 'dict'
-            if keys:
-                return {
-                    key: data[key]
-                    for key
-                    in keys
-                }
-            else:
-                return data        
-    
-    @property
-    def folder_count(
-        self
     ) -> int:
         """
-        Get the number of folders.
+        Get the number of items (videos or albums).
+        :param what: What to fetch. Either 'videos' or 'albums' (=='showcases').
         """
-        return self.get_count(
-            what = 'projects'
-        ) # type: ignore
+        if not refresh:
+            if what == 'videos' and self._videos_data:
+                return self._videos_data['total']  # why is that an error? It should be a dict.
+            elif what == 'albums' and self._albums_data:
+                return self._albums_data['total']
+            elif what == 'projects' and self._folders_data:
+                return self._folders_data['total']
+
+        response = self.client.get(
+            f'/me/{what}',
+            params={
+                'page': 1,
+                'per_page': 1
+            }
+        )
+        if response.status_code != 200:
+            raise Exception(f'Error getting {what}: {response.text}')
+
+        return response.json()['total']
 
     def get_folders(
         self,
         returning: Literal[
             'objects',  # alias for 'object'
             'object',
             'folder',  # alias for 'object'
@@ -435,102 +448,15 @@
         returning = transform_returning(returning) # type: ignore
 
         return self._get_items(
             what='projects',
             returning=returning, # type: ignore
             refresh=refresh
         ) # type: ignore
-
-    def items_property(
-        self,
-        property: str,
-        what: Literal['videos', 'albums', 'projects'] = 'videos',
-        refresh: bool = False
-    ) -> List[str]:
-        """
-        Fetch the property of the items specified in 'what'.
-
-        :param property: This parameter supports the same dot notation as the Vimeo API.
-        :param refresh: bool
-        :return: list of str
-        """
-        stored_data = self._data_stored(what=what)
-        stored_items = self._items_stored(what=what)
-
-        if not refresh and stored_data is not None:
-            data_base = stored_data['data']
-            
-            if '.' in property:
-                for key in property.split('.'):
-                    data_base = data_base[key]
-
-            return [
-                item[property]
-                for item
-                in data_base
-            ]
-        elif not refresh and stored_items is not None:
-            return [
-                item.items_property(property)  # refresh implicitely False
-                for item
-                in stored_items
-            ]
-        else:
-            original_property = property
-            if property == 'code':
-                property = 'uri'
-                original_property = 'code'
-            
-            uri = f'{self.uri}/{what}?fields={property}'  # dot notation allowed!
-            property_list = []
-            page = 1
-            while True:
-                response = self.client.get(
-                    uri,
-                    params={
-                        'page': page,
-                        'per_page': 100
-                    }
-                )
-                if response.status_code != 200:
-                    raise Exception(f'Error getting {what}: {response.text}')      
-                
-                data = response.json()
-                
-                property_list.extend([
-                    nested_value(data=item, path=property) for item in data['data']
-                ])
-
-                if data['paging']['next'] is None:
-                    break
-                
-                page += 1
-
-            if original_property:
-                property_list = [
-                    item.split('/')[-1]
-                    for item
-                    in property_list
-                ]
-            return property_list
-
-    @property
-    def showcases(
-        self
-    ) -> List[VimeoShowcase]:
-        """
-        Get all showcases.
-        :return: list of VimeoShowcase objects
-
-        This property is always refreshed.
-        """
-        return self.get_showcases(
-            returning='objects'
-        ) # type: ignore
-    
+        
     def get_showcases(
         self,
         returning: Literal[
             'objects',
             'object',
             'showcase',  # alias for 'object'
             'showcases',  # alias for 'objects'
@@ -561,186 +487,14 @@
         returning = transform_returning(returning) # type: ignore
 
         return self._get_items(
             what='albums',
             returning=returning,  # type: ignore
             refresh=refresh
         ) # type: ignore
-    
-    def refresh(
-        self,
-        what: Literal[
-            'videos',
-            'albums',
-            'showcases',
-            'account',
-            'all'
-        ] = 'all'
-    ) -> None:
-        """
-        Refresh data.
-        """
-        what = transform_what(what) # type: ignore
-
-        if what in ('account', 'all'):
-            self._get_account_data(
-                refresh=True
-            )
-        if what in ('albums', 'all'):
-            self._get_items(
-                what='albums',
-                refresh=True
-            )
-        if what in ('videos', 'all'):
-            self._get_items(
-                what='videos',
-                refresh=True
-            )
-
-    @property
-    def showcase_codes(
-        self,
-        refresh: bool = False
-    ) -> List[str]:
-        """
-        Fetch the codes of all videos.
-        :param refresh: bool
-        :return: list of str
-        """
-        if not refresh and self._albums_data is not None:  # fastest way
-            return [
-                album['code']
-                for album
-                in self._albums_data['data']
-            ]
-        elif not refresh and self._albums is not None:
-            return [
-                album.get_code()  # refresh implicitely False
-                for album
-                in self._albums
-            ]
-        else:
-            return [
-                uri.split('/')[-1]
-                for uri
-                in self.showcase_uris
-            ]
-
-    @property
-    def showcase_count(
-        self
-    ) -> int:
-        """
-        Get the number of showcases.
-        :return: int
-        """
-        return self.get_count(
-            what='albums'
-        )
-
-    @property
-    def showcase_uris(
-        self,
-        refresh: bool = False
-    ) -> List[str]:
-        """
-        Fetch the uris of all videos.
-        :param refresh: bool
-        :return: list of str
-        """
-        if not refresh and self._albums_data is not None:
-            return [
-                album['uri']
-                for album
-                in self._albums_data['data']
-            ]
-        elif not refresh and self._albums is not None:
-            return [
-                album.get_uri()  # refresh implicitely False
-                for album
-                in self._albums
-            ]
-        else:
-            return self.items_property(
-                property='uri',
-                what='albums',
-                refresh=refresh
-            )
-
-    @property
-    def video_codes(
-        self,
-        refresh: bool = False
-    ) -> List[str]:
-        """
-        Fetch the codes of all videos.
-        :param refresh: bool
-        :return: list of str
-        """
-        if not refresh and self._videos_data is not None:  # fastest way
-            return [
-                video['code']
-                for video
-                in self._videos_data['data']
-            ]
-        elif not refresh and self._videos is not None:
-            return [
-                video.get_code()  # refresh implicitely False
-                for video
-                in self._videos
-            ]
-        else:
-            return [
-                uri.split('/')[-1]
-                for uri
-                in self.video_uris
-            ]
-    
-    @property
-    def video_uris(
-        self,
-        refresh: bool = False
-    ) -> List[str]:
-        """
-        Fetch the uris of all videos.
-        :param refresh: bool
-        :return: list of str
-        """
-        if not refresh and self._videos_data is not None:
-            return [
-                video['uri']
-                for video
-                in self._videos_data['data']
-            ]
-        elif not refresh and self._videos is not None:
-            return [
-                video.get_uri()  # refresh implicitely False
-                for video
-                in self._videos
-            ]
-        else:
-            return self.items_property(
-                property='uri',
-                what='videos',
-                refresh=refresh
-            )
-        
-    @property
-    def videos(
-        self
-    ) -> List[VimeoVideo]:
-        """
-        Get all videos.
-        :return: list of VimeoVideo objects
-
-        Refresh is implicitely False.
-        """
-        return self.get_videos(
-            returning='objects'
-        ) # type: ignore
 
     def get_videos(
         self,
         returning: Literal[
             'object',
             'objects',
             'video',
@@ -771,27 +525,14 @@
 
         return self._get_items(
             what='videos',
             returning=returning,  # type: ignore
             refresh=refresh
         ) # type: ignore
 
-    @property
-    def video_count(
-        self
-    ) -> int:
-        """
-        Get the number of videos.
-        :param refresh: bool
-        :return: int
-        """
-        return self.get_count(
-            what='videos'
-        )
-
     def get_videos_from_showcase(
         self,
         showcase: Union[str, VimeoShowcase],
         returning: Literal[
             'object',
             'objects',
             'dict',
@@ -861,15 +602,15 @@
                 return album_data['data']
             elif returning == 'json':
                 return json.dumps(album_data)
             else:
                 raise ValueError(
                     f'Invalid value for returning: {returning}'
                 )
-        
+            
     def get_videos_with_tag(
         self,
         tag: str,
         returning: Literal[
             'object',
             'objects',
             'dict',
@@ -919,82 +660,131 @@
                 for video
                 in video['data']
             ]
         elif returning == 'json':
             return json.dumps(video, indent=4)
         else:
             raise ValueError(f'Unknown returning value: {returning}')
+        
+    def info(
+        self
+    ) -> str:
+        """
+        Return a string with information about the account and
+        informations about the videos, folders and albums.
 
-    def _show_data(
+        Be warned that this method will make a lot of requests to the
+        Vimeo API, so it may take a while to complete.
+
+        :return: str
+        """
+        lines = [
+            f'Object: {VimeoConnection.__repr__(self)}',
+            f'  - Account:'
+        ]
+        lines += self.show_account(
+            mode='minimal',
+            indent=4,
+            returning='lines'
+        )
+        lines += self.show_videos(
+            mode='minimal',
+            indent=4,
+            returning='lines'
+        )
+        lines += self.show_folders(
+            mode='minimal',
+            indent=4,
+            returning='lines'
+        )
+        lines += self.show_showcases(
+            mode='minimal',
+            indent=4,
+            returning='lines'
+        )
+
+        lines.append(f'  - {self.get_count(what="videos")} Videos')
+        lines.append(f'  - {self.get_count(what="projects")} Folders')
+        lines.append(f'  - {self.get_count(what="albums")} Showcases')
+
+        return '\n'.join(lines)  
+    
+    def items_property(
         self,
-        what: Literal[
-            'videos',
-            'video',
-            'album',
-            'albums',
-            'showcase',
-            'showcases',
-            'folder',
-            'folders',
-            'project',
-            'projects',
-            'account'
-        ],
-        mode: str = 'default',
-        ignore_keys: List[str] = [],
-        show_keys: List[str] = [],
-        indent: int = 0,
-        refresh: bool = False,
-        returning: Literal['str', 'lines'] = 'str'
-    ) -> Union[str, List[str]]:
-        what = transform_what(what) # type: ignore
+        property: str,
+        what: Literal['videos', 'albums', 'projects'] = 'videos',
+        refresh: bool = False
+    ) -> List[str]:
+        """
+        Fetch the property of the items specified in 'what'.
 
-        data = {}
+        :param property: This parameter supports the same dot notation as the Vimeo API.
+        :param refresh: bool
+        :return: list of str
+        """
+        stored_data = self._data_stored(what=what)
+        stored_items = self._items_stored(what=what)
 
-        if what == 'account':
-            data = self._get_account_data(
-                returning='dict',
-                refresh=refresh
-            )
-        elif what in ('videos', 'albums'):
-            data = self._get_items(
-                what=what,
-                returning='dict',
-                refresh=refresh
-            )
-        elif what == 'projects':
-            data = self.get_folders(
-                returning='dict',
-                refresh=refresh
-            )
-        else:
-            raise ValueError(f'Unknown value for what: {what}')
-        
-        if show_keys:
-            ignore_keys = [
-                key
-                for key
-                in data.keys() # type: ignore (impossible that it's not a dict)
-                if key not in show_keys
+        if not refresh and stored_data is not None:
+            data_base = stored_data['data']
+            
+            if '.' in property:
+                for key in property.split('.'):
+                    data_base = data_base[key]
+
+            return [
+                item[property]
+                for item
+                in data_base
             ]
-        elif not ignore_keys:  # use mode only if no ignore_keys and no show_keys
-            if mode == 'default':
-                ignore_keys = ['pictures', 'metadata']
-            elif mode == 'minimal':
-                ignore_keys += MIN_KEYS[what]
-            elif mode == 'max':
-                ignore_keys = []
-        
-        return self._print(
-            data=data, # type: ignore (impossible that it's not a dict)
-            ignore_keys=ignore_keys,
-            indent=indent,
-            returning=returning
-        )
-    
+        elif not refresh and stored_items is not None:
+            return [
+                item.items_property(property)  # refresh implicitely False
+                for item
+                in stored_items
+            ]
+        else:
+            original_property = property
+            if property == 'code':
+                property = 'uri'
+                original_property = 'code'
+            
+            uri = f'{self.uri}/{what}?fields={property}'  # dot notation allowed!
+            property_list = []
+            page = 1
+            while True:
+                response = self.client.get(
+                    uri,
+                    params={
+                        'page': page,
+                        'per_page': 100
+                    }
+                )
+                if response.status_code != 200:
+                    raise Exception(f'Error getting {what}: {response.text}')      
+                
+                data = response.json()
+                
+                property_list.extend([
+                    nested_value(data=item, path=property) for item in data['data']
+                ])
+
+                if data['paging']['next'] is None:
+                    break
+                
+                page += 1
+
+            if original_property:
+                property_list = [
+                    item.split('/')[-1]
+                    for item
+                    in property_list
+                ]
+            return property_list
+
     def load(
         self,
         file: Union[Path, str] = Path('vimeo_data.json'),
         format: Optional[Literal['json', 'pickle']] = None,
         refresh: bool = False
     ) -> None:
         if isinstance(file, str):
@@ -1021,26 +811,236 @@
         self._data = data
 
         # redundant!
         self._account_data = data['account']
         self._videos_data = data['videos']
         self._folders_data = data['projects']
         self._albums_data = data['albums']
+        
+    @property
+    def nb_folders(
+        self
+    ) -> int:
+        """
+        Get the number of folders.
+        """
+        return self.get_count(
+            what = 'projects'
+        ) # type: ignore
+
+    @property
+    def nb_showcases(
+        self
+    ) -> int:
+        """
+        Get the number of showcases.
+        :return: int
+        """
+        return self.get_count(
+            what='albums'
+        )
+
+    @property
+    def nb_videos(
+        self
+    ) -> int:
+        """
+        Get the number of videos.
+        :param refresh: bool
+        :return: int
+        """
+        return self.get_count(
+            what='videos'
+        )
+    
+    def refresh(
+        self,
+        what: Literal[
+            'videos',
+            'albums',
+            'showcases',
+            'account',
+            'all'
+        ] = 'all'
+    ) -> None:
+        """
+        Refresh data.
+        """
+        what = transform_what(what) # type: ignore
+
+        if what in ('account', 'all'):
+            self._get_account_data(
+                refresh=True
+            )
+        if what in ('albums', 'all'):
+            self._get_items(
+                what='albums',
+                refresh=True
+            )
+        if what in ('videos', 'all'):
+            self._get_items(
+                what='videos',
+                refresh=True
+            )
+
+    @property
+    def showcases(
+        self
+    ) -> List[VimeoShowcase]:
+        """
+        Get all showcases.
+        :return: list of VimeoShowcase objects
+
+        This property is always refreshed.
+        """
+        return self.get_showcases(
+            returning='objects'
+        ) # type: ignore
     
+    @property
+    def showcase_codes(
+        self,
+        refresh: bool = False
+    ) -> List[str]:
+        """
+        Fetch the codes of all videos.
+        :param refresh: bool
+        :return: list of str
+        """
+        if not refresh and self._albums_data is not None:  # fastest way
+            return [
+                album['code']
+                for album
+                in self._albums_data['data']
+            ]
+        elif not refresh and self._albums is not None:
+            return [
+                album.get_code()  # refresh implicitely False
+                for album
+                in self._albums
+            ]
+        else:
+            return [
+                uri.split('/')[-1]
+                for uri
+                in self.showcase_uris
+            ]
+
+    @property
+    def showcase_uris(
+        self,
+        refresh: bool = False
+    ) -> List[str]:
+        """
+        Fetch the uris of all videos.
+        :param refresh: bool
+        :return: list of str
+        """
+        if not refresh and self._albums_data is not None:
+            return [
+                album['uri']
+                for album
+                in self._albums_data['data']
+            ]
+        elif not refresh and self._albums is not None:
+            return [
+                album.get_uri()  # refresh implicitely False
+                for album
+                in self._albums
+            ]
+        else:
+            return self.items_property(
+                property='uri',
+                what='albums',
+                refresh=refresh
+            )
+
+    @property
+    def video_codes(
+        self,
+        refresh: bool = False
+    ) -> List[str]:
+        """
+        Fetch the codes of all videos.
+        :param refresh: bool
+        :return: list of str
+        """
+        if not refresh and self._videos_data is not None:  # fastest way
+            return [
+                video['code']
+                for video
+                in self._videos_data['data']
+            ]
+        elif not refresh and self._videos is not None:
+            return [
+                video.get_code()  # refresh implicitely False
+                for video
+                in self._videos
+            ]
+        else:
+            return [
+                uri.split('/')[-1]
+                for uri
+                in self.video_uris
+            ]
+    
+    @property
+    def video_uris(
+        self,
+        refresh: bool = False
+    ) -> List[str]:
+        """
+        Fetch the uris of all videos.
+        :param refresh: bool
+        :return: list of str
+        """
+        if not refresh and self._videos_data is not None:
+            return [
+                video['uri']
+                for video
+                in self._videos_data['data']
+            ]
+        elif not refresh and self._videos is not None:
+            return [
+                video.get_uri()  # refresh implicitely False
+                for video
+                in self._videos
+            ]
+        else:
+            return self.items_property(
+                property='uri',
+                what='videos',
+                refresh=refresh
+            )
+        
+    @property
+    def videos(
+        self
+    ) -> List[VimeoVideo]:
+        """
+        Get all videos.
+        :return: list of VimeoVideo objects
+
+        Refresh is implicitely False.
+        """
+        return self.get_videos(
+            returning='objects'
+        ) # type: ignore
+
     def save(
         self,
-        file: Optional[Union[Path, str]] = Path('vimeo_data.json'),
+        file: Union[Path, str] = Path('vimeo_data.json'),
         format: Optional[Literal['json', 'pickle']] = None,
         refresh: bool = False
     ) -> None:
         if isinstance(file, str):
             file = Path(file)
         
         if not format:
-            format = file.suffix[1:]  # type: ignore
+            format = file.suffix[1:]  # type: ignore (impossible that it's not a Path)
 
         data_to_save = {
             'account': self._get_account_data(
                 returning='dict',
                 refresh=refresh
             ),
             'videos': self._get_items(
```

### Comparing `vimeotools-0.0.2/src/vimeotools/vimeo_folder.py` & `vimeotools-0.0.3/src/vimeotools/vimeo_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,24 @@
         Get the items in the folder.
         :return: List[Union[VimeoVideo, VimeoFolder]]
         """
         videos = self.get_videos(refresh=refresh)
         folders = self.get_folders(refresh=refresh)
         return videos + folders
     
+    @property
+    def nb_videos(
+        self
+    ) -> int:
+        """
+        Get the number of videos in the folder.
+        :return: int
+        """
+        return self._data['metadata']['connections']['videos']['total']  # type: ignore
+
     def remove_video(
         self,
         video: Union[str, 'VimeoVideo']
     ):
         """
         Remove a video from the folder.
         :param video: Union[str, VimeoVideo]
```

### Comparing `vimeotools-0.0.2/src/vimeotools/vimeo_showcase.py` & `vimeotools-0.0.3/src/vimeotools/vimeo_showcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,15 @@
     SHOWCASE_ALLOWED_KEYS_TO_SET
 )
 from vimeo_video import VimeoVideo as VimeoVideo_
 
 if TYPE_CHECKING:
     from vimeo_connection import VimeoConnection
     from vimeo_data import VimeoData
-"""
-if TYPE_CHECKING:
     from vimeo_video import VimeoVideo
-"""
 
 class VimeoShowcase(VimeoItem):
     """
     A class to represent a Vimeo showcase.
     """
     BASE_URI = '/albums'
     API_URI = '/me/albums'
@@ -53,15 +50,15 @@
     def __init__(
         self,
         connection: VimeoConnection,
         code_or_uri: Optional[str] = None,
         name: Optional[str] = None,
         data: Optional[Dict[str, Any]] = None,
         data_object: Optional[VimeoData] = None,
-        videos: List[VimeoVideo_] = [],
+        videos: List['VimeoVideo'] = [],
         creation_data: Optional[Dict[str, Any]] = {},  # for creation, must at least contain 'name'
     ):
         """
         Initialize a Vimeo showcase.
         :param client: Union[vimeo.VimeoClient, Dict[str, str]]
         :param code_or_uri: Optional[str]
         :param creation_data: Optional[Dict[str, Any]]
@@ -144,27 +141,19 @@
         self,
         picture: str
     ):
         """
         Add a thumbnail to the showcase.
         """
         raise NotImplementedError
-    
-    @property
-    def videos(
-        self
-    ) -> List[VimeoVideo_]:
-        """
-        Get the videos of the showcase.
-        """
-        return self.get_videos()
+
 
     def add_video(
         self,
-        video: Union[str, VimeoVideo_]  # code or object
+        video: Union[str, 'VimeoVideo']  # code or object
     ):
         """
         Add a video to the showcase.
         """
         if isinstance(video, VimeoVideo_):
             video = video.code # type: ignore
 
@@ -211,23 +200,14 @@
         logo_id: str
     ):
         """
         Get the logo of the showcase.
         """
         raise NotImplementedError
     
-    @property
-    def logos(
-        self
-    ):
-        """
-        Get the logos of the showcase.
-        """
-        raise NotImplementedError
-    
     def get_videos(
         self,
         refresh: bool = False,
         returning: Literal[
             'code',
             'codes',
             'uri',
@@ -239,15 +219,15 @@
             'object',
             'objects',
             'json'
         ] = 'object'
     ) -> Union[
             Dict[str, Any],
             List[Dict[str, Any]],
-            List[VimeoVideo_],
+            List['VimeoVideo'],
             List[str],
             str
         ]:
         """
         Get the videos of the showcase.
         """
         returning = transform_returning(returning)
@@ -320,14 +300,32 @@
         self
     ):
         """
         Get the thumbnails of the showcase.
         """
         raise NotImplementedError
 
+    @property
+    def logos(
+        self
+    ):
+        """
+        Get the logos of the showcase.
+        """
+        raise NotImplementedError
+    
+    @property
+    def nb_videos(
+        self
+    ) -> int:
+        """
+        Get the number of videos in the showcase.
+        """
+        return self._data['metadata']['connections']['videos']['total']  # type: ignore
+
     def remove_video(
         self,
         video: str
     ):
         """
         Remove a video from the showcase.
         """
@@ -340,18 +338,18 @@
         response = self.client.delete(uri)
         if response.status_code == 204:
             pass
         elif response.status_code == 403:
             raise PermissionError('You do not have permission to remove a video from this showcase.')
         elif response.status_code == 404:
             raise ValueError('The showcase or video does not exist.')
-    
+
     def replace_videos(
         self,
-        videos: List[Union[str, VimeoVideo_]]  # codes, uris or objects
+        videos: List[Union[str, 'VimeoVideo']]  # codes, uris or objects
     ):
         """
         Replace all the videos of the showcase.
         """
         uri = f'{self.API_URI}/{self.code}/videos'
 
         if isinstance(videos[0], str):
@@ -391,7 +389,16 @@
         video_id: str
     ):
         """
         Set the featured video of the showcase.
         """
         raise NotImplementedError
 
+    @property
+    def videos(
+        self
+    ) -> List['VimeoVideo']:
+        """
+        Get the videos of the showcase.
+        """
+        return self.get_videos()  # no idea why this is should be an error
+
```

### Comparing `vimeotools-0.0.2/src/vimeotools/vimeo_video.py` & `vimeotools-0.0.3/src/vimeotools/vimeo_video.py`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.2/src/vimeotools.egg-info/PKG-INFO` & `vimeotools-0.0.3/src/vimeotools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vimeotools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for Vimeo
 Home-page: https://github.com/georgpfolz/vimeotools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/georgpfolz/vimeotools/issues
 Project-URL: Documentation, https://georgpfolz.github.io/vimeotools
@@ -40,19 +40,26 @@
 
 You can also opt to create or set an object in live mode, so everytime a property is queried, the appropriate request is made on Vimeo first.
 
 ## documentation
 The (Sphinx) documentation is very crude (created with autodoc) currently and will be improved in subsequent versions.
 
 # History
+## 0.0.3 (2023-07-13)
+- **VimeoShocase** und **VimeoFolder**: property **nb_videos**
+- **VimeoData** changed property names
+	- video_count -> nb_videos
+	- showcases_count -> nb_showcases
+	- folders_count -> nb_folders
+
 ## 0.0.2 (2023-07-12)
 - VimeoData gets the methods **save** and **load**, to save or load data as json or pickle. 
 - the **__init__** of VimeoVideo, VimeoShowcase, VimeoFolder gets a parameter **data**, where the data can be passed when the object is created, so no request is needed.
 - Objects have a new attribute **temp_data** (dictionary) where you can store data relevant to your runing program directly on the object.
-- The **VimeoData** object can be added to **VimeoVideo**, **VimeoShowcase** and **VimeoFolder** instances. So the data object can be updated if there is a change in one of those insetances.
+- The **VimeoData** object can be added to **VimeoVideo**, **VimeoShowcase** and **VimeoFolder** instances. So the data object can be updated if there is a change in one of those instances.
 - using **pathlib** (instead of os.path): all filepath parameters accept Path objects.
 
 Still no unit tests, this is still very much in beta!
 
 ## 0.0.1 (2023-07-07)
 This is the first version. It provides the **VimeoConnection**, **VimeoData**, **Video** and **VimeoShowcase** and **VimeoFolder** classes.
```

