# Comparing `tmp/picimagesearch-3.9.3.tar.gz` & `tmp/picimagesearch-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picimagesearch-3.9.3.tar", max compression
+gzip compressed data, was "picimagesearch-3.9.4.tar", max compression
```

## Comparing `picimagesearch-3.9.3.tar` & `picimagesearch-3.9.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/LICENSE
--rw-r--r--   0        0        0      251 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/__init__.py
--rw-r--r--   0        0        0     2145 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/ascii2d.py
--rw-r--r--   0        0        0     1267 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/baidu.py
--rw-r--r--   0        0        0     1433 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/ehentai.py
--rw-r--r--   0        0        0     2421 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/google.py
--rw-r--r--   0        0        0     1215 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/iqdb.py
--rw-r--r--   0        0        0      397 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/__init__.py
--rw-r--r--   0        0        0     3108 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/ascii2d.py
--rw-r--r--   0        0        0      778 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/baidu.py
--rw-r--r--   0        0        0     1895 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/ehentai.py
--rw-r--r--   0        0        0     2234 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/google.py
--rw-r--r--   0        0        0     3711 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/iqdb.py
--rw-r--r--   0        0        0     5170 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/saucenao.py
--rw-r--r--   0        0        0     2755 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/tracemoe.py
--rw-r--r--   0        0        0     1312 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/yandex.py
--rw-r--r--   0        0        0     4510 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/network.py
--rw-r--r--   0        0        0     4702 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/saucenao.py
--rw-r--r--   0        0        0     1518 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/sync.py
--rw-r--r--   0        0        0     4829 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/tracemoe.py
--rw-r--r--   0        0        0     1945 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/yandex.py
--rw-r--r--   0        0        0     1999 2023-07-10 19:01:35.061855 picimagesearch-3.9.3/README.md
--rw-r--r--   0        0        0     1179 2023-07-10 19:01:35.061855 picimagesearch-3.9.3/pyproject.toml
--rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 picimagesearch-3.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/LICENSE
+-rw-r--r--   0        0        0      251 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/__init__.py
+-rw-r--r--   0        0        0     2061 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/ascii2d.py
+-rw-r--r--   0        0        0     1257 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/baidu.py
+-rw-r--r--   0        0        0     1415 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/ehentai.py
+-rw-r--r--   0        0        0     2381 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/google.py
+-rw-r--r--   0        0        0     1193 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/iqdb.py
+-rw-r--r--   0        0        0      397 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/__init__.py
+-rw-r--r--   0        0        0     3375 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/ascii2d.py
+-rw-r--r--   0        0        0      778 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/baidu.py
+-rw-r--r--   0        0        0     1895 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/ehentai.py
+-rw-r--r--   0        0        0     2234 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/google.py
+-rw-r--r--   0        0        0     3711 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/iqdb.py
+-rw-r--r--   0        0        0     5170 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/saucenao.py
+-rw-r--r--   0        0        0     2755 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/tracemoe.py
+-rw-r--r--   0        0        0     1312 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/yandex.py
+-rw-r--r--   0        0        0     4576 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/network.py
+-rw-r--r--   0        0        0     4639 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/saucenao.py
+-rw-r--r--   0        0        0     1518 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/sync.py
+-rw-r--r--   0        0        0     4770 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/tracemoe.py
+-rw-r--r--   0        0        0     1909 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/yandex.py
+-rw-r--r--   0        0        0     1999 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/README.md
+-rw-r--r--   0        0        0     1179 2023-07-13 00:29:39.810856 picimagesearch-3.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 picimagesearch-3.9.4/PKG-INFO
```

### Comparing `picimagesearch-3.9.3/LICENSE` & `picimagesearch-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/ascii2d.py` & `picimagesearch-3.9.4/PicImageSearch/ascii2d.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,24 +40,22 @@
         • .raw[0].url = First index of url source that was found\n
         • .raw[0].authors = First index of authors that was found\n
         • .raw[0].thumbnail = First index of url image that was found\n
         • .raw[0].detail = First index of details image that was found
         """
         if url:
             ascii2d_url = "https://ascii2d.net/search/uri"
-            resp_text, resp_url, _ = await self.post(ascii2d_url, data={"uri": url})
+            resp = await self.post(ascii2d_url, data={"uri": url})
         elif file:
             ascii2d_url = "https://ascii2d.net/search/file"
             files: Dict[str, Any] = {
                 "file": file if isinstance(file, bytes) else open(file, "rb")
             }
-            resp_text, resp_url, _ = await self.post(ascii2d_url, files=files)
+            resp = await self.post(ascii2d_url, files=files)
         else:
             raise ValueError("url or file is required")
 
         # 如果启用bovw选项，第一次请求是向服务器提交文件
         if self.bovw:
-            resp_text, resp_url, _ = await self.get(
-                resp_url.replace("/color/", "/bovw/")
-            )
+            resp = await self.get(resp.url.replace("/color/", "/bovw/"))
 
-        return Ascii2DResponse(resp_text, resp_url)
+        return Ascii2DResponse(resp.text, resp.url)
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/baidu.py` & `picimagesearch-3.9.4/PicImageSearch/baidu.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,16 @@
             files = (
                 {"image": file}
                 if isinstance(file, bytes)
                 else {"image": open(file, "rb")}
             )
         else:
             raise ValueError("url or file is required")
-        resp_text, _, _ = await self.post(
+        resp = await self.post(
             "https://graph.baidu.com/upload", params=params, files=files
         )
-        next_url = (json_loads(resp_text))["data"]["url"]
-        resp_text, resp_url, _ = await self.get(next_url)
-        next_url = (re.search(r'"firstUrl":"([^"]+)"', resp_text)[1]).replace(r"\/", "/")  # type: ignore
-        resp_text, _, _ = await self.get(next_url)
-        return BaiDuResponse(json_loads(resp_text), resp_url)
+        next_url = (json_loads(resp.text))["data"]["url"]
+        resp = await self.get(next_url)
+        final_url = resp.url
+        next_url = (re.search(r'"firstUrl":"([^"]+)"', resp.text)[1]).replace(r"\/", "/")  # type: ignore
+        resp = await self.get(next_url)
+        return BaiDuResponse(json_loads(resp.text), final_url)
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/ehentai.py` & `picimagesearch-3.9.4/PicImageSearch/ehentai.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,9 +38,9 @@
             raise ValueError("url or file is required")
         if self.covers:
             data["fs_covers"] = "on"
         if self.similar:
             data["fs_similar"] = "on"
         if self.exp:
             data["fs_exp"] = "on"
-        resp_text, resp_url, _ = await self.post(url=_url, data=data, files=files)
-        return EHentaiResponse(resp_text, resp_url)
+        resp = await self.post(url=_url, data=data, files=files)
+        return EHentaiResponse(resp.text, resp.url)
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/google.py` & `picimagesearch-3.9.4/PicImageSearch/yandex.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,60 @@
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
-from .model import GoogleResponse
+from .model import YandexResponse
 from .network import HandOver
 
 
-class Google(HandOver):
+class Yandex(HandOver):
     """
