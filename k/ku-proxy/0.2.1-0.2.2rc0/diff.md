# Comparing `tmp/ku_proxy-0.2.1-py3-none-any.whl.zip` & `tmp/ku_proxy-0.2.2rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,15 @@
-Zip file size: 10563 bytes, number of entries: 10
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-08 13:23 ku/__init__.py
--rw-r--r--  2.0 unx    12013 b- defN 23-Jul-08 13:23 ku/ku.py
--rw-r--r--  2.0 unx     9453 b- defN 23-Jul-08 13:23 ku/kun.py
--rw-r--r--  2.0 unx      943 b- defN 23-Jul-08 13:23 ku/util.py
--rw-rw-rw-  2.0 unx     1064 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3462 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        3 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      753 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/RECORD
-10 files, 27869 bytes uncompressed, 9289 bytes compressed:  66.7%
+Zip file size: 12691 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-13 12:40 ku/__init__.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-13 12:40 ku/__main__.py
+-rw-r--r--  2.0 unx     2713 b- defN 23-Jul-13 12:40 ku/iautil.py
+-rw-r--r--  2.0 unx    12424 b- defN 23-Jul-13 12:40 ku/ku.py
+-rw-r--r--  2.0 unx     8182 b- defN 23-Jul-13 12:40 ku/kun.py
+-rw-r--r--  2.0 unx     1693 b- defN 23-Jul-13 12:40 ku/kun_sessions.py
+-rw-r--r--  2.0 unx     2069 b- defN 23-Jul-13 12:40 ku/util.py
+-rw-rw-rw-  2.0 unx     1064 b- defN 23-Jul-13 12:40 ku_proxy-0.2.2rc0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3738 b- defN 23-Jul-13 12:40 ku_proxy-0.2.2rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 12:40 ku_proxy-0.2.2rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-Jul-13 12:40 ku_proxy-0.2.2rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        3 b- defN 23-Jul-13 12:40 ku_proxy-0.2.2rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      985 b- defN 23-Jul-13 12:40 ku_proxy-0.2.2rc0.dist-info/RECORD
+13 files, 33095 bytes uncompressed, 11065 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,31 +1,40 @@
 Filename: ku/__init__.py
 Comment: 
 
+Filename: ku/__main__.py
+Comment: 
+
+Filename: ku/iautil.py
+Comment: 
+
 Filename: ku/ku.py
 Comment: 
 
 Filename: ku/kun.py
 Comment: 
 
+Filename: ku/kun_sessions.py
+Comment: 
+
 Filename: ku/util.py
 Comment: 
 
-Filename: ku_proxy-0.2.1.dist-info/LICENSE
+Filename: ku_proxy-0.2.2rc0.dist-info/LICENSE
 Comment: 
 
-Filename: ku_proxy-0.2.1.dist-info/METADATA
+Filename: ku_proxy-0.2.2rc0.dist-info/METADATA
 Comment: 
 
-Filename: ku_proxy-0.2.1.dist-info/WHEEL
+Filename: ku_proxy-0.2.2rc0.dist-info/WHEEL
 Comment: 
 
-Filename: ku_proxy-0.2.1.dist-info/entry_points.txt
+Filename: ku_proxy-0.2.2rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ku_proxy-0.2.1.dist-info/top_level.txt
+Filename: ku_proxy-0.2.2rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: ku_proxy-0.2.1.dist-info/RECORD
+Filename: ku_proxy-0.2.2rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ku/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .ku import * # NOQA
-version = '0.2.1'
+version = '0.2.2-pre'
```

## ku/ku.py

```diff
@@ -1,29 +1,38 @@
 """
     Ku
     ==
-    single-threaded async mitm tcp proxy
+    threaded async mitm tcp proxy
 """
 
-from threading import Thread, currentThread
+from threading import Thread, currentThread, get_ident, Lock
 from select import select
-from socket import socket, SOL_SOCKET, AF_INET, AF_INET6
+from socket import socket, AF_INET6, AF_INET, SOL_SOCKET
 import logging
 
 from typing import Union, Tuple, List
 
 from enum import Enum
 from time import time, sleep
-from re import match
 
 from platform import system
+from .util import split
+from .iautil import resolve_proto
 
 # https://learn.microsoft.com/en-us/windows/win32/winsock/so-conditional-accept
 SO_CONDITIONAL_ACCEPT = 0x3002
 
+lock = Lock()
+def tsafe(fun):
+    def wrapper(*args, **kwargs):
+        with lock:
+            return fun(get_ident(), *args, **kwargs)
+    return wrapper
+print = tsafe(print)
+
 class Reject(object):
     pass
 
 class Pass(object):
     pass
 
 class state(Enum):
