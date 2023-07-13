# Comparing `tmp/bframe-0.0.8-py3-none-any.whl.zip` & `tmp/bframe-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 20332 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat     1376 b- defN 23-Apr-07 14:46 bframe/__init__.py
--rw-rw-rw-  2.0 fat     5176 b- defN 23-Apr-07 12:56 bframe/_frame.py
+Zip file size: 21039 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat     1376 b- defN 23-Apr-08 03:32 bframe/__init__.py
+-rw-rw-rw-  2.0 fat     6090 b- defN 23-Apr-08 03:28 bframe/_frame.py
 -rw-rw-rw-  2.0 fat     2346 b- defN 23-Apr-06 12:36 bframe/ctx.py
--rw-rw-rw-  2.0 fat     4062 b- defN 23-Apr-07 13:54 bframe/frame.py
+-rw-rw-rw-  2.0 fat     4062 b- defN 23-Apr-08 03:09 bframe/frame.py
 -rw-rw-rw-  2.0 fat     2044 b- defN 23-Apr-07 12:56 bframe/local.py
 -rw-rw-rw-  2.0 fat     2477 b- defN 23-Apr-07 12:56 bframe/logger.py
--rw-rw-rw-  2.0 fat     6855 b- defN 23-Apr-07 14:23 bframe/route.py
+-rw-rw-rw-  2.0 fat     7795 b- defN 23-Apr-08 02:54 bframe/route.py
 -rw-rw-rw-  2.0 fat     3424 b- defN 23-Apr-07 12:56 bframe/server.py
 -rw-rw-rw-  2.0 fat     3118 b- defN 23-Apr-05 12:31 bframe/utils.py
--rw-rw-rw-  2.0 fat     7220 b- defN 23-Apr-07 14:15 bframe/wrappers.py
+-rw-rw-rw-  2.0 fat     7221 b- defN 23-Apr-07 16:00 bframe/wrappers.py
 -rw-rw-rw-  2.0 fat     3331 b- defN 23-Apr-07 12:56 bframe/wsgi.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Apr-07 14:49 bframe-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2731 b- defN 23-Apr-07 14:49 bframe-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-07 14:49 bframe-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-07 14:49 bframe-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1178 b- defN 23-Apr-07 14:49 bframe-0.0.8.dist-info/RECORD
-16 files, 46523 bytes uncompressed, 18444 bytes compressed:  60.4%
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Apr-08 03:37 bframe-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2726 b- defN 23-Apr-08 03:37 bframe-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-08 03:37 bframe-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-08 03:37 bframe-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1178 b- defN 23-Apr-08 03:37 bframe-0.0.9.dist-info/RECORD
+16 files, 48373 bytes uncompressed, 19151 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: bframe/wrappers.py
 Comment: 
 
 Filename: bframe/wsgi.py
 Comment: 
 
-Filename: bframe-0.0.8.dist-info/LICENSE
+Filename: bframe-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: bframe-0.0.8.dist-info/METADATA
+Filename: bframe-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: bframe-0.0.8.dist-info/WHEEL
+Filename: bframe-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: bframe-0.0.8.dist-info/top_level.txt
+Filename: bframe-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bframe-0.0.8.dist-info/RECORD
+Filename: bframe-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bframe/__init__.py

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 __all__ = ["request", "g", "Frame", "Redirect", "Logger", "abort", "WSGIProxy"]
 
 from .ctx import g, request
 from .frame import Frame
 from .logger import Logger
```

## bframe/_frame.py

```diff
@@ -18,24 +18,27 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import inspect
+import os
 import threading
 from typing import Callable, Union
 
 from bframe import __version__
+from bframe import request as req
 from bframe.server import HTTP_METHOD
 from bframe.server import Request
 from bframe.server import SimpleHTTPServer, SimpleRequestHandler
 from bframe.logger import Logger as Log
 from bframe.logger import init_logger
 from bframe.route import Tree
