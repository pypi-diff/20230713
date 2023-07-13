# Comparing `tmp/mb_netmgmt-0.0.8.tar.gz` & `tmp/mb_netmgmt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mb_netmgmt-0.0.8.tar", last modified: Sun Jun 12 19:42:19 2022, max compression
+gzip compressed data, was "mb_netmgmt-0.0.9.tar", last modified: Mon Jun 13 07:34:10 2022, max compression
```

## Comparing `mb_netmgmt-0.0.8.tar` & `mb_netmgmt-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       29 2022-06-10 12:37:21.272670 mb_netmgmt-0.0.8/.gitignore
--rw-r--r--   0        0        0     1063 2022-05-12 07:55:21.636265 mb_netmgmt-0.0.8/AUTHORS
--rw-r--r--   0        0        0      528 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.8/CODEOWNERS
--rw-r--r--   0        0        0     5489 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4530 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.8/CONTRIBUTING.md
--rw-r--r--   0        0        0    18092 2022-05-12 07:42:27.649671 mb_netmgmt-0.0.8/COPYING
--rw-r--r--   0        0        0      173 2022-05-16 14:19:22.315290 mb_netmgmt-0.0.8/Dockerfile
--rw-r--r--   0        0        0     4248 2022-05-12 15:16:00.210932 mb_netmgmt-0.0.8/README.md
--rw-r--r--   0        0        0     2046 2022-06-12 19:41:45.685120 mb_netmgmt-0.0.8/mb_netmgmt/__init__.py
--rwxr-xr-x   0        0        0     3560 2022-06-12 18:57:24.622529 mb_netmgmt-0.0.8/mb_netmgmt/__main__.py
--rwxr-xr-x   0        0        0     1044 2022-06-10 12:50:34.479268 mb_netmgmt-0.0.8/mb_netmgmt/netconf.py
--rw-r--r--   0        0        0      279 2022-05-12 15:45:50.527927 mb_netmgmt-0.0.8/mb_netmgmt/protocols.json
--rw-r--r--   0        0        0     4262 2022-05-18 12:23:11.443961 mb_netmgmt-0.0.8/mb_netmgmt/snmp.py
--rw-r--r--   0        0        0     3828 2022-06-12 19:40:04.468538 mb_netmgmt-0.0.8/mb_netmgmt/ssh.py
--rw-r--r--   0        0        0     2949 2022-06-12 18:57:48.395872 mb_netmgmt-0.0.8/mb_netmgmt/telnet.py
--rw-r--r--   0        0        0      140 2022-05-12 11:32:43.680335 mb_netmgmt-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1725 2022-06-12 19:39:22.388581 mb_netmgmt-0.0.8/test/test_mb_netmgmt.py
--rw-r--r--   0        0        0      107 1970-01-01 00:00:00.000000 mb_netmgmt-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       29 2022-06-10 12:37:21.272670 mb_netmgmt-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1063 2022-05-12 07:55:21.636265 mb_netmgmt-0.0.9/AUTHORS
+-rw-r--r--   0        0        0      528 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.9/CODEOWNERS
+-rw-r--r--   0        0        0     5489 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4530 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0    18092 2022-05-12 07:42:27.649671 mb_netmgmt-0.0.9/COPYING
+-rw-r--r--   0        0        0      173 2022-05-16 14:19:22.315290 mb_netmgmt-0.0.9/Dockerfile
+-rw-r--r--   0        0        0     4248 2022-05-12 15:16:00.210932 mb_netmgmt-0.0.9/README.md
+-rw-r--r--   0        0        0     2083 2022-06-13 07:33:52.801133 mb_netmgmt-0.0.9/mb_netmgmt/__init__.py
+-rwxr-xr-x   0        0        0     3560 2022-06-12 18:57:24.622529 mb_netmgmt-0.0.9/mb_netmgmt/__main__.py
+-rwxr-xr-x   0        0        0     1044 2022-06-10 12:50:34.479268 mb_netmgmt-0.0.9/mb_netmgmt/netconf.py
+-rw-r--r--   0        0        0      279 2022-05-12 15:45:50.527927 mb_netmgmt-0.0.9/mb_netmgmt/protocols.json
+-rw-r--r--   0        0        0     4262 2022-05-18 12:23:11.443961 mb_netmgmt-0.0.9/mb_netmgmt/snmp.py
+-rw-r--r--   0        0        0     3828 2022-06-12 19:40:04.468538 mb_netmgmt-0.0.9/mb_netmgmt/ssh.py
+-rw-r--r--   0        0        0     2949 2022-06-12 18:57:48.395872 mb_netmgmt-0.0.9/mb_netmgmt/telnet.py
+-rw-r--r--   0        0        0      140 2022-05-12 11:32:43.680335 mb_netmgmt-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1628 2022-06-12 19:46:42.858320 mb_netmgmt-0.0.9/test/test_mb_netmgmt.py
+-rw-r--r--   0        0        0      107 1970-01-01 00:00:00.000000 mb_netmgmt-0.0.9/PKG-INFO
```

### Comparing `mb_netmgmt-0.0.8/AUTHORS` & `mb_netmgmt-0.0.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/CODEOWNERS` & `mb_netmgmt-0.0.9/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/CODE_OF_CONDUCT.md` & `mb_netmgmt-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/CONTRIBUTING.md` & `mb_netmgmt-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/COPYING` & `mb_netmgmt-0.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/README.md` & `mb_netmgmt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/mb_netmgmt/__init__.py` & `mb_netmgmt-0.0.9/mb_netmgmt/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with mb-netmgmt. If not, see <https://www.gnu.org/licenses/
 
 """Network Management Protocols for Mountebank"""
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import os
 import subprocess
 import time
 from contextlib import contextmanager
 
 import requests
