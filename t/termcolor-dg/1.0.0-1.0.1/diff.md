# Comparing `tmp/termcolor_dg-1.0.0.tar.gz` & `tmp/termcolor_dg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termcolor_dg-1.0.0.tar", last modified: Wed May 24 22:39:02 2023, max compression
+gzip compressed data, was "termcolor_dg-1.0.1.tar", last modified: Thu Jul 13 12:00:26 2023, max compression
```

## Comparing `termcolor_dg-1.0.0.tar` & `termcolor_dg-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-05-24 22:39:02.112514 termcolor_dg-1.0.0/
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      302 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/.pylintrc
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2208 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/CHANGES.md
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      512 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/INSTALL.md
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     1073 2022-02-05 13:13:56.000000 termcolor_dg-1.0.0/LICENSE
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      300 2023-01-11 10:23:58.000000 termcolor_dg-1.0.0/MANIFEST.in
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     3046 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/Makefile
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    12208 2023-05-24 22:39:02.112514 termcolor_dg-1.0.0/PKG-INFO
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     8908 2023-05-24 22:38:59.000000 termcolor_dg-1.0.0/README.md
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      119 2022-02-22 22:00:05.000000 termcolor_dg-1.0.0/TODO.md
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)   113637 2022-02-10 07:54:40.000000 termcolor_dg-1.0.0/color_logs.png
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)   158505 2022-02-05 13:13:56.000000 termcolor_dg-1.0.0/colors.png
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      106 2022-02-05 13:13:56.000000 termcolor_dg-1.0.0/pyproject.toml
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     1999 2023-05-24 22:39:02.113514 termcolor_dg-1.0.0/setup.cfg
--rwxrwxr-x   0 dgunchev  (1000) dgunchev  (1000)      809 2022-03-21 14:32:23.000000 termcolor_dg-1.0.0/setup.py
-drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-05-24 22:39:02.111514 termcolor_dg-1.0.0/src/
-drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-05-24 22:39:02.112514 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    12208 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/PKG-INFO
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      452 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/SOURCES.txt
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)        1 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/dependency_links.txt
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      118 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/entry_points.txt
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)        1 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/not-zip-safe
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)       13 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/top_level.txt
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    20170 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/src/termcolor_dg.py
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2723 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/termcolor_dg.spec
-drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-05-24 22:39:02.112514 termcolor_dg-1.0.0/test/
--rwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)    13743 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/test/test_termcolor_dg.py
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2285 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/tox.ini
+drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-07-13 12:00:26.451961 termcolor_dg-1.0.1/
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      532 2023-07-13 11:53:46.000000 termcolor_dg-1.0.1/.editorconfig
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      302 2023-05-24 22:28:57.000000 termcolor_dg-1.0.1/.pylintrc
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      323 2023-05-24 22:28:57.000000 termcolor_dg-1.0.1/.pylintrc2
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2208 2023-05-24 22:28:57.000000 termcolor_dg-1.0.1/CHANGES.md
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      512 2023-05-24 22:28:57.000000 termcolor_dg-1.0.1/INSTALL.md
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     1073 2022-02-05 13:13:56.000000 termcolor_dg-1.0.1/LICENSE
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      341 2023-07-13 11:53:46.000000 termcolor_dg-1.0.1/MANIFEST.in
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     3016 2023-07-13 11:53:46.000000 termcolor_dg-1.0.1/Makefile
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    12208 2023-07-13 12:00:26.451961 termcolor_dg-1.0.1/PKG-INFO
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     8908 2023-07-13 12:00:24.000000 termcolor_dg-1.0.1/README.md
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      119 2022-02-22 22:00:05.000000 termcolor_dg-1.0.1/TODO.md
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)   113637 2022-02-10 07:54:40.000000 termcolor_dg-1.0.1/color_logs.png
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)   158505 2022-02-05 13:13:56.000000 termcolor_dg-1.0.1/colors.png
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      106 2022-02-05 13:13:56.000000 termcolor_dg-1.0.1/pyproject.toml
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     1897 2023-07-13 12:00:26.451961 termcolor_dg-1.0.1/setup.cfg
+-rwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)     1025 2023-07-13 11:53:46.000000 termcolor_dg-1.0.1/setup.py
+drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-07-13 12:00:26.450960 termcolor_dg-1.0.1/src/
+drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-07-13 12:00:26.451961 termcolor_dg-1.0.1/src/termcolor_dg.egg-info/
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    12208 2023-07-13 12:00:26.000000 termcolor_dg-1.0.1/src/termcolor_dg.egg-info/PKG-INFO
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      477 2023-07-13 12:00:26.000000 termcolor_dg-1.0.1/src/termcolor_dg.egg-info/SOURCES.txt
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)        1 2023-07-13 12:00:26.000000 termcolor_dg-1.0.1/src/termcolor_dg.egg-info/dependency_links.txt
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      118 2023-07-13 12:00:26.000000 termcolor_dg-1.0.1/src/termcolor_dg.egg-info/entry_points.txt
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)        1 2023-07-13 12:00:26.000000 termcolor_dg-1.0.1/src/termcolor_dg.egg-info/not-zip-safe
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)       13 2023-07-13 12:00:26.000000 termcolor_dg-1.0.1/src/termcolor_dg.egg-info/top_level.txt
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    20355 2023-07-13 11:53:46.000000 termcolor_dg-1.0.1/src/termcolor_dg.py
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2741 2023-07-13 11:53:46.000000 termcolor_dg-1.0.1/termcolor_dg.spec
+drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-07-13 12:00:26.451961 termcolor_dg-1.0.1/test/
+-rwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)    13946 2023-07-13 11:53:46.000000 termcolor_dg-1.0.1/test/test_termcolor_dg.py
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2294 2023-07-13 11:53:46.000000 termcolor_dg-1.0.1/tox.ini
```

### Comparing `termcolor_dg-1.0.0/CHANGES.md` & `termcolor_dg-1.0.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `termcolor_dg-1.0.0/INSTALL.md` & `termcolor_dg-1.0.1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `termcolor_dg-1.0.0/LICENSE` & `termcolor_dg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `termcolor_dg-1.0.0/Makefile` & `termcolor_dg-1.0.1/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 TOP := $(shell dirname "$(abspath $(lastword $(MAKEFILE_LIST)))")
+PYTHON ?= python
+PIP ?= pip
+COVERAGE ?= coverage
+PYLINT ?= pylint
 PYLINT_RCFILE ?= .pylintrc
 
 .PHONY: help
 help:
 	@echo
 	@echo "▐ Help"
 	@echo "▝▀▀▀▀▀▀"
@@ -24,67 +28,65 @@
 	@echo  "    test_upload:        use twine to upload to the test pypi repo"
 	@echo  "    upload:             use twine to upload to the pypi repo"
 	@echo
 
 
 .PHONY: develop
 develop:
-	PYTHONPATH=. python setup.py develop -O1 --install-dir .
+	PYTHONPATH=. $(PYTHON) setup.py develop -O1 --install-dir .
 
 
 .PHONY: test
 test:
-	coverage erase
-	PYTHONPATH=src coverage run -m unittest discover --verbose -s test
-	# coverage combine  # Will fail if only one run...
-	coverage report -m --skip-empty
-	# pylint2 --rcfile .pylintrc2 $(shell git ls-files '*.py')
-	# pylint $(shell git ls-files '*.py')
-	pylint --rcfile $(PYLINT_RCFILE) *.py */*.py
+	$(COVERAGE) erase
+	PYTHONPATH=src $(COVERAGE) run -m unittest discover --verbose -s test
+	$(COVERAGE) report -m # --skip-empty
+	$(PYLINT) --rcfile $(PYLINT_RCFILE) *.py */*.py
 
 
 .PHONY: clean
 clean:
-	coverage erase
+	$(COVERAGE) erase
 	rm -rf ./.tox ./.coverage* ./coverage.json ./coverage.xml ./htmlcov/ ./build/ ./dist/
 	rm -rf ./easy-install* ./easy_install* ./setuptools.pth ./*.egg-link termcolor_dg_demo termcolor_dg_demo_log
 	find . -depth -name '__pycache__' -exec rm -rf \{\} \;
 	find . -depth \( -name '*.pyc' -o -name '*.pyo' -o -name '*.egg-info' -o -name '*.py,cover'  \) -exec rm -rf \{\} \;
 
 
 .PHONY: build
 build: clean
 	# https://stackoverflow.com/a/46875147 - Fix the image locations, version/tag detection would be nice.
 	# Remove URLs
 	sed -i 's#https://raw.githubusercontent.com/gunchev/termcolor_dg/.*/##g' README.md
 	# Redirect to github
 	sed -i 's#](\([a-zA-Z0-9/:_%]*\.png\)#](https://raw.githubusercontent.com/gunchev/termcolor_dg/master/\1#g' README.md
-	python -m build
+	$(PYTHON) -m build
+	# With "$(PYTHON) setup.py sdist" we can get more source formats, but can't upload more than one anyways.
 	# Remove URLs
 	sed -i 's#https://raw.githubusercontent.com/gunchev/termcolor_dg/.*/##g' README.md
-	# With "python setup.py sdist" we can get more source formats, but can't upload more than one anyways.
 
 
 .PHONY: test_install
 test_install:
-	pip install --user -i https://test.pypi.org/simple/ termcolor_dg
+	$(PIP) install --user -i https://test.pypi.org/simple/ termcolor_dg
 
 
 .PHONY: install
 install:
-	pip install --user termcolor_dg
+	$(PIP) install --user termcolor_dg
 
 
 .PHONY: uninstall
 uninstall:
-	pip uninstall termcolor_dg
+	$(PIP) uninstall termcolor_dg
 
 
 .PHONY: rpm
-rpm: build
+rpm:
+	$(PYTHON) setup.py sdist
 	rpmbuild -ba termcolor_dg.spec --define "_sourcedir $(TOP)/dist"
 
 
 # https://packaging.python.org/en/latest/guides/using-testpypi/
 # Upload to https://test.pypi.org/
 .PHONY: test_upload
 test_upload: build
```

