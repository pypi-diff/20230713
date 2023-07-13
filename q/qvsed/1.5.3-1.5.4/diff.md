# Comparing `tmp/qvsed-1.5.3.tar.gz` & `tmp/qvsed-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.3.tar", last modified: Thu Jul 13 12:54:32 2023, max compression
+gzip compressed data, was "qvsed-1.5.4.tar", last modified: Thu Jul 13 13:11:41 2023, max compression
```

## Comparing `qvsed-1.5.3.tar` & `qvsed-1.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 12:54:32.244646 qvsed-1.5.3/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.3/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-13 12:54:32.243646 qvsed-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     6653 2023-07-13 12:44:21.000000 qvsed-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 12:54:32.218605 qvsed-1.5.3/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.3/qvsed/__init__.py
--rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.5.3/qvsed/config_default.py
--rw-rw-rw-   0        0        0    25677 2023-07-13 12:53:09.000000 qvsed-1.5.3/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.3/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     3754 2023-07-13 10:44:09.000000 qvsed-1.5.3/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-13 12:54:32.242524 qvsed-1.5.3/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-13 12:54:32.000000 qvsed-1.5.3/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-13 12:54:32.000000 qvsed-1.5.3/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 12:54:32.000000 qvsed-1.5.3/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 12:54:32.000000 qvsed-1.5.3/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 12:54:32.000000 qvsed-1.5.3/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 12:54:32.000000 qvsed-1.5.3/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 12:54:32.244646 qvsed-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-13 12:54:07.000000 qvsed-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:11:41.461550 qvsed-1.5.4/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-13 13:11:41.460466 qvsed-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6653 2023-07-13 12:44:21.000000 qvsed-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 13:11:41.444951 qvsed-1.5.4/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.4/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.5.4/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    25720 2023-07-13 13:11:04.000000 qvsed-1.5.4/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.4/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     3754 2023-07-13 10:44:09.000000 qvsed-1.5.4/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-13 13:11:41.459258 qvsed-1.5.4/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 13:11:41.461550 qvsed-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-13 13:11:24.000000 qvsed-1.5.4/setup.py
```

### Comparing `qvsed-1.5.3/LICENSE.txt` & `qvsed-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.3/PKG-INFO` & `qvsed-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.3
+Version: 1.5.4
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.3/README.md` & `qvsed-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.3/qvsed/config_default.py` & `qvsed-1.5.4/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.3/qvsed/qvsed.py` & `qvsed-1.5.4/qvsed/qvsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,18 @@
 
         stylesheet = f"""
 QMainWindow, QDialog {{
     color: {text_color};
     background: {background_color};
 }}
 
+QLabel {{
+    color: {text_color};
+}}
+
 QPlainTextEdit, QLineEdit {{
     padding: 8px;
     border: none;
 }}
 
 QPlainTextEdit {{
     color: {text_color};
```

### Comparing `qvsed-1.5.3/qvsed/qvsed.ui` & `qvsed-1.5.4/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.3/qvsed/qvsed_dialog.ui` & `qvsed-1.5.4/qvsed/qvsed_dialog.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.3/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.4/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.3
+Version: 1.5.4
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.3/setup.py` & `qvsed-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.3',
+    version='1.5.4',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

