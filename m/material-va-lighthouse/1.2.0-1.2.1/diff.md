# Comparing `tmp/material-va-lighthouse-1.2.0.tar.gz` & `tmp/material-va-lighthouse-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material-va-lighthouse-1.2.0.tar", last modified: Wed Jun 28 21:54:15 2023, max compression
+gzip compressed data, was "material-va-lighthouse-1.2.1.tar", last modified: Thu Jul 13 00:08:43 2023, max compression
```

## Comparing `material-va-lighthouse-1.2.0.tar` & `material-va-lighthouse-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-06-28 21:54:15.882222 material-va-lighthouse-1.2.0/
--rw-r--r--   0 alastairdawson   (501) staff       (20)     1327 2023-05-19 16:12:29.000000 material-va-lighthouse-1.2.0/LICENSE
--rw-r--r--   0 alastairdawson   (501) staff       (20)      267 2023-06-28 21:54:15.882096 material-va-lighthouse-1.2.0/PKG-INFO
--rw-r--r--   0 alastairdawson   (501) staff       (20)      968 2023-06-28 21:47:16.000000 material-va-lighthouse-1.2.0/README.md
-drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-06-28 21:54:15.880999 material-va-lighthouse-1.2.0/material_va_lighthouse/
--rw-r--r--   0 alastairdawson   (501) staff       (20)        0 2023-05-19 16:12:29.000000 material-va-lighthouse-1.2.0/material_va_lighthouse/__init__.py
--rw-r--r--   0 alastairdawson   (501) staff       (20)      915 2023-05-19 16:12:29.000000 material-va-lighthouse-1.2.0/material_va_lighthouse/plugin.py
--rw-r--r--   0 alastairdawson   (501) staff       (20)     1233 2023-06-28 21:47:16.000000 material-va-lighthouse-1.2.0/material_va_lighthouse/va_lighthouse.css
--rw-r--r--   0 alastairdawson   (501) staff       (20)     3180 2023-05-19 16:12:29.000000 material-va-lighthouse-1.2.0/material_va_lighthouse/va_lighthouse_logo.png
-drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-06-28 21:54:15.881876 material-va-lighthouse-1.2.0/material_va_lighthouse.egg-info/
--rw-r--r--   0 alastairdawson   (501) staff       (20)      267 2023-06-28 21:54:15.000000 material-va-lighthouse-1.2.0/material_va_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 alastairdawson   (501) staff       (20)      459 2023-06-28 21:54:15.000000 material-va-lighthouse-1.2.0/material_va_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)        1 2023-06-28 21:54:15.000000 material-va-lighthouse-1.2.0/material_va_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)       99 2023-06-28 21:54:15.000000 material-va-lighthouse-1.2.0/material_va_lighthouse.egg-info/entry_points.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)       66 2023-06-28 21:54:15.000000 material-va-lighthouse-1.2.0/material_va_lighthouse.egg-info/requires.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)       23 2023-06-28 21:54:15.000000 material-va-lighthouse-1.2.0/material_va_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)       38 2023-06-28 21:54:15.882275 material-va-lighthouse-1.2.0/setup.cfg
--rw-r--r--   0 alastairdawson   (501) staff       (20)      762 2023-06-28 21:50:43.000000 material-va-lighthouse-1.2.0/setup.py
+drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-07-13 00:08:43.428575 material-va-lighthouse-1.2.1/
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     1327 2023-05-19 16:12:29.000000 material-va-lighthouse-1.2.1/LICENSE
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     1276 2023-07-13 00:08:43.428439 material-va-lighthouse-1.2.1/PKG-INFO
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      968 2023-06-28 21:47:16.000000 material-va-lighthouse-1.2.1/README.md
+drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-07-13 00:08:43.427298 material-va-lighthouse-1.2.1/material_va_lighthouse/
+-rw-r--r--   0 alastairdawson   (501) staff       (20)        0 2023-05-19 16:12:29.000000 material-va-lighthouse-1.2.1/material_va_lighthouse/__init__.py
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      915 2023-05-19 16:12:29.000000 material-va-lighthouse-1.2.1/material_va_lighthouse/plugin.py
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     1233 2023-06-28 21:47:16.000000 material-va-lighthouse-1.2.1/material_va_lighthouse/va_lighthouse.css
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     3180 2023-05-19 16:12:29.000000 material-va-lighthouse-1.2.1/material_va_lighthouse/va_lighthouse_logo.png
+drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-07-13 00:08:43.428218 material-va-lighthouse-1.2.1/material_va_lighthouse.egg-info/
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     1276 2023-07-13 00:08:43.000000 material-va-lighthouse-1.2.1/material_va_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      459 2023-07-13 00:08:43.000000 material-va-lighthouse-1.2.1/material_va_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)        1 2023-07-13 00:08:43.000000 material-va-lighthouse-1.2.1/material_va_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)       99 2023-07-13 00:08:43.000000 material-va-lighthouse-1.2.1/material_va_lighthouse.egg-info/entry_points.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)       66 2023-07-13 00:08:43.000000 material-va-lighthouse-1.2.1/material_va_lighthouse.egg-info/requires.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)       23 2023-07-13 00:08:43.000000 material-va-lighthouse-1.2.1/material_va_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)       38 2023-07-13 00:08:43.428634 material-va-lighthouse-1.2.1/setup.cfg
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     1019 2023-07-12 23:53:06.000000 material-va-lighthouse-1.2.1/setup.py
```

### Comparing `material-va-lighthouse-1.2.0/LICENSE` & `material-va-lighthouse-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.2.0/README.md` & `material-va-lighthouse-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.2.0/material_va_lighthouse/plugin.py` & `material-va-lighthouse-1.2.1/material_va_lighthouse/plugin.py`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.2.0/material_va_lighthouse/va_lighthouse.css` & `material-va-lighthouse-1.2.1/material_va_lighthouse/va_lighthouse.css`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.2.0/material_va_lighthouse/va_lighthouse_logo.png` & `material-va-lighthouse-1.2.1/material_va_lighthouse/va_lighthouse_logo.png`

 * *Files identical despite different names*