-    Google
+    Yandex
     -----------
-    Reverse image from https://www.google.com\n
+    Reverse image from https://yandex.com/images/search\n
 
 
     Params Keys
     -----------
-    :param **request_kwargs: proxies settings
+    :param **request_kwargs: proxies setting.\n
     """
 
     def __init__(self, **request_kwargs: Any):
         super().__init__(**request_kwargs)
-        self.url = "https://www.google.com/searchbyimage"
-
-    async def pre_page(self, resp: GoogleResponse) -> Optional[GoogleResponse]:
-        index = resp.pages.index(resp.url)
-        if index == 0:
-            return None
-        resp_text, resp_url, _ = await self.get(resp.pages[index - 1])
-        return GoogleResponse(resp_text, resp_url)
-
-    async def next_page(self, resp: GoogleResponse) -> Optional[GoogleResponse]:
-        index = resp.pages.index(resp.url)
-        if index == len(resp.pages) - 1:
-            return None
-        resp_text, resp_url, _ = await self.get(resp.pages[index + 1])
-        return GoogleResponse(resp_text, resp_url)
+        self.url = "https://yandex.com/images/search"
 
     async def search(
         self, url: Optional[str] = None, file: Union[str, bytes, Path, None] = None
-    ) -> GoogleResponse:
+    ) -> YandexResponse:
         """
