# Comparing `tmp/zest.pocompile-1.6.0.tar.gz` & `tmp/zest.pocompile-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zest.pocompile-1.6.0.tar", last modified: Tue Sep 13 21:04:01 2022, max compression
+gzip compressed data, was "zest.pocompile-2.0.0a1.tar", last modified: Thu Jul 13 21:38:06 2023, max compression
```

## Comparing `zest.pocompile-1.6.0.tar` & `zest.pocompile-2.0.0a1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-13 21:04:01.027965 zest.pocompile-1.6.0/
--rw-r--r--   0 maurits    (501) staff       (20)     1425 2022-09-13 21:03:59.000000 zest.pocompile-1.6.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       45 2022-09-13 21:03:59.000000 zest.pocompile-1.6.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     7979 2022-09-13 21:04:01.028052 zest.pocompile-1.6.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5677 2022-09-13 21:03:59.000000 zest.pocompile-1.6.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)       67 2022-09-13 21:04:01.028489 zest.pocompile-1.6.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1552 2022-09-13 21:03:59.000000 zest.pocompile-1.6.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-13 21:04:01.025336 zest.pocompile-1.6.0/zest/
--rw-r--r--   0 maurits    (501) staff       (20)      245 2022-09-13 21:03:59.000000 zest.pocompile-1.6.0/zest/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-13 21:04:01.027797 zest.pocompile-1.6.0/zest/pocompile/
--rw-r--r--   0 maurits    (501) staff       (20)       37 2022-09-13 21:03:59.000000 zest.pocompile-1.6.0/zest/pocompile/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4070 2022-09-13 21:03:59.000000 zest.pocompile-1.6.0/zest/pocompile/compile.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-13 21:04:01.027365 zest.pocompile-1.6.0/zest.pocompile.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     7979 2022-09-13 21:04:00.000000 zest.pocompile-1.6.0/zest.pocompile.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      437 2022-09-13 21:04:00.000000 zest.pocompile-1.6.0/zest.pocompile.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-09-13 21:04:00.000000 zest.pocompile-1.6.0/zest.pocompile.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      154 2022-09-13 21:04:00.000000 zest.pocompile-1.6.0/zest.pocompile.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2022-09-13 21:04:00.000000 zest.pocompile-1.6.0/zest.pocompile.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-09-13 21:04:00.000000 zest.pocompile-1.6.0/zest.pocompile.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       26 2022-09-13 21:04:00.000000 zest.pocompile-1.6.0/zest.pocompile.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2022-09-13 21:04:00.000000 zest.pocompile-1.6.0/zest.pocompile.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:38:06.117040 zest.pocompile-2.0.0a1/
+-rw-r--r--   0 maurits    (501) staff       (20)     1611 2023-07-13 21:38:05.000000 zest.pocompile-2.0.0a1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       45 2023-07-13 21:38:05.000000 zest.pocompile-2.0.0a1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     8125 2023-07-13 21:38:06.116847 zest.pocompile-2.0.0a1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5677 2023-07-13 21:38:05.000000 zest.pocompile-2.0.0a1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       71 2023-07-13 21:38:05.000000 zest.pocompile-2.0.0a1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-13 21:38:06.117144 zest.pocompile-2.0.0a1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1529 2023-07-13 21:38:05.000000 zest.pocompile-2.0.0a1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:38:06.112752 zest.pocompile-2.0.0a1/zest/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:38:06.116569 zest.pocompile-2.0.0a1/zest/pocompile/
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2023-07-13 21:38:05.000000 zest.pocompile-2.0.0a1/zest/pocompile/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4041 2023-07-13 21:38:05.000000 zest.pocompile-2.0.0a1/zest/pocompile/compile.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:38:06.115911 zest.pocompile-2.0.0a1/zest.pocompile.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     8125 2023-07-13 21:38:06.000000 zest.pocompile-2.0.0a1/zest.pocompile.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      378 2023-07-13 21:38:06.000000 zest.pocompile-2.0.0a1/zest.pocompile.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 21:38:06.000000 zest.pocompile-2.0.0a1/zest.pocompile.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      154 2023-07-13 21:38:06.000000 zest.pocompile-2.0.0a1/zest.pocompile.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 21:38:06.000000 zest.pocompile-2.0.0a1/zest.pocompile.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2023-07-13 21:38:06.000000 zest.pocompile-2.0.0a1/zest.pocompile.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        5 2023-07-13 21:38:06.000000 zest.pocompile-2.0.0a1/zest.pocompile.egg-info/top_level.txt
```

### Comparing `zest.pocompile-1.6.0/CHANGES.rst` & `zest.pocompile-2.0.0a1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+2.0.0a1 (2023-07-13)
+--------------------
+
+- Require Python 3.8+ and switch to native namespace packages.
+  This is needed because ``zest.releaser`` 9.0.0a1 does the same.
+  [maurits]
+
+
 1.6.0 (2022-09-13)
 ------------------
 
 - Add ``zest.pocompile.available``.
   You can use this to let the full release of a package fail early when ``zest.pocompile`` is not available.
   Edit its ``setup.cfg``, and add a ``[zest.releaser]`` section with value
   ``prereleaser.before = zest.pocompile.available``
