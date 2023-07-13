# Comparing `tmp/sevent-0.4.8.tar.gz` & `tmp/sevent-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sevent-0.4.8.tar", last modified: Sat Jan 22 06:41:46 2022, max compression
+gzip compressed data, was "dist/sevent-0.4.9.tar", last modified: Sun Mar  6 06:28:08 2022, max compression
```

## Comparing `sevent-0.4.8.tar` & `sevent-0.4.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-01-22 06:41:46.992571 sevent-0.4.8/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2020-02-22 03:29:00.000000 sevent-0.4.8/.gitignore
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2022-01-22 06:41:46.990571 sevent-0.4.8/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1787 2021-09-03 10:01:07.000000 sevent-0.4.8/README.md
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-01-22 06:41:46.197283 sevent-0.4.8/example/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      659 2020-02-22 03:29:00.000000 sevent-0.4.8/example/tcpclient.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      660 2020-02-22 03:29:00.000000 sevent-0.4.8/example/tcpserver.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      312 2020-02-22 03:29:00.000000 sevent-0.4.8/example/udpclient.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      285 2020-02-22 03:29:00.000000 sevent-0.4.8/example/udpserver.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)       38 2022-01-22 06:41:46.993567 sevent-0.4.8/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1166 2022-01-22 06:30:52.000000 sevent-0.4.8/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-01-22 06:41:46.415191 sevent-0.4.8/sevent/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      913 2022-01-22 06:30:52.000000 sevent-0.4.8/sevent/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12292 2021-09-03 09:40:16.000000 sevent-0.4.8/sevent/buffer.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    55710 2020-08-19 10:25:15.000000 sevent-0.4.8/sevent/cbuffer.c
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-01-22 06:41:46.693018 sevent-0.4.8/sevent/coroutines/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       56 2021-01-28 06:18:26.000000 sevent-0.4.8/sevent/coroutines/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2015 2021-02-02 12:02:50.000000 sevent-0.4.8/sevent/coroutines/chain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      523 2020-05-09 08:52:07.000000 sevent-0.4.8/sevent/coroutines/dns.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1852 2021-09-09 03:26:24.000000 sevent-0.4.8/sevent/coroutines/event.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3614 2021-09-03 09:40:16.000000 sevent-0.4.8/sevent/coroutines/future.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3041 2021-09-09 04:04:30.000000 sevent-0.4.8/sevent/coroutines/loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11445 2022-01-21 15:47:23.000000 sevent-0.4.8/sevent/coroutines/pipe.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11429 2021-09-03 09:26:02.000000 sevent-0.4.8/sevent/coroutines/tcp.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7764 2021-09-03 09:30:42.000000 sevent-0.4.8/sevent/coroutines/udp.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12153 2021-09-01 06:11:44.000000 sevent-0.4.8/sevent/dns.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      576 2021-02-01 08:30:46.000000 sevent-0.4.8/sevent/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5627 2021-09-03 09:40:16.000000 sevent-0.4.8/sevent/event.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-01-22 06:41:46.881901 sevent-0.4.8/sevent/helpers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       57 2021-02-01 09:08:14.000000 sevent-0.4.8/sevent/helpers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1926 2022-01-22 05:01:29.000000 sevent-0.4.8/sevent/helpers/__main__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11765 2022-01-22 06:29:55.000000 sevent-0.4.8/sevent/helpers/arproxy.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8626 2022-01-22 06:29:40.000000 sevent-0.4.8/sevent/helpers/proxy2proxy.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6922 2022-01-22 05:44:49.000000 sevent-0.4.8/sevent/helpers/redirect2proxy.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6393 2022-01-22 05:44:49.000000 sevent-0.4.8/sevent/helpers/simple_proxy.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9365 2022-01-22 05:44:49.000000 sevent-0.4.8/sevent/helpers/tcp2proxy.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    23980 2022-01-22 05:44:49.000000 sevent-0.4.8/sevent/helpers/tcp_forward.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18429 2022-01-22 05:44:49.000000 sevent-0.4.8/sevent/helpers/tcp_reverse.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2242 2022-01-22 06:11:04.000000 sevent-0.4.8/sevent/helpers/utils.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-01-22 06:41:46.975568 sevent-0.4.8/sevent/impl/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       23 2020-02-22 03:29:00.000000 sevent-0.4.8/sevent/impl/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      657 2020-04-20 14:30:27.000000 sevent-0.4.8/sevent/impl/epoll_loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1608 2020-04-20 14:40:35.000000 sevent-0.4.8/sevent/impl/kqueue_loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1253 2020-04-20 14:30:27.000000 sevent-0.4.8/sevent/impl/select_loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8940 2021-09-03 09:40:16.000000 sevent-0.4.8/sevent/loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12096 2022-01-22 04:46:52.000000 sevent-0.4.8/sevent/pipe.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    28192 2022-01-21 16:14:48.000000 sevent-0.4.8/sevent/tcp.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18119 2022-01-21 15:40:36.000000 sevent-0.4.8/sevent/udp.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      757 2021-09-03 09:40:16.000000 sevent-0.4.8/sevent/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2939 2021-02-25 03:22:35.000000 sevent-0.4.8/sevent/waker.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-01-22 06:41:46.474985 sevent-0.4.8/sevent.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2022-01-22 06:41:45.000000 sevent-0.4.8/sevent.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1081 2022-01-22 06:41:45.000000 sevent-0.4.8/sevent.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-01-22 06:41:45.000000 sevent-0.4.8/sevent.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       30 2022-01-22 06:41:45.000000 sevent-0.4.8/sevent.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       22 2022-01-22 06:41:45.000000 sevent-0.4.8/sevent.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-03-06 06:28:10.805403 sevent-0.4.9/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2020-02-22 03:29:00.000000 sevent-0.4.9/.gitignore
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2022-03-06 06:28:10.805403 sevent-0.4.9/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1787 2021-09-03 10:01:07.000000 sevent-0.4.9/README.md
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-03-06 06:28:09.926492 sevent-0.4.9/example/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      659 2020-02-22 03:29:00.000000 sevent-0.4.9/example/tcpclient.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      660 2020-02-22 03:29:00.000000 sevent-0.4.9/example/tcpserver.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      312 2020-02-22 03:29:00.000000 sevent-0.4.9/example/udpclient.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      285 2020-02-22 03:29:00.000000 sevent-0.4.9/example/udpserver.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       38 2022-03-06 06:28:10.805403 sevent-0.4.9/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1166 2022-03-06 06:27:40.000000 sevent-0.4.9/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-03-06 06:28:10.177338 sevent-0.4.9/sevent/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      913 2022-03-06 06:27:40.000000 sevent-0.4.9/sevent/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12292 2021-09-03 09:40:16.000000 sevent-0.4.9/sevent/buffer.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    55710 2020-08-19 10:25:15.000000 sevent-0.4.9/sevent/cbuffer.c
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-03-06 06:28:10.459838 sevent-0.4.9/sevent/coroutines/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       56 2021-01-28 06:18:26.000000 sevent-0.4.9/sevent/coroutines/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2015 2021-02-02 12:02:50.000000 sevent-0.4.9/sevent/coroutines/chain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      523 2020-05-09 08:52:07.000000 sevent-0.4.9/sevent/coroutines/dns.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1852 2021-09-09 03:26:24.000000 sevent-0.4.9/sevent/coroutines/event.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3614 2021-09-03 09:40:16.000000 sevent-0.4.9/sevent/coroutines/future.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3041 2021-09-09 04:04:30.000000 sevent-0.4.9/sevent/coroutines/loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11445 2022-01-21 15:47:23.000000 sevent-0.4.9/sevent/coroutines/pipe.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11429 2021-09-03 09:26:02.000000 sevent-0.4.9/sevent/coroutines/tcp.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7764 2021-09-03 09:30:42.000000 sevent-0.4.9/sevent/coroutines/udp.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12153 2021-09-01 06:11:44.000000 sevent-0.4.9/sevent/dns.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      576 2021-02-01 08:30:46.000000 sevent-0.4.9/sevent/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5627 2021-09-03 09:40:16.000000 sevent-0.4.9/sevent/event.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-03-06 06:28:10.702719 sevent-0.4.9/sevent/helpers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       57 2021-02-01 09:08:14.000000 sevent-0.4.9/sevent/helpers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1926 2022-01-22 05:01:29.000000 sevent-0.4.9/sevent/helpers/__main__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11765 2022-01-22 06:29:55.000000 sevent-0.4.9/sevent/helpers/arproxy.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8626 2022-01-22 06:29:40.000000 sevent-0.4.9/sevent/helpers/proxy2proxy.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6922 2022-01-22 05:44:49.000000 sevent-0.4.9/sevent/helpers/redirect2proxy.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6393 2022-01-22 05:44:49.000000 sevent-0.4.9/sevent/helpers/simple_proxy.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9365 2022-01-22 05:44:49.000000 sevent-0.4.9/sevent/helpers/tcp2proxy.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    23980 2022-01-22 05:44:49.000000 sevent-0.4.9/sevent/helpers/tcp_forward.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    19386 2022-03-06 06:23:08.000000 sevent-0.4.9/sevent/helpers/tcp_reverse.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2242 2022-01-22 06:11:04.000000 sevent-0.4.9/sevent/helpers/utils.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-03-06 06:28:10.789380 sevent-0.4.9/sevent/impl/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       23 2020-02-22 03:29:00.000000 sevent-0.4.9/sevent/impl/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      657 2020-04-20 14:30:27.000000 sevent-0.4.9/sevent/impl/epoll_loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1608 2020-04-20 14:40:35.000000 sevent-0.4.9/sevent/impl/kqueue_loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1253 2020-04-20 14:30:27.000000 sevent-0.4.9/sevent/impl/select_loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8940 2021-09-03 09:40:16.000000 sevent-0.4.9/sevent/loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12096 2022-01-22 04:46:52.000000 sevent-0.4.9/sevent/pipe.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    28192 2022-01-21 16:14:48.000000 sevent-0.4.9/sevent/tcp.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18119 2022-01-21 15:40:36.000000 sevent-0.4.9/sevent/udp.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      757 2021-09-03 09:40:16.000000 sevent-0.4.9/sevent/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2939 2021-02-25 03:22:35.000000 sevent-0.4.9/sevent/waker.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2022-03-06 06:28:10.240252 sevent-0.4.9/sevent.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2022-03-06 06:28:08.000000 sevent-0.4.9/sevent.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1081 2022-03-06 06:28:09.000000 sevent-0.4.9/sevent.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-03-06 06:28:08.000000 sevent-0.4.9/sevent.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       30 2022-03-06 06:28:08.000000 sevent-0.4.9/sevent.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       22 2022-03-06 06:28:08.000000 sevent-0.4.9/sevent.egg-info/top_level.txt
```

### Comparing `sevent-0.4.8/PKG-INFO` & `sevent-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sevent
-Version: 0.4.8
+Version: 0.4.9
 Summary: lightweight event loop
 Home-page: https://github.com/snower/sevent
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `sevent-0.4.8/README.md` & `sevent-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/example/tcpclient.py` & `sevent-0.4.9/example/tcpclient.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/example/tcpserver.py` & `sevent-0.4.9/example/tcpserver.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/setup.py` & `sevent-0.4.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with open("README.md") as fp:
             long_description = fp.read()
 else:
     long_description = ''
 
 setup(
     name='sevent',
-    version='0.4.8',
+    version='0.4.9',
     packages=['sevent', 'sevent.impl', 'sevent.coroutines', 'sevent.helpers'],
     ext_modules=ext_modules,
     package_data={
         '': ['README.md'],
     },
     install_requires=[
         'dnslib>=0.9.7',
```