-        Google
+        Yandex
         -----------
-        Reverse image from https://www.google.com\n
+        Reverse image from https://yandex.com/images/search\n
 
 
         Return Attributes
         -----------
         • .origin = Raw data from scrapper\n
         • .raw = Simplified data from scrapper\n
-        • .raw[2] = Third index of simplified data that was found <Should start from index 2,
-                    because from there is matching image>\n
-        • .raw[2].title = Third index of title that was found\n
-        • .raw[2].url = Third index of url source that was found\n
-        • .raw[2].thumbnail = Third index of base64 string image that was found
+        • .raw[0] = First index of simplified data that was found\n
+        • .raw[0].title = First index of title that was found\n
+        • .raw[0].url = First index of url source that was found\n
+        • .raw[0].thumbnail = First index of url image that was found\n
+        • .raw[0].source = First index of source that was found\n
+        • .raw[0].content = First index of content that was found\n
+        • .raw[0].size = First index of size that was found\n
         """
-        params: Dict[str, Any] = {"sbisrc": 1}
+
+        params = {"rpt": "imageview"}
         if url:
-            params["image_url"] = url
-            resp_text, resp_url, _ = await self.get(self.url, params=params)
+            params["url"] = url
+            resp = await self.get(self.url, params=params)
         elif file:
-            files = {
-                "encoded_image": file if isinstance(file, bytes) else open(file, "rb")
+            files: Dict[str, Any] = {
+                "upfile": file if isinstance(file, bytes) else open(file, "rb")
             }
-            resp_text, resp_url, _ = await self.post(
-                f"{self.url}/upload", data=params, files=files
+            resp = await self.post(
+                self.url, params=params, data={"prg": 1}, files=files
             )
         else:
             raise ValueError("url or file is required")
-        return GoogleResponse(resp_text, resp_url)
+
+        return YandexResponse(resp.text, resp.url)
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/iqdb.py` & `picimagesearch-3.9.4/PicImageSearch/iqdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     ) -> IqdbResponse:
         iqdb_url = "https://3d.iqdb.org/" if is_3d else "https://iqdb.org/"
         data: Dict[str, Any] = {}
         if force_gray:  # 忽略颜色
             data["forcegray"] = "on"
         if url:
             data["url"] = url
-            resp_text, _, _ = await self.post(iqdb_url, data=data)
+            resp = await self.post(iqdb_url, data=data)
         elif file:
             files = {"file": file if isinstance(file, bytes) else open(file, "rb")}
-            resp_text, _, _ = await self.post(iqdb_url, data=data, files=files)
+            resp = await self.post(iqdb_url, data=data, files=files)
         else:
             raise ValueError("url or file is required")
-        return IqdbResponse(resp_text)
+        return IqdbResponse(resp.text)
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/model/ascii2d.py` & `picimagesearch-3.9.4/PicImageSearch/model/ascii2d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from typing import List, Tuple
+from collections import namedtuple
+from typing import List
 
 from lxml.html import HTMLParser, fromstring
 from pyquery import PyQuery
 
-SUPPORTED_SOURCES = ["pixiv", "twitter", "fanbox", "fantia", "ニコニコ静画", "ニジエ"]
 BASE_URL = "https://ascii2d.net"
+SUPPORTED_SOURCES = ["pixiv", "twitter", "fanbox", "fantia", "ニコニコ静画", "ニジエ"]
+URL = namedtuple("URL", ["href", "text"])
 
 
 class Ascii2DItem:
     def __init__(self, data: PyQuery):
         self.origin: PyQuery = data  # 原始数据
         # 原图长宽，类型，大小
         self.hash: str = data("div.hash").eq(0).text()
         self.detail: str = data("small").eq(0).text()
         self.thumbnail: str = BASE_URL + data("img").eq(0).attr("src")
         self.url: str = ""
-        self.url_list: List[Tuple[str, str]] = []
+        self.url_list: List[URL] = []
         self.title: str = ""
         self.author: str = ""
         self.author_url: str = ""
         self._arrange(data)
 
     def _arrange(self, data: PyQuery) -> None:
         infos = data.find("div.detail-box.gray-link")
         if infos:
             links = infos.find("a")
             self.url_list = (
-                [(i.attr("href"), i.text()) for i in links.items()] if links else []
+                [URL(i.attr("href"), i.text()) for i in links.items()] if links else []
             )
             mark = infos("small").eq(-1).text() if links else ""
             self._arrange_links(infos, links, mark)
             self._arrange_title(infos)
         self._normalize_url_list()
         if not self.url_list:
             self._arrange_backup_links(data)
@@ -46,33 +48,35 @@
                 )
             elif links.eq(0).parents("small"):
                 infos.remove("small")
                 self.title = infos.text()
 
     def _arrange_title(self, infos: PyQuery) -> None:
         if not self.title:
-            self.title = infos.find("h6").text() or self._extract_external_text(infos)
+            self.title = self._extract_external_text(infos) or infos.find("h6").text()
+        if self.title and any(i in self.title for i in {"詳細掲示板のログ", "2ちゃんねるのログ"}):
+            self.title = ""
 
     @staticmethod
     def _extract_external_text(infos: PyQuery) -> str:
-        external = infos.find("div.external")
+        external = infos.find(".external")
         external.remove("a")
-        return external.text() or ""
+        return "\n".join((i.text() for i in external.items() if i.text())) or ""
 
     def _normalize_url_list(self) -> None:
         self.url_list = [
-            (BASE_URL + x[0], x[1]) if x[0].startswith("/") else x
-            for x in self.url_list
+            URL(BASE_URL + url.href, url.text) if url.href.startswith("/") else url
+            for url in self.url_list
         ]
 
     def _arrange_backup_links(self, data: PyQuery) -> None:
         links = data.find("div.pull-xs-right > a")
         if links:
             self.url = links.eq(0).attr("href")
-            self.url_list = [(self.url, links.eq(0).text())]
+            self.url_list = [URL(self.url, links.eq(0).text())]
 
 
 class Ascii2DResponse:
     def __init__(self, resp_text: str, resp_url: str):
         utf8_parser = HTMLParser(encoding="utf-8")
         data = PyQuery(fromstring(resp_text, parser=utf8_parser))
         self.origin: PyQuery = data  # 原始数据
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/model/baidu.py` & `picimagesearch-3.9.4/PicImageSearch/model/baidu.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/model/ehentai.py` & `picimagesearch-3.9.4/PicImageSearch/model/ehentai.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/model/google.py` & `picimagesearch-3.9.4/PicImageSearch/model/google.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/model/iqdb.py` & `picimagesearch-3.9.4/PicImageSearch/model/iqdb.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/model/saucenao.py` & `picimagesearch-3.9.4/PicImageSearch/model/saucenao.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/model/tracemoe.py` & `picimagesearch-3.9.4/PicImageSearch/model/tracemoe.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/model/yandex.py` & `picimagesearch-3.9.4/PicImageSearch/model/yandex.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/network.py` & `picimagesearch-3.9.4/PicImageSearch/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from collections import namedtuple
 from types import TracebackType
-from typing import Any, Dict, Optional, Tuple, Type, Union
+from typing import Any, Dict, Optional, Type, Union
 
 from httpx import AsyncClient, QueryParams
 
 DEFAULT_HEADERS = {
     "User-Agent": (
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
         "AppleWebKit/537.36 (KHTML, like Gecko) "
         "Chrome/99.0.4844.82 Safari/537.36"
     )
 }
+RESP = namedtuple("RESP", ["text", "url", "status_code"])
 
 
 class Network:
     def __init__(
         self,
         internal: bool = False,
         proxies: Optional[str] = None,
@@ -100,45 +102,45 @@
         self.proxies: Optional[str] = proxies
         self.headers: Optional[Dict[str, str]] = headers
         self.cookies: Optional[str] = cookies
         self.timeout: float = timeout
 
     async def get(
         self, url: str, params: Optional[Dict[str, str]] = None, **kwargs: Any
-    ) -> Tuple[str, str, int]:
+    ) -> RESP:
         async with ClientManager(
             self.client,
             self.proxies,
             self.headers,
             self.cookies,
             self.timeout,
         ) as client:
             resp = await client.get(url, params=params, **kwargs)
-            return resp.text, str(resp.url), resp.status_code
+            return RESP(resp.text, str(resp.url), resp.status_code)
 
     async def post(
         self,
         url: str,
         params: Union[Dict[str, Any], QueryParams, None] = None,
         data: Optional[Dict[Any, Any]] = None,
         files: Optional[Dict[str, Any]] = None,
         json: Optional[Dict[str, Any]] = None,
         **kwargs: Any
-    ) -> Tuple[str, str, int]:
+    ) -> RESP:
         async with ClientManager(
             self.client,
             self.proxies,
             self.headers,
             self.cookies,
             self.timeout,
         ) as client:
             resp = await client.post(
                 url, params=params, data=data, files=files, json=json, **kwargs
             )
-            return resp.text, str(resp.url), resp.status_code
+            return RESP(resp.text, str(resp.url), resp.status_code)
 
     async def download(self, url: str) -> bytes:
         async with ClientManager(
             self.client,
             self.proxies,
             self.headers,
             self.cookies,
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/saucenao.py` & `picimagesearch-3.9.4/PicImageSearch/saucenao.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,11 @@
             files = (
                 {"file": file}
                 if isinstance(file, bytes)
                 else {"file": open(file, "rb")}
             )
         else:
             raise ValueError("url or file is required")
-        resp_text, _, resp_status = await self.post(
-            self.url,
-            params=params,
-            files=files,
-        )
-        resp_json = json_loads(resp_text)
-        resp_json.update({"status_code": resp_status})
+        resp = await self.post(self.url, params=params, files=files)
+        resp_json = json_loads(resp.text)
+        resp_json.update({"status_code": resp.status_code})
         return SauceNAOResponse(resp_json)
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/sync.py` & `picimagesearch-3.9.4/PicImageSearch/sync.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/PicImageSearch/tracemoe.py` & `picimagesearch-3.9.4/PicImageSearch/tracemoe.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         super().__init__(**request_kwargs)
         self.size: Optional[str] = size
         self.mute: bool = mute
 
     # 获取自己的信息
     async def me(self, key: Optional[str] = None) -> TraceMoeMe:
         params = {"key": key} if key else None
-        resp_text, _, _ = await self.get(self.me_url, params=params)
-        return TraceMoeMe(json_loads(resp_text))
+        resp = await self.get(self.me_url, params=params)
+        return TraceMoeMe(json_loads(resp.text))
 
     @staticmethod
     def set_params(
         url: Optional[str],
         anilist_id: Optional[int],
         cut_borders: bool,
     ) -> Dict[str, Union[bool, int, str]]:
@@ -131,18 +131,15 @@
             files = (
                 {"file": file}
                 if isinstance(file, bytes)
                 else {"file": open(file, "rb")}
             )
         else:
             raise ValueError("url or file is required")
-        resp_text, _, _ = await self.post(
-            self.search_url,
-            headers=headers,
-            params=params,
-            files=files,
+        resp = await self.post(
+            self.search_url, headers=headers, params=params, files=files
         )
-        result = TraceMoeResponse(json_loads(resp_text), self.mute, self.size)
+        result = TraceMoeResponse(json_loads(resp.text), self.mute, self.size)
         await asyncio.gather(
             *[self.update_anime_info(item, chinese_title) for item in result.raw]
         )
         return result
```

### Comparing `picimagesearch-3.9.3/PicImageSearch/yandex.py` & `picimagesearch-3.9.4/PicImageSearch/google.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
-from .model import YandexResponse
+from .model import GoogleResponse
 from .network import HandOver
 
 
-class Yandex(HandOver):
+class Google(HandOver):
     """