@@ -62,11 +62,12 @@
         f"http://{host}:2525/imposters",
         {"replayable": True, "removeProxies": True},
     )
     yaml.safe_dump(response.json(), open(f"{name}.yaml", "w"))
 
 
 def load_imposters(host, name):
-    put_imposters(
-        host,
-        yaml.safe_load(open(f"{name}.yaml").read())["imposters"],
-    )
+    put_imposters(host, read_imposters(name))
+
+
+def read_imposters(name):
+    return yaml.safe_load(open(f"{name}.yaml").read())["imposters"]
```

### Comparing `mb_netmgmt-0.0.8/mb_netmgmt/__main__.py` & `mb_netmgmt-0.0.9/mb_netmgmt/__main__.py`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/mb_netmgmt/netconf.py` & `mb_netmgmt-0.0.9/mb_netmgmt/netconf.py`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/mb_netmgmt/snmp.py` & `mb_netmgmt-0.0.9/mb_netmgmt/snmp.py`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/mb_netmgmt/ssh.py` & `mb_netmgmt-0.0.9/mb_netmgmt/ssh.py`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/mb_netmgmt/telnet.py` & `mb_netmgmt-0.0.9/mb_netmgmt/telnet.py`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.8/test/test_mb_netmgmt.py` & `mb_netmgmt-0.0.9/test/test_mb_netmgmt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from threading import Thread
 
 import paramiko
 import pytest
 from mb_netmgmt import mb, ssh
 from mb_netmgmt.__main__ import create_server
 
@@ -18,15 +17,15 @@
 
 def test_ssh():
     with mb(
         [
             {
                 "protocol": "ssh",
                 "port": port,
-                "stubs": [{"responses": [{"is": {"response": prompt}}]}],
+                "stubs": [prompt_stub()],
             }
         ]
     ):
         client = connect_ssh()
         chan = client.invoke_shell()
         out = chan.recv(1024)
         assert out == prompt
@@ -35,19 +34,15 @@
 def test_ssh_proxy():
     with mb(
         [
             {
                 "protocol": "ssh",
                 "port": port,
                 "stubs": [
-                    {
-                        "responses": [
-                            {"is": {"response": prompt}},
-                        ]
-                    },
+                    prompt_stub(),
                     {
                         "responses": [
                             {"proxy": {"to": "localhost"}},
                         ]
                     },
                 ],
             }
@@ -55,14 +50,18 @@
     ):
         client = connect_ssh()
         chan = client.invoke_shell()
         out = chan.recv(1024)
         assert out == prompt
 
 
+def prompt_stub():
+    return {"responses": [{"is": {"response": prompt}}]}
+
+
 def test_create_ssh_server():
     server = create_server(ssh, port, None)
     Thread(target=server.serve_forever).start()
     connect_ssh().close()
     server.shutdown()
```