### Comparing `sevent-0.4.8/sevent/__init__.py` & `sevent-0.4.9/sevent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
-version = '0.4.8'
-version_info = (0, 4, 8)
+version = '0.4.9'
+version_info = (0, 4, 9)
 
 from .utils import is_py3, set_logger
 from .loop import instance, current
 from .event import EventEmitter
 from . import tcp
 from . import udp
 from . import pipe
```

### Comparing `sevent-0.4.8/sevent/buffer.py` & `sevent-0.4.9/sevent/buffer.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/cbuffer.c` & `sevent-0.4.9/sevent/cbuffer.c`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/coroutines/chain.py` & `sevent-0.4.9/sevent/coroutines/chain.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/coroutines/dns.py` & `sevent-0.4.9/sevent/coroutines/dns.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/coroutines/event.py` & `sevent-0.4.9/sevent/coroutines/event.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/coroutines/future.py` & `sevent-0.4.9/sevent/coroutines/future.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/coroutines/loop.py` & `sevent-0.4.9/sevent/coroutines/loop.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/coroutines/pipe.py` & `sevent-0.4.9/sevent/coroutines/pipe.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/coroutines/tcp.py` & `sevent-0.4.9/sevent/coroutines/tcp.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/coroutines/udp.py` & `sevent-0.4.9/sevent/coroutines/udp.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/dns.py` & `sevent-0.4.9/sevent/dns.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/errors.py` & `sevent-0.4.9/sevent/errors.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/event.py` & `sevent-0.4.9/sevent/event.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/helpers/__main__.py` & `sevent-0.4.9/sevent/helpers/__main__.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/helpers/arproxy.py` & `sevent-0.4.9/sevent/helpers/arproxy.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/helpers/proxy2proxy.py` & `sevent-0.4.9/sevent/helpers/proxy2proxy.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/helpers/redirect2proxy.py` & `sevent-0.4.9/sevent/helpers/redirect2proxy.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/helpers/simple_proxy.py` & `sevent-0.4.9/sevent/helpers/simple_proxy.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/helpers/tcp2proxy.py` & `sevent-0.4.9/sevent/helpers/tcp2proxy.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/helpers/tcp_forward.py` & `sevent-0.4.9/sevent/helpers/tcp_forward.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/helpers/tcp_reverse.py` & `sevent-0.4.9/sevent/helpers/tcp_reverse.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         conns.pop(id(remote_conn), None)
 
     logging.info("tcp forward closed %s:%d -> %s:%d %s %s %.2fms", local_conn.address[0], local_conn.address[1],
                  remote_conn.address[0], remote_conn.address[1], format_data_len(status["send_len"]),
                  format_data_len(status["recv_len"]),
                  (time.time() - start_time) * 1000)
 
-async def handle_remote_connection(conn, forward_address, key, proxy_type, conns, status):
+async def server_handle_remote_connect(conn, forward_address, key, proxy_type, conns, status):
     setattr(conn, "_connected_time", time.time())
     def on_close(conn):
         if conn not in status["remote_conn"]:
             return
         status["remote_conn"].remove(conn)
         logging.info("remote conn waited close %s:%d", conn.address[0], conn.address[1])
 
@@ -176,17 +176,17 @@
             logging.info("tcp forward error %s:%d -> %s:%d %s\r%s", conn.address[0], conn.address[1],
                          forward_address[0], forward_address[1], e, traceback.format_exc())
         return
 
     await conn.closeof()
     logging.info("remote conn unsupport connect type %s:%d %s", conn.address[0], conn.address[1], key)
 
-async def handle_local_connection(conn, forward_address, key, proxy_type, conns, status):
+async def server_handle_local_connect(conn, forward_address, key, proxy_type, conns, status):
     try:
-        forward_address = (await parse_forward_address(conn, proxy_type)) if proxy_type else None
+        forward_address = (await parse_forward_address(conn, proxy_type)) if proxy_type else forward_address
     except Exception as e:
         logging.info("parse proxy forward address error %s", e)
         return
 
     setattr(conn, "_connected_forward_address", forward_address)
     setattr(conn, "_connected_time", time.time())
     if status["remote_conn"]:
@@ -202,49 +202,51 @@
             return
         status["local_conn"].remove(conn)
         logging.info("local conn waited close %s:%d", conn.address[0], conn.address[1])
     status["local_conn"].append(conn)
     conn.on_close(on_close)
     logging.info("local conn waiting %s:%d", conn.address[0], conn.address[1])
 
-async def run_server(server, forward_address, key, proxy_type, conns, status, handle):
+async def server_run_server(server, forward_address, key, proxy_type, conns, status, handle):
     while True:
         try:
             conn = await server.accept()
             sevent.current().call_async(handle, conn, forward_address, key, proxy_type, conns, status)
         except sevent.errors.SocketClosed as e:
             sevent.current().call_async(sevent.current().stop)
             raise e
 
-async def run_connect(remote_address, forward_address, key, conns, status):
+async def client_run_connect(remote_address, forward_address, key, conns, status):
     while True:
         start_time = time.time()
         try:
             conn = create_socket(remote_address)
             await conn.connectof(remote_address)
             sign_key = gen_sign_key(key)
             await conn.send(struct.pack("!BB", 1, len(sign_key)) + sign_key)
             connect_type = (await conn.recv(1)).read(1)
             if connect_type == b'\x01':
-                forward_address = await read_forward_address(conn)
+                current_forward_address = await read_forward_address(conn)
+            else:
+                current_forward_address = forward_address
             forward_status = {"recv_len": 0, "send_len": 0, "last_time": time.time(), "check_recv_len": 0,
                               "check_send_len": 0}
-            sevent.current().call_async(tcp_forward, conn, forward_address, conns, forward_status)
+            sevent.current().call_async(tcp_forward, conn, current_forward_address, conns, forward_status)
         except sevent.errors.SocketClosed as e:
             logging.info("connect error %s:%d %s", remote_address[0], remote_address[1], e)
             if time.time() - start_time < 5:
                 await sevent.sleep(5)
         except (sevent.errors.ResolveError, ConnectionRefusedError) as e:
             logging.info("connect error %s:%d %s", remote_address[0], remote_address[1], e)
             await sevent.sleep(5)
         except Exception as e:
             sevent.current().call_async(sevent.current().stop)
             raise e
 
-async def handle_local_connect(conn, remote_address, key, proxy_type, conns, status):
+async def client_handle_local_connect(conn, remote_address, key, proxy_type, conns, status):
     start_time = time.time()
     conn.write, pconn = warp_write(conn, status, "recv_len"), None
 
     try:
         forward_address = (await parse_forward_address(conn, proxy_type)) if proxy_type else None
 
         pconn = create_socket(remote_address)
@@ -272,20 +274,20 @@
         conns.pop(id(conn), None)
 
     logging.info("tcp forward closed %s:%d -> %s:%d %s %s %.2fms", conn.address[0], conn.address[1],
                  remote_address[0], remote_address[1], format_data_len(status["send_len"]),
                  format_data_len(status["recv_len"]),
                  (time.time() - start_time) * 1000)
 
-async def run_local_server(server, remote_address, key, proxy_type, conns):
+async def client_run_server(server, remote_address, key, proxy_type, conns):
     while True:
         try:
             conn = await server.accept()
             status = {"recv_len": 0, "send_len": 0, "last_time": time.time(), "check_recv_len": 0, "check_send_len": 0}
-            sevent.current().call_async(handle_local_connect, conn, remote_address, key, proxy_type, conns, status)
+            sevent.current().call_async(client_handle_local_connect, conn, remote_address, key, proxy_type, conns, status)
             conns[id(conn)] = (conn, conn, status)
         except sevent.errors.SocketClosed as e:
             sevent.current().call_async(sevent.current().stop)
             raise e
 
 async def check_timeout(conns, conn_status, timeout):
     def run_check():
@@ -321,56 +323,73 @@
         check_thread = threading.Thread(target=run_check)
         check_thread.setDaemon(True)
         check_thread.start()
     await sevent.Future()
 
 def main(argv):
     parser = argparse.ArgumentParser(description='tcp reverse port forward')
-    parser.add_argument('-c', dest='is_client_mode', nargs='?', const=True, default=False, type=bool, help='is client mode (defualt: False)')
-    parser.add_argument('-k', dest='key', default='', type=str, help='auth key (defualt: "")')
-    parser.add_argument('-b', dest='bind', default="0.0.0.0", help='server mode bind host (default: 0.0.0.0)')
-    parser.add_argument('-r', dest='remote_port', default=8088, type=int, help='server mode remote bind port (default: 8088)')
-    parser.add_argument('-l', dest='local_port', default=0, type=int, help='server mode  local bind port (default: 8089)')
-    parser.add_argument('-H', dest='host', default="127.0.0.1", help='client mode connect server host (default: 127.0.0.1)')
-    parser.add_argument('-P', dest='port', default=8088, type=int, help='client mode connect server port (default: 8088)')
-    parser.add_argument('-f', dest='forward_host', default="127.0.0.1:80", help='client mode forward host , accept format [remote_host:remote_port] (default: 127.0.0.1:80)')
-    parser.add_argument('-T', dest='proxy_type', default="", choices=("raw", "http", "socks5", "redirect"), help='local listen proxy type (default: raw)')
-    parser.add_argument('-t', dest='timeout', default=7200, type=int, help='no read/write timeout (default: 7200)')
+    parser.add_argument('-c', dest='is_client_mode', nargs='?', const=True, default=False, type=bool,
+                        help='is client mode (defualt: False)')
+    parser.add_argument('-k', dest='key', default='', type=str,
+                        help='auth key (defualt: "")')
+    parser.add_argument('-b', dest='bind_host', default="0.0.0.0",
+                        help='server and client mode local bind host (default: 0.0.0.0)')
+    parser.add_argument('-p', dest='bind_port', default=0, type=int,
+                        help='server and client mode local bind port (default: 8089)')
+    parser.add_argument('-r', dest='listen_host', default="0.0.0.0",
+                        help='server mode reverse server listen host (default: 0.0.0.0)')
+    parser.add_argument('-l', dest='listen_port', default=8088, type=int,
+                        help='server mode reverse server listen port (default: 8088)')
+    parser.add_argument('-H', dest='connect_host', default="127.0.0.1",
+                        help='client mode reverse client connect server host (default: 127.0.0.1)')
+    parser.add_argument('-P', dest='connect_port', default=8088, type=int,
+                        help='client mode reverse client connect server port (default: 8088)')
+    parser.add_argument('-f', dest='forward_host', default="",
+                        help='server and client mode forward host , accept format [remote_host:remote_port] (default: )')
+    parser.add_argument('-T', dest='proxy_type', default="",
+                        choices=("raw", "http", "socks5", "redirect"), help='server and client mode local listen proxy type (default: raw)')
+    parser.add_argument('-t', dest='timeout', default=7200,
+                        type=int, help='no read/write timeout (default: 7200)')
     args = parser.parse_args(args=argv)
     config_signal()
 
-    forward_info = args.forward_host.split(":")
-    if len(forward_info) == 1:
-        if not forward_info[0].isdigit():
-            forward_host, forward_port = forward_info[0], 8088
-        else:
-            forward_host, forward_port = "127.0.0.1", int(forward_info[0])
+    if not args.forward_host:
+        forward_address = None
     else:
-        forward_host, forward_port = forward_info[0], int(forward_info[1])
+        forward_info = args.forward_host.split(":")
+        if len(forward_info) == 1:
+            if not forward_info[0].isdigit():
+                forward_address = (forward_info[0], 8088)
+            else:
+                forward_address = ("127.0.0.1", int(forward_info[0]))
+        else:
+            forward_address = (forward_info[0], int(forward_info[1]))
 
     if not args.is_client_mode:
-        remote_server = create_server((args.bind, args.remote_port))
-        local_server = create_server((args.bind, args.local_port or 8089))
-        logging.info("listen %s %d -> %d", args.bind, args.local_port or 8089, args.remote_port)
+        remote_server = create_server((args.listen_host, args.listen_port))
+        local_server = create_server((args.bind_host, args.bind_port or 8089))
+        logging.info("listen %s %d -> %s:%d", args.bind_host, args.bind_port or 8089, args.listen_host, args.listen_port)
 
-        sevent.instance().call_async(run_server, remote_server, (forward_host, forward_port),
+        sevent.instance().call_async(server_run_server, remote_server,
+                                     forward_address if forward_address else ("127.0.0.1", 80),
                                      sevent.utils.ensure_bytes(args.key), args.proxy_type,
-                                     conns, status, handle_remote_connection)
-        sevent.instance().call_async(run_server, local_server, (forward_host, forward_port),
+                                     conns, status, server_handle_remote_connect)
+        sevent.instance().call_async(server_run_server, local_server, forward_address,
                                      sevent.utils.ensure_bytes(args.key), args.proxy_type,
-                                     conns, status, handle_local_connection)
+                                     conns, status, server_handle_local_connect)
     else:
-        if args.local_port:
-            local_server = create_server((args.bind, args.local_port))
-            logging.info("listen %s %d", args.bind, args.local_port)
-            sevent.instance().call_async(run_local_server, local_server, (args.host, args.port),
+        if args.bind_port:
+            local_server = create_server((args.bind_host, args.bind_port))
+            logging.info("listen %s %d", args.bind_host, args.bind_port)
+            sevent.instance().call_async(client_run_server, local_server, (args.connect_host, args.connect_port),
                                          sevent.utils.ensure_bytes(args.key), args.proxy_type, conns)
 
-        logging.info("connect %s:%d -> %s:%d", args.host, args.port, forward_host, forward_port)
-        sevent.instance().call_async(run_connect, (args.host, args.port), (forward_host, forward_port),
+        logging.info("connect %s:%d -> %s", args.connect_host, args.connect_port, forward_address)
+        sevent.instance().call_async(client_run_connect, (args.connect_host, args.connect_port),
+                                     forward_address if forward_address else ("127.0.0.1", 80),
                                      sevent.utils.ensure_bytes(args.key), conns, status)
     sevent.current().call_async(check_timeout, conns, status, args.timeout)
 
 if __name__ == '__main__':
     logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)1.1s %(message)s',
                         datefmt='%Y-%m-%d %H:%M:%S', filemode='a+')
     try:
```

### Comparing `sevent-0.4.8/sevent/helpers/utils.py` & `sevent-0.4.9/sevent/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/impl/epoll_loop.py` & `sevent-0.4.9/sevent/impl/epoll_loop.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/impl/kqueue_loop.py` & `sevent-0.4.9/sevent/impl/kqueue_loop.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/impl/select_loop.py` & `sevent-0.4.9/sevent/impl/select_loop.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/loop.py` & `sevent-0.4.9/sevent/loop.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/pipe.py` & `sevent-0.4.9/sevent/pipe.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/tcp.py` & `sevent-0.4.9/sevent/tcp.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/udp.py` & `sevent-0.4.9/sevent/udp.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/utils.py` & `sevent-0.4.9/sevent/utils.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent/waker.py` & `sevent-0.4.9/sevent/waker.py`

 * *Files identical despite different names*

### Comparing `sevent-0.4.8/sevent.egg-info/PKG-INFO` & `sevent-0.4.9/sevent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sevent
-Version: 0.4.8
+Version: 0.4.9
 Summary: lightweight event loop
 Home-page: https://github.com/snower/sevent
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `sevent-0.4.8/sevent.egg-info/SOURCES.txt` & `sevent-0.4.9/sevent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