-    Yandex
+    Google
     -----------
-    Reverse image from https://yandex.com/images/search\n
+    Reverse image from https://www.google.com\n
 
 
     Params Keys
     -----------
-    :param **request_kwargs: proxies setting.\n
+    :param **request_kwargs: proxies settings
     """
 
     def __init__(self, **request_kwargs: Any):
         super().__init__(**request_kwargs)
-        self.url = "https://yandex.com/images/search"
+        self.url = "https://www.google.com/searchbyimage"
+
+    async def _navigate_page(self, resp: GoogleResponse, offset: int) -> Optional[GoogleResponse]:
+        index = resp.pages.index(resp.url)
+        new_index = index + offset
+        if new_index < 0 or new_index >= len(resp.pages):
+            return None
+        _resp = await self.get(resp.pages[new_index])
+        return GoogleResponse(_resp.text, _resp.url)
+
+    async def pre_page(self, resp: GoogleResponse) -> Optional[GoogleResponse]:
+        return await self._navigate_page(resp, -1)
+
+    async def next_page(self, resp: GoogleResponse) -> Optional[GoogleResponse]:
+        return await self._navigate_page(resp, 1)
 
     async def search(
         self, url: Optional[str] = None, file: Union[str, bytes, Path, None] = None
-    ) -> YandexResponse:
+    ) -> GoogleResponse:
         """
