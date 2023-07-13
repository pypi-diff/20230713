# Comparing `tmp/helperfns-0.0.5.tar.gz` & `tmp/helperfns-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\helperfns-0.0.5.tar", last modified: Thu Jul 13 11:20:16 2023, max compression
+gzip compressed data, was "dist\helperfns-0.0.6.tar", last modified: Thu Jul 13 11:24:38 2023, max compression
```

## Comparing `helperfns-0.0.5.tar` & `helperfns-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.117739 helperfns-0.0.5/
--rw-rw-rw-   0        0        0     1089 2022-07-19 04:53:06.000000 helperfns-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     8507 2023-07-13 11:20:16.107741 helperfns-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6791 2023-07-13 11:18:11.000000 helperfns-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:15.987743 helperfns-0.0.5/helperfns/
--rw-rw-rw-   0        0        0        0 2022-07-19 06:30:21.000000 helperfns-0.0.5/helperfns/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.077741 helperfns-0.0.5/helperfns/tables/
--rw-rw-rw-   0        0        0     1917 2023-07-03 10:15:06.000000 helperfns-0.0.5/helperfns/tables/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.083742 helperfns-0.0.5/helperfns/text/
--rw-rw-rw-   0        0        0     4766 2022-09-01 09:10:36.000000 helperfns-0.0.5/helperfns/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.088742 helperfns-0.0.5/helperfns/torch/
--rw-rw-rw-   0        0        0        0 2022-09-01 09:23:02.000000 helperfns-0.0.5/helperfns/torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.090741 helperfns-0.0.5/helperfns/torch/accuracy/
--rw-rw-rw-   0        0        0     1981 2022-08-25 07:48:07.000000 helperfns-0.0.5/helperfns/torch/accuracy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.094743 helperfns-0.0.5/helperfns/torch/models/
--rw-rw-rw-   0        0        0      971 2022-09-06 05:59:54.000000 helperfns-0.0.5/helperfns/torch/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.098742 helperfns-0.0.5/helperfns/torch/text/
--rw-rw-rw-   0        0        0     4848 2022-09-01 10:27:12.000000 helperfns-0.0.5/helperfns/torch/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.101741 helperfns-0.0.5/helperfns/utils/
--rw-rw-rw-   0        0        0      775 2022-08-25 07:27:13.000000 helperfns-0.0.5/helperfns/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.104740 helperfns-0.0.5/helperfns/visualization/
--rw-rw-rw-   0        0        0    12054 2023-07-13 11:18:19.000000 helperfns-0.0.5/helperfns/visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.069740 helperfns-0.0.5/helperfns.egg-info/
--rw-rw-rw-   0        0        0     8507 2023-07-13 11:20:11.000000 helperfns-0.0.5/helperfns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-07-13 11:20:15.000000 helperfns-0.0.5/helperfns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 11:20:11.000000 helperfns-0.0.5/helperfns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-07-13 11:20:13.000000 helperfns-0.0.5/helperfns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 11:20:14.000000 helperfns-0.0.5/helperfns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 11:20:16.119740 helperfns-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2157 2023-07-13 11:18:07.000000 helperfns-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.195171 helperfns-0.0.6/
+-rw-rw-rw-   0        0        0     1089 2022-07-19 04:53:06.000000 helperfns-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     8507 2023-07-13 11:24:38.177169 helperfns-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6791 2023-07-13 11:18:11.000000 helperfns-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.020171 helperfns-0.0.6/helperfns/
+-rw-rw-rw-   0        0        0        0 2022-07-19 06:30:21.000000 helperfns-0.0.6/helperfns/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.100172 helperfns-0.0.6/helperfns/tables/
+-rw-rw-rw-   0        0        0     1917 2023-07-03 10:15:06.000000 helperfns-0.0.6/helperfns/tables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.104171 helperfns-0.0.6/helperfns/text/
+-rw-rw-rw-   0        0        0     4766 2022-09-01 09:10:36.000000 helperfns-0.0.6/helperfns/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.107168 helperfns-0.0.6/helperfns/torch/
+-rw-rw-rw-   0        0        0        0 2022-09-01 09:23:02.000000 helperfns-0.0.6/helperfns/torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.127172 helperfns-0.0.6/helperfns/torch/accuracy/
+-rw-rw-rw-   0        0        0     1981 2022-08-25 07:48:07.000000 helperfns-0.0.6/helperfns/torch/accuracy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.137172 helperfns-0.0.6/helperfns/torch/models/
+-rw-rw-rw-   0        0        0      971 2022-09-06 05:59:54.000000 helperfns-0.0.6/helperfns/torch/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.146171 helperfns-0.0.6/helperfns/torch/text/
+-rw-rw-rw-   0        0        0     4848 2022-09-01 10:27:12.000000 helperfns-0.0.6/helperfns/torch/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.159167 helperfns-0.0.6/helperfns/utils/
+-rw-rw-rw-   0        0        0      775 2022-08-25 07:27:13.000000 helperfns-0.0.6/helperfns/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.173168 helperfns-0.0.6/helperfns/visualization/
+-rw-rw-rw-   0        0        0    12054 2023-07-13 11:18:19.000000 helperfns-0.0.6/helperfns/visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.095171 helperfns-0.0.6/helperfns.egg-info/
+-rw-rw-rw-   0        0        0     8507 2023-07-13 11:24:34.000000 helperfns-0.0.6/helperfns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-07-13 11:24:37.000000 helperfns-0.0.6/helperfns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 11:24:35.000000 helperfns-0.0.6/helperfns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-13 11:24:36.000000 helperfns-0.0.6/helperfns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 11:24:36.000000 helperfns-0.0.6/helperfns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 11:24:38.202191 helperfns-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2157 2023-07-13 11:24:08.000000 helperfns-0.0.6/setup.py
```

### Comparing `helperfns-0.0.5/LICENSE` & `helperfns-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/PKG-INFO` & `helperfns-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helperfns
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package provide some python helper functions that are useful in machine learning.
 Author: Crispen Gari
 Author-email: <crispengari@gmail.com>
 Keywords: helperfns,python,python3,helper-functions,text cleaning,visualization,machine-learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `helperfns-0.0.5/README.md` & `helperfns-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/helperfns/tables/__init__.py` & `helperfns-0.0.6/helperfns/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/helperfns/text/__init__.py` & `helperfns-0.0.6/helperfns/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/helperfns/torch/accuracy/__init__.py` & `helperfns-0.0.6/helperfns/torch/accuracy/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/helperfns/torch/models/__init__.py` & `helperfns-0.0.6/helperfns/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/helperfns/torch/text/__init__.py` & `helperfns-0.0.6/helperfns/torch/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/helperfns/utils/__init__.py` & `helperfns-0.0.6/helperfns/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/helperfns/visualization/__init__.py` & `helperfns-0.0.6/helperfns/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.5/helperfns.egg-info/PKG-INFO` & `helperfns-0.0.6/helperfns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helperfns
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package provide some python helper functions that are useful in machine learning.
 Author: Crispen Gari
 Author-email: <crispengari@gmail.com>
 Keywords: helperfns,python,python3,helper-functions,text cleaning,visualization,machine-learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `helperfns-0.0.5/setup.py` & `helperfns-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "This package provide some python helper functions that are useful in machine learning."
 # setting up
 setup(
     name="helperfns",
     version=VERSION,
     author="Crispen Gari",
     author_email="<crispengari@gmail.com>",
```

