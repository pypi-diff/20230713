# Comparing `tmp/qvsed-1.4.6.tar.gz` & `tmp/qvsed-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.4.6.tar", last modified: Wed Jul 12 15:24:00 2023, max compression
+gzip compressed data, was "qvsed-1.5.0.tar", last modified: Thu Jul 13 11:16:44 2023, max compression
```

## Comparing `qvsed-1.4.6.tar` & `qvsed-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:24:00.641591 qvsed-1.4.6/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-12 15:24:00.641591 qvsed-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     7228 2023-07-11 10:35:02.000000 qvsed-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 15:24:00.621207 qvsed-1.4.6/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.4.6/qvsed/__init__.py
--rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.4.6/qvsed/config_default.py
--rw-rw-rw-   0        0        0    22683 2023-07-12 15:23:21.000000 qvsed-1.4.6/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.4.6/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-12 15:24:00.639592 qvsed-1.4.6/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 15:24:00.000000 qvsed-1.4.6/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:24:00.642610 qvsed-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-12 15:23:46.000000 qvsed-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:16:44.650379 qvsed-1.5.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-13 11:16:44.649109 qvsed-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7228 2023-07-11 10:35:02.000000 qvsed-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 11:16:44.637898 qvsed-1.5.0/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.0/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.5.0/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    25820 2023-07-13 11:15:40.000000 qvsed-1.5.0/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.0/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     3754 2023-07-13 10:44:09.000000 qvsed-1.5.0/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-13 11:16:44.648117 qvsed-1.5.0/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 11:16:44.650379 qvsed-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-13 11:05:52.000000 qvsed-1.5.0/setup.py
```

### Comparing `qvsed-1.4.6/LICENSE.txt` & `qvsed-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.6/PKG-INFO` & `qvsed-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.4.6
+Version: 1.5.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.4.6/README.md` & `qvsed-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.6/qvsed/config_default.py` & `qvsed-1.5.0/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.6/qvsed/qvsed.py` & `qvsed-1.5.0/qvsed/qvsed.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import os
 import sys
 import shutil
 import importlib.util
 import pkg_resources
 from PyQt5.QtWidgets import (
     QApplication, QMainWindow, QWidget, QFileDialog,
-    QAction, QShortcut
+    QAction, QShortcut, QDialog
 )
 from PyQt5.QtGui import (
     QKeySequence, QFont, QDragEnterEvent, QDropEvent,
     QTextCursor
 )
 from PyQt5.QtCore import (
     Qt, QTextCodec, QEvent, QObject, QTimer
@@ -343,31 +343,37 @@
                                echo_area_color, scroll_bar_color, scroll_bar_background_color,
                                scroll_bar_hover_color, scroll_bar_pressed_color)
 
         if None in (text_color, background_color, button_color, button_hover_color):
             self.echo_area_update("config.py appears to be broken, generating a new one.")
             self.generate_config()
 
-    def load_from_file(self, file_path = None):
+    def load_from_file(self, file_path=None):
         """
         Open a file dialog, and load the contents of a file into the Text Area.
         """
         text_area = self.textArea
 
         if not file_path:
-            file_path, _ = QFileDialog.getOpenFileName(self, "Open File")
+            dialog_box = FileDialogBox("open", self)
+            if dialog_box.exec_():
+                file_path = dialog_box.get_selected_file_path()
+            else:
+                return
 
         if file_path:
             try:
                 with open(file_path, "r", encoding="utf-8") as file:
                     text_area.setPlainText(file.read())
                 file_name = os.path.basename(file_path)
                 self.echo_area_update(f"Opened file {file_name}.")
             except Exception as error:
                 self.echo_area_update(f"Error opening file: {str(error)}")
+        else:
+            self.echo_area_update("Invalid or missing file path.")
 
     def load_ui_file(self):
         """
         Load the UI file for the QVSED window.
         """
         current_dir = os.path.dirname(os.path.abspath(__file__))
         ui_file = os.path.join(current_dir, "qvsed.ui")