@@ -63,96 +72,82 @@
         self._state = new_state
 
     def terminate(self) -> None:
         self.proxy.terminate(self)
 
     def __repr__(self):        
         if self._state != state.CONNECTED:
+            st = self._state
+        else:
+            st = round((time() - self.estab_time), 2)
+        try:
+            return f"<#{id(self)}[{st}] {self.client.getpeername()}->{self.client.getsockname()}::{self.server.getsockname()}->{self.server.getpeername()}>"
+        except:
             return super().__repr__()
-        return f"<#{id(self)}[{round((time() - self.estab_time), 2)}] {self.client.getpeername()}->{self.client.getsockname()}::{self.server.getsockname()}->{self.server.getpeername()}>"
 
 class ku(object):
 
     fd: List[socket]  # tracked file descriptors
     wai: List[socket] # wa
     ss: List[tcpsession]
 
     sockets: Tuple[socket]  # listening socket
-    thread: Thread  # polling thread
+    threads: List[Thread]  # polling threads
     upstream: tuple  # upstream proto, host, port
 
     alive: bool = True  # alive marker
     pause: bool = False # you can temporarily stop polling
     PSM = 0.00001 # power Save Mode, reduces cpu cycles count
+    POLL_TO = 0.3 # Event polling timeout
 
-    @staticmethod
-    def _resolve_proto(host: str):
-
-        IPv6 = r"^(\[[\d\D]{1,}\])$"
-        IP6 = r"^([a-f0-9:]{1,})$"
-        IPv4 = r"^([0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3})$"
-        TLD = r"^([A-z0-9._-]{1,})$"
-
-        PATTERNS = [IPv6, IPv4, TLD, IP6]
-
-        for pattern in PATTERNS:
-            i = match(pattern, host)
-            if i:
-                if pattern is IPv6:
-                    return AF_INET6
-                
-                elif pattern is IP6:
-                    return AF_INET6
-
-                elif pattern is IPv4:
-                    return AF_INET
-
-                elif pattern is TLD:
-                    return -1
-
-    def __init__(self, listen: tuple, upstream: tuple, session: tcpsession = tcpsession, session_args: tuple = (), maxcon: int = -1, upstream_6: bool = False, loglevel = logging.ERROR):
+    def __init__(self, listen: tuple, upstream: tuple, session: tcpsession = tcpsession, session_args: tuple = (), maxcon: int = -1, upstream_6: bool = False, loglevel = logging.ERROR, parallelism: int = 1):
 
         self.fd: list = []
         self.wai: list = []
         self.ss: list = []
 
         self._logger = logging.getLogger("ku.devel")
         self._logger.setLevel(loglevel)
 
-        proto = self._resolve_proto(upstream[0])
+        proto = resolve_proto(upstream[0])
         self.upstream = (AF_INET6 if upstream_6 else AF_INET if proto == -1 else proto, upstream[0], upstream[1])
         self._logger.debug(f"Upstreaming to - {'v6' if self.upstream[0] is AF_INET6 else 'v4'} {upstream[0]}:{upstream[1]}")
 
         self.session = session
         self.maxcon = maxcon
         self.session_args = session_args
+        self.parallelism = parallelism
 
         self.sockets = ()
         for i in range(0, len(listen), 2):
-            proto, host, port = self._resolve_proto(listen[i]), *listen[i:i+2]
+            proto, host, port = resolve_proto(listen[i]), *listen[i:i+2]
 
             sock = socket(proto, 1)
             self._logger.debug(f"Listening at - {'v6' if proto is AF_INET6 else 'v4'} {host}:{port}")
             sock.bind((host, port))
             if system() == "Windows":
                 sock.setsockopt(SOL_SOCKET, SO_CONDITIONAL_ACCEPT, 1)
             sock.listen()
             self.fd.append(sock)
             self.sockets = (*self.sockets, sock)
 
-        self.thread = Thread(target=self.poll, name=f"Ku poller #{id(self)}", daemon=True)
-        self.thread.start()
+        self.threads = []
+
+        for p in range(0, parallelism):
+            thread = Thread(target=self.poll, name=f"Ku poller {p} of #{id(self)}", daemon=True, args=[p])
+            thread.start()
+            self.threads.append(thread)
 
     def shutdown(self):
         # can't be called from handler!)
-        if currentThread() is self.thread:
+        if currentThread() in self.threads:
             raise RuntimeError(f"People stuck at {currentThread()}")
 
         self.alive = False
