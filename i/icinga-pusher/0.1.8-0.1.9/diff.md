# Comparing `tmp/icinga_pusher-0.1.8.tar.gz` & `tmp/icinga_pusher-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icinga_pusher-0.1.8.tar", max compression
+gzip compressed data, was "icinga_pusher-0.1.9.tar", max compression
```

## Comparing `icinga_pusher-0.1.8.tar` & `icinga_pusher-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.8/README.md
--rw-r--r--   0        0        0     3126 2023-07-13 15:36:06.142741 icinga_pusher-0.1.8/icinga_pusher/__init__.py
--rw-r--r--   0        0        0      388 2023-07-13 15:36:29.229604 icinga_pusher-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.9/README.md
+-rw-r--r--   0        0        0     3172 2023-07-13 15:38:26.773929 icinga_pusher-0.1.9/icinga_pusher/__init__.py
+-rw-r--r--   0        0        0      388 2023-07-13 15:38:50.350764 icinga_pusher-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.9/PKG-INFO
```

### Comparing `icinga_pusher-0.1.8/LICENSE` & `icinga_pusher-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `icinga_pusher-0.1.8/icinga_pusher/__init__.py` & `icinga_pusher-0.1.9/icinga_pusher/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 logger = logging.getLogger("icinga_pusher")
 logger.setFormatter(logging.Formatter("[%(asctime)s %(name)s: %(levelname)s] %(message)s"))
 logger.setLevel(logging.INFO)
 
 ICINGA_DRY_RUN = "ICINGA_DRY_RUN"
 
+requests.packages.urllib3.disable_warnings()
+
 
 class IcingaService(object):
 
     def __init__(self, icinga, mon_host, service):
         self.icinga = icinga
         self.mon_host = mon_host
         self.service = service
```

