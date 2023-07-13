# Comparing `tmp/embeddingcache-0.0.1.tar.gz` & `tmp/embeddingcache-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embeddingcache-0.0.1.tar", last modified: Thu Jul 13 12:21:26 2023, max compression
+gzip compressed data, was "embeddingcache-0.1.0.tar", last modified: Thu Jul 13 16:29:24 2023, max compression
```

## Comparing `embeddingcache-0.0.1.tar` & `embeddingcache-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 12:21:26.821890 embeddingcache-0.0.1/
--rw-r--r--   0 joseph     (501) staff       (20)     1081 2023-07-13 10:50:51.000000 embeddingcache-0.0.1/LICENSE.txt
--rw-r--r--   0 joseph     (501) staff       (20)     2654 2023-07-13 12:21:26.820624 embeddingcache-0.0.1/PKG-INFO
--rw-r--r--   0 joseph     (501) staff       (20)      180 2023-07-13 12:17:53.000000 embeddingcache-0.0.1/README.md
--rw-r--r--   0 joseph     (501) staff       (20)     6178 2023-07-13 12:18:19.000000 embeddingcache-0.0.1/pyproject.toml
--rw-r--r--   0 joseph     (501) staff       (20)       38 2023-07-13 12:21:26.822116 embeddingcache-0.0.1/setup.cfg
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 12:21:26.802537 embeddingcache-0.0.1/src/
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 12:21:26.813963 embeddingcache-0.0.1/src/embeddingcache.egg-info/
--rw-r--r--   0 joseph     (501) staff       (20)     2654 2023-07-13 12:21:26.000000 embeddingcache-0.0.1/src/embeddingcache.egg-info/PKG-INFO
--rw-r--r--   0 joseph     (501) staff       (20)      383 2023-07-13 12:21:26.000000 embeddingcache-0.0.1/src/embeddingcache.egg-info/SOURCES.txt
--rw-r--r--   0 joseph     (501) staff       (20)        1 2023-07-13 12:21:26.000000 embeddingcache-0.0.1/src/embeddingcache.egg-info/dependency_links.txt
--rw-r--r--   0 joseph     (501) staff       (20)       39 2023-07-13 12:21:26.000000 embeddingcache-0.0.1/src/embeddingcache.egg-info/entry_points.txt
--rw-r--r--   0 joseph     (501) staff       (20)       50 2023-07-13 12:21:26.000000 embeddingcache-0.0.1/src/embeddingcache.egg-info/requires.txt
--rw-r--r--   0 joseph     (501) staff       (20)        7 2023-07-13 12:21:26.000000 embeddingcache-0.0.1/src/embeddingcache.egg-info/top_level.txt
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 12:21:26.817995 embeddingcache-0.0.1/src/sample/
--rw-r--r--   0 joseph     (501) staff       (20)      111 2023-07-13 12:17:53.000000 embeddingcache-0.0.1/src/sample/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)        9 2023-07-13 12:17:53.000000 embeddingcache-0.0.1/src/sample/package_data.dat
--rw-r--r--   0 joseph     (501) staff       (20)       43 2023-07-13 12:17:53.000000 embeddingcache-0.0.1/src/sample/simple.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 12:21:26.819278 embeddingcache-0.0.1/tests/
--rw-r--r--   0 joseph     (501) staff       (20)      417 2023-07-13 10:50:51.000000 embeddingcache-0.0.1/tests/test_simple.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 16:29:24.493692 embeddingcache-0.1.0/
+-rw-r--r--   0 joseph     (501) staff       (20)      555 2023-07-13 15:28:45.000000 embeddingcache-0.1.0/LICENSE.txt
+-rw-r--r--   0 joseph     (501) staff       (20)     5415 2023-07-13 16:29:24.486614 embeddingcache-0.1.0/PKG-INFO
+-rw-r--r--   0 joseph     (501) staff       (20)     3555 2023-07-13 16:28:32.000000 embeddingcache-0.1.0/README.md
+-rw-r--r--   0 joseph     (501) staff       (20)     6365 2023-07-13 16:28:32.000000 embeddingcache-0.1.0/pyproject.toml
+-rw-r--r--   0 joseph     (501) staff       (20)       38 2023-07-13 16:29:24.494005 embeddingcache-0.1.0/setup.cfg
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 16:29:24.434968 embeddingcache-0.1.0/src/
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 16:29:24.459359 embeddingcache-0.1.0/src/embeddingcache/
+-rw-r--r--   0 joseph     (501) staff       (20)      111 2023-07-13 15:27:06.000000 embeddingcache-0.1.0/src/embeddingcache/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1398 2023-07-13 15:27:09.000000 embeddingcache-0.1.0/src/embeddingcache/computeembeddings.py
+-rw-r--r--   0 joseph     (501) staff       (20)      965 2023-07-13 15:49:08.000000 embeddingcache-0.1.0/src/embeddingcache/embeddingcache.py
+-rw-r--r--   0 joseph     (501) staff       (20)     7466 2023-07-13 15:49:09.000000 embeddingcache-0.1.0/src/embeddingcache/embeddingdb.py
+-rw-r--r--   0 joseph     (501) staff       (20)     6690 2023-07-13 15:49:09.000000 embeddingcache-0.1.0/src/embeddingcache/hashstringdb.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 16:29:24.466354 embeddingcache-0.1.0/src/embeddingcache.egg-info/
+-rw-r--r--   0 joseph     (501) staff       (20)     5415 2023-07-13 16:29:24.000000 embeddingcache-0.1.0/src/embeddingcache.egg-info/PKG-INFO
+-rw-r--r--   0 joseph     (501) staff       (20)      444 2023-07-13 16:29:24.000000 embeddingcache-0.1.0/src/embeddingcache.egg-info/SOURCES.txt
+-rw-r--r--   0 joseph     (501) staff       (20)        1 2023-07-13 16:29:24.000000 embeddingcache-0.1.0/src/embeddingcache.egg-info/dependency_links.txt
+-rw-r--r--   0 joseph     (501) staff       (20)       98 2023-07-13 16:29:24.000000 embeddingcache-0.1.0/src/embeddingcache.egg-info/requires.txt
+-rw-r--r--   0 joseph     (501) staff       (20)       15 2023-07-13 16:29:24.000000 embeddingcache-0.1.0/src/embeddingcache.egg-info/top_level.txt
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-07-13 16:29:24.467914 embeddingcache-0.1.0/tests/
+-rw-r--r--   0 joseph     (501) staff       (20)     1096 2023-07-13 15:27:06.000000 embeddingcache-0.1.0/tests/test_caching.py
```

### Comparing `embeddingcache-0.0.1/pyproject.toml` & `embeddingcache-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 name = "embeddingcache"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.1"  # Required
+version = "0.1.0"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
-description = "A sample Python project"  # Optional
+description = "Retrieve text embeddings, but cache them locally if we have already computed them."
 
 # This is an optional longer description of your project that represents
 # the body of text which users will see when they visit PyPI.
 #
 # Often, this is the same as your README, so you can just read it in from
 # that file directly (as we have already done above)
 #