+from bframe.utils import abort
 
 MethodSenquenceAlias = Union[tuple, list]
 
 
 class _Frame():
 
     version = "bframe/%s" % __version__
@@ -47,42 +50,48 @@
     # 路由
     RouteMap: Tree = Tree()
     RouteMapLock: threading.Lock = threading.Lock()
 
     # 日志
     Logger: Log = init_logger(__name__)
 
-    def __init__(self, name: str = None) -> None:
+    def __init__(self, name: str = None, static_url="static", static_folder="static"):
         self.app_name = name
         if name is None:
             self.app_name = __name__
+        self.root_path = os.path.dirname(os.path.abspath(self.app_name))
+
+        self.static_url = static_url if static_url.startswith("/") \
+            else "/%s" % static_url
+        self.static_folder = os.path.join(self.root_path, static_folder)
+        self.add_route("%s/<*:x>" % self.static_url, self.static, "GET")
 
     def add_route(self,
                   url: str,
                   func_or_class: Callable,
                   method: MethodSenquenceAlias = None):
         def _add_class_handle(cls):
             meth = [method.lower()
                     for method in HTTP_METHOD if hasattr(cls, method.lower())]
             for m in meth:
-                _url = "%s/%s" % (url, m.upper())
+                _url = "%s/%s" % (m.upper(), url)
                 self.RouteMap.add(_url, getattr(cls(), m))
 
         with self.RouteMapLock:
             _methods = method
             if _methods is None:
                 _methods = ["GET"]
             if not isinstance(_methods, (tuple, list)):
                 _methods = [_methods]
 
             if inspect.isclass(func_or_class):
                 _add_class_handle(func_or_class)
                 return
             for m in _methods:
-                _url = "%s/%s" % (url, m.upper())
+                _url = "%s/%s" % (m.upper(), url)
                 self.RouteMap.add(_url, func_or_class)
 
     def get(self, url: str):
         def wrapper(f):
             self.add_route(url, f, "GET")
             return f
         return wrapper
@@ -107,14 +116,25 @@
 
     def route(self, url: str, method: MethodSenquenceAlias = None):
         def wrapper(f):
             self.add_route(url, f, method)
             return f
         return wrapper
 
