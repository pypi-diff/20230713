# Comparing `tmp/tkWidgetsRfzorzi-0.1.3.tar.gz` & `tmp/tkWidgetsRfzorzi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkWidgetsRfzorzi-0.1.3.tar", last modified: Thu Jul 13 20:05:48 2023, max compression
+gzip compressed data, was "tkWidgetsRfzorzi-0.1.4.tar", last modified: Thu Jul 13 20:41:52 2023, max compression
```

## Comparing `tkWidgetsRfzorzi-0.1.3.tar` & `tkWidgetsRfzorzi-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 20:05:48.049982 tkWidgetsRfzorzi-0.1.3/
--rw-rw-rw-   0        0        0     1210 2023-07-13 17:06:57.000000 tkWidgetsRfzorzi-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      383 2023-07-13 20:05:48.046475 tkWidgetsRfzorzi-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      994 2023-07-13 17:06:57.000000 tkWidgetsRfzorzi-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 20:05:47.956342 tkWidgetsRfzorzi-0.1.3/estiloWidgets/
--rw-rw-rw-   0        0        0        0 2023-07-13 17:06:57.000000 tkWidgetsRfzorzi-0.1.3/estiloWidgets/__init__.py
--rw-rw-rw-   0        0        0      509 2023-07-13 20:05:41.000000 tkWidgetsRfzorzi-0.1.3/estiloWidgets/setup.py
--rw-rw-rw-   0        0        0     6553 2023-07-07 12:53:03.000000 tkWidgetsRfzorzi-0.1.3/estiloWidgets/widgets_Glac.py
--rw-rw-rw-   0        0        0       42 2023-07-13 20:05:48.051481 tkWidgetsRfzorzi-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      509 2023-07-13 20:05:26.000000 tkWidgetsRfzorzi-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 20:05:48.039466 tkWidgetsRfzorzi-0.1.3/tkWidgetsRfzorzi.egg-info/
--rw-rw-rw-   0        0        0      383 2023-07-13 20:05:47.000000 tkWidgetsRfzorzi-0.1.3/tkWidgetsRfzorzi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-13 20:05:47.000000 tkWidgetsRfzorzi-0.1.3/tkWidgetsRfzorzi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 20:05:47.000000 tkWidgetsRfzorzi-0.1.3/tkWidgetsRfzorzi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-13 20:05:47.000000 tkWidgetsRfzorzi-0.1.3/tkWidgetsRfzorzi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 20:41:52.029443 tkWidgetsRfzorzi-0.1.4/
+-rw-rw-rw-   0        0        0     1210 2023-07-13 17:06:57.000000 tkWidgetsRfzorzi-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      383 2023-07-13 20:41:52.029443 tkWidgetsRfzorzi-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2023-07-13 17:06:57.000000 tkWidgetsRfzorzi-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 20:41:52.029443 tkWidgetsRfzorzi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      528 2023-07-13 20:41:43.000000 tkWidgetsRfzorzi-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:41:51.998191 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi/
+-rw-rw-rw-   0        0        0        0 2023-07-13 17:06:57.000000 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi/__init__.py
+-rw-rw-rw-   0        0        0      528 2023-07-13 20:41:43.000000 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi/setup.py
+-rw-rw-rw-   0        0        0     6553 2023-07-07 12:53:03.000000 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi/widgets_Glac.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:41:52.029443 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-07-13 20:41:51.000000 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-07-13 20:41:51.000000 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 20:41:51.000000 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-13 20:41:51.000000 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-13 20:41:51.000000 tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi.egg-info/top_level.txt
```

### Comparing `tkWidgetsRfzorzi-0.1.3/LICENSE` & `tkWidgetsRfzorzi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tkWidgetsRfzorzi-0.1.3/README.md` & `tkWidgetsRfzorzi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tkWidgetsRfzorzi-0.1.3/estiloWidgets/widgets_Glac.py` & `tkWidgetsRfzorzi-0.1.4/tkWidgetsRfzorzi/widgets_Glac.py`

 * *Files identical despite different names*

