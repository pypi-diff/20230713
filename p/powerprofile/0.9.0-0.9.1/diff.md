# Comparing `tmp/powerprofile-0.9.0.tar.gz` & `tmp/powerprofile-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/powerprofile-0.9.0.tar", last modified: Tue Dec 28 15:33:13 2021, max compression
+gzip compressed data, was "dist/powerprofile-0.9.1.tar", last modified: Wed Dec 29 16:48:36 2021, max compression
```

## Comparing `powerprofile-0.9.0.tar` & `powerprofile-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-28 15:33:13.000000 powerprofile-0.9.0/
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-28 15:33:13.000000 powerprofile-0.9.0/powerprofile.egg-info/
--rw-r--r--   0 afita     (1000) afita     (1000)       13 2021-12-28 15:33:13.000000 powerprofile-0.9.0/powerprofile.egg-info/top_level.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      346 2021-12-28 15:33:13.000000 powerprofile-0.9.0/powerprofile.egg-info/SOURCES.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      731 2021-12-28 15:33:13.000000 powerprofile-0.9.0/powerprofile.egg-info/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)        1 2021-12-28 15:33:13.000000 powerprofile-0.9.0/powerprofile.egg-info/dependency_links.txt
--rw-r--r--   0 afita     (1000) afita     (1000)       20 2021-12-28 15:33:13.000000 powerprofile-0.9.0/powerprofile.egg-info/requires.txt
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-28 15:33:13.000000 powerprofile-0.9.0/powerprofile/
--rw-rw-r--   0 afita     (1000) afita     (1000)    14026 2021-12-28 15:29:26.000000 powerprofile-0.9.0/powerprofile/powerprofile.py
--rw-r--r--   0 afita     (1000) afita     (1000)      117 2020-04-16 15:12:51.000000 powerprofile-0.9.0/powerprofile/__init__.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     1000 2021-12-28 15:29:26.000000 powerprofile-0.9.0/powerprofile/exceptions.py
--rw-rw-r--   0 afita     (1000) afita     (1000)      731 2021-12-28 15:33:13.000000 powerprofile-0.9.0/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)       38 2021-12-28 15:33:13.000000 powerprofile-0.9.0/setup.cfg
--rw-rw-r--   0 afita     (1000) afita     (1000)     1102 2021-12-28 15:29:39.000000 powerprofile-0.9.0/setup.py
--rw-r--r--   0 afita     (1000) afita     (1000)       41 2020-11-17 16:33:16.000000 powerprofile-0.9.0/requirements-dev.txt
--rw-r--r--   0 afita     (1000) afita     (1000)    34520 2020-03-06 07:34:05.000000 powerprofile-0.9.0/LICENSE
--rw-r--r--   0 afita     (1000) afita     (1000)       70 2020-03-31 13:12:37.000000 powerprofile-0.9.0/MANIFEST.in
--rw-r--r--   0 afita     (1000) afita     (1000)      129 2020-03-31 13:31:34.000000 powerprofile-0.9.0/README.md
--rw-r--r--   0 afita     (1000) afita     (1000)       20 2020-03-31 13:22:43.000000 powerprofile-0.9.0/requirements.txt
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-29 16:48:36.000000 powerprofile-0.9.1/
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-29 16:48:36.000000 powerprofile-0.9.1/powerprofile.egg-info/
+-rw-r--r--   0 afita     (1000) afita     (1000)       13 2021-12-29 16:48:36.000000 powerprofile-0.9.1/powerprofile.egg-info/top_level.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      346 2021-12-29 16:48:36.000000 powerprofile-0.9.1/powerprofile.egg-info/SOURCES.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      731 2021-12-29 16:48:36.000000 powerprofile-0.9.1/powerprofile.egg-info/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)        1 2021-12-29 16:48:36.000000 powerprofile-0.9.1/powerprofile.egg-info/dependency_links.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)       20 2021-12-29 16:48:36.000000 powerprofile-0.9.1/powerprofile.egg-info/requires.txt
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-29 16:48:36.000000 powerprofile-0.9.1/powerprofile/
+-rw-rw-r--   0 afita     (1000) afita     (1000)    14007 2021-12-29 16:47:10.000000 powerprofile-0.9.1/powerprofile/powerprofile.py
+-rw-r--r--   0 afita     (1000) afita     (1000)      117 2020-04-16 15:12:51.000000 powerprofile-0.9.1/powerprofile/__init__.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)     1000 2021-12-28 15:29:26.000000 powerprofile-0.9.1/powerprofile/exceptions.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)      731 2021-12-29 16:48:36.000000 powerprofile-0.9.1/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)       38 2021-12-29 16:48:36.000000 powerprofile-0.9.1/setup.cfg
+-rw-rw-r--   0 afita     (1000) afita     (1000)     1102 2021-12-29 16:47:20.000000 powerprofile-0.9.1/setup.py
+-rw-r--r--   0 afita     (1000) afita     (1000)       41 2020-11-17 16:33:16.000000 powerprofile-0.9.1/requirements-dev.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)    34520 2020-03-06 07:34:05.000000 powerprofile-0.9.1/LICENSE
+-rw-r--r--   0 afita     (1000) afita     (1000)       70 2020-03-31 13:12:37.000000 powerprofile-0.9.1/MANIFEST.in
+-rw-r--r--   0 afita     (1000) afita     (1000)      129 2020-03-31 13:31:34.000000 powerprofile-0.9.1/README.md
+-rw-r--r--   0 afita     (1000) afita     (1000)       20 2020-03-31 13:22:43.000000 powerprofile-0.9.1/requirements.txt
```

### Comparing `powerprofile-0.9.0/powerprofile.egg-info/PKG-INFO` & `powerprofile-0.9.1/powerprofile.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerprofile
-Version: 0.9.0
+Version: 0.9.1
 Summary: Library to manage power profiles
 Home-page: https://github.com/gisce/powerprofile
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: GNU Affero General Public License v3
 Description: # powerprofile
         Electric Power Curve and Profiles library