+    def static(self, *args, **kwds):
+        try:
+            file_path = req.path[len(self.static_url):].lstrip("/")
+            file_full_path = os.path.join(self.static_folder, file_path)
+            if not (os.path.exists(file_full_path) and os.path.isfile(file_full_path)):
+                return abort(404)
+            with open(file_full_path, "rb") as f:
+                return f.read()
+        except Exception as e:
+            return abort(500)
+
     def run(self, address: str = "127.0.0.1", port: int = 7256):
         self.Logger.info("run mode: no wsgi")
         try:
             if self.Server is None:
                 with self.ServerLock:
                     self.Server = SimpleHTTPServer(server_address=(address, port),  # noqa
                                                    RequestHandlerClass=SimpleRequestHandler,  # noqa
```

## bframe/frame.py

```diff
@@ -37,15 +37,15 @@
 class Frame(_Frame):
 
     before_funs_list = list()
     after_funs_list = list()
     error_funs_dict = dict()
 
     def match_handle(self) -> Callable:
-        url = "%s/%s" % (req.Path, req.Method)
+        url = "%s/%s" % (req.Method, req.Path)
         return self.RouteMap.find(req.set_path_args, url)
 
     def wrapper_response(self, resp: Any) -> Response:
         if isinstance(resp, Response):
             resp.Body = to_bytes(resp.Body)
             return resp
         if isinstance(resp, (str, bytes)):
```

## bframe/route.py

```diff
@@ -17,15 +17,16 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from typing import Callable, List, TypeVar
+import re
+from typing import Callable, List, TypeVar, Union
 
 from bframe.logger import __logger as logger
 
 logger.module = __name__
 
 
 AnyPath = TypeVar('AnyPath', int, str)
@@ -98,30 +99,40 @@
         return node.__find(nodes, n+1)
 
 
 class MatchTree():
 
     def __init__(self):
         """
-        <str:name>
-        <int:pk>
-        <reg:name>
+        <str:name>  # 字符串路径参数
+        <int:pk>    # 数字路径参数
+        <reg:name>  # 正则匹配路径参数
+        <*:name>    # 静态文件
         """
         self.left = "<"
         self.right = ">"
         self.split = ":"
         self.node = None
         self.node_type = None
         self.node_name = None
         self.rule = {
-            "str": str,
-            "int": int,
-            # "reg": "",
+            "str": lambda x : str(x),
+            "int": lambda x: int(x),
+            "reg": self.reg_match,  # 支持命名式正则匹配    eg: /api/<reg:(?P<version>v\d+$)>/users
+            "*": lambda x: str(x),  # 静态文件的支持
         }
 
+    @staticmethod
+    def reg_match(pattern, x):
+        reg = re.compile(pattern)
+        ret = reg.match(x)
+        if not ret:
+            raise
+        return ret.groupdict()
+
     def is_support_match(self, node: str) -> bool:
         """节点是否支持匹配"""
         if node.startswith(self.left) and node.endswith(self.right) and self.split in node:
             self.node = node
             self.initialization()
             if self.node_type not in self.rule.keys():
                 return False
@@ -132,16 +143,24 @@
         """解析node"""
         self.node_type, self.node_name = self.node.removeprefix(self.left).\
             removesuffix(self.right).\
             split(self.split, 1)
 
     def match(self, _node: str):
         """匹配新节点"""
+        is_break = False
+        if self.node_type in ["reg"]:
+            v = self.rule.get(self.node_type)(self.node_name, _node)
+            return True, v, is_break
+
+        if self.node_type in ["*"]:
+            is_break = True
+
         v = self.rule.get(self.node_type)(_node)
-        return True, {self.node_name: v}
+        return True, {self.node_name: v}, is_break
 
 
 class Tree(BaseTree):
 
     def __init__(self, root: str = "", func: Callable = "", children: list = None) -> None:
         super().__init__(root, func, children)
         self.match = False
@@ -154,24 +173,25 @@
     def find(self, call_back: Callable, path: str = "") -> Callable:
         node = self.split_path(path)
         func = self.__match_find(node, call_back)
         if not callable(func):
             raise NoSetControllerException("%s 未配置请求控制器" % "/".join(node))
         return func
 
-    def find_match_node(self, node: str, call_back: Callable = None, open_match=True) -> object:
+    def find_match_node(self, node: str, call_back: Callable = None, open_match=True) -> Union[object, bool]:
         for _node in self.children:
             if open_match and _node.match and self.match_tree.is_support_match(_node.root):
-                status, value = self.match_tree.match(node)
+                # 匹配静态资源 匹配成功直接返回，不再继续匹配
+                status, value, is_break = self.match_tree.match(node)
                 if status and call_back:
                     call_back(**value)
-                    return _node
+                    return _node, is_break
             elif _node.root == node:
-                return _node
-        return None
+                return _node, False
+        return None, False
 
     def __match_add(self, nodes: List[AnyPath], func: Callable, n: int = 0) -> bool:
         if callable(self.__find_conflict(nodes)):
             raise ReqRepeatException("%s 请求配置重复" % "/".join(nodes))
 
         if len(nodes) == n:
             self.func = func
@@ -187,20 +207,22 @@
         return node.__match_add(nodes, func, n+1)
 
     def __find_conflict(self, nodes: List[AnyPath], n: int = 0):
         if len(nodes) == n:
             return self.func
 
         # 查找是否出现相同的匹配树
-        node = self.find_match_node(nodes[n], open_match=False)
+        node, _ = self.find_match_node(nodes[n], open_match=False)
         if not node:
             return ""
         return node.__match_find(nodes, n+1)
 
     def __match_find(self, nodes: List[AnyPath], call_back: Callable, n: int = 0) -> Callable:
         if len(nodes) == n:
             return self.func
 
-        node = self.find_match_node(nodes[n], call_back)
+        node, is_break = self.find_match_node(nodes[n], call_back)
         if not node:
             return ""
+        if is_break:
+            return node.func
         return node.__match_find(nodes, call_back, n+1)
```

## bframe/wrappers.py

```diff
@@ -55,15 +55,15 @@
     Method: str = ""
     Path: str = ""
     Args: dict = {}
     Protoc: str = ""
     Headers: dict = {}
     Body: str = b""
     Data: dict = {}
-    File: dict[str:BaseFile] = {}
+    File: dict[str, BaseFile] = {}
     Path_Args: dict = {}
 
     def __init__(self,
                  method: str = "",
                  path: str = "",
                  protoc: str = "",
                  headers: dict = None):
```

## Comparing `bframe-0.0.8.dist-info/LICENSE` & `bframe-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bframe-0.0.8.dist-info/METADATA` & `bframe-0.0.9.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bframe
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple python web server frame
 Home-page: https://github.com/Bean-jun/bframe
 Author: Bean-jun
 Author-email: 1342104001@qq.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -15,33 +15,33 @@
 License-File: LICENSE
 
 # A simple python web server frame
 
 > `wranning`: same flask, not flask!
 
 
-### use
+# 1. 快速安装使用
 
 ```shell
 pip install bframe -i https://pypi.org/simple
 ```
 
 or 
 
 ```shell
 git clone https://github.com/Bean-jun/bframe.git
 python setup.py install
 ```
 
-### demo
+# 2. 样例demo
 
 -> main.py
 
 
-### web server 自定义协议
+# 3. web server 自定义协议
 
 ```python
 from bframe import request, Redirect
 from bframe import Frame
 
 
 app = Frame(__name__)
@@ -63,15 +63,15 @@
     return request.Headers
 
 
 if __name__ == "__main__":
     app.run(address="0.0.0.0")
 ```
 
-### wsgi支持
+# 4. wsgi支持
 
 若您需要使用wsgi功能的支持，使用`WSGIProxy`类进行包装即可
 
 ```python
 from bframe import request, Redirect
 from bframe import Frame
 
@@ -101,46 +101,50 @@
 
     with make_server('', 7256, WSGIProxy(app)) as httpd:
         print("Serving on port 7256...")
         httpd.serve_forever()
 ```
 
 
-### 添加钩子支持
+# 4. 添加钩子支持
 
 
-1. 定义请求钩子 
+定义请求钩子 
 
-    ```python
-    # 定义请求钩子
-    @app.add_before_handle
-    def before_02():
-        if request.Method == "POST":
-            return "disallow method"
-    ```
-2. 定义响应钩子 
+```python
+# 定义请求钩子
+@app.add_before_handle
+def before_02():
+    if request.Method == "POST":
+        return "disallow method"
+```
+
+定义响应钩子 
 
-    ```python
-    # 定义响应钩子
-    @app.add_after_handle
-    def after_xx(resp: Response):
-        print("resp:", resp.Code)
-        return resp
-    ```
-3. 自定义错误响应 
+```python
+# 定义响应钩子
+@app.add_after_handle
+def after_xx(resp: Response):
+    print("resp:", resp.Code)
+    return resp
+```
+
+自定义错误响应 
+
+```python
+# 自定义错误响应
+@app.add_error_handle(401)
+def err_401():
+    return "401 error"
+```
 
-    ```python
-    # 自定义错误响应
-    @app.add_error_handle(401)
-    def err_401():
-        return "401 error"
-    ```
 
+# 5. 支持重定向
 
-### 支持重定向
+# 6. 支持g变量
 
-### 支持g变量
+# 7. 解析请求体
 
-### 解析请求体
+# 8. 支持路径参数匹配(字符串、数字、正则)
 
-### 支持简易路径参数匹配
+# 9. 支持静态文件
```

## Comparing `bframe-0.0.8.dist-info/RECORD` & `bframe-0.0.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-bframe/__init__.py,sha256=Tc7Z62dMtjUq7wI20DWV8U26itrLwSORjXIPFs-juMw,1376
-bframe/_frame.py,sha256=Qad13K1HgpD3YSGZ9GDK6wO-L2kcixAlXi1hCqh-ccM,5176
+bframe/__init__.py,sha256=ij1kLL5jrVTZUbdXi36cErTb27HWhfHa_ZCeDg_DSTE,1376
+bframe/_frame.py,sha256=qIx_fj4XsEVs2fy8Xd2wSg182TucO_-4G7nQwe8YOyA,6090
 bframe/ctx.py,sha256=FRgJMMJgvIT5HiEAV1WU-HC0Rs6WEAWvet7luh7IAsY,2346
-bframe/frame.py,sha256=vKLg5Mj9_iLsi-tluWpYDFWwJDaD9ykfuc3kVSPxXtQ,4062
+bframe/frame.py,sha256=C9WhKPIbDXDO0uGcpRM9NcBz6MDMbeptzRyqLbEZ4UY,4062
 bframe/local.py,sha256=l6jpZWL_yzKsDFAkwiwdYpD6g6h7wvwXlBaeoLjhL5g,2044
 bframe/logger.py,sha256=vwTaKLsQLzAlPWMcUtuWTmjasz7R5LlHS4sjd-O-f08,2477
-bframe/route.py,sha256=pA_IM2_dnERCbqGk4_N2l4iIpS-xBsu-ULWMm7Jgc8U,6855
+bframe/route.py,sha256=v9o4BYEVLDWAuwPB-uzHYnN865lOnr4tfInIHDA9jjk,7795
 bframe/server.py,sha256=YvX8U9KpHAhhsnTreE3zOUVhsE5SsLDrBP3I6FPNlAI,3424
 bframe/utils.py,sha256=GQgpa9MI3GQnCWvZl-tpB4D8lV1vpCI6bErwotnAx1U,3118
-bframe/wrappers.py,sha256=HvzVZ2HCT9gMTob8rkB7pv-1sOrq6cVFCVhb9q454wM,7220
+bframe/wrappers.py,sha256=T_qXD5hblVeimg8rBj38wd0Gdxq2M_pmL9HPd_BUkRQ,7221
 bframe/wsgi.py,sha256=DLj6GAPkj2pKQ87PsuYF9cVst2bdMCCGeFSxJQAAAog,3331
-bframe-0.0.8.dist-info/LICENSE,sha256=FXr8F6wm6dk9rxduIjT7Ng9MfCPMstiIGjY3VJ6o9zI,1086
-bframe-0.0.8.dist-info/METADATA,sha256=_NgXtCymj8SMjMlIIgW3qXBB3AejDWFKHKVGdlNTqMk,2731
-bframe-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bframe-0.0.8.dist-info/top_level.txt,sha256=PeDbmSXgHToxWfl01ss4qrgm712xSjHxzS5JxkoDeFI,7
-bframe-0.0.8.dist-info/RECORD,,
+bframe-0.0.9.dist-info/LICENSE,sha256=FXr8F6wm6dk9rxduIjT7Ng9MfCPMstiIGjY3VJ6o9zI,1086
+bframe-0.0.9.dist-info/METADATA,sha256=Uv7LwxZHC0HBYmBRwJUn6MVWr7NjvMXxJMt_imOO6s0,2726
+bframe-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bframe-0.0.9.dist-info/top_level.txt,sha256=PeDbmSXgHToxWfl01ss4qrgm712xSjHxzS5JxkoDeFI,7
+bframe-0.0.9.dist-info/RECORD,,
```

