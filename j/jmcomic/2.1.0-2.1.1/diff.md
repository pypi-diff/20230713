# Comparing `tmp/jmcomic-2.1.0.tar.gz` & `tmp/jmcomic-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.1.0.tar", last modified: Thu Jul 13 09:15:06 2023, max compression
+gzip compressed data, was "jmcomic-2.1.1.tar", last modified: Thu Jul 13 14:04:49 2023, max compression
```

## Comparing `jmcomic-2.1.0.tar` & `jmcomic-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:15:06.803159 jmcomic-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-13 09:14:57.000000 jmcomic-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-13 09:15:06.803159 jmcomic-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-13 09:14:57.000000 jmcomic-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:15:06.803159 jmcomic-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-13 09:14:57.000000 jmcomic-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:15:06.799159 jmcomic-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:15:06.803159 jmcomic-2.1.0/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:15:06.803159 jmcomic-2.1.0/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:04:49.065920 jmcomic-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-13 14:04:34.000000 jmcomic-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-13 14:04:49.065920 jmcomic-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-13 14:04:34.000000 jmcomic-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:04:49.065920 jmcomic-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-13 14:04:34.000000 jmcomic-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:04:49.061920 jmcomic-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:04:49.065920 jmcomic-2.1.1/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:04:49.065920 jmcomic-2.1.1/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.1.0/LICENSE` & `jmcomic-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.0/PKG-INFO` & `jmcomic-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.1.0/README.md` & `jmcomic-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.0/setup.py` & `jmcomic-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.0/src/jmcomic/api.py` & `jmcomic-2.1.1/src/jmcomic/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
              f'章节数: [{len(album)}]'
              f'标题: [{album.title}], '
              )
 
     def download_photo(photo: JmPhotoDetail,
                        debug_topic='photo',
                        ):
-        jm_client.ensure_photo_can_use(photo)
+        jm_client.check_photo(photo)
 
         jm_debug(debug_topic,
                  f'开始下载章节: {photo.id} ({photo.album_id}[{photo.index}/{len(album)}]), '
                  f'标题: [{photo.title}], '
                  f'图片数为[{len(photo)}]')
 
         download_by_photo_detail(photo, option)
@@ -84,15 +84,15 @@
     @param option: 选项
     """
     option, jm_client = build_client(option)
 
     # 下载准备
     use_cache = option.download_cache
     decode_image = option.download_image_decode
-    jm_client.ensure_photo_can_use(photo_detail)
+    jm_client.check_photo(photo_detail)
 
     # 下载每个图片的函数
     def download_image(index, image: JmImageDetail, debug_topic='image'):
         img_save_path = option.decide_image_filepath(photo_detail, index)
         debug_tag = f'{image.aid}/{image.filename} [{index + 1}/{len(photo_detail)}]'
 
         # 已下载过，缓存命中
```

### Comparing `jmcomic-2.1.0/src/jmcomic/jm_client_impl.py` & `jmcomic-2.1.1/src/jmcomic/jm_client_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         @param request: 请求方法
         @param url: 图片url / path (/album/xxx)
         @param domain_index: 域名下标
         @param retry_count: 重试次数
         @param kwargs: 请求方法的kwargs
         """
         if domain_index >= len(self.domain_list):
-            raise AssertionError(f"请求重试全部失败: [{url}], {self.domain_list}")
+            self.fallback(request, url, domain_index, retry_count, **kwargs)
 
         if url.startswith('/'):
             # path
             domain = self.domain_list[domain_index]
             url = self.of_api_url(url, domain)
             jm_debug('api', url)
         else:
@@ -77,15 +77,14 @@
             self.before_retry(e, kwargs, retry_count, url)
 
         if retry_count < self.retry_times:
             return self.request_with_retry(request, url, domain_index, retry_count + 1, **kwargs)
         else:
             return self.request_with_retry(request, url, domain_index + 1, 0, **kwargs)
 
-
     # noinspection PyMethodMayBeStatic, PyUnusedLocal
     def before_retry(self, e, kwargs, retry_count, url):
         jm_debug('error', str(e))
 
     def enable_cache(self, debug=False):
         def wrap_func_cache(func_name, cache_dict_name):
             import common
