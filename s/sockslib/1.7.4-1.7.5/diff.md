# Comparing `tmp/sockslib-1.7.4.tar.gz` & `tmp/sockslib-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockslib-1.7.4.tar", last modified: Thu Jul 13 15:25:09 2023, max compression
+gzip compressed data, was "sockslib-1.7.5.tar", last modified: Thu Jul 13 16:24:16 2023, max compression
```

## Comparing `sockslib-1.7.4.tar` & `sockslib-1.7.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 15:25:09.021764 sockslib-1.7.4/
--rw-r--r--   0 coyote     (501) staff       (20)     1076 2023-07-13 14:22:00.000000 sockslib-1.7.4/LICENSE
--rw-r--r--   0 coyote     (501) staff       (20)       19 2023-07-13 14:22:00.000000 sockslib-1.7.4/MANIFEST.in
--rw-r--r--   0 coyote     (501) staff       (20)     7452 2023-07-13 15:25:09.021237 sockslib-1.7.4/PKG-INFO
--rw-r--r--   0 coyote     (501) staff       (20)     7040 2023-07-13 15:21:23.000000 sockslib-1.7.4/README.md
--rw-r--r--   0 coyote     (501) staff       (20)       38 2023-07-13 15:25:09.021902 sockslib-1.7.4/setup.cfg
--rw-r--r--   0 coyote     (501) staff       (20)      816 2023-07-13 15:16:21.000000 sockslib-1.7.4/setup.py
-drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 15:25:09.016243 sockslib-1.7.4/sockslib/
--rw-r--r--   0 coyote     (501) staff       (20)       85 2023-07-13 15:16:50.000000 sockslib-1.7.4/sockslib/__init__.py
--rw-r--r--   0 coyote     (501) staff       (20)    13339 2023-07-13 14:48:46.000000 sockslib-1.7.4/sockslib/socks.py
--rw-r--r--   0 coyote     (501) staff       (20)      948 2023-07-13 14:22:00.000000 sockslib-1.7.4/sockslib/socksauth.py
-drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 15:25:09.018536 sockslib-1.7.4/sockslib.egg-info/
--rw-r--r--   0 coyote     (501) staff       (20)     7452 2023-07-13 15:25:08.000000 sockslib-1.7.4/sockslib.egg-info/PKG-INFO
--rw-r--r--   0 coyote     (501) staff       (20)      272 2023-07-13 15:25:09.000000 sockslib-1.7.4/sockslib.egg-info/SOURCES.txt
--rw-r--r--   0 coyote     (501) staff       (20)        1 2023-07-13 15:25:08.000000 sockslib-1.7.4/sockslib.egg-info/dependency_links.txt
--rw-r--r--   0 coyote     (501) staff       (20)        9 2023-07-13 15:25:08.000000 sockslib-1.7.4/sockslib.egg-info/top_level.txt
-drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 15:25:09.019997 sockslib-1.7.4/tests/
--rw-r--r--   0 coyote     (501) staff       (20)     2999 2023-07-13 14:28:50.000000 sockslib-1.7.4/tests/test_socks.py
--rw-r--r--   0 coyote     (501) staff       (20)     1337 2023-07-13 15:09:21.000000 sockslib-1.7.4/tests/test_socks_ipv6.py
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 16:24:16.554312 sockslib-1.7.5/
+-rw-r--r--   0 coyote     (501) staff       (20)     1076 2023-07-13 14:22:00.000000 sockslib-1.7.5/LICENSE
+-rw-r--r--   0 coyote     (501) staff       (20)       19 2023-07-13 14:22:00.000000 sockslib-1.7.5/MANIFEST.in
+-rw-r--r--   0 coyote     (501) staff       (20)     7518 2023-07-13 16:24:16.553825 sockslib-1.7.5/PKG-INFO
+-rw-r--r--   0 coyote     (501) staff       (20)     7106 2023-07-13 16:07:19.000000 sockslib-1.7.5/README.md
+-rw-r--r--   0 coyote     (501) staff       (20)       38 2023-07-13 16:24:16.554466 sockslib-1.7.5/setup.cfg
+-rw-r--r--   0 coyote     (501) staff       (20)      816 2023-07-13 16:18:09.000000 sockslib-1.7.5/setup.py
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 16:24:16.548996 sockslib-1.7.5/sockslib/
+-rw-r--r--   0 coyote     (501) staff       (20)       85 2023-07-13 16:17:57.000000 sockslib-1.7.5/sockslib/__init__.py
+-rw-r--r--   0 coyote     (501) staff       (20)    13617 2023-07-13 16:14:14.000000 sockslib-1.7.5/sockslib/socks.py
+-rw-r--r--   0 coyote     (501) staff       (20)      948 2023-07-13 14:22:00.000000 sockslib-1.7.5/sockslib/socksauth.py
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 16:24:16.551027 sockslib-1.7.5/sockslib.egg-info/
+-rw-r--r--   0 coyote     (501) staff       (20)     7518 2023-07-13 16:24:16.000000 sockslib-1.7.5/sockslib.egg-info/PKG-INFO
+-rw-r--r--   0 coyote     (501) staff       (20)      272 2023-07-13 16:24:16.000000 sockslib-1.7.5/sockslib.egg-info/SOURCES.txt
+-rw-r--r--   0 coyote     (501) staff       (20)        1 2023-07-13 16:24:16.000000 sockslib-1.7.5/sockslib.egg-info/dependency_links.txt
+-rw-r--r--   0 coyote     (501) staff       (20)        9 2023-07-13 16:24:16.000000 sockslib-1.7.5/sockslib.egg-info/top_level.txt
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 16:24:16.552678 sockslib-1.7.5/tests/
+-rw-r--r--   0 coyote     (501) staff       (20)     2999 2023-07-13 16:07:39.000000 sockslib-1.7.5/tests/test_socks.py
+-rw-r--r--   0 coyote     (501) staff       (20)     1337 2023-07-13 15:09:21.000000 sockslib-1.7.5/tests/test_socks_ipv6.py
```

### Comparing `sockslib-1.7.4/LICENSE` & `sockslib-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sockslib-1.7.4/PKG-INFO` & `sockslib-1.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockslib
-Version: 1.7.4
+Version: 1.7.5
 Summary: Simple Socks proxy library
 Home-page: https://github.com/woo200/sockslib
 Author: Jack Woo
 Author-email: woo.jack.06@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -64,14 +64,15 @@
 
 #### Set a default proxy
 Default proxies can be useful for situations when other libraries use sockets to communicate and you want to force that library to use a proxy instead of a direct connection
 ```python
 sockslib.set_default_proxy(
 	('127.0.0.1', 0),      # Ip, Port
 	sockslib.Socks.SOCKS5, # SOCKS5/SOCKS4, (Optional) (Default SOCKS5)
+    socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
 	authentication         # Array of authentication methods (Optional) (Default NoAuth)
 )
 ```
 
 #### URLLib Proxied
 ```python
 import urllib.request
```