@@ -53,40 +53,41 @@
 # larger catalog.
 keywords = ["sample", "setuptools", "development"]  # Optional
 
 # This should be your name or the name of the organization who originally
 # authored the project, and a valid email address corresponding to the name
 # listed.
 authors = [
-  {name = "A. Random Developer", email = "author@example.com" } # Optional
+  {name = "Joseph Turian", email = "lastname@gmail.com" } # Optional
 ]
 
 # This should be your name or the names of the organization who currently
 # maintains the project, and a valid email address corresponding to the name
 # listed.
-maintainers = [
-  {name = "A. Great Maintainer", email = "maintainer@example.com" } # Optional
-]
+#maintainers = [
+#  {name = "A. Great Maintainer", email = "maintainer@example.com" } # Optional
+#]
 
 # Classifiers help users find your project by categorizing it.
 #
 # For a list of valid classifiers, see https://pypi.org/classifiers/
 classifiers = [  # Optional
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
   "Development Status :: 3 - Alpha",
 
   # Indicate who your project is intended for
   "Intended Audience :: Developers",
-  "Topic :: Software Development :: Build Tools",
+  "Intended Audience :: Science/Research",
+  "Topic :: Scientific/Engineering :: Artificial Intelligence",
 
   # Pick your license as you wish
-  "License :: OSI Approved :: MIT License",
+  "License :: OSI Approved :: Apache Software License",
 
   # Specify the Python versions you support here. In particular, ensure
   # that you indicate you support Python 3. These classifiers are *not*
   # checked by "pip install". See instead "python_requires" below.
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
@@ -99,15 +100,19 @@
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ # Optional
-  "peppercorn"
+  "SQLAlchemy",
+  "tqdm",
+  "python-slugify",
+  "sentence_transformers",
+  "numpy",
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
@@ -125,24 +130,24 @@
 # https://packaging.python.org/specifications/core-metadata/#home-page-optional
 #
 # Examples listed include a pattern for specifying where the package tracks
 # issues, where the source is hosted, where to say thanks to the package
 # maintainers, and where to support the project financially. The key is
 # what's used to render the link text on PyPI.
 [project.urls]  # Optional
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Reports" = "https://github.com/pypa/sampleproject/issues"
-"Funding" = "https://donate.pypi.org"
-"Say Thanks!" = "http://saythanks.io/to/example"
-"Source" = "https://github.com/pypa/sampleproject/"
+"Homepage" = "https://github.com/turian/embeddingcache"
+"Bug Reports" = "https://github.com/turian/embeddingcache"
+#"Funding" = "https://donate.pypi.org"
+#"Say Thanks!" = "http://saythanks.io/to/example"
+"Source" = "https://github.com/turian/embeddingcache"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
-[project.scripts]  # Optional
-sample = "sample:main"
+#[project.scripts]  # Optional
+#sample = "sample:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = {"sample" = ["*.dat"]}
```

