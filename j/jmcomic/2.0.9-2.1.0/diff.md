# Comparing `tmp/jmcomic-2.0.9.tar.gz` & `tmp/jmcomic-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.0.9.tar", last modified: Wed Jun 28 04:38:58 2023, max compression
+gzip compressed data, was "jmcomic-2.1.0.tar", last modified: Thu Jul 13 09:15:06 2023, max compression
```

## Comparing `jmcomic-2.0.9.tar` & `jmcomic-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 04:38:58.578172 jmcomic-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-28 04:38:49.000000 jmcomic-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-28 04:38:58.578172 jmcomic-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-28 04:38:49.000000 jmcomic-2.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 04:38:58.582172 jmcomic-2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-28 04:38:49.000000 jmcomic-2.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 04:38:58.578172 jmcomic-2.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 04:38:58.578172 jmcomic-2.0.9/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 04:38:49.000000 jmcomic-2.0.9/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-28 04:38:49.000000 jmcomic-2.0.9/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-06-28 04:38:49.000000 jmcomic-2.0.9/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-28 04:38:49.000000 jmcomic-2.0.9/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-28 04:38:49.000000 jmcomic-2.0.9/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-28 04:38:49.000000 jmcomic-2.0.9/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-28 04:38:49.000000 jmcomic-2.0.9/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-06-28 04:38:49.000000 jmcomic-2.0.9/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 04:38:58.578172 jmcomic-2.0.9/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-28 04:38:58.000000 jmcomic-2.0.9/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-28 04:38:58.000000 jmcomic-2.0.9/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 04:38:58.000000 jmcomic-2.0.9/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 04:38:58.000000 jmcomic-2.0.9/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-28 04:38:58.000000 jmcomic-2.0.9/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:15:06.803159 jmcomic-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-13 09:14:57.000000 jmcomic-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-13 09:15:06.803159 jmcomic-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-13 09:14:57.000000 jmcomic-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:15:06.803159 jmcomic-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-13 09:14:57.000000 jmcomic-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:15:06.799159 jmcomic-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:15:06.803159 jmcomic-2.1.0/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-13 09:14:57.000000 jmcomic-2.1.0/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:15:06.803159 jmcomic-2.1.0/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 09:15:06.000000 jmcomic-2.1.0/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.0.9/LICENSE` & `jmcomic-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.9/PKG-INFO` & `jmcomic-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.9
+Version: 2.1.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.0.9/README.md` & `jmcomic-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.9/setup.py` & `jmcomic-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.9/src/jmcomic/api.py` & `jmcomic-2.1.0/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.9/src/jmcomic/jm_client_impl.py` & `jmcomic-2.1.0/src/jmcomic/jm_client_impl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .jm_client_interface import *
 
 
+# noinspection PyAbstractClass
 class AbstractJmClient(
     JmcomicClient,
     PostmanProxy,
 ):
 
     def __init__(self,
                  postman: Postman,
@@ -35,43 +36,55 @@
     def request_with_retry(self,
                            request,
                            url,
                            domain_index=0,
                            retry_count=0,
                            **kwargs,
                            ):
+        """
+        统一请求，支持重试
+        @param request: 请求方法
+        @param url: 图片url / path (/album/xxx)
+        @param domain_index: 域名下标
+        @param retry_count: 重试次数
+        @param kwargs: 请求方法的kwargs
+        """
         if domain_index >= len(self.domain_list):
-            raise AssertionError("All domains failed.")
-
-        domain = self.domain_list[domain_index]
+            raise AssertionError(f"请求重试全部失败: [{url}], {self.domain_list}")
 
-        if not url.startswith(JmModuleConfig.PROT):
+        if url.startswith('/'):
+            # path
+            domain = self.domain_list[domain_index]
             url = self.of_api_url(url, domain)
             jm_debug('api', url)
+        else:
+            # 图片url
+            pass
 
-        if domain_index != 0 and retry_count != 0:
+        if domain_index != 0 or retry_count != 0:
             jm_debug(
-                f'请求重试',
+                f'request_retry',
                 ', '.join([
                     f'次数: [{retry_count}/{self.retry_times}]',
-                    f'域名: [{domain} ({domain_index}/{len(self.domain_list)})]',
+                    f'域名: [{domain_index} of {self.domain_list}]',
                     f'路径: [{url}]',
                     f'参数: [{kwargs if "login" not in url else "#login_form#"}]'
                 ])
             )
 
         try:
             return request(url, **kwargs)
         except Exception as e:
             self.before_retry(e, kwargs, retry_count, url)
 
-            if retry_count < self.retry_times:
-                return self.request_with_retry(request, url, domain_index, retry_count + 1, **kwargs)
-            else:
-                return self.request_with_retry(request, url, domain_index + 1, 0, **kwargs)
+        if retry_count < self.retry_times:
+            return self.request_with_retry(request, url, domain_index, retry_count + 1, **kwargs)
+        else:
+            return self.request_with_retry(request, url, domain_index + 1, 0, **kwargs)
+
 
     # noinspection PyMethodMayBeStatic, PyUnusedLocal
     def before_retry(self, e, kwargs, retry_count, url):
         jm_debug('error', str(e))
 
     def enable_cache(self, debug=False):
         def wrap_func_cache(func_name, cache_dict_name):
@@ -233,15 +246,68 @@
                   f"URL=[{resp.url}]，" \
                   + (f"响应文本=[{resp.text}]" if len(resp.text) < 200 else
                      f'响应文本过长(len={len(resp.text)})，不打印'
                      )
         raise AssertionError(msg)
 
     def get_jm_image(self, img_url) -> JmImageResp:
-        return JmImageResp(self.get(img_url))
+
+        def get_if_fail_raise(url):
+            """
+            使用此方法包装 self.get
+            """
+            resp = JmImageResp(self.get(url))
+
+            if resp.is_success:
+                return resp
+
+            self.raise_request_error(
+                resp.resp, resp.get_error_msg()
+            )
+
+            return resp
+
+        return self.request_with_retry(get_if_fail_raise, img_url)
+
+    def album_comment(self,
+                      video_id,
+                      comment,
+                      originator='',
+                      status='true',
+                      comment_id=None,
+                      **kwargs,
+                      ) -> JmAcResp:
+        data = {
+            'video_id': video_id,
+            'comment': comment,
+            'originator': originator,
+            'status': status,
+        }
+
+        # 处理回复评论
+        if comment_id is not None:
+            data.pop('status')
+            data['comment_id'] = comment_id
+            data['is_reply'] = 1
+            data['forum_subject'] = 1
+
+        jm_debug('album_comment',
+                 f'{video_id}: [{comment}]' +
+                 (f' to ({comment_id})' if comment_id is not None else '')
+                 )
+
+        resp = self.post('https://18comic.vip/ajax/album_comment',
+                         headers=JmModuleConfig.album_comment_headers,
+                         data=data,
+                         )
+
+        ret = JmAcResp(resp)
+        jm_debug('album_comment', f'{video_id}: [{comment}] ← ({ret.model().cid})')
+
+        return ret
 
     @classmethod
     def require_resp_success_else_raise(cls, resp, req_url):
         # 1. 检查是否 album_missing
         error_album_missing = '/error/album_missing'
         if resp.url.endswith(error_album_missing) and not req_url.endswith(error_album_missing):
             cls.raise_request_error(
```

### Comparing `jmcomic-2.0.9/src/jmcomic/jm_client_interface.py` & `jmcomic-2.1.0/src/jmcomic/jm_client_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,39 @@
 
 class JmResp(CommonResp):
 
     @property
     def is_success(self) -> bool:
         return self.http_code == 200 and len(self.content) != 0
 
+    def json(self, **kwargs) -> Dict:
+        raise NotImplementedError
+
+    def model(self) -> DictModel:
+        return DictModel(self.json())
+
 
 class JmImageResp(JmResp):
 
+    def json(self, **kwargs) -> Dict:
+        raise AssertionError
+
     def require_success(self):
         if self.is_success:
             return
 
+        raise AssertionError(self.get_error_msg())
+
+    def get_error_msg(self):
         msg = f'禁漫图片获取失败: [{self.url}]'
         if self.http_code != 200:
             msg += f'，http状态码={self.http_code}'
         if len(self.content) == 0:
             msg += f'，响应数据为空'
-
-        raise AssertionError(msg)
+        return msg
 
     def transfer_to(self,
                     path,
                     scramble_id,
                     decode_image=True,
                     img_url=None,
                     ):
@@ -102,23 +113,33 @@
         self.require_success()
         from json import loads
         return loads(self.decoded_data)
 
     def json(self, **kwargs) -> Dict:
         return self.resp.json()
 
-    def model(self) -> DictModel:
-        return DictModel(self.json())
-
     @property
     def model_data(self) -> DictModel:
         self.require_success()
         return DictModel(self.res_data)
 
 
+# album-comment
+class JmAcResp(JmResp):
+
+    def is_success(self) -> bool:
+        return super().is_success and self.json()['err'] is False
+
+    def json(self, **kwargs) -> Dict:
+        return self.resp.json()
+
+    def model(self) -> DictModel:
+        return DictModel(self.json())
+
+
 """
 
 Client Interface
 
 """
 
 
@@ -150,14 +171,33 @@
               password,
               refresh_client_cookies=True,
               id_remember='on',
               login_remember='on',
               ):
         raise NotImplementedError
 
+    def album_comment(self,
+                      video_id,
+                      comment,
+                      originator='',
+                      status='true',
+                      comment_id=None,
+                      **kwargs,
+                      ) -> JmAcResp:
+        """
+        评论漫画/评论回复
+        @param video_id: album_id/photo_id
+        @param comment: 评论内容
+        @param status: 是否 "有劇透"
+        @param comment_id: 被回复评论的id
+        @param originator:
+        @return: JmAcResp 对象
+        """
+        raise NotImplementedError
+
 
 class JmImageClient:
 
     # -- 下载图片 --
 
     def download_image(self,
                        img_url: str,
@@ -200,14 +240,15 @@
         raise NotImplementedError
 
     @classmethod
     def img_is_not_need_to_decode(cls, data_original: str, _resp):
         return data_original.endswith('.gif')
 
 
+# noinspection PyAbstractClass
 class JmcomicClient(
     JmImageClient,
     JmDetailClient,
     JmUserClient,
     Postman,
 ):
     def get_jmcomic_url(self, postman=None):
```

### Comparing `jmcomic-2.0.9/src/jmcomic/jm_config.py` & `jmcomic-2.1.0/src/jmcomic/jm_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,22 +61,22 @@
         if cls.DOMAIN is None:
             from .jm_toolkit import JmcomicText
             cls.DOMAIN = JmcomicText.parse_to_jm_domain(cls.get_jmcomic_url(postman))
 
         return cls.DOMAIN  # jmcomic默认域名
 
     @classmethod
-    def headers(cls, authority=None):
+    def headers(cls, domain='18comic.vip'):
         return {
-            'authority': authority or '18comic.vip',
+            'authority': domain,
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,'
                       'application/signed-exchange;v=b3;q=0.7',
             'accept-language': 'zh-CN,zh;q=0.9',
             'cache-control': 'no-cache',
-            'referer': 'https://18comic.vip',
+            'referer': f'https://{domain}',
             'pragma': 'no-cache',
             'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'document',
             'sec-fetch-mode': 'navigate',
             'sec-fetch-site': 'none',
@@ -126,10 +126,30 @@
         resp = postman.get(cls.JM_PUB_URL)
         if resp.status_code != 200:
             raise AssertionError(resp.text)
 
         from .jm_toolkit import JmcomicText
         return JmcomicText.analyse_jm_pub_html(resp.text)
 
+    album_comment_headers = {
+        'authority': '18comic.vip',
+        'accept': 'application/json, text/javascript, */*; q=0.01',
+        'accept-language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+        'cache-control': 'no-cache',
+        'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
+        'origin': 'https://18comic.vip',
+        'pragma': 'no-cache',
+        'referer': 'https://18comic.vip/album/248965/',
+        'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
+        'sec-ch-ua-mobile': '?0',
+        'sec-ch-ua-platform': '"Windows"',
+        'sec-fetch-dest': 'empty',
+        'sec-fetch-mode': 'cors',
+        'sec-fetch-site': 'same-origin',
+        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) '
+                      'Chrome/114.0.0.0 Safari/537.36',
+        'x-requested-with': 'XMLHttpRequest',
+    }
+
 
 jm_debug = JmModuleConfig.jm_debug
 disable_jm_debug = JmModuleConfig.disable_jm_debug
```

### Comparing `jmcomic-2.0.9/src/jmcomic/jm_entity.py` & `jmcomic-2.1.0/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.9/src/jmcomic/jm_option.py` & `jmcomic-2.1.0/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.9/src/jmcomic/jm_toolkit.py` & `jmcomic-2.1.0/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.9/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.1.0/src/jmcomic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.9
+Version: 2.1.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