### Comparing `sockslib-1.7.4/README.md` & `sockslib-1.7.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 #### Set a default proxy
 Default proxies can be useful for situations when other libraries use sockets to communicate and you want to force that library to use a proxy instead of a direct connection
 ```python
 sockslib.set_default_proxy(
 	('127.0.0.1', 0),      # Ip, Port
 	sockslib.Socks.SOCKS5, # SOCKS5/SOCKS4, (Optional) (Default SOCKS5)
+    socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
 	authentication         # Array of authentication methods (Optional) (Default NoAuth)
 )
 ```
 
 #### URLLib Proxied
 ```python
 import urllib.request
```

### Comparing `sockslib-1.7.4/setup.py` & `sockslib-1.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="sockslib",
-    version="1.7.4",
+    version="1.7.5",
     description="Simple Socks proxy library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/woo200/sockslib",
     author="Jack Woo",
     author_email="woo.jack.06@gmail.com",
     license="MIT",
```

### Comparing `sockslib-1.7.4/sockslib/socks.py` & `sockslib-1.7.5/sockslib/socks.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,24 +162,27 @@
 
     def close(self):
         self.hopper.close()
 
 
 class SocksSocket(socket.socket):
     def __init__(self, *args, **kwargs):
-        global default_proxy, default_proxy_auth, default_proxy_type
+        global default_proxy, default_proxy_auth, default_proxy_type, default_proxy_ip_protocol
         defaults = {
             "udp": False,
             "socketobject": None,
             "debug": False,
             "ip_version": socket.AF_INET
         }
         kwargs = {**defaults, **kwargs}
 
         self.ip_version = kwargs["ip_version"]
+        if default_proxy_ip_protocol is not None:
+            self.ip_version = default_proxy_ip_protocol
+            
         # validate ip version
         if self.ip_version not in [socket.AF_INET, socket.AF_INET6]:
             raise ValueError("Invalid IP Version provided (AF_INET or AF_INET6 required)")
 
         super().__init__(self.ip_version, socket.SOCK_STREAM)
 
         self.proxy = default_proxy
@@ -421,17 +424,19 @@
         else:
             raise SocksException(f"Unknown proxy type {self.socktype}")
 
 
 default_proxy = None
 default_proxy_auth = [NoAuth()]
 default_proxy_type = Socks.SOCKS5
+default_proxy_ip_protocol = None
 
 
-def set_default_proxy(proxy, socktype=Socks.SOCKS5, auth=[NoAuth()]):
+def set_default_proxy(proxy, socktype=Socks.SOCKS5, ip_protocol=socket.AF_INET, auth=[NoAuth()]):
     """
     Set the proxy for all sockssockets to use by default
     """
-    global default_proxy, default_proxy_auth, default_proxy_type
+    global default_proxy, default_proxy_auth, default_proxy_type, default_proxy_ip_protocol
     default_proxy = proxy
     default_proxy_type = socktype
     default_proxy_auth = auth
+    default_proxy_ip_protocol = ip_protocol
```

### Comparing `sockslib-1.7.4/sockslib/socksauth.py` & `sockslib-1.7.5/sockslib/socksauth.py`

 * *Files identical despite different names*

### Comparing `sockslib-1.7.4/sockslib.egg-info/PKG-INFO` & `sockslib-1.7.5/sockslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockslib
-Version: 1.7.4
+Version: 1.7.5
 Summary: Simple Socks proxy library
 Home-page: https://github.com/woo200/sockslib
 Author: Jack Woo
 Author-email: woo.jack.06@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -64,14 +64,15 @@
 
 #### Set a default proxy
 Default proxies can be useful for situations when other libraries use sockets to communicate and you want to force that library to use a proxy instead of a direct connection
 ```python
 sockslib.set_default_proxy(
 	('127.0.0.1', 0),      # Ip, Port
 	sockslib.Socks.SOCKS5, # SOCKS5/SOCKS4, (Optional) (Default SOCKS5)
+    socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
 	authentication         # Array of authentication methods (Optional) (Default NoAuth)
 )
 ```
 
 #### URLLib Proxied
 ```python
 import urllib.request
```

### Comparing `sockslib-1.7.4/tests/test_socks.py` & `sockslib-1.7.5/tests/test_socks.py`

 * *Files identical despite different names*

### Comparing `sockslib-1.7.4/tests/test_socks_ipv6.py` & `sockslib-1.7.5/tests/test_socks_ipv6.py`

 * *Files identical despite different names*

