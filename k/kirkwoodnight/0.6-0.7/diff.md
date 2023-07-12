# Comparing `tmp/kirkwoodnight-0.6.tar.gz` & `tmp/kirkwoodnight-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-0.6.tar", last modified: Wed Jul 12 21:45:35 2023, max compression
+gzip compressed data, was "kirkwoodnight-0.7.tar", last modified: Wed Jul 12 22:20:16 2023, max compression
```

## Comparing `kirkwoodnight-0.6.tar` & `kirkwoodnight-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 21:45:35.645242 kirkwoodnight-0.6/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.6/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 21:45:35.644826 kirkwoodnight-0.6/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.6/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 21:45:35.641053 kirkwoodnight-0.6/kirkwoodnight/
--rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-0.6/kirkwoodnight/__init__.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2720 2023-07-12 21:24:52.000000 kirkwoodnight-0.6/kirkwoodnight/command_line.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)    15900 2023-07-12 20:40:52.000000 kirkwoodnight-0.6/kirkwoodnight/kirkwoodnight.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 21:45:35.644277 kirkwoodnight-0.6/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 21:45:35.000000 kirkwoodnight-0.6/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      341 2023-07-12 21:45:35.000000 kirkwoodnight-0.6/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 21:45:35.000000 kirkwoodnight-0.6/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       52 2023-07-12 21:45:35.000000 kirkwoodnight-0.6/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 21:45:35.000000 kirkwoodnight-0.6/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-12 21:45:35.000000 kirkwoodnight-0.6/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 21:45:35.645404 kirkwoodnight-0.6/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1075 2023-07-12 21:44:59.000000 kirkwoodnight-0.6/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:20:16.866853 kirkwoodnight-0.7/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.7/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 22:20:16.866500 kirkwoodnight-0.7/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.7/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:20:16.864090 kirkwoodnight-0.7/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-0.7/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2753 2023-07-12 22:18:40.000000 kirkwoodnight-0.7/kirkwoodnight/command_line.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    15900 2023-07-12 22:18:18.000000 kirkwoodnight-0.7/kirkwoodnight/source.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:20:16.866105 kirkwoodnight-0.7/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 22:20:16.000000 kirkwoodnight-0.7/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      334 2023-07-12 22:20:16.000000 kirkwoodnight-0.7/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 22:20:16.000000 kirkwoodnight-0.7/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-12 22:20:16.000000 kirkwoodnight-0.7/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 22:20:16.000000 kirkwoodnight-0.7/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-12 22:20:16.000000 kirkwoodnight-0.7/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 22:20:16.866964 kirkwoodnight-0.7/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-12 22:20:12.000000 kirkwoodnight-0.7/setup.py
```

### Comparing `kirkwoodnight-0.6/LICENSE.txt` & `kirkwoodnight-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.6/PKG-INFO` & `kirkwoodnight-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 0.6
+Version: 0.7
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-0.6/README.md` & `kirkwoodnight-0.7/README.md`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.6/kirkwoodnight/command_line.py` & `kirkwoodnight-0.7/kirkwoodnight/command_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
                 "Would you like to change Kirkwood's maximum altitude limit (in degrees)? (Type value if desired, otherwise hit ENTER. Default is 80.)",
                 "Would you like to change the minimum mandated distance (in degrees) from the Moon? (Type value if desired, otherwise hit ENTER. Default is 5.)",
                 "Would you like to specify a maximum allowed airmass? (Type value if desired, otherwise hit ENTER. Default is None.)",
                 "Would you like to specify a desired level of darkness for the night? (If desired, type 'civ' or 'naut' or 'astro' to respectively signify civil, nautical, or astronomical twilight. Otherwise hit ENTER. Default is None.)",
                 "Would you like to specify a maximum brightness level for the moon? (If desired, type 'grey' or 'dark', otherwise hit ENTER. Default is None.)",
                 "How often do you want to re-check for observability (in hours)? (type value if desired, otherwise hit ENTER. Default is 0.5, which creates a schedule in 30 minute intervals.)"]
 
+def test():
+       print("Hi!")
+
 def main():   
 # print interactive prompts in terminal
     print()
     print("------------------------------------------------------------------------")
     print("KIRKWOOD OBSERVING PLANNER")
     print("CREATED BY: ARMAAN GOYAL, BRANDON RADZOM, JESSICA RANSHAW, XIAN-YU WANG")
     print("LAST UPDATED ON 2023-07-14")
```

### Comparing `kirkwoodnight-0.6/kirkwoodnight/kirkwoodnight.py` & `kirkwoodnight-0.7/kirkwoodnight/source.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.6/kirkwoodnight.egg-info/PKG-INFO` & `kirkwoodnight-0.7/kirkwoodnight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 0.6
+Version: 0.7
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-0.6/setup.py` & `kirkwoodnight-0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
@@ -22,15 +22,15 @@
     classifiers=[
         "License :: OSI Approved :: MIT License"
     ],
 
     # Specify console scripts
     entry_points={
         'console_scripts': [
-            'kirkwoodnight = command_line:main',
+            'kirkwoodnight = kirkwoodnight.command_line:main',
         ],
     },
 
     # Include additional files into the package
     package_data={'': ['obj_list.csv']},
 
     install_requires= get_requires(),
```

