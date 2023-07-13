# Comparing `tmp/py_go_goose-1.0.tar.gz` & `tmp/py_go_goose-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_go_goose-1.0.tar", last modified: Thu Jul 13 12:11:09 2023, max compression
+gzip compressed data, was "py_go_goose-1.1.tar", last modified: Thu Jul 13 12:34:05 2023, max compression
```

## Comparing `py_go_goose-1.0.tar` & `py_go_goose-1.1.tar`

### file list

```diff
@@ -1,19 +1,34 @@
-drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:11:09.892595 py_go_goose-1.0/
--rw-r--r--   0 dongmengnan   (501) staff       (20)    11325 2023-07-12 13:06:02.000000 py_go_goose-1.0/LICENSE
--rw-r--r--   0 dongmengnan   (501) staff       (20)       14 2023-07-13 11:02:03.000000 py_go_goose-1.0/MANIFEST.in
--rw-r--r--   0 dongmengnan   (501) staff       (20)       96 2023-07-13 12:11:09.892434 py_go_goose-1.0/PKG-INFO
--rw-r--r--   0 dongmengnan   (501) staff       (20)     2663 2023-07-12 13:06:02.000000 py_go_goose-1.0/README.md
-drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:11:09.888571 py_go_goose-1.0/go_goose/
--rw-r--r--   0 dongmengnan   (501) staff       (20)      337 2023-07-13 12:04:14.000000 py_go_goose-1.0/go_goose/go_goose.go
-drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:11:09.891157 py_go_goose-1.0/py_go_goose/
--rw-r--r--   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:05:01.000000 py_go_goose-1.0/py_go_goose/__init__.py
--rw-r--r--   0 dongmengnan   (501) staff       (20)    12554 2023-07-13 12:05:01.000000 py_go_goose-1.0/py_go_goose/build.py
--rw-r--r--   0 dongmengnan   (501) staff       (20)    48182 2023-07-13 12:05:01.000000 py_go_goose-1.0/py_go_goose/go.py
--rw-r--r--   0 dongmengnan   (501) staff       (20)     3110 2023-07-13 12:05:01.000000 py_go_goose-1.0/py_go_goose/go_goose.py
-drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:11:09.892196 py_go_goose-1.0/py_go_goose.egg-info/
--rw-r--r--   0 dongmengnan   (501) staff       (20)       96 2023-07-13 12:11:09.000000 py_go_goose-1.0/py_go_goose.egg-info/PKG-INFO
--rw-r--r--   0 dongmengnan   (501) staff       (20)      286 2023-07-13 12:11:09.000000 py_go_goose-1.0/py_go_goose.egg-info/SOURCES.txt
--rw-r--r--   0 dongmengnan   (501) staff       (20)        1 2023-07-13 12:11:09.000000 py_go_goose-1.0/py_go_goose.egg-info/dependency_links.txt
--rw-r--r--   0 dongmengnan   (501) staff       (20)       12 2023-07-13 12:11:09.000000 py_go_goose-1.0/py_go_goose.egg-info/top_level.txt
--rw-r--r--   0 dongmengnan   (501) staff       (20)       38 2023-07-13 12:11:09.892703 py_go_goose-1.0/setup.cfg
--rw-r--r--   0 dongmengnan   (501) staff       (20)      184 2023-07-13 12:04:59.000000 py_go_goose-1.0/setup.py
+drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:34:05.738419 py_go_goose-1.1/
+-rw-r--r--   0 dongmengnan   (501) staff       (20)    11325 2023-07-12 13:06:02.000000 py_go_goose-1.1/LICENSE
+-rw-r--r--   0 dongmengnan   (501) staff       (20)       14 2023-07-13 11:02:03.000000 py_go_goose-1.1/MANIFEST.in
+-rw-r--r--   0 dongmengnan   (501) staff       (20)       75 2023-07-13 12:34:05.738252 py_go_goose-1.1/PKG-INFO
+-rw-r--r--   0 dongmengnan   (501) staff       (20)     2663 2023-07-12 13:06:02.000000 py_go_goose-1.1/README.md
+drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:34:05.732744 py_go_goose-1.1/go_goose/
+-rw-r--r--   0 dongmengnan   (501) staff       (20)      337 2023-07-13 12:04:14.000000 py_go_goose-1.1/go_goose/go_goose.go
+drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:34:05.734135 py_go_goose-1.1/py_go_goose/
+-rw-r--r--   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:05:01.000000 py_go_goose-1.1/py_go_goose/__init__.py
+-rw-r--r--   0 dongmengnan   (501) staff       (20)    12554 2023-07-13 12:05:01.000000 py_go_goose-1.1/py_go_goose/build.py
+-rw-r--r--   0 dongmengnan   (501) staff       (20)    48182 2023-07-13 12:05:01.000000 py_go_goose-1.1/py_go_goose/go.py
+-rw-r--r--   0 dongmengnan   (501) staff       (20)     3110 2023-07-13 12:05:01.000000 py_go_goose-1.1/py_go_goose/go_goose.py
+drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:34:05.734804 py_go_goose-1.1/py_go_goose.egg-info/
+-rw-r--r--   0 dongmengnan   (501) staff       (20)       75 2023-07-13 12:34:05.000000 py_go_goose-1.1/py_go_goose.egg-info/PKG-INFO
+-rw-r--r--   0 dongmengnan   (501) staff       (20)      587 2023-07-13 12:34:05.000000 py_go_goose-1.1/py_go_goose.egg-info/SOURCES.txt
+-rw-r--r--   0 dongmengnan   (501) staff       (20)        1 2023-07-13 12:34:05.000000 py_go_goose-1.1/py_go_goose.egg-info/dependency_links.txt
+-rw-r--r--   0 dongmengnan   (501) staff       (20)       48 2023-07-13 12:34:05.000000 py_go_goose-1.1/py_go_goose.egg-info/top_level.txt
+-rw-r--r--   0 dongmengnan   (501) staff       (20)      189 2023-07-13 12:33:58.000000 py_go_goose-1.1/pyproject.toml
+-rw-r--r--   0 dongmengnan   (501) staff       (20)       38 2023-07-13 12:34:05.738480 py_go_goose-1.1/setup.cfg
+drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:34:05.731397 py_go_goose-1.1/venv/
+drwxr-xr-x   0 dongmengnan   (501) staff       (20)        0 2023-07-13 12:34:05.737966 py_go_goose-1.1/venv/bin/
+-rw-r--r--   0 dongmengnan   (501) staff       (20)     1175 2023-07-13 10:18:49.000000 py_go_goose-1.1/venv/bin/activate_this.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      667 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2html.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      789 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2html4.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)     1124 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2html5.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      866 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2latex.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      689 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2man.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      855 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2odt.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      661 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      674 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      710 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2s5.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      946 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      675 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rst2xml.py
+-rwxr-xr-x   0 dongmengnan   (501) staff       (20)      743 2023-07-13 11:05:06.000000 py_go_goose-1.1/venv/bin/rstpep2html.py
```

### Comparing `py_go_goose-1.0/LICENSE` & `py_go_goose-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_go_goose-1.0/README.md` & `py_go_goose-1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_go_goose-1.0/py_go_goose/build.py` & `py_go_goose-1.1/py_go_goose/build.py`

 * *Files identical despite different names*

### Comparing `py_go_goose-1.0/py_go_goose/go.py` & `py_go_goose-1.1/py_go_goose/go.py`

 * *Files identical despite different names*

### Comparing `py_go_goose-1.0/py_go_goose/go_goose.py` & `py_go_goose-1.1/py_go_goose/go_goose.py`

 * *Files identical despite different names*

