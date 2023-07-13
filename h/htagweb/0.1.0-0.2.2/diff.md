# Comparing `tmp/htagweb-0.1.0.tar.gz` & `tmp/htagweb-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.1.0.tar", max compression
+gzip compressed data, was "htagweb-0.2.2.tar", max compression
```

## Comparing `htagweb-0.1.0.tar` & `htagweb-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-02 14:54:01.041032 htagweb-0.1.0/LICENSE
--rw-r--r--   0        0        0     3028 2023-07-02 14:54:01.041032 htagweb-0.1.0/README.md
--rw-r--r--   0        0        0    11430 2023-07-02 14:54:01.389034 htagweb-0.1.0/htagweb/__init__.py
--rw-r--r--   0        0        0     2519 2023-07-02 14:54:01.041032 htagweb-0.1.0/htagweb/crypto.py
--rw-r--r--   0        0        0    10365 2023-07-02 14:54:01.041032 htagweb-0.1.0/htagweb/manager.py
--rw-r--r--   0        0        0      625 2023-07-02 14:54:01.041032 htagweb-0.1.0/htagweb/shm.py
--rw-r--r--   0        0        0     1085 2023-07-02 14:54:01.389034 htagweb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 htagweb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-13 21:48:51.868659 htagweb-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2985 2023-07-13 21:48:51.868659 htagweb-0.2.2/README.md
+-rw-r--r--   0        0        0     9938 2023-07-13 21:48:52.164664 htagweb-0.2.2/htagweb/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-13 21:48:51.868659 htagweb-0.2.2/htagweb/crypto.py
+-rw-r--r--   0        0        0     3732 2023-07-13 21:48:51.868659 htagweb-0.2.2/htagweb/manager.py
+-rw-r--r--   0        0        0     4695 2023-07-13 21:48:51.868659 htagweb-0.2.2/htagweb/uidprocess.py
+-rw-r--r--   0        0        0     1124 2023-07-13 21:48:52.164664 htagweb-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4187 1970-01-01 00:00:00.000000 htagweb-0.2.2/PKG-INFO
```

### Comparing `htagweb-0.1.0/LICENSE` & `htagweb-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.1.0/README.md` & `htagweb-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,48 +2,47 @@
 
 [![Test](https://github.com/manatlan/htagweb/actions/workflows/on_commit_do_all_unittests.yml/badge.svg)](https://github.com/manatlan/htagweb/actions/workflows/on_commit_do_all_unittests.yml)
 
 <a href="https://pypi.org/project/htagweb/">
     <img src="https://badge.fury.io/py/htagweb.svg?x" alt="Package version">
 </a>
 
-**IMPORTANT**: not compatible with **uvloop** !!!
-
 This "htagweb" module provides two htag's "runners":
 
  * WebServer     : for http only exchanges
  * WebServerWS   : for http/ws exchanges (first rendering is on http)
 
 Theses runners are a lot more complete than the defaults ones (WebHTTP & WebWS, provided nativly with htag)
 If you want to expose your HTag apps on the web : **they are the only real/official solutions**.
 Theses are a lot robust and IRL tested.
 
  * based on [starlette](https://pypi.org/project/starlette/)
- * each htag app is runned in its own process, per user (real isolation!)
+ * compatible with **uvloop** !!!
+ * compatible with multiple gunicorn webworkers !!!
+ * works on gnu/linux or windows !
+ * Each user has its own process (for session, and htag app)
  * real starlette session available (in htag instance, and starlette request)
- * compatible with oauth2 authents ( [authlib](https://pypi.org/project/Authlib/) )
- * works with multiple uvicorn/gunicorn webworkers
+ * compatible with oauth2 authent ( [authlib](https://pypi.org/project/Authlib/) )
  * real process managments (interactions timeout, process expirations, ...)
  * **NOT READY YET** parano mode (can aes encrypt all communications between client & server ... to avoid mitm'proxies)
 
 But be aware : it's production ready (at least, for me). It may not be free of bugs or security holes: USE AT YOUR OWN RISK.
 Htag and this module are youngs, and not widely tested (by experts/hackers). But due to the nature of htag, and theses runners,
 the risk may be minimal (only DoS), stealing datas may not be possible.
 
 The concepts are the same :
 
- - one user can run only one instance(process) of an htag app at one time (like in desktop mode).
- - All user's instances(process) are destroyed, after an inactivity timeout (not like in desktop mode, to preserve healthy of the webserver)
+ - one user can run only one instance of an htag app at one time (like in desktop mode).
+ - All user processes are destroyed, after an inactivity timeout (not like in desktop mode, to preserve healthy of the webserver)
  - the "session" live as long as the server live (may not be a problem on many hosting service (where they shutdown the server after inactivities))
 
 ## Roadmap / futur
 
-- make it uvloop compatible
+- ? replace starlette by fastapi ?
 - better logging !!!!
-- graceful shutdown of the manager
 - more parameters (session size, etc ...)
 - parano mode
 - perhaps a bi-modal version (use ws, and fallback to http when ws com error)
 
 
 ## Examples
```

### Comparing `htagweb-0.1.0/htagweb/__init__.py` & `htagweb-0.2.2/htagweb/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,67 +3,67 @@
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.1.0" # auto updated
-
-try:
-    import uvloop
-    raise Exception("htagweb is not compatible with uvloop, yet")
-except ImportError:
-    pass
+__version__ = "0.2.2" # auto updated
 
 """
 WebServer & WebServerWS
 ~~~~~~~~~~~~~~~~~~~~~~~~
 - new versions of oldest WebHTTP & WebWS (nearly compatibles)
-- concept of an htag app application server (manager), which communicate with child process, with queue (web workers communicate with the manager using tcp socket)
-- Htag App runned in its own process, per user (real isolation!)
-- htag app can exit with .exit() (process killed)
+- concept of an htag app application server (manager), which communicate with child process, with queue
+- Htag Apps runned in a process, per user (real isolation!)
 - when session expire (after inactivity timeout), child process are destroyed
-- real shared session by user (really isolated!)
-- works with multiple uvicorn webworkers
+- works with multiple uvicorn webworkers, and uvloop
 - WebServerWS use ws/wss sockets to interact (instead of http/post)
 - 30s timeout for interactions/render times
-- parano mode (aes encryption in exchanges)
+- TODO: parano mode (aes encryption in exchanges)
 """
 import uvicorn
+import json,os
+from types import ModuleType
+import uuid,logging
+import contextlib
 
 from htag import Tag
-from htag.render import HRenderer
 from htag.runners import commons
 
 from starlette.applications import Starlette
-from starlette.responses import HTMLResponse,JSONResponse,PlainTextResponse
+from starlette.responses import HTMLResponse,PlainTextResponse
 from starlette.routing import Route,WebSocketRoute
 from starlette.endpoints import WebSocketEndpoint
+from starlette.middleware import Middleware
+from starlette.datastructures import MutableHeaders
+from starlette.requests import HTTPConnection
+from starlette.types import ASGIApp, Message, Receive, Scope, Send
 
 #=-=-=-=-=-=-
-from . import shm
 from .manager import Manager
+from .uidprocess import Users
 from .crypto import decrypt,encrypt,JSCRYPTO
 #=-=-=-=-=-=-
 
-import os
-import json
-import asyncio,pickle
-from types import ModuleType
-from datetime import datetime
-
+logger = logging.getLogger(__name__)
 #=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=
-import json
-import sys
-import uuid
 
-from starlette.datastructures import MutableHeaders
-from starlette.requests import HTTPConnection
-from starlette.types import ASGIApp, Message, Receive, Scope, Send
+# python3 -m pytest --cov-report html --cov=htagweb .
+
+
+
+@contextlib.asynccontextmanager
+async def htagweb_life(app):
+    async with Manager() as m:
+        app.state.manager = m
+        pid=os.getpid()
+        logger.info("Startup [%s] %s",pid,m.is_server() and "***MANAGER RUNNED***" or "")
+        yield
+        logger.info("Stopping [%s]",pid)
 
 
 class WebServerSession:  # ASGI Middleware, for starlette
     def __init__(
         self,
         app: ASGIApp,
         https_only: bool = False,
@@ -82,25 +82,23 @@
             return
 
         connection = HTTPConnection(scope)
 
         if self.session_cookie in connection.cookies:
             uid = connection.cookies[self.session_cookie]
         else:
-            uid=str(uuid.uuid4())
+            uid = str(uuid.uuid4())
 
         #!!!!!!!!!!!!!!!!!!!!!!!!!!!
         scope["uid"] = uid
-        scope["session"] = shm.session(uid) # create a smd
-
-        # declare session
-        glob=shm.wses()
-        glob[uid]=datetime.now()
+        scope["session"] = Users.use(uid).session   # CREATE a session if uid not known
         #!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
+        logger.debug("request for %s, scope=%s",uid,scope)
+
         async def send_wrapper(message: Message) -> None:
             if message["type"] == "http.response.start":
                 # send it back, in all cases
                 headers = MutableHeaders(scope=message)
                 header_value = "{session_cookie}={data}; path={path}; {max_age}{security_flags}".format(  # noqa E501
                     session_cookie=self.session_cookie,
                     data=uid,
@@ -109,50 +107,14 @@
                     security_flags=self.security_flags,
                 )
                 headers.append("Set-Cookie", header_value)
             await send(message)
 
         await self.app(scope, receive, send_wrapper)
 
-#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=
-def startManager(port,timeout): #sec (timeout session)
-    try:
-        Manager(port).run(timeout)
-        print("Manager started!")
-    except Exception as e:
-        print("Manager can't started (already running?)")
-#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=
-
-
-class ManagerClient:
-    def __init__(self,port):
-        self.port=port
-
-    def __getattr__(self,name:str):
-        async def _(*a,**k):
-            reader, writer = await asyncio.open_connection("127.0.0.1", self.port)
-
-            question = pickle.dumps( (name,a,k) )
-            # logger.debug('Sending data of size: %s',len(question))
-            writer.write(question)
-
-            await writer.drain()
-            writer.write_eof()
-
-            data = await reader.read()
-            # logger.debug('recept data of size: %s',len(data))
-            reponse = pickle.loads( data )
-            if isinstance(reponse,Exception):
-                raise reponse
-
-            writer.close()
-            await writer.wait_closed()
-            return reponse
-        return _
-
 
 
 
 def findfqn(x) -> str:
     if isinstance(x,str):
         if "." not in x:
             raise Exception(f"'{x}' is not a 'full qualified name' (expected 'module.name') of an App (htag.Tag class)")
@@ -167,52 +129,40 @@
     elif issubclass(x,Tag):
         tagClass=x
     else:
         raise Exception(f"!!! wtf ({x}) ???")
 
     return tagClass.__module__+"."+tagClass.__qualname__
 
+
 class WebBase(Starlette):
 
     def __init__(self,obj=None,timeout=5*60, routes=None):
         # self.crypt="test"   # or None
         self.crypt=None
 
-        port=27777 # manager server port
-        self.manager = ManagerClient(port)
-
-        async def _startManager():
-            import multiprocessing
-            p = multiprocessing.Process(target=startManager,args=(port,timeout,),name="ManagerServer")
-            p.start()
-
-        async def _stopManager():
-            await self.manager.shutdown()
-
-        Starlette.__init__(self,debug=True, on_startup=[_startManager,],on_shutdown=[_stopManager],routes=routes)
+        Starlette.__init__(self,debug=True, lifespan=htagweb_life,routes=routes,middleware=[Middleware(WebServerSession)])
 
         if obj:
             async def handleHome(request):
                 return await self.serve(request,obj)
             self.add_route( '/', handleHome )
 
-        Starlette.add_middleware(self,WebServerSession )
-
 
     def run(self, host="0.0.0.0", port=8000, openBrowser=False):   # localhost, by default !!
         if openBrowser:
             import webbrowser
             webbrowser.open_new_tab(f"http://localhost:{port}")
 
         uvicorn.run(self, host=host, port=port)
 
 
     async def interact(self,uid:str,fqn:str,query:str) -> str:
         data = self._str2dict( query )
-        actions = await self.manager.ht_interact(uid, fqn, data )
+        actions = await self.state.manager.ht_interact(uid,fqn,data)
         if isinstance(actions,dict):
             return self._dict2str( actions )
         else:
             return ""   # manager on dead objects/session
 
     async def render(self,request, uid:str,fqn:str,js:str,renew:bool) -> str:
 
@@ -226,16 +176,15 @@
         else:
             fjs = """
 async function str2dict(s) { return JSON.parse(s); }
 async function dict2str(d) { return JSON.stringify(d); }
             """+js
 
         init_params = commons.url2ak( str(request.url) )
-        html = await self.manager.ht_render(uid,fqn,init_params, fjs, renew )
-
+        html = await request.app.state.manager.ht_create(uid, fqn, fjs, init_params, renew=renew)
         return html
 
     def _dict2str(self,dico:dict) -> str:
         if self.crypt:
             return encrypt( json.dumps(dico).encode() , self.crypt)
         else:
             return json.dumps(dico)
@@ -252,14 +201,15 @@
     """ Like WebHTTP, but a lot better """
     def __init__(self,obj=None, timeout=5*60):
         """ obj can be a module (which contain a 'App' (tagClass)) on a tagClass (like before)"""
         WebBase.__init__(self,obj,timeout,[Route('/{fqn:str}', self.POST, methods=["POST"])] )
 
     async def serve(self,request, obj, renew=False ) -> HTMLResponse:
         # assert obj is correct type
+
         uid=request.scope["uid"]    # WebServerSession made that possible
         fqn=findfqn(obj)
 
         js = """
 async function interact( o ) {
     let q=await dict2str(o);
     let r=await (await window.fetch("/%s",{method:"POST", body:q})).text();
@@ -293,15 +243,14 @@
     """ Like WebWS, but a lot better """
 
     def __init__(self,obj=None, timeout=5*60,wss:bool=False):
         """ obj can be a module (which contain a 'App' (tagClass)) or a tagClass (like before), or a string/fqn"""
         self.wss=wss
 
         class WsInteract(WebSocketEndpoint):
-            # encoding = "json"
             encoding = "text"
 
             async def on_receive(this, websocket, query:str):
                 uid=websocket.scope["uid"]    # WebServerSession made that possible
                 fqn=websocket.query_params['fqn']
 
                 response = await self.interact(uid, fqn, query )
@@ -334,8 +283,7 @@
 """ % (
     "wss" if self.wss else "ws",
     fqn,
 )
         html = await self.render(request,uid,fqn, js,renew )
         return HTMLResponse( html )
 
-
```

### Comparing `htagweb-0.1.0/htagweb/crypto.py` & `htagweb-0.2.2/htagweb/crypto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-# -*- coding: utf-8 -*-
-# #############################################################################
-# Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
-#
-# MIT licence
-#
-# https://github.com/manatlan/htag
-# #############################################################################
-
 from Cryptodome.Cipher import AES # pip3 install pycryptodomex
 import hashlib
 import base64,os
 # https://hackernoon.com/how-to-use-aes-256-cipher-python-cryptography-examples-6tbh37cr
 
 def decrypt(b64:bytes,key:str) -> bytes:   # text
     data=base64.b64decode(b64)
```

### Comparing `htagweb-0.1.0/pyproject.toml` & `htagweb-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.1.0" # auto-updated
+version = "0.2.2" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
@@ -19,17 +19,18 @@
 [tool.poetry.dependencies]
 # https://python-poetry.org/docs/dependency-specification/
 python = "^3.8"
 htag = ">= 0.9.44"
 starlette = ">= 0.21.0"
 uvicorn = ">= 0.22.0"
 pycryptodomex = ">= 3.0.0"
-shared_memory_dict = ">= 0.7.2"
+shared_memory_dict = ">= 0.7.2"         # need py ^3.8
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21"
+httpx = "^0.24"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `htagweb-0.1.0/PKG-INFO` & `htagweb-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.1.0
+Version: 0.2.2
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -31,48 +31,47 @@
 
 [![Test](https://github.com/manatlan/htagweb/actions/workflows/on_commit_do_all_unittests.yml/badge.svg)](https://github.com/manatlan/htagweb/actions/workflows/on_commit_do_all_unittests.yml)
 
 <a href="https://pypi.org/project/htagweb/">
     <img src="https://badge.fury.io/py/htagweb.svg?x" alt="Package version">
 </a>
 
-**IMPORTANT**: not compatible with **uvloop** !!!
-
 This "htagweb" module provides two htag's "runners":
 
  * WebServer     : for http only exchanges
  * WebServerWS   : for http/ws exchanges (first rendering is on http)
 
 Theses runners are a lot more complete than the defaults ones (WebHTTP & WebWS, provided nativly with htag)
 If you want to expose your HTag apps on the web : **they are the only real/official solutions**.
 Theses are a lot robust and IRL tested.
 
  * based on [starlette](https://pypi.org/project/starlette/)
- * each htag app is runned in its own process, per user (real isolation!)
+ * compatible with **uvloop** !!!
+ * compatible with multiple gunicorn webworkers !!!
+ * works on gnu/linux or windows !
+ * Each user has its own process (for session, and htag app)
  * real starlette session available (in htag instance, and starlette request)
- * compatible with oauth2 authents ( [authlib](https://pypi.org/project/Authlib/) )
- * works with multiple uvicorn/gunicorn webworkers
+ * compatible with oauth2 authent ( [authlib](https://pypi.org/project/Authlib/) )
  * real process managments (interactions timeout, process expirations, ...)
  * **NOT READY YET** parano mode (can aes encrypt all communications between client & server ... to avoid mitm'proxies)
 
 But be aware : it's production ready (at least, for me). It may not be free of bugs or security holes: USE AT YOUR OWN RISK.
 Htag and this module are youngs, and not widely tested (by experts/hackers). But due to the nature of htag, and theses runners,
 the risk may be minimal (only DoS), stealing datas may not be possible.
 
 The concepts are the same :
 
- - one user can run only one instance(process) of an htag app at one time (like in desktop mode).
- - All user's instances(process) are destroyed, after an inactivity timeout (not like in desktop mode, to preserve healthy of the webserver)
+ - one user can run only one instance of an htag app at one time (like in desktop mode).
+ - All user processes are destroyed, after an inactivity timeout (not like in desktop mode, to preserve healthy of the webserver)
  - the "session" live as long as the server live (may not be a problem on many hosting service (where they shutdown the server after inactivities))
 
 ## Roadmap / futur
 
-- make it uvloop compatible
+- ? replace starlette by fastapi ?
 - better logging !!!!
-- graceful shutdown of the manager
 - more parameters (session size, etc ...)
 - parano mode
 - perhaps a bi-modal version (use ws, and fallback to http when ws com error)
 
 
 ## Examples
```

