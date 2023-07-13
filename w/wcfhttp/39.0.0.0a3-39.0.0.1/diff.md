# Comparing `tmp/wcfhttp-39.0.0.0a3.tar.gz` & `tmp/wcfhttp-39.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-39.0.0.0a3.tar", last modified: Wed Jul 12 15:08:07 2023, max compression
+gzip compressed data, was "wcfhttp-39.0.0.1.tar", last modified: Thu Jul 13 16:19:43 2023, max compression
```

## Comparing `wcfhttp-39.0.0.0a3.tar` & `wcfhttp-39.0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:08:07.855589 wcfhttp-39.0.0.0a3/
--rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     1830 2023-07-12 15:08:07.854591 wcfhttp-39.0.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 15:08:07.855589 wcfhttp-39.0.0.0a3/setup.cfg
--rw-rw-rw-   0        0        0     1423 2023-07-12 15:07:53.000000 wcfhttp-39.0.0.0a3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:08:07.837591 wcfhttp-39.0.0.0a3/wcfhttp/
--rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a3/wcfhttp/__init__.py
--rw-rw-rw-   0        0        0    14705 2023-07-12 15:08:00.000000 wcfhttp-39.0.0.0a3/wcfhttp/core.py
--rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a3/wcfhttp/main.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:08:07.851588 wcfhttp-39.0.0.0a3/wcfhttp.egg-info/
--rw-rw-rw-   0        0        0     1830 2023-07-12 15:08:07.000000 wcfhttp-39.0.0.0a3/wcfhttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-12 15:08:07.000000 wcfhttp-39.0.0.0a3/wcfhttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:08:07.000000 wcfhttp-39.0.0.0a3/wcfhttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-12 15:08:07.000000 wcfhttp-39.0.0.0a3/wcfhttp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-07-12 15:08:07.000000 wcfhttp-39.0.0.0a3/wcfhttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 15:08:07.000000 wcfhttp-39.0.0.0a3/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 16:19:43.734645 wcfhttp-39.0.0.1/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1828 2023-07-13 16:19:43.734645 wcfhttp-39.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-13 16:19:43.734645 wcfhttp-39.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2023-07-13 15:41:43.000000 wcfhttp-39.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:19:43.719024 wcfhttp-39.0.0.1/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.1/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    15462 2023-07-13 16:18:20.000000 wcfhttp-39.0.0.1/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.1/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:19:43.719024 wcfhttp-39.0.0.1/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1828 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-39.0.0.0a3/PKG-INFO` & `wcfhttp-39.0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 39.0.0.0a3
+Version: 39.0.0.1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

### Comparing `wcfhttp-39.0.0.0a3/setup.py` & `wcfhttp-39.0.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             'wcfhttp=wcfhttp.main:main'
         ]
     },
     install_requires=[
         "setuptools",
         "fastapi",
         "uvicorn[standard]",
-        "wcferry==39.0.0.0a3",
+        "wcferry>=39.0.0.0",
     ],
     classifiers=[
         "Environment :: Win32 (MS Windows)",
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Topic :: Communications :: Chat",
         "Operating System :: Microsoft :: Windows",
```

### Comparing `wcfhttp-39.0.0.0a3/wcfhttp/core.py` & `wcfhttp-39.0.0.1/wcfhttp/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 import requests
 from fastapi import Body, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "39.0.0.0a3"
+__version__ = "39.0.0.1"
 
 
 class Msg(BaseModel):
     id: str
     type: int
     xml: str
     sender: str
@@ -51,14 +51,15 @@
         self.add_api_route("/image", self.send_image, methods=["POST"], summary="发送图片消息")
         self.add_api_route("/file", self.send_file, methods=["POST"], summary="发送文件消息")
         # self.add_api_route("/xml", self.send_xml, methods=["POST"], summary="发送 XML 消息")
         # self.add_api_route("/emotion", self.send_emotion, methods=["POST"], summary="发送表情消息")
         self.add_api_route("/sql", self.query_sql, methods=["POST"], summary="执行 SQL，如果数据量大注意分页，以免 OOM")
         self.add_api_route("/new-friend", self.accept_new_friend, methods=["POST"], summary="通过好友申请")
         self.add_api_route("/chatroom-member", self.add_chatroom_members, methods=["POST"], summary="添加群成员")
+        self.add_api_route("/chatroom-member", self.del_chatroom_members, methods=["DELETE"], summary="删除群成员")
         self.add_api_route("/transfer", self.receive_transfer, methods=["POST"], summary="接收转账")
         self.add_api_route("/dec-image", self.decrypt_image, methods=["POST"], summary="解密图片")
 
     def _set_cb(self, cb):
         def callback(msg: WxMsg):
             data = {}
             data["id"] = msg.id
@@ -152,21 +153,21 @@
         """示例回调方法，简单打印消息"""
         print(f"收到消息：{msg}")
         return {"status": 0, "message": "成功"}
 
     def send_text(
             self, msg: str = Body(description="要发送的消息，换行用\\n表示"),
             receiver: str = Body("filehelper", description="消息接收者，roomid 或者 wxid"),
-            aters: str = Body("", description="要 @ 的 wxid，多个用逗号分隔；@所有人 用 nofity@all")) -> dict:
+            aters: str = Body("", description="要 @ 的 wxid，多个用逗号分隔；@所有人 用 notify@all")) -> dict:
         """发送文本消息，可参考：https://github.com/lich0821/WeChatRobot/blob/master/robot.py 里 sendTextMsg
 
         Args:
             msg (str): 要发送的消息，换行使用 `\\n`；如果 @ 人的话，需要带上跟 `aters` 里数量相同的 @
             receiver (str): 消息接收人，wxid 或者 roomid
-            aters (str): 要 @ 的 wxid，多个用逗号分隔；`@所有人` 只需要 `nofity@all`
+            aters (str): 要 @ 的 wxid，多个用逗号分隔；`@所有人` 只需要 `notify@all`
 
         Returns:
             int: 0 为成功，其他失败
         """
         ret = self.wcf.send_text(msg, receiver, aters)
         return {"status": ret, "message": "成功"if ret == 0 else "失败"}
 
@@ -287,14 +288,29 @@
 
         Returns:
             int: 1 为成功，其他失败
         """
         ret = self.wcf.add_chatroom_members(roomid, wxids)
         return {"status": ret, "message": "成功"if ret == 1 else "失败"}
 
+    def del_chatroom_members(self,
+                             roomid: str = Body("xxxxxxxx@chatroom", description="群的 id"),
+                             wxids: str = Body("wxid_xxxxxxxxxxxxx", description="要删除的 wxid，多个用逗号分隔")) -> dict:
+        """删除群成员
+
+        Args:
+            roomid (str): 群的 id
+            wxids (str): 要删除的 wxid，多个用逗号分隔
+
+        Returns:
+            int: 1 为成功，其他失败
+        """
+        ret = self.wcf.del_chatroom_members(roomid, wxids)
+        return {"status": ret, "message": "成功"if ret == 1 else "失败"}
+
     def receive_transfer(self,
                          wxid: str = Body("wxid_xxxxxxxxxxxxx", description="转账消息里的发送人 wxid"),
                          transferid: str = Body("transferid", description="转账消息里的 transferid"),
                          transactionid: str = Body("transactionid", description="转账消息里的 transactionid")) -> dict:
         """接收转账
 
         Args:
```

### Comparing `wcfhttp-39.0.0.0a3/wcfhttp/main.py` & `wcfhttp-39.0.0.1/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-39.0.0.0a3/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-39.0.0.1/wcfhttp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 39.0.0.0a3
+Version: 39.0.0.1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

