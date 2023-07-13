# Comparing `tmp/pyexifwrangle-0.1.1.tar.gz` & `tmp/pyexifwrangle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyexifwrangle-0.1.1.tar", last modified: Wed Jul 12 18:35:05 2023, max compression
+gzip compressed data, was "dist/pyexifwrangle-0.1.2.tar", last modified: Thu Jul 13 15:40:02 2023, max compression
```

## Comparing `pyexifwrangle-0.1.1.tar` & `pyexifwrangle-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/
--rw-r--r--   0 stephanie   (501) staff       (20)      589 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/PKG-INFO
--rw-r--r--   0 stephanie   (501) staff       (20)      609 2023-07-03 15:33:11.000000 pyexifwrangle-0.1.1/README.md
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle/
--rw-r--r--   0 stephanie   (501) staff       (20)      132 2023-07-12 18:27:14.000000 pyexifwrangle-0.1.1/pyexifwrangle/__init__.py
--rw-r--r--   0 stephanie   (501) staff       (20)     2690 2023-07-12 18:15:44.000000 pyexifwrangle-0.1.1/pyexifwrangle/wrangle.py
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/
--rw-r--r--   0 stephanie   (501) staff       (20)      589 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/PKG-INFO
--rw-r--r--   0 stephanie   (501) staff       (20)      253 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/SOURCES.txt
--rw-r--r--   0 stephanie   (501) staff       (20)        1 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/dependency_links.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/requires.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       14 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/top_level.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/setup.cfg
--rw-r--r--   0 stephanie   (501) staff       (20)      915 2023-07-05 13:58:25.000000 pyexifwrangle-0.1.1/setup.py
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/
+-rw-r--r--   0 stephanie   (501) staff       (20)     5328 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/PKG-INFO
+-rw-r--r--   0 stephanie   (501) staff       (20)     3898 2023-07-13 15:33:15.000000 pyexifwrangle-0.1.2/README.md
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/pyexifwrangle/
+-rw-r--r--   0 stephanie   (501) staff       (20)      132 2023-07-13 15:36:05.000000 pyexifwrangle-0.1.2/pyexifwrangle/__init__.py
+-rw-r--r--   0 stephanie   (501) staff       (20)     2690 2023-07-12 18:15:44.000000 pyexifwrangle-0.1.2/pyexifwrangle/wrangle.py
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/
+-rw-r--r--   0 stephanie   (501) staff       (20)     5328 2023-07-13 15:40:01.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/PKG-INFO
+-rw-r--r--   0 stephanie   (501) staff       (20)      253 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/SOURCES.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)        1 2023-07-13 15:40:01.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/dependency_links.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-13 15:40:01.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/requires.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       14 2023-07-13 15:40:01.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/top_level.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/setup.cfg
+-rw-r--r--   0 stephanie   (501) staff       (20)     1167 2023-07-13 15:34:41.000000 pyexifwrangle-0.1.2/setup.py
```

### Comparing `pyexifwrangle-0.1.1/pyexifwrangle/wrangle.py` & `pyexifwrangle-0.1.2/pyexifwrangle/wrangle.py`

 * *Files identical despite different names*

### Comparing `pyexifwrangle-0.1.1/setup.py` & `pyexifwrangle-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 from pyexifwrangle import __version__
 
+# read the contents of README file
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 extra_test = [
     'pytest>=4',
     'pytest-cov>=2',
 ]
 
 extra_dev = [
     *extra_test,
 ]
 
 setup(
     name='pyexifwrangle',
     version=__version__,
     description='A helper package for wrangling image EXIF data',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/stephaniereinders/pyexifwrangle',
     author='Stephanie Reinders',
     author_email='reinders.stephanie@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['tests', 'tests.*']),
 
     classifiers=[
```

