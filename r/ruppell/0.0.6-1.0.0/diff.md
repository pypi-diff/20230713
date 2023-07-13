# Comparing `tmp/ruppell-0.0.6.tar.gz` & `tmp/ruppell-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ruppell-0.0.6.tar", last modified: Thu Apr 23 20:40:52 2020, max compression
+gzip compressed data, was "ruppell-1.0.0.tar", last modified: Thu Jul 13 19:14:56 2023, max compression
```

## Comparing `ruppell-0.0.6.tar` & `ruppell-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 jorge.melgarejo (132277) domain users (131512)        0 2020-04-23 20:40:52.000000 ruppell-0.0.6/
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)       79 2020-04-23 20:40:52.000000 ruppell-0.0.6/setup.cfg
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      371 2020-04-23 20:40:52.000000 ruppell-0.0.6/PKG-INFO
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)        0 2020-04-22 21:51:54.000000 ruppell-0.0.6/__init__.py
-drwxr-xr-x   0 jorge.melgarejo (132277) domain users (131512)        0 2020-04-23 20:40:52.000000 ruppell-0.0.6/readers/
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)       53 2020-04-22 21:45:55.000000 ruppell-0.0.6/readers/__init__.py
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      413 2020-04-15 00:31:24.000000 ruppell-0.0.6/readers/AbstractReader.py
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      275 2020-04-16 21:57:43.000000 ruppell-0.0.6/readers/DocxReader.py
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      495 2020-04-20 18:19:01.000000 ruppell-0.0.6/readers/ImageReader.py
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      293 2020-04-23 01:06:54.000000 ruppell-0.0.6/readers/PdfReader.py
-drwxr-xr-x   0 jorge.melgarejo (132277) domain users (131512)        0 2020-04-23 20:40:52.000000 ruppell-0.0.6/utils/
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)        0 2020-04-16 23:13:51.000000 ruppell-0.0.6/utils/__init__.py
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      488 2020-04-23 01:05:49.000000 ruppell-0.0.6/utils/utils.py
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)     1874 2020-04-23 20:31:19.000000 ruppell-0.0.6/ruppell.py
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)     2498 2020-04-23 20:34:08.000000 ruppell-0.0.6/README.md
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      927 2020-04-23 20:34:31.000000 ruppell-0.0.6/setup.py
-drwxr-xr-x   0 jorge.melgarejo (132277) domain users (131512)        0 2020-04-23 20:40:52.000000 ruppell-0.0.6/ruppell.egg-info/
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      350 2020-04-23 20:40:52.000000 ruppell-0.0.6/ruppell.egg-info/SOURCES.txt
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      371 2020-04-23 20:40:52.000000 ruppell-0.0.6/ruppell.egg-info/PKG-INFO
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)      103 2020-04-23 20:40:52.000000 ruppell-0.0.6/ruppell.egg-info/requires.txt
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)        1 2020-04-23 20:40:52.000000 ruppell-0.0.6/ruppell.egg-info/dependency_links.txt
--rw-r--r--   0 jorge.melgarejo (132277) domain users (131512)       15 2020-04-23 20:40:52.000000 ruppell-0.0.6/ruppell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:56.807659 ruppell-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 19:14:45.000000 ruppell-1.0.0/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 19:14:45.000000 ruppell-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 19:14:45.000000 ruppell-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-13 19:14:56.807659 ruppell-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-13 19:14:45.000000 ruppell-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:45.000000 ruppell-1.0.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:56.807659 ruppell-1.0.0/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/AbstractReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/DocxReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/ImageReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/PdfReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 19:14:45.000000 ruppell-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:56.807659 ruppell-1.0.0/ruppell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-13 19:14:45.000000 ruppell-1.0.0/ruppell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 19:14:56.807659 ruppell-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 19:14:45.000000 ruppell-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:56.807659 ruppell-1.0.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:45.000000 ruppell-1.0.0/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-13 19:14:45.000000 ruppell-1.0.0/utils/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ruppell-0.0.6/ruppell.py` & `ruppell-1.0.0/ruppell.py`

 * *Files identical despite different names*

### Comparing `ruppell-0.0.6/README.md` & `ruppell-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ## How to use
 
 ```python
 import ruppell
 
 
 # Configure your documents language, defaults to eng if not specified!
-ruppell.setup_language(language='documents_lang')
+ruppell.setup_language(language='eng')
 
 
 # Extract text from pdf
 text = ruppell.pdf_to_string(file_path='file_path.pdf')
 
 
 # Extract text from docx
@@ -71,16 +71,14 @@
 >>> import ruppell
 >>> ruppell.image_to_string('image.png')
 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer id bibendum sapien.'
 ```
 
 ## Supported Languages
 
-All supported languages can be found [here](http://succeed-project.eu/wiki/index.php/Tesseract_3.02#Supported_languages).
-
 The language codes are **ISO 639-2/B** or **ISO 639-2/T**.
 
 All languages codes [here](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes).
 
 ## Contributing
 	
 If you think that we can do the Ruppell more powerful please contribute with this project. And let's improve it to help other developers.
```

### Comparing `ruppell-0.0.6/setup.py` & `ruppell-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
-with open("README.md", "r") as fh:
+with open("DESCRIPTION.md", "r") as fh:
     long_description = fh.read()
 
 PACKAGE_NAME = 'ruppell'
 PACKAGES = ['', 'readers', 'utils']
-VERSION = '0.0.6'
+VERSION = '1.0.0'
 DESCRIPTION = "Ruppell is a Python package to help in text extraction from documents."
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     url='https://github.com/joorgelm/ruppell',
     download_url=f'https://github.com/joorgelm/ruppell/archive/{VERSION}.tar.gz',
     package_dir={PACKAGE_NAME: ''},
     packages=PACKAGES,
     license='MIT License',
     author='Jorge Melgarejo',
     author_email='melgarejo.colarte@gmail.com',
     keywords='ocr text extractor',
-    description=u'text extractor based in tesseract ocr',
+    long_description_content_type='text/markdown',
+    description=DESCRIPTION,
+    long_description=long_description,
     install_requires=[
-        'Pillow>=7.0.0',
-        'pytesseract>=0.3.1',
-        'setuptools>=46.1.3',
-        'pdfminer.six>=20200402',
-        'docx2txt>=0.8',
-        'pandas>=1.0.3'
+        'Pillow~=10.0.0',
+        'pytesseract~=0.3.10',
+        'setuptools~=68.0.0',
+        'pdfminer.six==20221105',
+        'docx2txt~=0.8',
+        'pandas~=2.0.3'
     ],
 )
```

