# Comparing `tmp/pxsecurityapi-1.0.3.tar.gz` & `tmp/pxsecurityapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxsecurityapi-1.0.3.tar", last modified: Thu Jul  6 23:51:58 2023, max compression
+gzip compressed data, was "pxsecurityapi-1.0.4.tar", last modified: Wed Jul 12 23:46:41 2023, max compression
```

## Comparing `pxsecurityapi-1.0.3.tar` & `pxsecurityapi-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 23:51:58.082123 pxsecurityapi-1.0.3/
--rw-rw-rw-   0        0        0      333 2023-07-06 23:51:58.082123 pxsecurityapi-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxsecurityapi-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      523 2023-07-06 23:51:58.082123 pxsecurityapi-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 23:51:58.066502 pxsecurityapi-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 23:51:58.066502 pxsecurityapi-1.0.3/src/pxsecurityapi/
--rw-rw-rw-   0        0        0     1870 2023-07-06 22:49:22.000000 pxsecurityapi-1.0.3/src/pxsecurityapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 23:51:58.082123 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/
--rw-rw-rw-   0        0        0      333 2023-07-06 23:51:58.000000 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-06 23:51:58.000000 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 23:51:58.000000 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-06 23:51:58.000000 pxsecurityapi-1.0.3/src/pxsecurityapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 23:46:41.264552 pxsecurityapi-1.0.4/
+-rw-rw-rw-   0        0        0      333 2023-07-12 23:46:41.264552 pxsecurityapi-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxsecurityapi-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      523 2023-07-12 23:46:41.264552 pxsecurityapi-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 23:46:41.264552 pxsecurityapi-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 23:46:41.264552 pxsecurityapi-1.0.4/src/pxsecurityapi/
+-rw-rw-rw-   0        0        0     2192 2023-07-12 23:43:45.000000 pxsecurityapi-1.0.4/src/pxsecurityapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:46:41.264552 pxsecurityapi-1.0.4/src/pxsecurityapi.egg-info/
+-rw-rw-rw-   0        0        0      333 2023-07-12 23:46:41.000000 pxsecurityapi-1.0.4/src/pxsecurityapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-12 23:46:41.000000 pxsecurityapi-1.0.4/src/pxsecurityapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 23:46:41.000000 pxsecurityapi-1.0.4/src/pxsecurityapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 23:46:41.000000 pxsecurityapi-1.0.4/src/pxsecurityapi.egg-info/top_level.txt
```

### Comparing `pxsecurityapi-1.0.3/setup.cfg` & `pxsecurityapi-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7873 6563 7572 6974 7961 7069   = pxsecurityapi
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 330d 0a61 7574 686f 7220 3d20 506f 756e  3..author = Poun
+00000030: 340d 0a61 7574 686f 7220 3d20 506f 756e  4..author = Poun
 00000040: 6465 7820 4173 736f 6369 6174 6573 2043  dex Associates C
 00000050: 6f72 706f 7261 7469 6f6e 0d0a 6175 7468  orporation..auth
 00000060: 6f72 5f65 6d61 696c 203d 2069 7440 706f  or_email = it@po
 00000070: 756e 6465 782e 636f 6d0d 0a64 6573 6372  undex.com..descr
 00000080: 6970 7469 6f6e 203d 200d 0a6c 6f6e 675f  iption = ..long_
 00000090: 6465 7363 7269 7074 696f 6e20 3d20 0d0a  description = ..
 000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `pxsecurityapi-1.0.3/src/pxsecurityapi/__init__.py` & `pxsecurityapi-1.0.4/src/pxsecurityapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,8 +43,20 @@
             encrypted_pair = self.getFile()
             return self.DecHMAC(encrypted_pair, self.key)
         except Exception as e:
             raise e
     
     def getSimpleDict(self) -> dict:
         d = self.get()
-        return {k: v["value"] for k, v in d.items()}
+        return {k: v["value"] for k, v in d.items()}
+    
+    def getSQL(self, name) -> str:
+        d = self.get()
+        assert name in d
+        assert d[name]["type"] == "Stored Procedure"
+        # Go read the SQL File.
+        file_path = d[name]["value"]
+        with open(file_path, 'r') as f:
+            sql = f.read()
+            return sql
+
+
```