-        while self.thread.is_alive():
+        while max([t.is_alive() for t in self.threads]):
             pass
 
         for s in self.ss:
             if s._state == state.CONNECTED:
                 s.shutdown()
 
             s.client.shutdown(1)
@@ -160,29 +155,29 @@
             s._change_state(state.DISCONNECTED)
 
         del self.fd
         del self.ss        
         for sock in self.sockets:
             sock.close()
         del self.sockets
-        del self.thread
+        del self.threads
 
     def terminate(self, session: tcpsession):
         session._change_state(state.DISCONNECTED)
         # Call handlers
         session.connection_lost(None, RuntimeError("Internal terminate request"))
         # Remove descriptors from polling
         self.fd.remove(session.client)
         self.fd.remove(session.server)
         # Shutdown sockets
         session.client.shutdown(2)
         session.server.shutdown(2)
         # Delete session
         self.ss.remove(session)
-        self._logger.debug(f"#{id(session)} terminated [ITR]")
+        self._logger.debug(f"[Thr {get_ident()}] #{id(session)} terminated [ITR]")
 
     def _handle_socket_disconnect(self, fd, err):            
         s = self.lookup_session(fd)        
         if not s:
             # ITR
             return
 
@@ -196,15 +191,15 @@
 
         # Destroy session instance
         self.ss.remove(s)
 
         s._change_state(state.DISCONNECTED)
         s.connection_lost(fd, err)
 
-        self._logger.debug(f"#{id(s)} terminated")
+        self._logger.debug(f"[Thr {get_ident()}] #{id(s)} terminated")
 
     def lookup_session(self, fd: socket):
         for s in self.ss:
             if s.client == fd or s.server == fd:
                 return s
 
     def send(self, fd: socket, data: bytes) -> None:
@@ -223,91 +218,95 @@
             except:
                 pass
             return
         
         # create new instance of tcpsession class
         s = object.__new__(self.session)
         s.proxy = self
-        self._logger.debug(f"#{id(s)} Begin new connection request processing")
+        self._logger.debug(f"[Thr {get_ident()}] #{id(s)} Begin new connection request processing")
 
         # new client
         try:
             c, addr = fd.accept()
         except Exception as e:
             self._logger.warning(f"Failed to accept new client: {e}")
-            self._logger.debug(f"#{id(s)} terminated")
+            self._logger.debug(f"[Thr {get_ident()}] #{id(s)} terminated")
             return
             
-        self._logger.debug(f"#{id(s)} client: {addr}")
+        self._logger.debug(f"[Thr {get_ident()}] #{id(s)} client: {addr}")
         s.client = c
 
         s._change_state(state.CLIENT_W_U)
 
         # new upstream
         u = socket(self.upstream[0], 1)
         u.settimeout(0)
         s.server = u
 
         try:                        
             u.connect(self.upstream[1:])
         except BlockingIOError:
             pass
 
-        self._logger.debug(f"#{id(s)} upstreaming initiated, waiting...")        
+        self._logger.debug(f"[Thr {get_ident()}] #{id(s)} upstreaming initiated, waiting...")        
 
         self.ss.append(s)                    
         self.wai.append(u)
 
-    def poll(self):
-        self._logger.debug("Begin polling")
+    def poll(self, shard_num: int):
+        self._logger.debug(f"Begin polling as {currentThread()}")
 
         while self.alive:
             # select()
-            fds, puo, puf = select(self.fd, self.wai, self.wai, 0)
-            if not (fds or puo or puf) or self.pause:
+            shard_fd = split(self.fd, self.parallelism)[shard_num]
+            shard_wai = split(self.wai, self.parallelism)[shard_num]
+
+            if not (shard_fd or shard_wai) or self.pause:
                 if self.PSM:
                     sleep(self.PSM)
                 continue
 
+            fds, puo, puf = select(shard_fd, shard_wai, shard_wai, self.POLL_TO)
             for fd in puo:                
-                s = self.lookup_session(fd)
-                self._logger.debug(f"#{id(s)} upstreamed, initiating trasmisson")
-
                 # Remove upstream from waiting list
                 self.wai.remove(fd)
 
-                # Add client & upstream to watging list
-                self.fd.append(fd)
-                self.fd.append(s.client)
+                s = self.lookup_session(fd)
+                self._logger.debug(f"[Thr {get_ident()}] #{id(s)} upstreamed, initiating trasmisson")
 
-                # Change session state
-                s._change_state(state.CONNECTED)
 
                 s.estab_time = time()
 
                 # Init session
                 s.__init__(s.client, fd, self, *self.session_args)
 
-            for fd in puf:
-                s = self.lookup_session(fd)
-                self._logger.debug(f"#{id(s)} Failed to upstream")
+                # Change session state
+                s._change_state(state.CONNECTED)
 
