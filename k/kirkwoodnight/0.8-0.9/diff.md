# Comparing `tmp/kirkwoodnight-0.8.tar.gz` & `tmp/kirkwoodnight-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-0.8.tar", last modified: Wed Jul 12 22:26:49 2023, max compression
+gzip compressed data, was "kirkwoodnight-0.9.tar", last modified: Wed Jul 12 22:28:40 2023, max compression
```

## Comparing `kirkwoodnight-0.8.tar` & `kirkwoodnight-0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:26:49.562750 kirkwoodnight-0.8/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.8/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 22:26:49.562358 kirkwoodnight-0.8/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.8/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:26:49.558544 kirkwoodnight-0.8/kirkwoodnight/
--rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-0.8/kirkwoodnight/__init__.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2746 2023-07-12 22:25:38.000000 kirkwoodnight-0.8/kirkwoodnight/command_line.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)    15900 2023-07-12 22:18:18.000000 kirkwoodnight-0.8/kirkwoodnight/source.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:26:49.561839 kirkwoodnight-0.8/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 22:26:49.000000 kirkwoodnight-0.8/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      334 2023-07-12 22:26:49.000000 kirkwoodnight-0.8/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 22:26:49.000000 kirkwoodnight-0.8/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-12 22:26:49.000000 kirkwoodnight-0.8/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 22:26:49.000000 kirkwoodnight-0.8/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-12 22:26:49.000000 kirkwoodnight-0.8/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 22:26:49.562907 kirkwoodnight-0.8/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-12 22:26:46.000000 kirkwoodnight-0.8/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:28:40.072592 kirkwoodnight-0.9/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.9/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 22:28:40.072270 kirkwoodnight-0.9/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.9/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:28:40.069408 kirkwoodnight-0.9/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-0.9/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2746 2023-07-12 22:25:38.000000 kirkwoodnight-0.9/kirkwoodnight/command_line.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     7948 2023-07-12 14:27:02.000000 kirkwoodnight-0.9/kirkwoodnight/obj_list.csv
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    15900 2023-07-12 22:18:18.000000 kirkwoodnight-0.9/kirkwoodnight/source.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:28:40.071823 kirkwoodnight-0.9/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      361 2023-07-12 22:28:40.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 22:28:40.072709 kirkwoodnight-0.9/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-12 22:28:20.000000 kirkwoodnight-0.9/setup.py
```

### Comparing `kirkwoodnight-0.8/LICENSE.txt` & `kirkwoodnight-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.8/PKG-INFO` & `kirkwoodnight-0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 0.8
+Version: 0.9
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-0.8/README.md` & `kirkwoodnight-0.9/README.md`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.8/kirkwoodnight/command_line.py` & `kirkwoodnight-0.9/kirkwoodnight/command_line.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.8/kirkwoodnight/source.py` & `kirkwoodnight-0.9/kirkwoodnight/source.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.8/kirkwoodnight.egg-info/PKG-INFO` & `kirkwoodnight-0.9/kirkwoodnight.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 0.8
+Version: 0.9
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-0.8/setup.py` & `kirkwoodnight-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="0.8",
+    version="0.9",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
```

