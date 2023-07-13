# Comparing `tmp/sockslib-1.7.3.tar.gz` & `tmp/sockslib-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockslib-1.7.3.tar", last modified: Thu May  5 04:10:26 2022, max compression
+gzip compressed data, was "sockslib-1.7.4.tar", last modified: Thu Jul 13 15:25:09 2023, max compression
```

## Comparing `sockslib-1.7.3.tar` & `sockslib-1.7.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0 jack       (501) staff       (20)        0 2022-05-05 04:10:26.000000 sockslib-1.7.3/
--rwxrwxrwx   0 jack       (501) staff       (20)     1076 2021-09-02 04:44:18.000000 sockslib-1.7.3/LICENSE
--rwxrwxrwx   0 jack       (501) staff       (20)       19 2021-07-16 03:08:32.000000 sockslib-1.7.3/MANIFEST.in
--rwxrwxrwx   0 jack       (501) staff       (20)     6820 2022-05-05 04:10:26.000000 sockslib-1.7.3/PKG-INFO
--rwxrwxrwx   0 jack       (501) staff       (20)     6388 2021-09-02 01:30:06.000000 sockslib-1.7.3/README.md
--rwxrwxrwx   0 jack       (501) staff       (20)       38 2022-05-05 04:10:26.000000 sockslib-1.7.3/setup.cfg
--rwxrwxrwx   0 jack       (501) staff       (20)      816 2022-05-05 04:02:44.000000 sockslib-1.7.3/setup.py
-drwxrwxrwx   0 jack       (501) staff       (20)        0 2022-05-05 04:10:26.000000 sockslib-1.7.3/sockslib/
--rwxrwxrwx   0 jack       (501) staff       (20)       85 2022-05-05 03:53:42.000000 sockslib-1.7.3/sockslib/__init__.py
--rwxrwxrwx   0 jack       (501) staff       (20)    12928 2022-05-05 03:59:48.000000 sockslib-1.7.3/sockslib/socks.py
--rwxrwxrwx   0 jack       (501) staff       (20)      948 2022-05-05 04:01:32.000000 sockslib-1.7.3/sockslib/socksauth.py
-drwxrwxrwx   0 jack       (501) staff       (20)        0 2022-05-05 04:10:26.000000 sockslib-1.7.3/sockslib.egg-info/
--rwxrwxrwx   0 jack       (501) staff       (20)     6820 2022-05-05 04:10:24.000000 sockslib-1.7.3/sockslib.egg-info/PKG-INFO
--rwxrwxrwx   0 jack       (501) staff       (20)      227 2022-05-05 04:10:26.000000 sockslib-1.7.3/sockslib.egg-info/SOURCES.txt
--rwxrwxrwx   0 jack       (501) staff       (20)        1 2022-05-05 04:10:24.000000 sockslib-1.7.3/sockslib.egg-info/dependency_links.txt
--rwxrwxrwx   0 jack       (501) staff       (20)        9 2022-05-05 04:10:26.000000 sockslib-1.7.3/sockslib.egg-info/top_level.txt
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 15:25:09.021764 sockslib-1.7.4/
+-rw-r--r--   0 coyote     (501) staff       (20)     1076 2023-07-13 14:22:00.000000 sockslib-1.7.4/LICENSE
+-rw-r--r--   0 coyote     (501) staff       (20)       19 2023-07-13 14:22:00.000000 sockslib-1.7.4/MANIFEST.in
+-rw-r--r--   0 coyote     (501) staff       (20)     7452 2023-07-13 15:25:09.021237 sockslib-1.7.4/PKG-INFO
+-rw-r--r--   0 coyote     (501) staff       (20)     7040 2023-07-13 15:21:23.000000 sockslib-1.7.4/README.md
+-rw-r--r--   0 coyote     (501) staff       (20)       38 2023-07-13 15:25:09.021902 sockslib-1.7.4/setup.cfg
+-rw-r--r--   0 coyote     (501) staff       (20)      816 2023-07-13 15:16:21.000000 sockslib-1.7.4/setup.py
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 15:25:09.016243 sockslib-1.7.4/sockslib/
+-rw-r--r--   0 coyote     (501) staff       (20)       85 2023-07-13 15:16:50.000000 sockslib-1.7.4/sockslib/__init__.py
+-rw-r--r--   0 coyote     (501) staff       (20)    13339 2023-07-13 14:48:46.000000 sockslib-1.7.4/sockslib/socks.py
+-rw-r--r--   0 coyote     (501) staff       (20)      948 2023-07-13 14:22:00.000000 sockslib-1.7.4/sockslib/socksauth.py
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 15:25:09.018536 sockslib-1.7.4/sockslib.egg-info/
+-rw-r--r--   0 coyote     (501) staff       (20)     7452 2023-07-13 15:25:08.000000 sockslib-1.7.4/sockslib.egg-info/PKG-INFO
+-rw-r--r--   0 coyote     (501) staff       (20)      272 2023-07-13 15:25:09.000000 sockslib-1.7.4/sockslib.egg-info/SOURCES.txt
+-rw-r--r--   0 coyote     (501) staff       (20)        1 2023-07-13 15:25:08.000000 sockslib-1.7.4/sockslib.egg-info/dependency_links.txt
+-rw-r--r--   0 coyote     (501) staff       (20)        9 2023-07-13 15:25:08.000000 sockslib-1.7.4/sockslib.egg-info/top_level.txt
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 15:25:09.019997 sockslib-1.7.4/tests/
+-rw-r--r--   0 coyote     (501) staff       (20)     2999 2023-07-13 14:28:50.000000 sockslib-1.7.4/tests/test_socks.py
+-rw-r--r--   0 coyote     (501) staff       (20)     1337 2023-07-13 15:09:21.000000 sockslib-1.7.4/tests/test_socks_ipv6.py
```

### Comparing `sockslib-1.7.3/LICENSE` & `sockslib-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sockslib-1.7.3/PKG-INFO` & `sockslib-1.7.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sockslib
-Version: 1.7.3
-Summary: Simple Socks proxy library
-Home-page: https://github.com/woo200/sockslib
-Author: Jack Woo
-Author-email: woo.jack.06@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SocksLib
 
 Sockslib is a library designed to make the usage of socks proxies as easy as possible.
 This library can connect to proxies, authenticate, and then have the use of a normal python socket.
 
 ![Downloads](https://pepy.tech/badge/sockslib)  [![PyPI version fury.io](https://badge.fury.io/py/sockslib.svg)](https://pypi.python.org/pypi/sockslib/)
 
@@ -34,14 +19,15 @@
 
 ### Index
  1. [Intro](#intro)
     1. [Creating a socket](#creating-a-new-socket)
     2. [Setting the proxy](#setting-a-proxy)
     3. [Set the default proxy](#set-a-default-proxy)
     4. [URLLib proxied](#urllib-proxied)
+    5. [IPv6](#ipv6)
  2. [SOCKS5](#socks5)
     1. [TCP](#socks5-tcp)
     2. [UDP](#socks5-udp)
     3. [Using Other Authentication Methods](#using-other-authentication-methods)
     4. [Implementing Your Own Authentication Methods](#implementing-your-own-authentication-methods)
  3. [SOCKS4](#socks4)
     1. [No Authentication](#socks4)
@@ -82,14 +68,29 @@
 sockslib.set_default_proxy(('127.0.0.1', 9050)) # Set the default proxy
 socket.socket = sockslib.SocksSocket # Make the default socket object a SocksSocket
 
 html = urllib.request.urlopen('https://myexternalip.com/raw').read() # Request the page
 print(html)
 ```
 
+### IPv6
+To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor. 
+Here is an example of connecting to a remote IPv6 proxy:
+```python
+import sockslib
+import socket # import socket for the protocol specifiers 
+
+with sockslib.SocksSocket(ip_protocol=socket.AF_INET6) as sock:
+    sock.set_proxy(('::1', 9050)) # Set proxy
+
+    sock.connect(('myexternalip.com', 80)) # Connect to Server via proxy 
+    sock.sendall(b"GET /raw HTTP/1.1\r\nHost: myexternalip.com\r\n\r\n") # Send HTTP Request
+    print(sock.recv(1024)) # Print response
+```
+
 ## Examples
 
 ### SOCKS5
 
 ### Socks5 TCP
 This is an example usage that connects to a Socks5 proxy at `127.0.0.1:9050` and then requests the page http://myexternalip.com/raw
 ```python
@@ -189,9 +190,7 @@
 
 `pip3 install sockslib`
 
 ### Issues
 
 If you have any issues with this project please feel free to open a new issue on github
 https://github.com/woo200/sockslib/issues
-
-
```

### Comparing `sockslib-1.7.3/README.md` & `sockslib-1.7.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: sockslib
+Version: 1.7.4
+Summary: Simple Socks proxy library
+Home-page: https://github.com/woo200/sockslib
+Author: Jack Woo
+Author-email: woo.jack.06@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SocksLib
 
 Sockslib is a library designed to make the usage of socks proxies as easy as possible.
 This library can connect to proxies, authenticate, and then have the use of a normal python socket.
 
 ![Downloads](https://pepy.tech/badge/sockslib)  [![PyPI version fury.io](https://badge.fury.io/py/sockslib.svg)](https://pypi.python.org/pypi/sockslib/)
 
@@ -19,14 +33,15 @@
 
 ### Index
  1. [Intro](#intro)
     1. [Creating a socket](#creating-a-new-socket)
     2. [Setting the proxy](#setting-a-proxy)
     3. [Set the default proxy](#set-a-default-proxy)
     4. [URLLib proxied](#urllib-proxied)
+    5. [IPv6](#ipv6)
  2. [SOCKS5](#socks5)
     1. [TCP](#socks5-tcp)
     2. [UDP](#socks5-udp)
     3. [Using Other Authentication Methods](#using-other-authentication-methods)
     4. [Implementing Your Own Authentication Methods](#implementing-your-own-authentication-methods)
  3. [SOCKS4](#socks4)
     1. [No Authentication](#socks4)
@@ -67,14 +82,29 @@
 sockslib.set_default_proxy(('127.0.0.1', 9050)) # Set the default proxy
 socket.socket = sockslib.SocksSocket # Make the default socket object a SocksSocket
 
 html = urllib.request.urlopen('https://myexternalip.com/raw').read() # Request the page
 print(html)
 ```
 
+### IPv6
+To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor. 
+Here is an example of connecting to a remote IPv6 proxy:
+```python
+import sockslib
+import socket # import socket for the protocol specifiers 
+
+with sockslib.SocksSocket(ip_protocol=socket.AF_INET6) as sock:
+    sock.set_proxy(('::1', 9050)) # Set proxy
+
+    sock.connect(('myexternalip.com', 80)) # Connect to Server via proxy 
+    sock.sendall(b"GET /raw HTTP/1.1\r\nHost: myexternalip.com\r\n\r\n") # Send HTTP Request
+    print(sock.recv(1024)) # Print response
+```
+
 ## Examples
 
 ### SOCKS5
 
 ### Socks5 TCP
 This is an example usage that connects to a Socks5 proxy at `127.0.0.1:9050` and then requests the page http://myexternalip.com/raw
 ```python
```

### Comparing `sockslib-1.7.3/setup.py` & `sockslib-1.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="sockslib",
-    version="1.7.3",
+    version="1.7.4",
     description="Simple Socks proxy library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/woo200/sockslib",
     author="Jack Woo",
     author_email="woo.jack.06@gmail.com",
     license="MIT",
```

### Comparing `sockslib-1.7.3/sockslib/socks.py` & `sockslib-1.7.4/sockslib/socks.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,19 +166,25 @@
 
 class SocksSocket(socket.socket):
     def __init__(self, *args, **kwargs):
         global default_proxy, default_proxy_auth, default_proxy_type
         defaults = {
             "udp": False,
             "socketobject": None,
-            "debug": False
+            "debug": False,
+            "ip_version": socket.AF_INET
         }
         kwargs = {**defaults, **kwargs}
 
-        super().__init__(socket.AF_INET, socket.SOCK_STREAM)
+        self.ip_version = kwargs["ip_version"]
+        # validate ip version
+        if self.ip_version not in [socket.AF_INET, socket.AF_INET6]:
+            raise ValueError("Invalid IP Version provided (AF_INET or AF_INET6 required)")
+
+        super().__init__(self.ip_version, socket.SOCK_STREAM)
 
         self.proxy = default_proxy
         self.udp = kwargs["udp"]
         self.auth = default_proxy_auth
         self.socktype = default_proxy_type
         self.socketobject = kwargs["socketobject"]
         self.debug = kwargs["debug"]
@@ -379,32 +385,35 @@
 
         self.udpbind = (dstip, dstport)
 
     def initudp(self):
         if not self.udp:
             raise SocksException("Cannot initialize UDP proxy connection on TCP socket. Please see docs for proper UDP socket use.")
 
-        self.udpsocket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.udpsocket = socket.socket(self.ip_version, socket.SOCK_DGRAM)
         # self.udpsocket.bind(('', ))
         self.connect(None)
 
     def connect(self, hp):
         if self.udp and hp is not None:
             raise SocksException("Cannot initialize TCP proxy connection on UDP socket. Please see docs for proper TCP socket use.")
 
         if self.proxy is None:
             raise SocksException("No proxy selected")
 
         if self.debug:
             print(f"[DEBUG/INFO] Connecting to proxy: {self.proxy}")
 
-        if self.socketobject is not None:
-            self.socketobject.connect(self.proxy)
-        else:
-            super().connect(self.proxy)
+        try:
+            if self.socketobject is not None:
+                self.socketobject.connect(self.proxy)
+            else:
+                super().connect(self.proxy)
+        except Exception as e:
+            raise SocksException(f"Failed to connect to proxy: {e}")
 
         if self.debug:
             print("[DEBUG/INFO] Connected, Handshaking...")
 
         if self.socktype == Socks.SOCKS5:
             self.__handshake_5(hp, self.auth)
         elif self.socktype == Socks.SOCKS4:
```

### Comparing `sockslib-1.7.3/sockslib/socksauth.py` & `sockslib-1.7.4/sockslib/socksauth.py`

 * *Files identical despite different names*

### Comparing `sockslib-1.7.3/sockslib.egg-info/PKG-INFO` & `sockslib-1.7.4/sockslib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sockslib
-Version: 1.7.3
+Version: 1.7.4
 Summary: Simple Socks proxy library
 Home-page: https://github.com/woo200/sockslib
 Author: Jack Woo
 Author-email: woo.jack.06@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SocksLib
@@ -34,14 +33,15 @@
 
 ### Index
  1. [Intro](#intro)
     1. [Creating a socket](#creating-a-new-socket)
     2. [Setting the proxy](#setting-a-proxy)
     3. [Set the default proxy](#set-a-default-proxy)
     4. [URLLib proxied](#urllib-proxied)
+    5. [IPv6](#ipv6)
  2. [SOCKS5](#socks5)
     1. [TCP](#socks5-tcp)
     2. [UDP](#socks5-udp)
     3. [Using Other Authentication Methods](#using-other-authentication-methods)
     4. [Implementing Your Own Authentication Methods](#implementing-your-own-authentication-methods)
  3. [SOCKS4](#socks4)
     1. [No Authentication](#socks4)
@@ -82,14 +82,29 @@
 sockslib.set_default_proxy(('127.0.0.1', 9050)) # Set the default proxy
 socket.socket = sockslib.SocksSocket # Make the default socket object a SocksSocket
 
 html = urllib.request.urlopen('https://myexternalip.com/raw').read() # Request the page
 print(html)
 ```
 
+### IPv6
+To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor. 
+Here is an example of connecting to a remote IPv6 proxy:
+```python
+import sockslib
+import socket # import socket for the protocol specifiers 
+
+with sockslib.SocksSocket(ip_protocol=socket.AF_INET6) as sock:
+    sock.set_proxy(('::1', 9050)) # Set proxy
+
+    sock.connect(('myexternalip.com', 80)) # Connect to Server via proxy 
+    sock.sendall(b"GET /raw HTTP/1.1\r\nHost: myexternalip.com\r\n\r\n") # Send HTTP Request
+    print(sock.recv(1024)) # Print response
+```
+
 ## Examples
 
 ### SOCKS5
 
 ### Socks5 TCP
 This is an example usage that connects to a Socks5 proxy at `127.0.0.1:9050` and then requests the page http://myexternalip.com/raw
 ```python
@@ -189,9 +204,7 @@
 
 `pip3 install sockslib`
 
 ### Issues
 
 If you have any issues with this project please feel free to open a new issue on github
 https://github.com/woo200/sockslib/issues
-
-
```