+                # Add client & upstream to watging list
+                self.fd.append(fd)
+                self.fd.append(s.client)
+
+            for fd in puf:
                 # Remove upstream from waiting list
                 self.wai.remove(fd)
 
+                s = self.lookup_session(fd)
+                self._logger.debug(f"[Thr {get_ident()}] #{id(s)} Failed to upstream")
+
                 # Close associated client & upstream descriptors
                 s.client.close()
                 fd.close()
 
                 # Change session state
                 s._change_state(state.DISCONNECTED)
 
                 self.ss.remove(s)
 
-                self._logger.debug(f"#{id(s)} terminated")
+                self._logger.debug(f"[Thr {get_ident()}] #{id(s)} terminated")
 
             for sock in self.sockets:
                 if sock in fds:
                     self._accept(sock)
                     fds.remove(sock)
 
             for fd in fds:
@@ -316,25 +315,25 @@
 
                 s = self.lookup_session(fd)
                 bname = 'client' if fd is s.client else 'upstream'
 
                 try:
                     data = fd.recv(65535)
                 except Exception as e:
-                    self._logger.debug(f"#{id(s)}, {bname} lost connection: {e}")
+                    self._logger.debug(f"[Thr {get_ident()}] #{id(s)}, {bname} lost connection: {e}")
                     self._handle_socket_disconnect(fd, e)
                     continue
 
                 if len(data) < 1:
-                    self._logger.debug(f"#{id(s)}, {bname} disconnected")
+                    self._logger.debug(f"[Thr {get_ident()}] #{id(s)}, {bname} disconnected")
                     self._handle_socket_disconnect(fd, None)
                     continue
 
                 if fd is s.client:
-                    #self._logger.debug(f"#{id(s)} client -> server {round(len(data) / 1000, 2)}Kb")
+                    #self._logger.debug(f"[Thr {get_ident()}] #{id(s)} client -> server {round(len(data) / 1000, 2)}Kb")
                     hr = None
 
                     try:
                         hr = s.serverbound(data)
                     except Exception as e:
                         self._logger.error(f"Exception in {s.serverbound}: {e}")
 
@@ -346,19 +345,19 @@
 
                     elif hr is not Pass and hr is not None:
                         self._logger.error(F"#{id(s)} ServerBound handler returned unidentified type! {hr.__class__}")
 
                     try:
                         s.server.sendall(data)
                     except Exception as e:
-                        self._logger.debug(f"#{id(s)} Upstream dropped connection in the middle of data transmission process")
+                        self._logger.debug(f"[Thr {get_ident()}] #{id(s)} Upstream dropped connection in the middle of data transmission process")
                         self._handle_socket_disconnect(s.server, e)
 
                 else:
-                    #self._logger.debug(f"#{id(s)} server -> client {round(len(data) / 1000, 2)}Kb")
+                    #self._logger.debug(f"[Thr {get_ident()}] #{id(s)} server -> client {round(len(data) / 1000, 2)}Kb")
                     hr = None
 
                     try:
                         hr = s.clientbound(data)
                     except Exception as e:
                         self._logger.error(f"Exception in {s.clientbound}: {e}")                        
 
@@ -370,11 +369,11 @@
 
                     elif hr is not Pass and hr is not None:
                         self._logger.error(F"#{id(s)} ClientBound handler returned unidentified type! {hr.__class__}")
 
                     try:
                         s.client.sendall(data)
                     except Exception as e:
-                        self._logger.debug(f"#{id(s)} Client dropped connection in the middle of data transmission process")
+                        self._logger.debug(f"[Thr {get_ident()}] #{id(s)} Client dropped connection in the middle of data transmission process")
                         self._handle_socket_disconnect(s.client, e)
 