### Comparing `termcolor_dg-1.0.0/PKG-INFO` & `termcolor_dg-1.0.1/src/termcolor_dg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: termcolor_dg
-Version: 1.0.0
+Name: termcolor-dg
+Version: 1.0.1
 Summary: ANSI Color formatting for terminal output and log coloring
 Home-page: https://github.com/gunchev/termcolor_dg/
 Author: Konstantin Lepa
 Author-email: konstantin.lepa@gmail.com
 Maintainer: Doncho N. Gunchev
 Maintainer-email: dgunchev@gmail.com
 License: MIT
```

### Comparing `termcolor_dg-1.0.0/README.md` & `termcolor_dg-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `termcolor_dg-1.0.0/color_logs.png` & `termcolor_dg-1.0.1/color_logs.png`

 * *Files identical despite different names*

### Comparing `termcolor_dg-1.0.0/colors.png` & `termcolor_dg-1.0.1/colors.png`

 * *Files identical despite different names*

### Comparing `termcolor_dg-1.0.0/setup.cfg` & `termcolor_dg-1.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 [options]
 python_requires = >= 2.7
 package_dir = 
 	= src
 py_modules = termcolor_dg
 zip_safe = False
 include_package_data = True
-setup_requires = 
-	setuptools>=41.0
 packages = find:
 install_requires = 
 tests_require = 
 	coverage
 
 [options.packages.find]
 where = src