```

### Comparing `zest.pocompile-1.6.0/PKG-INFO` & `zest.pocompile-2.0.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: zest.pocompile
-Version: 1.6.0
+Version: 2.0.0a1
 Summary: Compile po files when releasing a package
 Home-page: https://github.com/zestsoftware/zest.pocompile
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL
 Keywords: i18n locales po compile release
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Buildout
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Internationalization
+Requires-Python: >=3.8
 
 Introduction
 ============
 
 This package compiles po files.
 It contains a `zest.releaser`_ entrypoint and a stand-alone command line tool.
 
@@ -148,14 +147,22 @@
 
 
 .. _`zest.releaser`: https://pypi.org/project/zest.releaser/
 
 Changelog
 =========
 
+2.0.0a1 (2023-07-13)
+--------------------
+
+- Require Python 3.8+ and switch to native namespace packages.
+  This is needed because ``zest.releaser`` 9.0.0a1 does the same.
+  [maurits]
+
+
 1.6.0 (2022-09-13)
 ------------------
 
 - Add ``zest.pocompile.available``.
   You can use this to let the full release of a package fail early when ``zest.pocompile`` is not available.
   Edit its ``setup.cfg``, and add a ``[zest.releaser]`` section with value
   ``prereleaser.before = zest.pocompile.available``
@@ -207,8 +214,7 @@
 
 
 1.0 (2010-10-19)
 ----------------
 
 - Initial release
 
-
```

### Comparing `zest.pocompile-1.6.0/README.rst` & `zest.pocompile-2.0.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `zest.pocompile-1.6.0/setup.py` & `zest.pocompile-2.0.0a1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-from setuptools import find_packages
+from pathlib import Path
 from setuptools import setup
 
 
-version = "1.6.0"
+version = "2.0.0a1"
+long_description = (
+    f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}\n"
+)
 
 setup(
     name="zest.pocompile",
     version=version,
     description="Compile po files when releasing a package",
-    long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
+    long_description=long_description,
     # Get more strings from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Buildout",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Internationalization",
     ],
     keywords="i18n locales po compile release",
     author="Maurits van Rees",
     author_email="m.van.rees@zestsoftware.nl",
     url="https://github.com/zestsoftware/zest.pocompile",
     license="GPL",
-    packages=find_packages(exclude=["ez_setup"]),
-    namespace_packages=["zest"],
+    packages=["zest.pocompile"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=["setuptools", "python-gettext"],
     entry_points={
         "console_scripts": ["pocompile = zest.pocompile.compile:main"],
         "zest.releaser.releaser.after_checkout": [
             "zest_pocompile = zest.pocompile.compile:compile_in_tag",
         ],
     },
```

### Comparing `zest.pocompile-1.6.0/zest/pocompile/compile.py` & `zest.pocompile-2.0.0a1/zest/pocompile/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Compiles po files.
 
 This walks through the given directories, finds all po translation
 files in a properly formed locales directory and compiles them info mo
 files.
 
 When no directories are specified, the current directory is taken.
@@ -96,16 +95,15 @@
                 "languages have no working translations.  Do you want "
                 "to continue with the release?"
             ):
                 sys.exit(1)
 
 
 def main(*args, **kwargs):
-    """Run as stand-alone program.
-    """
+    """Run as stand-alone program."""
     logging.basicConfig(level=logging.INFO, format="%(levelname)s: %(message)s")
 
     # Parsing arguments.  Note that the parse_args call might already
     # stop the program, displaying a help or usage message.
     usage = "usage: %prog [options] <directories>"
     parser = OptionParser(usage=usage, description=__doc__)
     parser.add_option(
```

### Comparing `zest.pocompile-1.6.0/zest.pocompile.egg-info/PKG-INFO` & `zest.pocompile-2.0.0a1/zest.pocompile.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: zest.pocompile
-Version: 1.6.0
+Version: 2.0.0a1
 Summary: Compile po files when releasing a package
 Home-page: https://github.com/zestsoftware/zest.pocompile
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL
 Keywords: i18n locales po compile release
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Buildout
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Internationalization
+Requires-Python: >=3.8
 
 Introduction
 ============
 
 This package compiles po files.
 It contains a `zest.releaser`_ entrypoint and a stand-alone command line tool.
 
@@ -148,14 +147,22 @@
 
 
 .. _`zest.releaser`: https://pypi.org/project/zest.releaser/
 
 Changelog
 =========
 
+2.0.0a1 (2023-07-13)
+--------------------
+
+- Require Python 3.8+ and switch to native namespace packages.
+  This is needed because ``zest.releaser`` 9.0.0a1 does the same.
+  [maurits]
+
+
 1.6.0 (2022-09-13)
 ------------------
 
 - Add ``zest.pocompile.available``.
   You can use this to let the full release of a package fail early when ``zest.pocompile`` is not available.
   Edit its ``setup.cfg``, and add a ``[zest.releaser]`` section with value
   ``prereleaser.before = zest.pocompile.available``
@@ -207,8 +214,7 @@
 
 
 1.0 (2010-10-19)
 ----------------
 
 - Initial release
 
-
```

