# Comparing `tmp/egorovsystem-0.0.7.tar.gz` & `tmp/egorovsystem-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\egorovsystem-0.0.7.tar", last modified: Thu Jul  6 04:23:28 2023, max compression
+gzip compressed data, was "egorovsystem-0.0.8.tar", last modified: Thu Jul 13 08:38:32 2023, max compression
```

## Comparing `egorovsystem-0.0.7.tar` & `egorovsystem-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.386759 egorovsystem-0.0.7/
--rw-rw-rw-   0        0        0     1083 2023-07-05 17:14:09.000000 egorovsystem-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1562 2023-07-06 04:23:28.385758 egorovsystem-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-07-05 19:50:38.000000 egorovsystem-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.330747 egorovsystem-0.0.7/egolocal/
--rw-rw-rw-   0        0        0     1662 2023-07-06 02:37:41.000000 egorovsystem-0.0.7/egolocal/main.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.335748 egorovsystem-0.0.7/egorovsystem/
--rw-rw-rw-   0        0        0     1880 2023-07-06 03:33:15.000000 egorovsystem-0.0.7/egorovsystem/__init__.py
--rw-rw-rw-   0        0        0      270 2023-07-06 03:38:42.000000 egorovsystem-0.0.7/egorovsystem/run_command.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.345750 egorovsystem-0.0.7/egorovsystem.egg-info/
--rw-rw-rw-   0        0        0     1562 2023-07-06 04:23:28.000000 egorovsystem-0.0.7/egorovsystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      872 2023-07-06 04:23:28.000000 egorovsystem-0.0.7/egorovsystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 04:23:28.000000 egorovsystem-0.0.7/egorovsystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2023-07-06 04:23:28.000000 egorovsystem-0.0.7/egorovsystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2023-07-06 04:23:28.000000 egorovsystem-0.0.7/egorovsystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-06 04:23:28.000000 egorovsystem-0.0.7/egorovsystem.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.350751 egorovsystem-0.0.7/egoserver/
--rw-rw-rw-   0        0        0        0 2023-07-06 02:03:41.000000 egorovsystem-0.0.7/egoserver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.361753 egorovsystem-0.0.7/egoserver/egoserver/
--rw-rw-rw-   0        0        0        0 2023-07-05 17:33:47.000000 egorovsystem-0.0.7/egoserver/egoserver/__init__.py
--rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.7/egoserver/egoserver/asgi.py
--rw-rw-rw-   0        0        0       83 2023-07-05 17:41:34.000000 egorovsystem-0.0.7/egoserver/egoserver/secret.py
--rw-rw-rw-   0        0        0     3369 2023-07-05 19:09:44.000000 egorovsystem-0.0.7/egoserver/egoserver/settings.py
--rw-rw-rw-   0        0        0      847 2023-07-05 17:55:04.000000 egorovsystem-0.0.7/egoserver/egoserver/urls.py
--rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.7/egoserver/egoserver/wsgi.py
--rw-rw-rw-   0        0        0      687 2023-07-05 17:33:47.000000 egorovsystem-0.0.7/egoserver/manage.py
--rw-rw-rw-   0        0        0      823 2023-07-06 02:10:10.000000 egorovsystem-0.0.7/egoserver/run.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.376756 egorovsystem-0.0.7/egoserver/server/
--rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.7/egoserver/server/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-05 17:41:04.000000 egorovsystem-0.0.7/egoserver/server/admin.py
--rw-rw-rw-   0        0        0      150 2023-07-05 17:35:32.000000 egorovsystem-0.0.7/egoserver/server/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.380757 egorovsystem-0.0.7/egoserver/server/migrations/
--rw-rw-rw-   0        0        0     1387 2023-07-05 18:07:03.000000 egorovsystem-0.0.7/egoserver/server/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.7/egoserver/server/migrations/__init__.py
--rw-rw-rw-   0        0        0      747 2023-07-05 18:02:46.000000 egorovsystem-0.0.7/egoserver/server/models.py
--rw-rw-rw-   0        0        0       63 2023-07-05 17:35:32.000000 egorovsystem-0.0.7/egoserver/server/tests.py
--rw-rw-rw-   0        0        0      405 2023-07-06 03:33:23.000000 egorovsystem-0.0.7/egoserver/server/urls.py
--rw-rw-rw-   0        0        0      215 2023-07-05 17:59:31.000000 egorovsystem-0.0.7/egoserver/server/utils.py
--rw-rw-rw-   0        0        0     2466 2023-07-06 03:33:36.000000 egorovsystem-0.0.7/egoserver/server/views.py
--rw-rw-rw-   0        0        0       42 2023-07-06 04:23:28.386759 egorovsystem-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-07-06 04:23:25.000000 egorovsystem-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:23:28.383757 egorovsystem-0.0.7/test/
--rw-rw-rw-   0        0        0        0 2023-07-05 19:43:29.000000 egorovsystem-0.0.7/test/__init__.py
--rw-rw-rw-   0        0        0       72 2023-07-06 02:57:10.000000 egorovsystem-0.0.7/test/a.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.481958 egorovsystem-0.0.8/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 17:14:09.000000 egorovsystem-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1562 2023-07-13 08:38:32.480959 egorovsystem-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2023-07-05 19:50:38.000000 egorovsystem-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.409933 egorovsystem-0.0.8/egolocal/
+-rw-rw-rw-   0        0        0     1662 2023-07-06 02:37:41.000000 egorovsystem-0.0.8/egolocal/main.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.413936 egorovsystem-0.0.8/egorovsystem/
+-rw-rw-rw-   0        0        0     1880 2023-07-11 08:58:51.000000 egorovsystem-0.0.8/egorovsystem/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-07-13 08:27:58.000000 egorovsystem-0.0.8/egorovsystem/run_command.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.444278 egorovsystem-0.0.8/egorovsystem.egg-info/
+-rw-rw-rw-   0        0        0     1562 2023-07-13 08:38:32.000000 egorovsystem-0.0.8/egorovsystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      922 2023-07-13 08:38:32.000000 egorovsystem-0.0.8/egorovsystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 08:38:32.000000 egorovsystem-0.0.8/egorovsystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2023-07-13 08:38:32.000000 egorovsystem-0.0.8/egorovsystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2023-07-13 08:38:32.000000 egorovsystem-0.0.8/egorovsystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-13 08:38:32.000000 egorovsystem-0.0.8/egorovsystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.448797 egorovsystem-0.0.8/egoserver/
+-rw-rw-rw-   0        0        0        0 2023-07-06 02:03:41.000000 egorovsystem-0.0.8/egoserver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.458875 egorovsystem-0.0.8/egoserver/egoserver/
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:33:47.000000 egorovsystem-0.0.8/egoserver/egoserver/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.8/egoserver/egoserver/asgi.py
+-rw-rw-rw-   0        0        0       83 2023-07-05 17:41:34.000000 egorovsystem-0.0.8/egoserver/egoserver/secret.py
+-rw-rw-rw-   0        0        0     3369 2023-07-05 19:09:44.000000 egorovsystem-0.0.8/egoserver/egoserver/settings.py
+-rw-rw-rw-   0        0        0      847 2023-07-05 17:55:04.000000 egorovsystem-0.0.8/egoserver/egoserver/urls.py
+-rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.8/egoserver/egoserver/wsgi.py
+-rw-rw-rw-   0        0        0      687 2023-07-05 17:33:47.000000 egorovsystem-0.0.8/egoserver/manage.py
+-rw-rw-rw-   0        0        0      568 2023-07-13 08:29:26.000000 egorovsystem-0.0.8/egoserver/run.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.471443 egorovsystem-0.0.8/egoserver/server/
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.8/egoserver/server/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-05 17:41:04.000000 egorovsystem-0.0.8/egoserver/server/admin.py
+-rw-rw-rw-   0        0        0      150 2023-07-05 17:35:32.000000 egorovsystem-0.0.8/egoserver/server/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.476431 egorovsystem-0.0.8/egoserver/server/migrations/
+-rw-rw-rw-   0        0        0     1387 2023-07-05 18:07:03.000000 egorovsystem-0.0.8/egoserver/server/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      413 2023-07-13 08:37:23.000000 egorovsystem-0.0.8/egoserver/server/migrations/0002_function_type.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.8/egoserver/server/migrations/__init__.py
+-rw-rw-rw-   0        0        0      820 2023-07-13 08:37:07.000000 egorovsystem-0.0.8/egoserver/server/models.py
+-rw-rw-rw-   0        0        0       63 2023-07-05 17:35:32.000000 egorovsystem-0.0.8/egoserver/server/tests.py
+-rw-rw-rw-   0        0        0      405 2023-07-06 03:33:23.000000 egorovsystem-0.0.8/egoserver/server/urls.py
+-rw-rw-rw-   0        0        0      215 2023-07-05 17:59:31.000000 egorovsystem-0.0.8/egoserver/server/utils.py
+-rw-rw-rw-   0        0        0     2543 2023-07-13 08:02:15.000000 egorovsystem-0.0.8/egoserver/server/views.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 08:38:32.481958 egorovsystem-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-13 08:38:13.000000 egorovsystem-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:38:32.479960 egorovsystem-0.0.8/test/
+-rw-rw-rw-   0        0        0        0 2023-07-05 19:43:29.000000 egorovsystem-0.0.8/test/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-06 02:57:10.000000 egorovsystem-0.0.8/test/a.py
```

### Comparing `egorovsystem-0.0.7/LICENSE` & `egorovsystem-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.7/PKG-INFO` & `egorovsystem-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egorovsystem
-Version: 0.0.7
+Version: 0.0.8
 Author: Yongyi Yang
 Author-email: yongyi@umich.edu
 License: MIT License
         
         Copyright (c) 2023 Yongyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `egorovsystem-0.0.7/egolocal/main.py` & `egorovsystem-0.0.8/egolocal/main.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.7/egorovsystem/__init__.py` & `egorovsystem-0.0.8/egorovsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.7/egorovsystem.egg-info/PKG-INFO` & `egorovsystem-0.0.8/egorovsystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egorovsystem
-Version: 0.0.7
+Version: 0.0.8
 Author: Yongyi Yang
 Author-email: yongyi@umich.edu
 License: MIT License
         
         Copyright (c) 2023 Yongyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `egorovsystem-0.0.7/egorovsystem.egg-info/SOURCES.txt` & `egorovsystem-0.0.8/egorovsystem.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,10 +24,11 @@
 egoserver/server/apps.py
 egoserver/server/models.py
 egoserver/server/tests.py
 egoserver/server/urls.py
 egoserver/server/utils.py
 egoserver/server/views.py
 egoserver/server/migrations/0001_initial.py