@@ -47,28 +45,26 @@
 	termcolor_dg_demo = termcolor_dg:termcolor_demo
 	termcolor_dg_demo_log = termcolor_dg:color_log_demo
 
 [bdist_wheel]
 universal = true
 
 [sdist]
-formats = zip,xztar
+formats = gztar,xztar,zip
 
 [coverage:run]
 branch = true
-command_line = -m unittest discover --verbose -s test
 concurrency = thread
 omit = 
 	test/*
 	tests/*
 
 [coverage:report]
 show_missing = true
 skip_covered = false
-skip_empty = true
 exclude_lines = 
 	pragma: no cover
 	
 	def __repr__
 	if self\.debug
 	
 	raise AssertionError
```

### Comparing `termcolor_dg-1.0.0/setup.py` & `termcolor_dg-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-#!/usr/bin/python
+#!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 """termcolor_dg setup"""
 
 from os.path import abspath, dirname, join as pjoin
 
 from setuptools import setup
 
 
-HERE = abspath(dirname(__file__))
-
-
-if __name__ == '__main__':
+def main():
+    """setuptools setup"""
     # https://github.com/pypa/sampleproject, https://stackoverflow.com/a/58534041/1136400
     # Any encoding works, all is latin-1 and allows for python2 compatibility.
-    with open(pjoin(HERE, 'src', 'termcolor_dg.py'), 'r') as src:
-        DATA = [i for i in src.readlines() if i.startswith('__')]
-    META = dict((i[0].strip(), i[1].strip().strip("'\"")) for i in (ln.split('=', 1) for ln in DATA))
+    here = abspath(dirname(__file__))
+    name = 'termcolor_dg'
+    with open(pjoin(here, 'src', name + '.py'), 'r') as src:
+        data = [i for i in src.readlines() if i.startswith('__')]
+    meta = dict((i[0].strip(), i[1].strip().strip("'\"")) for i in (ln.split('=', 1) for ln in data))
     setup(
-        author=META['__author__'],
-        author_email=META['__email__'],
-        maintainer=META['__maintainer__'],
-        maintainer_email=META['__maintainer_email__'],
+        name=name,
+        version=meta['__version__'],
+        author=meta['__author__'],  # Optional
+        author_email=meta['__email__'],  # Optional
+        maintainer=meta['__maintainer__'],  # Optional
+        maintainer_email=meta['__maintainer_email__'],  # Optional
+        test_suite=name + '_tests',
     )
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `termcolor_dg-1.0.0/src/termcolor_dg.egg-info/PKG-INFO` & `termcolor_dg-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: termcolor-dg
-Version: 1.0.0
+Name: termcolor_dg
+Version: 1.0.1
 Summary: ANSI Color formatting for terminal output and log coloring
 Home-page: https://github.com/gunchev/termcolor_dg/
 Author: Konstantin Lepa
 Author-email: konstantin.lepa@gmail.com
 Maintainer: Doncho N. Gunchev
 Maintainer-email: dgunchev@gmail.com
 License: MIT
```

### Comparing `termcolor_dg-1.0.0/src/termcolor_dg.py` & `termcolor_dg-1.0.1/src/termcolor_dg.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,35 +34,34 @@
 
 import logging
 import os
 import shutil
 import sys
 import time
 
-
 __all__ = ['always_colored', 'colored', 'cprint', 'rainbow_color', 'monkey_patch_logging', 'logging_basic_color_config',
            'COLOR_RESET_STR']
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __copyright__ = 'Copyright (c) 2008-2011 Volvox Development Team'
 __license__ = 'MIT'
 
 __author__ = 'Konstantin Lepa'
 __email__ = 'konstantin.lepa@gmail.com'
 
 __maintainer__ = 'Doncho N. Gunchev'
 __maintainer_email__ = 'dgunchev@gmail.com'
 
 __credits__ = ['Edmund Huber', 'Lukasz Balcerzak', 'Hendrik Buschmeier', 'Nat Meysenburg', 'Iulian PAUN']
 
-
 # Python 2 and 3 compatibility
 if sys.version_info >= (3, 0):  # pragma: no cover
     # raw_input = input  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
     # unicode = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
+    # noinspection PyShadowingBuiltins
     basestring = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
     # long = int  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
 
 DISABLED = (os.getenv('ANSI_COLORS_DISABLED') is not None or os.getenv('NO_COLOR') is not None) \
            or (not sys.stdout.isatty() and os.getenv('ANSI_COLORS_FORCE') is None)
 
 COLOR_RESET_STR = '\033[0m'
@@ -97,15 +96,15 @@
     'white': '97',
 }
 
 HIGHLIGHTS = dict((i[0], str(int(i[1]) + 10)) for i in COLORS.items())
 
 
 def color_fmt(color, colors16, cnum):
-    """Format the color/background escape sequence chunk"""
+    """Format the color/background escape sequence chunk."""
     if isinstance(color, basestring):
         if color.startswith('on_'):  # backwards compatibility
             color = color[3:]
         if color in colors16:
             return colors16[color]
         raise ValueError("Invalid color %r" % color)
 
@@ -119,27 +118,28 @@
             return '%d;2;%d;%d;%d' % (cnum, color[0], color[1], color[2])
         raise ValueError("Invalid color %r" % (color,))
 
     raise TypeError("Unsupported color type %s" % type(color).__name__)
 
 
 def always_colored(text, color=None, on_color=None, attrs=None, reset=True):
-    """Color text with ANSI escape codes
+    """Color text with ANSI escape codes.
 
     color (text color): 'black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'light_grey', 'dark_grey',
         'light_red', 'light_green', 'light_yellow', 'light_blue', 'light_magenta', 'light_cyan', 'white'.
 
-    on_color (text background): same as color but with 'on_' or 'on ' prefix.
+    On_color (text background): same as color but with 'on_' or 'on ' prefix.
 
-    attributes: 'bold', 'dark', 'underline', 'blink', 'reverse', 'concealed'.
+    Attributes: 'bold', 'dark', 'underline', 'blink', 'reverse', 'concealed'.
 
-    reset: if set to false do not emit reset sequence at the end.
+    Reset: If set to false, don't emit a reset sequence at the end.
 
     Additionally, if 256 colors are supported, any integer between 1 and 255 can be provided for both foreground
-    and background. A tuple/list with three integers (R, G, B) can be provided for 24 bit color.
+    and background.
+    A tuple/list with three integers (R, G, B) can be provided for 24-bit color.
 
     Examples:
         always_colored('Hello, World!', 'red', 'on_black', ['bold', 'blink'])
         always_colored('Hello, World!', 191, 182)
         always_colored('24bit color!', (255, 127, 127), (127, 127, 255), ['bold'])
     """
     pfx = []
@@ -174,15 +174,15 @@
         light_yellow, light_blue, light_magenta, light_cyan.
 
     Available text highlights:
         on_red, on_green, on_yellow, on_blue, on_magenta, on_cyan, on_black, on_white, on_light_grey, on_dark_grey,
         on_light_red, on_light_green, on_light_yellow, on_light_blue, on_light_magenta, light_cyan.
 
     Additionally, if 256 colors are supported, any integer between 1 and 255 can be provided for both
-    foreground and background. A tuple/list with three elements (R, G, B) can be used for 24 bit color.
+    foreground and background. A tuple/list with three elements (R, G, B) can be used for 24-bit color.
 
     Available attributes:
         bold, dark, underline, blink, reverse, concealed.
 
     Examples:
         colored('Hello, World!', 'red', 'on_black', ['bold', 'blink'])
         colored('Hello, World!', 191, 182)
@@ -199,15 +199,15 @@
 
     It accepts arguments of print function.
     """
     print(colored(text, color, on_color, attrs, reset), **kwargs)
 
 
 def rainbow_color(n, steps, nmax=255):
-    """Calculate rainbow color"""
+    """Calculate rainbow color."""
     if not isinstance(n, int) and isinstance(steps, int):
         raise TypeError('Arguments must be integers')
     if steps < 6:
         raise ValueError('Total must be at least 6')
 
     n %= steps
     progress = float(n) / steps
@@ -221,66 +221,67 @@
     progress = float(n) / steps
     b_value = max(0, min(nmax, abs(3 * nmax - 6 * progress * nmax) - nmax))
 
     return round(r_value), round(g_value), round(b_value)
 
 
 def monkey_patch_logging_format():
-    """Monkey patches the logging module format error report"""
+    """Monkey patches the logging module format error report."""
     if getattr(logging.LogRecord, 'distGetMessage', None) is not None:
         return
 
     logging.LogRecord.distGetMessage = logging.LogRecord.getMessage
 
     def print_log_record_on_error(func):
-        """Monkeypatch for logging.LogRecord.getMessage
+        """Monkeypatch for `logging.LogRecord.getMessage`.
 
         Credits: https://stackoverflow.com/questions/2477934/"""
 
         def wrap(self, *args, **kwargs):
-            """Generate wrapper function for logging.LogRecord.getMessage"""
+            """Generate wrapper function for `logging.LogRecord.getMessage`."""
             try:
                 return func(self, *args, **kwargs)
             except Exception as exc:  # pylint: disable=broad-except
                 return 'Error logging msg=%r, args=%r: %r' \
                     % (getattr(self, 'msg', '?'), getattr(self, 'args', '?'), exc)
 
         return wrap
 
-    # Monkeypatch the logging library for more informative formatting errors
+    # Monkeypatch the logging library for more informative formatting errors.
     logging.LogRecord.getMessage = print_log_record_on_error(logging.LogRecord.getMessage)
 
 
 def monkey_unpatch_logging_format():
-    """Undo monkey_patch_logging_format"""
+    """Undo monkey_patch_logging_format."""
     if getattr(logging.LogRecord, 'distGetMessage', None) is None:
         return
     # noinspection PyUnresolvedReferences
     logging.LogRecord.getMessage = logging.LogRecord.distGetMessage  # @UndefinedVariable
     delattr(logging.LogRecord, 'distGetMessage')
 
 
 def monkey_patch_logging(color_on_terminal=True):
-    """Monkey patches the logging module and add colors if enabled"""
+    """Monkey patches the logging module and adds color if enabled."""
 
     if getattr(logging, 'DistFormatter', None) is not None:
         return True
 
     monkey_patch_logging_format()
 
     if color_on_terminal and not DISABLED:
-        # Monkey patches the logging module to print in color'
+        # Monkey patches the logging module to print in color.
 
         def get_formatter(logging_formatter=logging.Formatter):
             """Get it? ;-)"""
 
             class ColoredFormatter(logging_formatter):
-                """Color console formatter"""
+                """Color console formatter."""
 
                 def format(self, record):
+                    """Color console formatter."""
                     output = logging_formatter.format(self, record)
                     tail = None
                     comment_pos = output.find('  # ')  # Intentionally require two spaces before
                     if comment_pos >= 0:
                         output, tail = output[:comment_pos], output[comment_pos:]
 
                     if record.levelno < logging.DEBUG:  # pylint: disable=fixme
@@ -314,36 +315,36 @@
         logging.DistFormatter = logging.Formatter
         logging.Formatter = get_formatter()
 
     return True
 
 
 def monkey_unpatch_logging():
-    """Undo monkey_patch_logging"""
+    """Undo monkey_patch_logging."""
 
     monkey_unpatch_logging_format()
 
     if getattr(logging, 'DistFormatter', None) is not None:
         # noinspection PyUnresolvedReferences
         logging.Formatter = logging.DistFormatter  # @UndefinedVariable
         delattr(logging, 'DistFormatter')
 
 
 def logging_basic_color_config(level='DEBUG', fmt='%(asctime)s %(message)s  # %(filename)s:%(lineno)d %(name)s',
                                color_on_terminal=True):
-    """Setup basic logging with fancy format and colors if running on terminal
+    """Setup basic logging with fancy format and colors if running on a terminal.
 
-    a very fancy fmt would be "%(asctime)s %(levelname)-8s: %(message)s  # %(filename)s:%(lineno)d %(name)s"
+    A very fancy fmt would be "%(asctime)s %(levelname)-8s: %(message)s  # %(filename)s:%(lineno)d %(name)s".
     """
     monkey_patch_logging(color_on_terminal=color_on_terminal)
     logging.basicConfig(level=level, format=fmt)
 
 
 def termcolor_demo_16():
-    """Base 16 color demo"""
+    """Base 16 color demo."""
     colors = ('black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'light_grey', 'dark_grey', 'light_red',
               'light_green', 'light_yellow', 'light_blue', 'light_magenta', 'light_cyan', 'white')
     max_len = max(len(color) for color in colors)
 
     print(RESET_STR, end='')
     print(('--- 16 color mode test on TERM=%r ' % os.getenv('TERM')).ljust(119, '-'))
 
@@ -385,20 +386,20 @@
     print(' [' + colored('Dark blink concealed white', 'white', attrs=['dark', 'blink', 'concealed']), end=']\n')
     print(' [' + '      Reversed blue       ', end=']')
     print(' [' + '    Concealed Magenta     ', end=']')
     print(' [' + 'Bold underline reverse red', end=']')
     print(' [' + 'Dark blink concealed white', end=']\n')
 
     def all_combos(values):
-        """Generate all combinations"""
+        """Generate all combinations."""
         values = tuple(values)
         if values:
-            for i in all_combos(values[1:]):
-                yield i
-                yield [values[0]] + i
+            for j in all_combos(values[1:]):
+                yield j
+                yield [values[0]] + j
         else:
             yield []
 
     print('\nAttribute salad (Bold, Dark, Underline, blinK, Reverse, Concealed):')
     for idx, attrs in enumerate(all_combos(all_attrs)):
         code = 'B' if 'bold' in attrs else 'b'
         code += 'D' if 'dark' in attrs else 'd'
@@ -406,15 +407,15 @@
         code += 'K' if 'blink' in attrs else 'k'
         code += 'R' if 'reverse' in attrs else 'r'
         code += 'C' if 'concealed' in attrs else 'c'
         print(' [' if idx % 16 == 0 else ' ' + colored(code, attrs=attrs), end='' if idx % 16 != 15 else ' ]\n')
 
 
 def termcolor_demo_256():
-    """256 color demo"""
+    """256 color demo."""
     print('\n--- 256 color mode test '.ljust(120, '-'))
     print(' First 16: [', end='')
     for i in range(16):
         cprint('%3d ' % i, color=15 - i, on_color=i, end='', reset=i == 15)
     print(']')
 
     print()
@@ -434,15 +435,15 @@
     for i in range(232, 256):
         # cprint('%4d' % i, color='white' if i < 244 else 'black', on_color=i, end='')
         cprint('%4d' % i, color=(232 + 255) - i, on_color=i, end='')
     print(']\n')
 
 
 def termcolor_demo_24bit():
-    """24 bit color demo"""
+    """24-bit color demo."""
     data = '=== 24 bit color mode test '.ljust(114, '=')
     for i in range(2 * len(data), -1, -1):
         print('\r   ', end='')
         grey = abs(i * 8 % 510 - 255)
         print(
             colored(
                 ''.join(colored(char, on_color=rainbow_color(step + i, len(data)), reset=False)
@@ -464,39 +465,40 @@
 
     print()
 
 
 def get_term_width():
     """Get terminal width, https://gist.github.com/mr700/c73af70357ff8bcfc3250ee6c84e164d, is an overkill."""
     try:
+        # noinspection PyUnresolvedReferences
         return shutil.get_terminal_size(fallback=(80, 32)).columns  # @UndefinedVariable
     except AttributeError:  # pragma: no cover
         return 120  # pragma: no cover
 
 
 def termcolor_demo():
-    """Demonstrate this module's capabilities"""
+    """Demonstrate this module's capabilities."""
     termcolor_demo_16()
     termcolor_demo_256()
     if get_term_width() >= 120 or os.getenv('ANSI_COLORS_FORCE') is not None:
         termcolor_demo_24bit()
     else:
         print("Need terminal width of 120 or more for this part...")  # pragma: no cover
 
 
 def color_log_demo():
-    """Test color logging on terminal and logging format error"""
+    """Test color logging on terminal and logging format error."""
     # monkey_patch_logging(color_on_terminal=True)
     logging_basic_color_config()
 
     log = logging.getLogger('logger')
     print('Logging test... levels and exception:')
 
     # Hack to skip the log level test
-    # noinspection PyTypeChecker
+    # noinspection PyTypeChecker, PyProtectedMember
     log._log(logging.NOTSET, 'Not set, below DEBUG, normally not show...', [])  # pylint: disable=W0212
     log.debug('Debug')
     log.info('Info')
     log.warning('Warning')
     log.error('Error')
     log.critical('Critical')
     log.error('x', 1)  # the mistake is intentional pylint: disable=logging-too-many-args
@@ -507,15 +509,15 @@
     except TypeError:
         log.exception('Exception')
     log.log(51, 'ABOVE CRITICAL!')
     log.info('Done.')
 
 
 def main():
-    """Main demo entry point, if no arguments - color demo, if any - colored logs demo"""
+    """Main demo entry point, if no arguments - color demo, if any - colored logs demo."""
     if len(sys.argv) == 1:  # pragma: no cover
         return termcolor_demo()  # pragma: no cover
     return color_log_demo()  # pragma: no cover
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `termcolor_dg-1.0.0/termcolor_dg.spec` & `termcolor_dg-1.0.1/termcolor_dg.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 %{?!python3_pkgversion:%global python3_pkgversion 3}
 
 %global srcname termcolor_dg
 
 Name:           python-%{srcname}
-Version:        1.0.0
+Version:        1.0.1
 Release:        0%{?dist}
 Summary:        ANSI Color formatting for terminal output and log coloring.
 License:        MIT
 URL:            https://github.com/gunchev/termcolor_dg/%{srcname}
-Source0:        https://github.com/gunchev/%{srcname}/archive/refs/tags/v%{version}.tar.gz?name=%{srcname}-%{version}.tar.gz
+Source0:        https://github.com/gunchev/%{srcname}/archive/refs/tags/%{version}.tar.gz?name=%{srcname}-%{version}.tar.gz
 
 BuildArch:      noarch
 
 BuildRequires:  python%{python3_pkgversion}-devel
 BuildRequires:  python%{python3_pkgversion}-setuptools
-BuildRequires:  python%{python3_pkgversion}-check-manifest >= 0.42
+# BuildRequires:  python%%{python3_pkgversion}-check-manifest >= 0.42
 BuildRequires:  python%{python3_pkgversion}-coverage
 BuildRequires:  python%{python3_pkgversion}-flake8
 BuildRequires:  python%{python3_pkgversion}-pylint
 
 
 %{?python_enable_dependency_generator}
 
@@ -68,15 +68,15 @@
 
 %install
 rm -rf "$RPM_BUILD_ROOT"
 %py3_install
 
 
 %check
-make test
+PYLINT=pylint-3 make test
 
 
 %files -n  python%{python3_pkgversion}-%{srcname}
 %license LICENSE
 %doc CHANGES.md README.md INSTALL.md TODO.md
 %{python3_sitelib}/%{srcname}.py
 %{python3_sitelib}/%{srcname}-%{version}-py%{python3_version}.egg-info/
```

### Comparing `termcolor_dg-1.0.0/test/test_termcolor_dg.py` & `termcolor_dg-1.0.1/test/test_termcolor_dg.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 import re
 import sys
 import time
 import unittest
 
 import termcolor_dg
 
-
 # Python 2 and 3 compatibility
 if sys.version_info[0] == 3:
-    raw_input = input  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
-    unicode = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
+    # raw_input = input  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
+    # unicode = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
+    # noinspection PyShadowingBuiltins
     basestring = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
-    long = int  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
+    # long = int  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
 
 
+# noinspection PyClassicStyleClass
 class CapturedOutput:
-    """Temporary replace sys.stdout and sys.stderr with io.StringIO or io.BytesIO"""
+    """Temporarily replace `sys.stdout` and `sys.stderr` with io.StringIO or io.BytesIO"""
 
     def __init__(self):
         self._buf = io.BytesIO() if sys.version_info < (3, 0) else io.StringIO()
         self._stdout, self._stderr = sys.stdout, sys.stderr
 
     def __enter__(self):
         sys.stdout, sys.stderr = self._buf, self._buf
@@ -40,14 +41,15 @@
         return False  # return True # To stop any exception from propagating
 
     def get_output(self):
         """Get what was written so far"""
         return self._buf.getvalue()
 
 
+# noinspection PyClassicStyleClass
 class Coffeine:
     """Temporary replace time.sleep() with pass"""
 
     def __init__(self):
         self._sleep = time.sleep
 
     def __enter__(self):
@@ -55,14 +57,15 @@
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):  # @UnusedVariable
         time.sleep = self._sleep
         return False  # return True # To stop any exception from propagating
 
 
+# noinspection PyPep8Naming,PyMissingOrEmptyDocstring
 class TestTermcolorDg(unittest.TestCase):
     """Test the termcolor_dg module"""
 
     def __init__(self, methodName='runTest'):
         unittest.TestCase.__init__(self, methodName=methodName)
         self._disabled = termcolor_dg.DISABLED
 
@@ -78,17 +81,17 @@
 
     def tearDown(self):
         unittest.TestCase.tearDown(self)
         termcolor_dg.DISABLED = self._disabled
 
     def test_main_exists(self):
         """Check if main is defined in the module"""
-        for fname in ('always_colored', 'colored', 'cprint', 'rainbow_color', 'monkey_patch_logging',
-                      'logging_basic_color_config', 'monkey_unpatch_logging', 'monkey_unpatch_logging_format'):
-            self.assertIn(fname, termcolor_dg.__dict__.keys(), '%r not defined?!?' % fname)
+        for file_name in ('always_colored', 'colored', 'cprint', 'rainbow_color', 'monkey_patch_logging',
+                          'logging_basic_color_config', 'monkey_unpatch_logging', 'monkey_unpatch_logging_format'):
+            self.assertIn(file_name, termcolor_dg.__dict__.keys(), '%r not defined?!?' % file_name)
 
     def test_cprint_no_color(self):
         """Check if main is printing the proper string"""
         with CapturedOutput() as out:
             termcolor_dg.cprint('test')
             output = out.get_output()
         self.assertEqual(output, 'test\n')
@@ -189,50 +192,51 @@
 
         for replacement in replacements:
             out_lines = [i.replace(replacement[0], replacement[1]) for i in out_lines]
 
         # self.assertEqual(''.join(out_lines), 1466)
         expected_lines = [
             'Logging test... levels and exception:',
-            '\x1b[30;44;2mYYYY-mm-dd HH:MM:SS,mss Not set, below DEBUG, normally not show...\x1b[0m\x1b[30;2m  ' \
-                '# src.py:123 logger\x1b[0m',
+            '\x1b[30;44;2mYYYY-mm-dd HH:MM:SS,mss Not set, below DEBUG, normally not show...\x1b[0m\x1b[30;2m  '
+            '# src.py:123 logger\x1b[0m',
             '\x1b[34;2mYYYY-mm-dd HH:MM:SS,mss Debug\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m',
             '\x1b[32;1mYYYY-mm-dd HH:MM:SS,mss Info\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m',
             '\x1b[33;1mYYYY-mm-dd HH:MM:SS,mss Warning\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m',
             '\x1b[31;1mYYYY-mm-dd HH:MM:SS,mss Error\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m',
             '\x1b[97;41;1mYYYY-mm-dd HH:MM:SS,mss Critical\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m',
-            "\x1b[31;1mYYYY-mm-dd HH:MM:SS,mss Error logging msg='x', args=(1,): TypeError('not all arguments " \
-                "converted during string formatting')\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m",
-            "\x1b[32;1mYYYY-mm-dd HH:MM:SS,mss Error logging msg='%d', args=(1, 2): TypeError('not all arguments " \
-                "converted during string formatting')\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m",
-            "\x1b[34;2mYYYY-mm-dd HH:MM:SS,mss Error logging msg='%d %d', args=('a', 2): TypeError('%d format: " \
-                "a real number is required, not str')\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m",
+            "\x1b[31;1mYYYY-mm-dd HH:MM:SS,mss Error logging msg='x', args=(1,): TypeError('not all arguments "
+            "converted during string formatting')\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m",
+            "\x1b[32;1mYYYY-mm-dd HH:MM:SS,mss Error logging msg='%d', args=(1, 2): TypeError('not all arguments "
+            "converted during string formatting')\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m",
+            "\x1b[34;2mYYYY-mm-dd HH:MM:SS,mss Error logging msg='%d %d', args=('a', 2): TypeError('%d format: "
+            "a real number is required, not str')\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m",
             '\x1b[31;1mYYYY-mm-dd HH:MM:SS,mss Exception\x1b[0m\x1b[30;2m  # src.py:123 logger',
             '\x1b[97;45;1m\x1b[2KTraceback (most recent call last):',
             "\x1b[2K    raise TypeError('msg')",
             '\x1b[2KTypeError: msg\x1b[0m\x1b[0m',
             '\x1b[33;41;1;4mYYYY-mm-dd HH:MM:SS,mss ABOVE CRITICAL!\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m',
             '\x1b[32;1mYYYY-mm-dd HH:MM:SS,mss Done.\x1b[0m\x1b[30;2m  # src.py:123 logger\x1b[0m']
         self.assertEqual(out_lines, expected_lines)
 
         # cover the "no tail" logging case
-        log_record = logging.LogRecord('name', logging.INFO, 'pathname', 1, 'test', [], None)
+        log_record = logging.LogRecord('name', logging.INFO, 'pathname', 1, 'test', {}, None)
         out = logging.Formatter('%(message)s').format(log_record)
         self.assertEqual(out, '\x1b[32;1mtest\x1b[0m')
         # Cover the disabled ...
         termcolor_dg.monkey_unpatch_logging()
         termcolor_dg.monkey_unpatch_logging()
         termcolor_dg.DISABLED = True
         self.assertTrue(termcolor_dg.monkey_patch_logging())
         self.assertTrue(termcolor_dg.monkey_patch_logging())
         termcolor_dg.DISABLED = False
 
     def test_color_demo(self):
         """Check the log demo output"""
         os.environ['ANSI_COLORS_FORCE'] = '1'
+        # noinspection PyUnusedLocal
         with CapturedOutput() as out, Coffeine() as a_stimulant:  # @UnusedVariable pylint: disable=unused-variable
             termcolor_dg.termcolor_demo()
             output = out.get_output()
 
         if len(output) != 477595:
             print("Bad output, len =", len(output))
             print(output)
```

### Comparing `termcolor_dg-1.0.0/tox.ini` & `termcolor_dg-1.0.1/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://tox.wiki/en/latest/example/basic.html
 # https://github.com/pypa/sampleproject/blob/main/tox.ini
 
 [tox]
-envlist = py27,py3{6,7,8,9,11},pypy{2,3}
+envlist = py27,py3{6,7,8,9,10,11},pypy{2,3}
 # At least this version is needed for PEP 517/518 support.
 minversion = 3.3.0
 # Activate isolated build environment. tox will use a virtual environment
 # to build a source distribution from the source tree. For build tools and
 # arguments use the pyproject.toml file as specified in PEP-517 and PEP-518.
 isolated_build = true
 
@@ -45,28 +45,28 @@
 
 
 # Detailed with formatting and stuff - only on the latest
 [testenv:py310]
 setenv =
     PYTHONPATH = {toxinidir}{:}{toxinidir}/src{:}{toxinidir}/test
 deps =
-    # check-manifest >= 0.42
+    check-manifest >= 0.42
     readme_renderer  # confirms your long_description will render correctly on PyPI.
     flake8
     coverage
     pylint
 commands =
-    # check-manifest --ignore 'tox.ini,test/**'   # confirm items checked into vcs are in your sdist
-    python setup.py check -m -s                 # confirm required package meta-data in setup.py
+    check-manifest --ignore '.idea/**,tox.ini,test/**'  # confirm items checked into vcs are in your sdist
+    python setup.py check -m -s  # confirm required package meta-data in setup.py
     flake8 .
     coverage erase
     coverage run -m unittest discover --verbose -s test {posargs}
     - coverage combine  # Will fail if only one run...
-    coverage report -m --skip-empty
+    coverage report -m # --skip-empty
     pylint setup.py src/termcolor_dg.py test/test_termcolor_dg.py
 
 
 [flake8]
-exclude = .tox, *.egg, build, data, .git, .eggs, __pycache__, test/, docs/, build/, dist/
+exclude = .tox, *.egg, build, data, .git, .eggs, __pycache__, test/, docs/, build/, dist/. .env/, .idea/
 select = E,W,F
 max-line-length = 120
 ignore = E226, N818, E24, E704, E126, E123, W503, E121, W504, E241
```

