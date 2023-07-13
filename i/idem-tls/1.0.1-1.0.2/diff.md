# Comparing `tmp/idem-tls-1.0.1.tar.gz` & `tmp/idem-tls-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-tls-1.0.1.tar", last modified: Wed Jul  5 23:52:13 2023, max compression
+gzip compressed data, was "idem-tls-1.0.2.tar", last modified: Thu Jul 13 16:02:45 2023, max compression
```

## Comparing `idem-tls-1.0.1.tar` & `idem-tls-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-07-05 23:51:58.000000 idem-tls-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5173 2023-07-05 23:52:13.618877 idem-tls-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4370 2023-07-05 23:51:58.000000 idem-tls-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/acct/tls/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/acct/tls/init.py
--rw-r--r--   0 root         (0) root         (0)     1319 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/exec/tls/
--rw-r--r--   0 root         (0) root         (0)     5305 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/exec/tls/certificate.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/exec/tls/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/states/tls/
--rw-r--r--   0 root         (0) root         (0)      169 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/states/tls/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/tool/tls/
--rw-r--r--   0 root         (0) root         (0)     2356 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/tool/tls/certificate.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5173 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 23:52:13.618877 idem-tls-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2716 2023-07-05 23:51:58.000000 idem-tls-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-07-13 16:02:31.000000 idem-tls-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5173 2023-07-13 16:02:45.194332 idem-tls-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4370 2023-07-13 16:02:31.000000 idem-tls-1.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls/acct/tls/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/acct/tls/init.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls/exec/tls/
+-rw-r--r--   0 root         (0) root         (0)     5326 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/exec/tls/certificate.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/exec/tls/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls/states/tls/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/states/tls/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls/tool/tls/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/tool/tls/certificate.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-13 16:02:44.000000 idem-tls-1.0.2/idem_tls/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5173 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 16:02:45.194332 idem-tls-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-07-13 16:02:31.000000 idem-tls-1.0.2/setup.py
```

### Comparing `idem-tls-1.0.1/LICENSE` & `idem-tls-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.1/PKG-INFO` & `idem-tls-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-tls
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-tls-1.0.1/README.rst` & `idem-tls-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.1/idem_tls/conf.py` & `idem-tls-1.0.2/idem_tls/conf.py`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.1/idem_tls/exec/tls/certificate.py` & `idem-tls-1.0.2/idem_tls/exec/tls/certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,18 +82,18 @@
 
     """
     result = dict(comment=[], ret=None, result=True)
 
     try:
         conn = await hub.tool.tls.certificate.get_ssl_connection(ctx, url)
         conn.do_handshake()
-    except SSL.Error as e:
+    except SSL.WantReadError as e:
         # ignore handshake error, connection has server certificate chain
         hub.log.info(f"SSL handshake error {e.__class__.__name__}: {e}")
-    except Exception as e:
+    except (SSL.Error, Exception) as e:
         result["comment"].append(f"{e.__class__.__name__}: {e}")
         result["result"] = False
         return result
 
     try:
         cert = conn.get_peer_cert_chain()[-1]
     finally:
```

### Comparing `idem-tls-1.0.1/idem_tls/tool/tls/certificate.py` & `idem-tls-1.0.2/idem_tls/tool/tls/certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 async def get_ssl_connection(hub, ctx, url):
     """
     Get the SSL connection for given website URL
     Args:
         url(string): The URL of the website to get the certificates from.
     Returns: SSL connection for url
     """
-    method = SSL.TLSv1_METHOD
+    method = SSL.TLSv1_2_METHOD
     # Retrieve method from credentials if provided
     if ctx.acct.get("method", None) and getattr(SSL, f"{ctx.acct.method}_METHOD", None):
         method = getattr(SSL, f"{ctx.acct.method}_METHOD", None)
     url_parts = urlparse(url).netloc.split(":")
     host = url_parts[0].strip()
     port = int(url_parts[1]) if len(url_parts) > 1 else 443
     context = SSL.Context(method=method)
```

### Comparing `idem-tls-1.0.1/idem_tls.egg-info/PKG-INFO` & `idem-tls-1.0.2/idem_tls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-tls
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-tls-1.0.1/setup.py` & `idem-tls-1.0.2/setup.py`

 * *Files identical despite different names*

