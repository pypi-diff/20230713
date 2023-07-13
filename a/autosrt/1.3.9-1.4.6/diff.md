# Comparing `tmp/autosrt-1.3.9.tar.gz` & `tmp/autosrt-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.3.9.tar", last modified: Wed Jun  7 20:06:20 2023, max compression
+gzip compressed data, was "autosrt-1.4.6.tar", last modified: Thu Jul 13 01:58:07 2023, max compression
```

## Comparing `autosrt-1.3.9.tar` & `autosrt-1.4.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.641807 autosrt-1.3.9/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.9/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-07 20:06:20.641807 autosrt-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.603597 autosrt-1.3.9/autosrt/
--rw-rw-rw-   0        0        0   115678 2023-06-07 20:05:48.000000 autosrt-1.3.9/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.626822 autosrt-1.3.9/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-07 20:06:20.645555 autosrt-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.638810 autosrt-1.3.9/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.3.9/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.3.9/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.3.9/test/test3.py
--rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.9/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:58:07.786406 autosrt-1.4.6/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-07-13 01:58:07.787156 autosrt-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 01:58:07.643716 autosrt-1.4.6/autosrt/
+-rw-rw-rw-   0        0        0   163312 2023-07-13 01:51:28.000000 autosrt-1.4.6/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:58:07.701405 autosrt-1.4.6/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-13 01:58:07.796146 autosrt-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:58:07.783431 autosrt-1.4.6/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.6/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.6/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.6/test/test3.py
+-rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.6/test/test4.py
```

### Comparing `autosrt-1.3.9/LICENSE` & `autosrt-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/PKG-INFO` & `autosrt-1.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.9
+Version: 1.4.6
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.9/README.md` & `autosrt-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/autosrt.egg-info/PKG-INFO` & `autosrt-1.4.6/autosrt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.9
+Version: 1.4.6
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.9/setup.py` & `autosrt-1.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/test/test1.py` & `autosrt-1.4.6/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/test/test2.py` & `autosrt-1.4.6/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/test/test3.py` & `autosrt-1.4.6/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/test/test4.py` & `autosrt-1.4.6/test/test4.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         )
 
         stderr = []
         base_popen_kwargs = self.base_popen_kwargs.copy()
         if popen_kwargs is not None:
             base_popen_kwargs.update(popen_kwargs)
 
-        if sys.platform == "wind32":
+        if sys.platform == "win32":
             self.process = subprocess.Popen(
                 cmd_with_progress,
                 **base_popen_kwargs,
                 creationflags=subprocess.CREATE_NO_WINDOW,
             )  # type: ignore
         else:
             self.process = subprocess.Popen(
```

