# Comparing `tmp/PythonODFTemplator-1.1.tar.gz` & `tmp/PythonODFTemplator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonODFTemplator-1.1.tar", last modified: Fri Mar  3 04:41:55 2023, max compression
+gzip compressed data, was "PythonODFTemplator-1.1.1.tar", last modified: Thu Jul 13 02:27:28 2023, max compression
```

## Comparing `PythonODFTemplator-1.1.tar` & `PythonODFTemplator-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 marvelph   (501) staff       (20)        0 2023-03-03 04:41:55.502604 PythonODFTemplator-1.1/
--rw-r--r--   0 marvelph   (501) staff       (20)     1078 2023-03-03 02:59:50.000000 PythonODFTemplator-1.1/LICENSE
--rw-r--r--   0 marvelph   (501) staff       (20)     1284 2023-03-03 04:41:55.502650 PythonODFTemplator-1.1/PKG-INFO
-drwxr-xr-x   0 marvelph   (501) staff       (20)        0 2023-03-03 04:41:55.502506 PythonODFTemplator-1.1/PythonODFTemplator.egg-info/
--rw-r--r--   0 marvelph   (501) staff       (20)     1284 2023-03-03 04:41:55.000000 PythonODFTemplator-1.1/PythonODFTemplator.egg-info/PKG-INFO
--rw-r--r--   0 marvelph   (501) staff       (20)      261 2023-03-03 04:41:55.000000 PythonODFTemplator-1.1/PythonODFTemplator.egg-info/SOURCES.txt
--rw-r--r--   0 marvelph   (501) staff       (20)        1 2023-03-03 04:41:55.000000 PythonODFTemplator-1.1/PythonODFTemplator.egg-info/dependency_links.txt
--rw-r--r--   0 marvelph   (501) staff       (20)       15 2023-03-03 04:41:55.000000 PythonODFTemplator-1.1/PythonODFTemplator.egg-info/requires.txt
--rw-r--r--   0 marvelph   (501) staff       (20)       13 2023-03-03 04:41:55.000000 PythonODFTemplator-1.1/PythonODFTemplator.egg-info/top_level.txt
--rw-r--r--   0 marvelph   (501) staff       (20)      598 2023-01-06 09:16:13.000000 PythonODFTemplator-1.1/README.md
--rw-r--r--   0 marvelph   (501) staff       (20)     3812 2023-03-03 02:02:09.000000 PythonODFTemplator-1.1/odftemplator.py
--rw-r--r--   0 marvelph   (501) staff       (20)      776 2023-03-03 04:41:55.502863 PythonODFTemplator-1.1/setup.cfg
--rw-r--r--   0 marvelph   (501) staff       (20)       59 2023-01-06 09:16:13.000000 PythonODFTemplator-1.1/setup.py
+drwxr-xr-x   0 marvelph   (501) staff       (20)        0 2023-07-13 02:27:28.770591 PythonODFTemplator-1.1.1/
+-rw-r--r--   0 marvelph   (501) staff       (20)     1078 2023-03-03 02:59:50.000000 PythonODFTemplator-1.1.1/LICENSE
+-rw-r--r--   0 marvelph   (501) staff       (20)     1286 2023-07-13 02:27:28.770658 PythonODFTemplator-1.1.1/PKG-INFO
+drwxr-xr-x   0 marvelph   (501) staff       (20)        0 2023-07-13 02:27:28.770460 PythonODFTemplator-1.1.1/PythonODFTemplator.egg-info/
+-rw-r--r--   0 marvelph   (501) staff       (20)     1286 2023-07-13 02:27:28.000000 PythonODFTemplator-1.1.1/PythonODFTemplator.egg-info/PKG-INFO
+-rw-r--r--   0 marvelph   (501) staff       (20)      261 2023-07-13 02:27:28.000000 PythonODFTemplator-1.1.1/PythonODFTemplator.egg-info/SOURCES.txt
+-rw-r--r--   0 marvelph   (501) staff       (20)        1 2023-07-13 02:27:28.000000 PythonODFTemplator-1.1.1/PythonODFTemplator.egg-info/dependency_links.txt
+-rw-r--r--   0 marvelph   (501) staff       (20)       15 2023-07-13 02:27:28.000000 PythonODFTemplator-1.1.1/PythonODFTemplator.egg-info/requires.txt
+-rw-r--r--   0 marvelph   (501) staff       (20)       13 2023-07-13 02:27:28.000000 PythonODFTemplator-1.1.1/PythonODFTemplator.egg-info/top_level.txt
+-rw-r--r--   0 marvelph   (501) staff       (20)      598 2023-01-06 09:16:13.000000 PythonODFTemplator-1.1.1/README.md
+-rw-r--r--   0 marvelph   (501) staff       (20)     3907 2023-07-13 02:09:57.000000 PythonODFTemplator-1.1.1/odftemplator.py
+-rw-r--r--   0 marvelph   (501) staff       (20)      778 2023-07-13 02:27:28.770916 PythonODFTemplator-1.1.1/setup.cfg
+-rw-r--r--   0 marvelph   (501) staff       (20)       59 2023-01-06 09:16:13.000000 PythonODFTemplator-1.1.1/setup.py
```

### Comparing `PythonODFTemplator-1.1/LICENSE` & `PythonODFTemplator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonODFTemplator-1.1/PKG-INFO` & `PythonODFTemplator-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonODFTemplator
-Version: 1.1
+Version: 1.1.1
 Summary: ODF templating library for python.
 Home-page: https://github.com/marvelph/PythonODFTemplator
 Author: Kenji Nishishiro
 Author-email: marvel@programmershigh.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PythonODFTemplator-1.1/PythonODFTemplator.egg-info/PKG-INFO` & `PythonODFTemplator-1.1.1/PythonODFTemplator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonODFTemplator
-Version: 1.1
+Version: 1.1.1
 Summary: ODF templating library for python.
 Home-page: https://github.com/marvelph/PythonODFTemplator
 Author: Kenji Nishishiro
 Author-email: marvel@programmershigh.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PythonODFTemplator-1.1/README.md` & `PythonODFTemplator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PythonODFTemplator-1.1/odftemplator.py` & `PythonODFTemplator-1.1.1/odftemplator.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
                     with pylokit.Office(self.__libreoffice_path) as office:
                         with office.documentLoad(document_file_path) as document:
                             document.saveAs(pdf_file_path)
                 elif self.__libreoffice_method == "command":
                     subprocess.call(
                         [
                             self.__libreoffice_path,
+                            "-env:UserInstallation=file://{}".format(document_directory_path),
                             "--convert-to",
                             "pdf",
                             "--outdir",
                             os.path.dirname(pdf_file_path),
                             document_file_path,
                         ]
                     )
```

### Comparing `PythonODFTemplator-1.1/setup.cfg` & `PythonODFTemplator-1.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PythonODFTemplator
-version = 1.1
+version = 1.1.1
 url = https://github.com/marvelph/PythonODFTemplator
 author = Kenji Nishishiro
 author_email = marvel@programmershigh.org
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
```

