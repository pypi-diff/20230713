# Comparing `tmp/reliableGPT-0.2.988.tar.gz` & `tmp/reliableGPT-0.2.989.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.988.tar", last modified: Thu Jul 13 16:47:22 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.989.tar", last modified: Thu Jul 13 16:49:51 2023, max compression
```

## Comparing `reliableGPT-0.2.988.tar` & `reliableGPT-0.2.989.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:47:22.048158 reliableGPT-0.2.988/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.988/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 16:47:22.048049 reliableGPT-0.2.988/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.988/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.988/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:47:22.046913 reliableGPT-0.2.988/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:47:22.047880 reliableGPT-0.2.988/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.988/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    21987 2023-07-13 16:42:56.000000 reliableGPT-0.2.988/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.988/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.988/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5370 2023-07-13 16:46:25.000000 reliableGPT-0.2.988/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 16:47:22.048202 reliableGPT-0.2.988/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 16:47:18.000000 reliableGPT-0.2.988/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:49:51.675617 reliableGPT-0.2.989/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.989/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 16:49:51.675498 reliableGPT-0.2.989/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.989/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.989/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:49:51.674320 reliableGPT-0.2.989/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 16:49:51.000000 reliableGPT-0.2.989/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 16:49:51.000000 reliableGPT-0.2.989/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 16:49:51.000000 reliableGPT-0.2.989/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 16:49:51.000000 reliableGPT-0.2.989/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 16:49:51.000000 reliableGPT-0.2.989/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:49:51.675192 reliableGPT-0.2.989/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3148 2023-07-13 16:49:27.000000 reliableGPT-0.2.989/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    21987 2023-07-13 16:42:56.000000 reliableGPT-0.2.989/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.989/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.989/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5370 2023-07-13 16:46:25.000000 reliableGPT-0.2.989/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 16:49:51.675663 reliableGPT-0.2.989/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 16:49:48.000000 reliableGPT-0.2.989/setup.py
```

### Comparing `reliableGPT-0.2.988/LICENSE` & `reliableGPT-0.2.989/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.988/README.md` & `reliableGPT-0.2.989/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.988/reliablegpt/Alerting.py` & `reliableGPT-0.2.989/reliablegpt/Alerting.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                alert_threshold=5,
                send_notifications=True,
                user_emails=set()):
     self.unhandled_errors = {
     }  # dictionary of openai errors + frequency count for that hour
     now = datetime.datetime.now()
     self.current_time_block = now.hour
-    self.set_cooldown = False
+    self.set_cooldown = True
     self.cooldown_start_time = time.time()
     self.send_notifications = send_notifications
     self.user_emails = user_emails
 
   def start_cooldown(self):
     self.set_cooldown = True
     self.cooldown_start_time = time.time()
```

### Comparing `reliableGPT-0.2.988/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.989/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.988/reliablegpt/Model.py` & `reliableGPT-0.2.989/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.988/reliablegpt/main.py` & `reliableGPT-0.2.989/reliablegpt/main.py`

 * *Files identical despite different names*

