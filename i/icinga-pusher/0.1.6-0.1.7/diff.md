# Comparing `tmp/icinga_pusher-0.1.6.tar.gz` & `tmp/icinga_pusher-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icinga_pusher-0.1.6.tar", max compression
+gzip compressed data, was "icinga_pusher-0.1.7.tar", max compression
```

## Comparing `icinga_pusher-0.1.6.tar` & `icinga_pusher-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.6/README.md
--rw-r--r--   0        0        0     3044 2023-07-05 07:44:38.557646 icinga_pusher-0.1.6/icinga_pusher/__init__.py
--rw-r--r--   0        0        0      388 2023-07-05 07:44:56.444349 icinga_pusher-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.7/README.md
+-rw-r--r--   0        0        0     3137 2023-07-13 14:24:41.132033 icinga_pusher-0.1.7/icinga_pusher/__init__.py
+-rw-r--r--   0        0        0      388 2023-07-13 14:25:14.695526 icinga_pusher-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.7/PKG-INFO
```

### Comparing `icinga_pusher-0.1.6/LICENSE` & `icinga_pusher-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `icinga_pusher-0.1.6/icinga_pusher/__init__.py` & `icinga_pusher-0.1.7/icinga_pusher/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                                  json=data,
                                  headers=headers,
                                  verify=self.icinga.ssl_verify,
                                  auth=(self.icinga.username, self.icinga.password))
             resp.raise_for_status()
         except requests.exceptions.RequestException as e:
             logger.error(f"Could not set Icinga status of service {self.service}. {e}")
-            if hasattr(e, "response") and hasattr(e.response, "text"):
+            if isinstance(e, requests.exceptions.HTTPError):
                 logger.error(f"Response: {e.response.text}")
         else:
             logger.info(f"Sucessfully set Icinga status for service {self.service}")
 
 
 class Icinga(object):
     CHECK_OK = 0
@@ -66,14 +66,16 @@
     def __init__(self, hostname: str, username: str, password: str, ssl_verify: bool = True) -> IcingaService:
         self.username = username
         self.password = password
         if not hostname.startswith("https://"):
             raise ValueError(f"Hostname must start with https {hostname=}")
         self.hostname = hostname
         self.ssl_verify = ssl_verify
+        logger.info("this is a test info message")
+        logger.debug("this is a test info message")
 
     def service(self, hostname, service):
         return IcingaService(self, hostname, service)
 
 
 if __name__ == '__main__':
     i = Icinga("https://icinga.example.com", "api-user", "api-password")
```

