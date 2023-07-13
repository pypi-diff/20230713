# Comparing `tmp/0x0-python-0.2.tar.gz` & `tmp/0x0-python-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "0x0-python-0.2.tar", last modified: Thu Jul 13 16:14:06 2023, max compression
+gzip compressed data, was "0x0-python-0.5.tar", last modified: Thu Jul 13 16:25:42 2023, max compression
```

## Comparing `0x0-python-0.2.tar` & `0x0-python-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:14:06.041328 0x0-python-0.2/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:14:06.041328 0x0-python-0.2/0x0_python.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      873 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      217 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-13 15:42:20.000000 0x0-python-0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-13 15:42:20.000000 0x0-python-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)      873 2023-07-13 16:14:06.045328 0x0-python-0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-07-13 16:09:38.000000 0x0-python-0.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-13 16:14:06.045328 0x0-python-0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      768 2023-07-13 16:12:58.000000 0x0-python-0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:25:42.648681 0x0-python-0.5/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:25:42.648681 0x0-python-0.5/0x0_python.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1343 2023-07-13 16:25:42.000000 0x0-python-0.5/0x0_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      217 2023-07-13 16:25:42.000000 0x0-python-0.5/0x0_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:25:42.000000 0x0-python-0.5/0x0_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:25:42.000000 0x0-python-0.5/0x0_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:25:42.000000 0x0-python-0.5/0x0_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-13 15:42:20.000000 0x0-python-0.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-13 15:42:20.000000 0x0-python-0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     1343 2023-07-13 16:25:42.648681 0x0-python-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      837 2023-07-13 16:24:35.000000 0x0-python-0.5/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-13 16:25:42.652681 0x0-python-0.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      761 2023-07-13 16:25:04.000000 0x0-python-0.5/setup.py
```

### Comparing `0x0-python-0.2/LICENSE` & `0x0-python-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `0x0-python-0.2/setup.py` & `0x0-python-0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from markdown import markdown
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description_md = f.read()
     long_description_html = markdown(long_description_md, extensions=['markdown.extensions.fenced_code'])
 
 setup(name='0x0-python',
-      version='0.2',
-      description='Библиотека для взаимодействия с 0x0 point через питон',
+      version='0.5',
+      description='Библиотека для взаимодействия с 0x0.st через Python',
       long_description=long_description_html,
       long_description_content_type='text/markdown',
       author_email='neso_hoshi_official@mail.ru',
       zip_safe=False,
       author='Neso Hiroshi',
       classifiers = [
     "Programming Language :: Python :: 3",
```