-        self._logger.debug(f"Stop polling")
+        self._logger.debug(f"Stop polling as {currentThread()}")
```

## ku/kun.py

```diff
@@ -2,151 +2,56 @@
     Kun
     ===
     Powerful fronted for ku-proxy
 """
 
 import argparse
 import logging
-from random import randint
-from re import findall
-from socket import gaierror, getaddrinfo
 from time import sleep, time
-from typing import Tuple
 
 from ku import ku, tcpsession
 from ku import version as ku_version
 
-from .util import CustomFormatter
+from .util import CustomFormatter, genrancol, ansicol, flock
+from .iautil import host_parse, resolve_host
+from .kun_sessions import stream, transit
 import statistics, curses
 import traceback
 
-reset = "\u001b[0m"
+version = '0.1.1'
 
-version = '0.1'
+print = flock(print) # lock print for multithreading
 
 banner = \
 f"""
  __    __                    
 |  \  /  \                   
 | $$ /  $$__    __  _______  
 | $$/  $$|  \  |  \|       \ 
 | $$  $$ | $$  | $$| $$$$$$$\\
 | $$$$$\ | $$  | $$| $$  | $$
 | $$ \$$\| $$__/ $$| $$  | $$
 | $$  \$$ \$$    $$| $$  | $$
  \$$   \$$ \$$$$$$  \$$   \$$ v{version}
 """
 
-def _host_parse(host: str) -> Tuple[str, int]:
-    
-    IPv6_PORT = r"^(\[[\d\D]{1,}\]):([0-9]{1,5})$"
-    IPv4_PORT = r"^([0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}):([0-9]{1,5})$"
-    TLD_PORT = r"^([A-z0-9._-]{1,}):([0-9]{1,5})$"
-
-    PATTERNS = [IPv6_PORT, IPv4_PORT, TLD_PORT]
-    for pattern in PATTERNS:
-        i = findall(pattern, host)
-        if i:
-            if pattern is IPv6_PORT:
-                proto = 23
-            elif pattern is IPv4_PORT:
-                proto = 2
-            else:
-                proto = -1
-
-            return proto, i[0][0], int(i[0][1])
-    raise RuntimeError('Failed to parse host string', host)
-
-def _resolve_host(host: str) -> Tuple[Tuple[int, str]]:
-    protocol = ku._resolve_proto(host)
-    if not protocol:
-        raise RuntimeError("Failed to define protocol(ipv4 or ipv6) for host:", host)
-    elif protocol == -1:
-        try:
-            host_addresses = getaddrinfo(host, 7)
-        except gaierror:
-            raise RuntimeError("Failed to resolve hostname:", host)
-        return [(addr[0], addr[4][0]) for addr in host_addresses]
-    return [[protocol, host]]
-
-def genrancol(brightness: int = 1) -> Tuple[int, int, int]:
-    cs = randint(0, 255), randint(0, 255), randint(0, 255)
-    while cs[0] + cs[1] + cs[2] < 250:
-        cs = randint(0, 255), randint(0, 255), randint(0, 255)
-    r, g, b = (min(255, int(c * brightness)) for c in cs)
-    return r, g, b
-
-def ansicol(r: int, g: int ,b: int) -> str:
-    return f"\x1b[38;2;{r};{g};{b}m"
-
-TOTAL = 0
-
-def mb(len: int) -> str:
-    val = round(len / 1024**2, 2)
-    if not val:
-        val = round(len / 1_000_000, 7)
-
-    return str(val)
-
-class sess(tcpsession):
-    def __init__(self, client, server, proxy):
-        self.id = id(self)   
-        self.color = ansicol(*genrancol(1.17))
-
-        print(self.color, F"#{self.id} {client.getpeername()}->{client.getsockname()}::{server.getsockname()}->{server.getpeername()}", reset)
-
-    def clientbound(self, data):
-        global TOTAL     
-        TOTAL += len(data)
-        print(self.color, F"#{self.id} server->client  {len(data)}", reset)
-    
-    def serverbound(self, data):        
-        global TOTAL
-        TOTAL += len(data)
-        print(self.color, F"#{self.id} client->server  {len(data)}", reset)
-    
-    def connection_made(self):
-        print(self.color, F"#{self.id} connection_made", reset)
-    
-    def connection_lost(self, side, err):
-        side = 'client' if side is self.client else 'server' if side is not None else 'proxy'
-        print(self.color, F"#{self.id} connection_lost by {side} due to {err}", reset)
-    
-class transit(tcpsession):
-
-    TX = 0
-    RX = 0
-
-    def clientbound(self, data):
-        global TOTAL     
-        self.RX += len(data)
-        TOTAL += len(data)
-
-    def serverbound(self, data):        
-        global TOTAL
-        self.TX += len(data)
-        TOTAL += len(data)
-                
-    def __repr__(self) -> str:
-        ttime = ".".join([i.zfill(2) for i in str(round((time() - self.estab_time), 2)).split('.')])
-        output = f"#{id(self)}[{ttime}] / {self.client.getpeername()} / RX:{mb(self.RX)}Mb TX: {mb(self.TX)}Mb"
-        return output
-    
 def entry_point():
     pcolor = ansicol(*genrancol(1.37))
-    print(pcolor, banner[1:], reset, sep='')
+    print(pcolor, banner[1:], "\u001b[0m", sep='')
 
     parser = argparse.ArgumentParser(description="Powerful fronted for ku-proxy")
     parser.add_argument("-v", action="store_true", help="If passed, enabling verbose logging")
     parser.add_argument("-l", action='append', help="Proxy listen addr (allowed multiple and dualstack hostnames) (enclose ipv6 like [::1])", metavar="localhost:65535", required=True)
     parser.add_argument("-u", help="Proxy upstream server addr", metavar="localhost:8000", required=True)
     parser.add_argument("-7", help="Tells proxy to upstream over IPv6", action="store_true", dest='u6')
     parser.add_argument("-ll", action="store_true", help="If passed, enables low level debug logging (ku-proxy debug)")
     parser.add_argument("-mc", type=int, help="Maximum of parralel clients (connection over the limit will be refused)", default=-1, metavar="15")
+    parser.add_argument("--nt", type=int, help="Number of simultaneous polling threads running", default=1, metavar="4")
     parser.add_argument("--transit", action="store_true", help="If passed, enables transit (no session orientated) displaying")
+    parser.add_argument("--silent", action="store_true", help="If passed, disables connections related logging")
     args = parser.parse_args()
 
     logger = logging.getLogger("[")
     logger.setLevel(logging.DEBUG if args.v else logging.INFO)
     stdout_handler = logging.StreamHandler()
     stdout_handler.setLevel(logging.DEBUG)
     stdout_handler.setFormatter(CustomFormatter('[%(asctime)s] [%(levelname)s] %(name)s:  %(message)s', pcolor))
@@ -155,74 +60,108 @@
     logging.getLogger("ku.devel").addHandler(stdout_handler)
     logging.getLogger("ku.devel").setLevel(logging.DEBUG if args.ll else logging.WARNING)
 
     logger.info(f"Running kun v{version} (ku v{ku_version})")
 
     listen = []
     for addr in args.l:
-        ler = _host_parse(addr)
-        addreses = _resolve_host(ler[1])
+        ler = host_parse(addr)
+        addreses = resolve_host(ler[1])
         for addr in addreses:
             addr = f"[{addr[1]}]" if addr[0] == 23 else addr[1]
                 
             listen.append(addr)
             listen.append(ler[2])
             logger.info(f"\u001b[97mListening \u001b[92m-> \u001b[97m{addr}:{ler[2]}")
 
-    upstream = _host_parse(args.u)
+    upstream = host_parse(args.u)
     logger.info(f"\u001b[97mUpstream {ansicol(120, 120, 120)}({'v6' if upstream[0] is 23 else 'v6' if (args.u6 and upstream[0] == -1) else 'v4'}) \u001b[92m-> \u001b[97m{upstream[1]}:{upstream[2]}")
+    session = tcpsession if args.silent else transit if args.transit else stream
 
-    logger.info("Starting...")
-    proxy = ku(listen, upstream[1:], transit if args.transit else sess, maxcon = args.mc, upstream_6 = args.u6)
+    logger.info("Starting...")    
+    proxy = ku(listen, upstream[1:], session, maxcon = args.mc, upstream_6 = args.u6, loglevel=logging.DEBUG if args.ll else logging.WARNING, parallelism=args.nt)
     logger.info("Started")
 
     if args.transit:
+        def main_screen(screen, height, width):
+            # Listen
+            curses.init_pair(3, 12, curses.COLOR_BLACK)                
+            for k, i in enumerate(range(0, len(listen), 2)):
+                screen.addstr(k + 2, width - 36, f"Listening -> {listen[i]}:{listen[i+1]}"[:36], curses.color_pair(3))
+
+            # Upstream
+            curses.init_pair(4, 8, curses.COLOR_BLACK)
+            screen.addstr(k + 4, width - 36, f"Upstream ({'v6' if upstream[0] is 23 else 'v6' if (args.u6 and upstream[0] == -1) else 'v4'}) -> {upstream[1]}:{upstream[2]}", curses.color_pair(4))
+
+            # Sessions
+            curses.init_pair(6, 13, curses.COLOR_BLACK)
+            screen.addstr(0, 0, f"Active sessions [{len(proxy.ss)}]:", curses.color_pair(6))
+
+            sess_offset = 1
+            for i, session in enumerate(proxy.ss):
+                curses.init_pair(5, 1, curses.COLOR_BLACK)
+                screen.addstr(sess_offset + i, 5, str(session), curses.color_pair(5))
+
+        def performance(screen, height, width):
+            curses.init_pair(8, 13, curses.COLOR_BLACK)
+            
+            screen.addstr(0, 0, "Threads:", curses.color_pair(8))
+            for i, thread in enumerate(proxy.threads):
+                screen.addstr(1 + i, 0, f"  {thread}", curses.color_pair(8))
+
+            conn = len(set(proxy.fd).difference(proxy.sockets))
+            listen = len(proxy.sockets)
+
+            curses.init_pair(9, 7, curses.COLOR_BLACK)
+            screen.addstr(3 + i, 0, f"Descriptors[{len(proxy.fd) + len(proxy.wai)}]:", curses.color_pair(9))
+            screen.addstr(4 + i, 0, f"  Listen / {listen}", curses.color_pair(9))
+            screen.addstr(5 + i, 0, f"  Connected / {conn}", curses.color_pair(9))
+            screen.addstr(6 + i, 0, f"  Sunrise / {len(proxy.wai)}", curses.color_pair(9))
+
+
         def transit_screen(screen):
 
             curses.start_color()
             curses.curs_set(0)
             screen.timeout(int(1000 / 25))
             fps = [0]
             button = 0
+            screens = [main_screen, performance]
+            current_screen = screens[0]
 
             while 7:
                 if button == 99:
                     proxy.pause = not proxy.pause
+                
+                if button == 261:
+                    ni = screens.index(current_screen) + 1
+                    if 0 <= ni <= len(screens) - 1:
+                        current_screen = screens[ni]
+                    elif len(screens) - 1 < ni:
+                        current_screen = screens[0]
+
+                elif button == 260:
+                    ni = screens.index(current_screen) - 1
+                    if 0 <= ni <= len(screens):
+                        current_screen = screens[ni]
+                    elif ni < 0:
+                        current_screen = screens[len(screens) - 1]
 
                 render_begin = time()
                     
                 screen.clear()
                 height, width = screen.getmaxyx()
 
-                # Banner
-                curses.init_pair(1, 8, curses.COLOR_BLACK)
-                screen.addstr(0, 0, banner[1:], curses.color_pair(1))
-
-                # Listen
-                curses.init_pair(3, 12, curses.COLOR_BLACK)                
-                for k, i in enumerate(range(0, len(listen), 2)):
-                    screen.addstr(k + 2, width - 36, f"Listening -> {listen[i]}:{listen[i+1]}"[:36], curses.color_pair(3))
-
-                # Upstream
-                curses.init_pair(4, 8, curses.COLOR_BLACK)
-                screen.addstr(k + 4, width - 36, f"Upstream ({'v6' if upstream[0] is 23 else 'v6' if (args.u6 and upstream[0] == -1) else 'v4'}) -> {upstream[1]}:{upstream[2]}", curses.color_pair(4))
-
-                # Sessions
-                curses.init_pair(6, 13, curses.COLOR_BLACK)
-                screen.addstr(10, 0, f"Active sessions [{len(proxy.ss)}]:", curses.color_pair(6))
-
-                sess_offset = 11
-                for i, session in enumerate(proxy.ss):
-                    curses.init_pair(5, 1, curses.COLOR_BLACK)
-                    screen.addstr(sess_offset + i, 5, str(session), curses.color_pair(5))
+                # draw screen
+                current_screen(screen, height, width)
 
                 # Actionbar
                 fps_fix = f"FPS: {round(statistics.median(fps), 2)}".ljust(10)
                 state = f"State: {'PAUSED' if proxy.pause else 'RUNNING' if proxy.alive else 'STOPP'}"
-                actionbar = f"{fps_fix}, {state}, {button}, Total transfered: {mb(TOTAL)}Mb".ljust(width - 1)
+                actionbar = f"{fps_fix}, {state}, {button}, {current_screen.__name__} [use arrows to switch screens]".ljust(width - 1)
                 curses.init_pair(2, curses.COLOR_BLACK, 15)
                 screen.addstr(height - 1, 0, actionbar, curses.color_pair(2))
 
                 try:
                     screen.refresh()
                     button = screen.getch()
                 except KeyboardInterrupt:
@@ -240,15 +179,15 @@
         except Exception as e:
             print(traceback.format_exc())
             proxy.shutdown()            
 
     else:
         while 7:
             try:
-                if not proxy.thread.is_alive():
+                if not min([t.is_alive() for t in proxy.threads]):
                     logger.warning(f"Proxy unexpectedly closed")
                     break
                 sleep(0.07)
             except KeyboardInterrupt:
                 logger.info("Shutting down...")
                 proxy.shutdown()
                 logger.info("Exiting...")
```

## ku/util.py

```diff
@@ -1,10 +1,15 @@
+"""
+    ## Misc
+"""
+
 import logging, os
 os.system('color')
-from typing import Optional
+from typing import Optional, Tuple
+from threading import Lock, get_ident
 
 class CustomFormatter(logging.Formatter):    
     
     grey = '\u001b[34m'
     blue = '\x1b[38;5;39m'
     yellow = '\x1b[38;5;226m'
     red = '\x1b[38;5;196m'
@@ -22,7 +27,43 @@
             logging.CRITICAL: self.bold_red + self.fmt + self.reset
         }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt, datefmt='%m/%d/%Y %I:%M:%S %p')
         return formatter.format(record)
+
+def split(a, n):
+    k, m = divmod(len(a), n)
+    return [a[i*k+min(i, m):(i+1)*k+min(i+1, m)] for i in range(n)]
+
+def genrancol(brightness: int = 1) -> Tuple[int, int, int]:
+    cs = os.urandom(1)[0], os.urandom(1)[0], os.urandom(1)[0]
+    while cs[0] + cs[1] + cs[2] < 250:
+        cs = os.urandom(1)[0], os.urandom(1)[0], os.urandom(1)[0]
+    r, g, b = (min(255, int(c * brightness)) for c in cs)
+    return r, g, b
+
+def ansicol(r: int, g: int ,b: int) -> str:
+    return f"\x1b[38;2;{r};{g};{b}m"
+
+def flock(fun, data = {}):
+    data[hash(fun)] = [Lock()]
+
+    def wrapper(*args, **kwargs):
+        with data[hash(fun)][0]:
+            return fun(get_ident(), *args, **kwargs)
+
+    return wrapper
+
+def format_bytes(size):
+    """
+        https://stackoverflow.com/questions/12523586/python-format-size-application-converting-b-to-kb-mb-gb-tb
+    """
+    # 2**10 = 1024
+    power = 2**10
+    n = 0
+    power_labels = {0 : '', 1: 'K', 2: 'M', 3: 'G', 4: 'T'}
+    while size > power:
+        size /= power
+        n += 1
+    return size, power_labels[n]+'B'
```

## Comparing `ku_proxy-0.2.1.dist-info/LICENSE` & `ku_proxy-0.2.2rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ku_proxy-0.2.1.dist-info/METADATA` & `ku_proxy-0.2.2rc0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ku-proxy
-Version: 0.2.1
+Version: 0.2.2rc0
 Summary: ku is fast, async, modern, little tcp man-in-the-middle proxy library, written in pure Python 3
 Home-page: https://gitlab.com/seeklay/ku
 Author: seeklay
 Author-email: rudeboy@seeklay.icu
 License: MIT
 Download-URL: https://gitlab.com/seeklay/ku
 Platform: OS Independent
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # ku
 ku is fast, async, modern, little tcp man-in-the-middle proxy library, written in pure [Python 3](https://www.python.org/).
 
-![](https://img.shields.io/badge/Made%20with-Python-1f425f.svg) ![](https://img.shields.io/gitlab/license/seeklay/ku.svg) ![](https://tokei.rs/b1/gitlab/seeklay/ku) ![](https://badgen.net/pypi/v/ku-proxy) ![](https://img.shields.io/pypi/dw/ku-proxy?style=flat&logo=pypi) ![](https://gitlab.com/seeklay/ku/badges/main/pipeline.svg) ![](https://gitlab.com/seeklay/ku/badges/main/coverage.svg)
+[![](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![](https://img.shields.io/gitlab/license/seeklay/ku.svg)](LICENSE/) [![](https://tokei.rs/b1/gitlab/seeklay/ku)](#) [![](https://badgen.net/pypi/v/ku-proxy) ![](https://img.shields.io/pypi/dw/ku-proxy?style=flat&logo=pypi)](https://pypi.org/project/ku-proxy/) [![](https://gitlab.com/seeklay/ku/badges/main/pipeline.svg)](https://gitlab.com/seeklay/ku/-/pipelines) [![](https://gitlab.com/seeklay/ku/badges/main/coverage.svg)](https://coveralls.io/gitlab/seeklay/ku)
 
 ### Features
  - Dump data between clients and server
  - Spoof data in both directions
  - Drop data selectively
  - IPv6 Ready (pass upstream_6 for upstreaming ipv6 or enclose ipv6 addr in brackets like [::1] for listening addrs
 
@@ -33,14 +33,18 @@
  - [x] Tcp mitm proxy library
  - [x] Proxy executable script (kun (alpha))
 
 ### Installation
 ```bash
 pip install -U ku-proxy
 ```
+
+### Docs
+Check out the latest documentation: [ku-proxy.seeklay.pp.ua](https://ku-proxy.seeklay.pp.ua)
+
 ### Author
 [seeklay](https://gitlab.com/seeklay/)
 
 ### License
 [MIT](LICENSE)
 
 ### Simple proxy usage:
```