```

### Comparing `powerprofile-0.9.0/powerprofile/powerprofile.py` & `powerprofile-0.9.1/powerprofile/powerprofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,21 +98,19 @@
         Given a list of fields, check all values are True in every register
         :param fields []:
         :return: list
         """
         for field in fields:
             try:
                 data = self.curve.loc[self.curve[field] == False]
+                if len(data) > 0:
+                    return False
             except KeyError as e:
                 raise PowerProfileMissingField(field)
-
-            if len(data) > 0:
-                return False
-            else:
-                return True
+        return True
 
     def has_duplicates(self):
         ''' Checks for duplicated hours'''
         uniques = len(self.curve[self.datetime_field].unique())
         if uniques != self.hours:
             return True
         return False
```

### Comparing `powerprofile-0.9.0/powerprofile/exceptions.py` & `powerprofile-0.9.1/powerprofile/exceptions.py`

 * *Files identical despite different names*

### Comparing `powerprofile-0.9.0/PKG-INFO` & `powerprofile-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerprofile
-Version: 0.9.0
+Version: 0.9.1
 Summary: Library to manage power profiles
 Home-page: https://github.com/gisce/powerprofile
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: GNU Affero General Public License v3
 Description: # powerprofile
         Electric Power Curve and Profiles library
```

### Comparing `powerprofile-0.9.0/setup.py` & `powerprofile-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     TEST_REQUIRES = [x.strip() for x in f.readlines()]
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="powerprofile",
-    version="0.9.0",
+    version="0.9.1",
     author="GISCE-TI, S.L.",
     author_email="devel@gisce.net",
     description=("Library to manage power profiles"),
     long_description=readme,
     long_description_content_type="text/x-markdown",
     url="https://github.com/gisce/powerprofile",
     license="GNU Affero General Public License v3",
```

### Comparing `powerprofile-0.9.0/LICENSE` & `powerprofile-0.9.1/LICENSE`

 * *Files identical despite different names*