-        Yandex
+        Google
         -----------
-        Reverse image from https://yandex.com/images/search\n
+        Reverse image from https://www.google.com\n
 
 
         Return Attributes
         -----------
         • .origin = Raw data from scrapper\n
         • .raw = Simplified data from scrapper\n
-        • .raw[0] = First index of simplified data that was found\n
-        • .raw[0].title = First index of title that was found\n
-        • .raw[0].url = First index of url source that was found\n
-        • .raw[0].thumbnail = First index of url image that was found\n
-        • .raw[0].source = First index of source that was found\n
-        • .raw[0].content = First index of content that was found\n
-        • .raw[0].size = First index of size that was found\n
+        • .raw[2] = Third index of simplified data that was found <Should start from index 2,
+                    because from there is matching image>\n
+        • .raw[2].title = Third index of title that was found\n
+        • .raw[2].url = Third index of url source that was found\n
+        • .raw[2].thumbnail = Third index of base64 string image that was found
         """
-
-        params = {"rpt": "imageview"}
+        params: Dict[str, Any] = {"sbisrc": 1}
         if url:
-            params["url"] = url
-            resp_text, resp_url, _ = await self.get(self.url, params=params)
+            params["image_url"] = url
+            resp = await self.get(self.url, params=params)
         elif file:
-            files: Dict[str, Any] = {
-                "upfile": file if isinstance(file, bytes) else open(file, "rb")
+            files = {
+                "encoded_image": file if isinstance(file, bytes) else open(file, "rb")
             }
-            resp_text, resp_url, _ = await self.post(
-                self.url, params=params, data={"prg": 1}, files=files
-            )
+            resp = await self.post(f"{self.url}/upload", data=params, files=files)
         else:
             raise ValueError("url or file is required")
-
-        return YandexResponse(resp_text, resp_url)
+        return GoogleResponse(resp.text, resp.url)
```

### Comparing `picimagesearch-3.9.3/README.md` & `picimagesearch-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.3/pyproject.toml` & `picimagesearch-3.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PicImageSearch"
-version = "3.9.3"
+version = "3.9.4"
 description = "PicImageSearch APIs for Python 3.x 适用于 Python 3 以图搜源整合API"
 authors = ["kitUIN <kulujun@gmail.com>"]
 maintainers = ["kitUIN <kulujun@gmail.com>", "lleans", "chinoll", "NekoAria"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "PicImageSearch" }
```

### Comparing `picimagesearch-3.9.3/PKG-INFO` & `picimagesearch-3.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picimagesearch
-Version: 3.9.3
+Version: 3.9.4
 Summary: PicImageSearch APIs for Python 3.x 适用于 Python 3 以图搜源整合API
 Home-page: https://github.com/kitUIN/PicImageSearch
 License: MIT
 Keywords: ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex
 Author: kitUIN
 Author-email: kulujun@gmail.com
 Maintainer: kitUIN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: picimagesearch Version: 3.9.3 Summary:
+Metadata-Version: 2.1 Name: picimagesearch Version: 3.9.4 Summary:
 PicImageSearch APIs for Python 3.x éç¨äº Python 3 ä»¥å¾ææºæ´åAPI
 Home-page: https://github.com/kitUIN/PicImageSearch License: MIT Keywords:
 ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex Author: kitUIN
 Author-email: kulujun@gmail.com Maintainer: kitUIN Maintainer-email:
 kulujun@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