@@ -126,14 +125,17 @@
 
     def get_jmcomic_url(self, postman=None):
         return JmModuleConfig.get_jmcomic_url(postman or self.get_root_postman())
 
     def get_jmcomic_domain_all(self, postman=None):
         return JmModuleConfig.get_jmcomic_domain_all(postman or self.get_root_postman())
 
+    def fallback(self, request, url, domain_index, retry_count, **kwargs):
+        raise AssertionError(f"请求重试全部失败: [{url}], {self.domain_list}")
+
 
 # 基于网页实现的JmClient
 class JmHtmlClient(AbstractJmClient):
 
     def get_album_detail(self, album_id) -> JmAlbumDetail:
         # 参数校验
         album_id = JmcomicText.parse_to_photo_id(album_id)
@@ -156,25 +158,14 @@
 
         # 一并获取该章节的所处本子
         if fetch_album is True:
             photo_detail.from_album = self.get_album_detail(photo_detail.album_id)
 
         return photo_detail
 
-    def ensure_photo_can_use(self, photo_detail: JmPhotoDetail):
-        # 检查 from_album
-        if photo_detail.from_album is None:
-            photo_detail.from_album = self.get_album_detail(photo_detail.album_id)
-
-        # 检查 page_arr 和 data_original_domain
-        if photo_detail.page_arr is None or photo_detail.data_original_domain is None:
-            new = self.get_photo_detail(photo_detail.photo_id, False)
-            new.from_album = photo_detail.from_album
-            photo_detail.__dict__.update(new.__dict__)
-
     def search_album(self, search_query, main_tag=0, page=1) -> JmSearchPage:
         params = {
             'main_tag': main_tag,
             'search_query': search_query,
             'page': page,
         }
 
@@ -222,15 +213,15 @@
     def get_jm_html(self, url, require_200=True, **kwargs):
         """
         请求禁漫网页的入口
         """
         resp = self.get(url, **kwargs)
 
         if require_200 is True and resp.status_code != 200:
-            write_text('./resp.html', resp.text)
+            # write_text('./resp.html', resp.text)
             self.check_special_http_code(resp)
             self.raise_request_error(resp)
 
         # 检查请求是否成功
         self.require_resp_success_else_raise(resp, url)
 
         return resp
```

### Comparing `jmcomic-2.1.0/src/jmcomic/jm_client_interface.py` & `jmcomic-2.1.1/src/jmcomic/jm_client_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -147,26 +147,33 @@
 
     def get_album_detail(self, album_id) -> JmAlbumDetail:
         raise NotImplementedError
 
     def get_photo_detail(self, photo_id, fetch_album=True) -> JmPhotoDetail:
         raise NotImplementedError
 
-    def ensure_photo_can_use(self, photo_detail: JmPhotoDetail):
-        raise NotImplementedError
-
     def search_album(self, search_query: str, main_tag: int = 0, page: int = 1) -> JmSearchPage:
         raise NotImplementedError
 
     def of_api_url(self, api_path, domain):
         raise NotImplementedError
 
     def enable_cache(self, debug=False):
         raise NotImplementedError
 
+    def check_photo(self, photo_detail: JmPhotoDetail):
+        # 检查 from_album
+        if photo_detail.from_album is None:
+            photo_detail.from_album = self.get_album_detail(photo_detail.album_id)
+
+        # 检查 page_arr 和 data_original_domain
+        if photo_detail.page_arr is None or photo_detail.data_original_domain is None:
+            new = self.get_photo_detail(photo_detail.photo_id, False)
+            new.from_album = photo_detail.from_album
+            photo_detail.__dict__.update(new.__dict__)
 
 class JmUserClient:
 
     def login(self,
               username,
               password,
               refresh_client_cookies=True,
```

### Comparing `jmcomic-2.1.0/src/jmcomic/jm_config.py` & `jmcomic-2.1.1/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.0/src/jmcomic/jm_entity.py` & `jmcomic-2.1.1/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.0/src/jmcomic/jm_option.py` & `jmcomic-2.1.1/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.0/src/jmcomic/jm_toolkit.py` & `jmcomic-2.1.1/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.0/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.1.1/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