+egoserver/server/migrations/0002_function_type.py
 egoserver/server/migrations/__init__.py
 test/__init__.py
 test/a.py
```

### Comparing `egorovsystem-0.0.7/egoserver/egoserver/settings.py` & `egorovsystem-0.0.8/egoserver/egoserver/settings.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.7/egoserver/egoserver/urls.py` & `egorovsystem-0.0.8/egoserver/egoserver/urls.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.7/egoserver/manage.py` & `egorovsystem-0.0.8/egoserver/manage.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.7/egoserver/server/migrations/0001_initial.py` & `egorovsystem-0.0.8/egoserver/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.7/egoserver/server/models.py` & `egorovsystem-0.0.8/egoserver/server/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     def __str__(self):
         return str(self.key)
     
 class Function(models.Model):
     key = models.TextField(default = "", blank = True, null = True)
     val = models.TextField(default = "", blank = True, null = True)
+    type = models.TextField(default = "cmd", blank = True, null = True)
 
     def __str__(self):
         return str(self.key)
 
 class Password(models.Model):
     key = models.TextField(default = "", blank = True, null = True)
     val = models.TextField(default = "", blank = True, null = True)
```

### Comparing `egorovsystem-0.0.7/egoserver/server/views.py` & `egorovsystem-0.0.8/egoserver/server/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,16 +57,19 @@
     val_raw = str(fun.val)
     val = val_raw
     for var in Variable.objects.all(): # 也许有不这么粗暴的方法...
         val = val.replace( "${" + str(var.key) + "}" , str(var.val))
 
 
     return JsonResponse({
-        "val": val , 
-        "val_raw": val_raw , 
+        "val": {
+            "content": val , 
+            "type": fun.type , 
+        } , 
+        "content_raw": val_raw , 
         "errorflag": False , 
     })
 
 def get_rand_str():
 	s = ""
 	for i in range(10):
 		s += "qwertyuioplkjhgfdsazxcvbnm"[random.randint(0,26-1)]
```

### Comparing `egorovsystem-0.0.7/setup.py` & `egorovsystem-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 print (find_packages())
 pkgs = [p for p in find_packages() if p.startswith("ego")]
 print(pkgs)
 
 setup(
 	name					= "egorovsystem",
-	version					= "0.0.7",
+	version					= "0.0.8",
 	description				= "",
 	long_description		= readme,
 	long_description_content_type	= "text/markdown",
 	license					= license,
 	author					= "Yongyi Yang",
 	author_email 			= "yongyi@umich.edu",
 	python_requires			= ">=3.6",
```