@@ -419,25 +425,30 @@
         """
         text_area = self.textArea
 
         if text_area.toPlainText() == "":
             self.echo_area_update("Text Area is blank, will not save.")
             return
 
-        file_path, _ = QFileDialog.getSaveFileName(self, "Save File")
+        dialog_box = FileDialogBox("save", self)
+        if dialog_box.exec_():
+            file_path = dialog_box.get_selected_file_path()
+        else:
+            return
 
         if file_path:
             try:
                 with open(file_path, "w", encoding="UTF-8") as file:
                     file.write(text_area.toPlainText())
                 file_name = os.path.basename(file_path)
                 self.echo_area_update(f"Saved file {file_name}.")
             except Exception as error:
                 self.echo_area_update(f"Error saving file: {str(error)}")
 
+
     def set_text_area_encoding(self, encoding):
         """
         Set the Text Area encoding.
 
         Args:
             encoding (str): The encoding to set for the Text Area.
         """
@@ -611,14 +622,98 @@
 
                 key_combination = "-".join(keys)
                 undefined_message = f"<{key_combination}> is undefined."
                 self.window.echo_area_update(undefined_message)
                 return True
         return super().eventFilter(obj, event)
 
+class FileDialogBox(QDialog):
+    """
+    Class for QVSED file dialogs.
+    """
+    def __init__(self, operation, parent=None):
+        super(FileDialogBox, self).__init__(parent)
+        self.load_ui_file()
+
+        self.operation = operation
+        self.selected_file_path = ""
+
+        self.setWindowTitle(f"{self.operation.capitalize()} File")
+
+        self.set_shortcuts()
+        self.update_labels()
+
+    def set_shortcuts(self):
+        """
+        Self-explanatory.
+        """
+        self.confirmButton.clicked.connect(self.accept)
+        self.confirmButton.setShortcut(QKeySequence(Qt.Key_Return))
+
+        self.cancelButton.clicked.connect(self.reject)
+        self.cancelButton.setShortcut(QKeySequence(Qt.Key_Escape))
+        self.cancelButton.setShortcut(QKeySequence("Alt+Q"))
+
+        self.openSystemDialogButton.clicked.connect(self.open_system_dialog)
+        self.openSystemDialogButton.setShortcut(QKeySequence("Ctrl+D"))
+
+    def load_ui_file(self):
+        """
+        Load the UI file for the QVSED dialog box.
+        """
+        current_dir = os.path.dirname(os.path.abspath(__file__))
+        ui_file = os.path.join(current_dir, "qvsed_dialog.ui")
+        loadUi(ui_file, self)
+
+    def open_file_dialog(self):
+        """
+        Used for opening files.
+        """
+        file_path, _ = QFileDialog.getOpenFileName(self, "Open File")
+        if file_path:
+            return os.path.abspath(file_path)
+        return ""
+
+    def save_file_dialog(self):
+        """
+        Used for saving files.
+        """
+        file_path, _ = QFileDialog.getSaveFileName(self, "Save File")
+        if file_path:
+            return os.path.abspath(file_path)
+        return ""
+
+    def open_system_dialog(self):
+        """
+        Used to open the system's file dialog.
+        """
+        file_dialog = QFileDialog()
+        file_path, _ = file_dialog.getOpenFileName(self, "Open File" if self.operation == "open" else "Save File")
+        if file_path:
+            self.filePathBox.setText(file_path)
+            self.selected_file_path = file_path
+
+    def get_selected_file_path(self):
+        """
+        Return the file path specified in the file path box.
+        """
+        file_path = self.filePathBox.text()
+        if os.name == 'nt' and file_path.startswith('~'):
+            file_path = os.path.expanduser(file_path.replace('~', os.path.expanduser('~')))
+        if file_path:
+            return file_path
+        return None
+
+    def update_labels(self):
+        """
+        Update the labels depending on the operation
+        """
+        self.mainLabel.setText(f"Enter the file path to {self.operation} (relative or absolute)")
+        self.confirmButton.setText(self.operation.capitalize())
+
 def main():
     """
     The entry point for the QVSED application.
     """
     app = QVSEDApp()
     app.run()
```

### Comparing `qvsed-1.4.6/qvsed/qvsed.ui` & `qvsed-1.5.0/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.6/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.0/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.4.6
+Version: 1.5.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.4.6/setup.py` & `qvsed-1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.4.6',
+    version='1.5.0',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
@@ -28,9 +28,9 @@
         'PyQt5'
     ],
     entry_points={
         'gui_scripts': [
             'qvsed = qvsed.qvsed:main',
         ],
     },
-    package_data={'qvsed': ['qvsed.ui']},
+    package_data={'qvsed': ['qvsed.ui', 'qvsed_dialog.ui']},
 )
```

