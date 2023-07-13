# Comparing `tmp/qvsed-1.5.1.tar.gz` & `tmp/qvsed-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.1.tar", last modified: Thu Jul 13 11:32:20 2023, max compression
+gzip compressed data, was "qvsed-1.5.2.tar", last modified: Thu Jul 13 12:04:06 2023, max compression
```

## Comparing `qvsed-1.5.1.tar` & `qvsed-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 11:32:20.724235 qvsed-1.5.1/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-13 11:32:20.722162 qvsed-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     6653 2023-07-13 11:27:44.000000 qvsed-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 11:32:20.696414 qvsed-1.5.1/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.1/qvsed/__init__.py
--rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.5.1/qvsed/config_default.py
--rw-rw-rw-   0        0        0    25829 2023-07-13 11:30:44.000000 qvsed-1.5.1/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.1/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     3754 2023-07-13 10:44:09.000000 qvsed-1.5.1/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-13 11:32:20.719955 qvsed-1.5.1/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 11:32:20.724235 qvsed-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-13 11:31:04.000000 qvsed-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:04:06.271438 qvsed-1.5.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-13 12:04:06.270142 qvsed-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6653 2023-07-13 11:27:44.000000 qvsed-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 12:04:06.254160 qvsed-1.5.2/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.2/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.5.2/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    26033 2023-07-13 12:02:40.000000 qvsed-1.5.2/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.2/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     3754 2023-07-13 10:44:09.000000 qvsed-1.5.2/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-13 12:04:06.270142 qvsed-1.5.2/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-13 12:04:06.000000 qvsed-1.5.2/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-13 12:04:06.000000 qvsed-1.5.2/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:04:06.000000 qvsed-1.5.2/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 12:04:06.000000 qvsed-1.5.2/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 12:04:06.000000 qvsed-1.5.2/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 12:04:06.000000 qvsed-1.5.2/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 12:04:06.272502 qvsed-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-13 12:03:52.000000 qvsed-1.5.2/setup.py
```

### Comparing `qvsed-1.5.1/LICENSE.txt` & `qvsed-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.1/PKG-INFO` & `qvsed-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.1
+Version: 1.5.2
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.1/README.md` & `qvsed-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.1/qvsed/config_default.py` & `qvsed-1.5.2/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.1/qvsed/qvsed.py` & `qvsed-1.5.2/qvsed/qvsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,20 +431,27 @@
 
         dialog_box = FileDialogBox("save", self)
         if dialog_box.exec_():
             file_path = dialog_box.get_selected_file_path()
         else:
             return
 
+        if not os.path.exists(file_path):
+            saved = "Saved new"
+            with open(file_path, "w", encoding="UTF-8"):
+                pass
+        else:
+            saved = "Saved"
+
         if file_path:
             try:
                 with open(file_path, "w", encoding="UTF-8") as file:
                     file.write(text_area.toPlainText())
                 file_name = os.path.basename(file_path)
-                self.echo_area_update(f"Saved file {file_name}.")
+                self.echo_area_update(f"{saved} file {file_name}.")
             except Exception as error:
                 self.echo_area_update(f"Error saving file: {str(error)}")
 
 
     def set_text_area_encoding(self, encoding):
         """
         Set the Text Area encoding.
```

### Comparing `qvsed-1.5.1/qvsed/qvsed.ui` & `qvsed-1.5.2/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.1/qvsed/qvsed_dialog.ui` & `qvsed-1.5.2/qvsed/qvsed_dialog.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.1/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.2/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.1
+Version: 1.5.2
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.1/setup.py` & `qvsed-1.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.1',
+    version='1.5.2',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

