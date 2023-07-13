# Comparing `tmp/qvsed-1.5.4.tar.gz` & `tmp/qvsed-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.4.tar", last modified: Thu Jul 13 13:11:41 2023, max compression
+gzip compressed data, was "qvsed-1.5.5.tar", last modified: Thu Jul 13 15:27:04 2023, max compression
```

## Comparing `qvsed-1.5.4.tar` & `qvsed-1.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 13:11:41.461550 qvsed-1.5.4/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.4/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-13 13:11:41.460466 qvsed-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     6653 2023-07-13 12:44:21.000000 qvsed-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 13:11:41.444951 qvsed-1.5.4/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.4/qvsed/__init__.py
--rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.5.4/qvsed/config_default.py
--rw-rw-rw-   0        0        0    25720 2023-07-13 13:11:04.000000 qvsed-1.5.4/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.4/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     3754 2023-07-13 10:44:09.000000 qvsed-1.5.4/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-13 13:11:41.459258 qvsed-1.5.4/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 13:11:41.000000 qvsed-1.5.4/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 13:11:41.461550 qvsed-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-13 13:11:24.000000 qvsed-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:27:04.502818 qvsed-1.5.5/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-13 15:27:04.501825 qvsed-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6653 2023-07-13 12:44:21.000000 qvsed-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 15:27:04.474974 qvsed-1.5.5/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.5/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      729 2023-07-13 13:56:47.000000 qvsed-1.5.5/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    26381 2023-07-13 15:26:19.000000 qvsed-1.5.5/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.5/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     4175 2023-07-13 15:16:38.000000 qvsed-1.5.5/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-13 15:27:04.499795 qvsed-1.5.5/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 15:27:04.502818 qvsed-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-13 15:26:45.000000 qvsed-1.5.5/setup.py
```

### Comparing `qvsed-1.5.4/LICENSE.txt` & `qvsed-1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.4/PKG-INFO` & `qvsed-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.4
+Version: 1.5.5
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.4/README.md` & `qvsed-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.4/qvsed/config_default.py` & `qvsed-1.5.5/qvsed/config_default.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 font_family = ["JetBrains Mono", "Cascadia Code", "Consolas", "Menlo", "monospace"]
 font_size = 11
 
 # Colours
 text_color = "#FFFFFF"
 background_color = "#282C34"
 
+button_text_color = "#FFFFFF"
 button_color = "#393F4A"
 button_hover_color = "#31353F"
 button_pressed_color = "#282C34"
 
+text_area_text_color = "#FFFFFF"
 text_area_color = "#31353F"
+
+echo_area_text_color = "#FFFFFF"
 echo_area_color = "#393F4A"
 
 scroll_bar_color = "#363D49"
 scroll_bar_background_color = "#282F3B"
 scroll_bar_hover_color = "#4F5664"
 scroll_bar_pressed_color = "#262B34"
```

### Comparing `qvsed-1.5.4/qvsed/qvsed.py` & `qvsed-1.5.5/qvsed/qvsed.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,18 +66,19 @@
         self.set_up_action_deck()
         self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         self.load_config()
         self.set_up_fonts()
         if self.check_if_file_parameter():
             self.load_from_file(sys.argv[1])
 
-    def apply_style_sheet(self, text_color, background_color, button_color,
-                          button_hover_color, button_pressed_color, text_area_color,
-                          echo_area_color, scroll_bar_color, scroll_bar_background_color,
-                          scroll_bar_hover_color, scroll_bar_pressed_color):
+    def apply_style_sheet(self, text_color, background_color, button_color, button_text_color,
+                            button_hover_color, button_pressed_color, text_area_color,
+                            text_area_text_color, echo_area_color, echo_area_text_color,
+                            scroll_bar_color, scroll_bar_background_color, scroll_bar_hover_color,
+                            scroll_bar_pressed_color):
         """
         Generate and apply a style sheet based on the config.py file.
         """
 
         stylesheet = f"""
 QMainWindow, QDialog {{
     color: {text_color};
@@ -90,25 +91,25 @@
 
 QPlainTextEdit, QLineEdit {{
     padding: 8px;
     border: none;
 }}
 
 QPlainTextEdit {{
-    color: {text_color};
+    color: {text_area_text_color};
     background: {text_area_color};
 }}
 
 QLineEdit {{
-    color: {text_color};
+    color: {echo_area_text_color};
     background: {echo_area_color};
 }}
 
 QPushButton {{
-    color: {text_color};
+    color: {button_text_color};
     border: 2px solid {button_hover_color};
     background: {button_color};
     padding: 2px;
 }}
 
 QPushButton:hover {{
     color: {text_color};
@@ -327,29 +328,33 @@
 
         # Load the colour scheme settings from the config file
         # We use the shorter American spellings because it's standard, I guess
         text_color = getattr(qvsed_config, 'text_color', None)
         background_color = getattr(qvsed_config, 'background_color', None)
 
         button_color = getattr(qvsed_config, 'button_color', None)
+        button_text_color = getattr(qvsed_config, 'button_text_color', text_color)
         button_hover_color = getattr(qvsed_config, 'button_hover_color', getattr(qvsed_config, 'button_focus_color', None))
         button_pressed_color = getattr(qvsed_config, 'button_pressed_color', background_color)
 
         text_area_color = getattr(qvsed_config, 'text_area_color', button_hover_color)
+        text_area_text_color = getattr(qvsed_config, 'text_area_text_color', text_color)
         echo_area_color = getattr(qvsed_config, 'echo_area_color', button_hover_color)
+        echo_area_text_color = getattr(qvsed_config, 'echo_area_text_color', text_color)
 
         scroll_bar_color = getattr(qvsed_config, 'scroll_bar_color', button_color)
         scroll_bar_background_color = getattr(qvsed_config, 'scroll_bar_background_color', button_hover_color)
         scroll_bar_hover_color = getattr(qvsed_config, 'scroll_bar_hover_color', button_pressed_color)
         scroll_bar_pressed_color = getattr(qvsed_config, 'scroll_bar_pressed_color', button_pressed_color)
 
-        self.apply_style_sheet(text_color, background_color, button_color,
+        self.apply_style_sheet(text_color, background_color, button_color, button_text_color,
                                button_hover_color, button_pressed_color, text_area_color,
-                               echo_area_color, scroll_bar_color, scroll_bar_background_color,
-                               scroll_bar_hover_color, scroll_bar_pressed_color)
+                               text_area_text_color, echo_area_color, echo_area_text_color,
+                               scroll_bar_color, scroll_bar_background_color, scroll_bar_hover_color,
+                               scroll_bar_pressed_color)
 
         if None in (text_color, background_color, button_color, button_hover_color):
             self.echo_area_update("config.py appears to be broken, generating a new one.")
             self.generate_config()
 
     def load_from_file(self, file_path=None):
         """
@@ -641,14 +646,18 @@
     """
     Class for QVSED file dialogs.
     """
     def __init__(self, operation, parent=None):
         super(FileDialogBox, self).__init__(parent)
         self.load_ui_file()
 
+        home_dir = os.path.expanduser("~")
+        cwd = os.getcwd().replace(home_dir, "~").replace("\\", "/")
+        self.cwdLabel.setText(f"Current working directory is {cwd}")
+
         self.operation = operation
         self.selected_file_path = ""
 
         self.setWindowTitle(f"{self.operation.capitalize()} File")
 
         self.set_shortcuts()
         self.update_labels()
@@ -676,15 +685,15 @@
         loadUi(ui_file, self)
 
     def open_system_dialog(self):
         """
         Used to open the system's file dialog.
         """
         file_dialog = QFileDialog()
-        
+
         if self.operation == "save":
             file_path, _ = file_dialog.getOpenFileName(self, "Save File")
         elif self.operation == "open":
             file_path, _ = file_dialog.getOpenFileName(self, "Open File")
 
         if file_path:
             self.filePathBox.setText(file_path)
```

### Comparing `qvsed-1.5.4/qvsed/qvsed.ui` & `qvsed-1.5.5/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.4/qvsed/qvsed_dialog.ui` & `qvsed-1.5.5/qvsed/qvsed_dialog.ui`

 * *Files 2% similar despite different names*

#### Comparing `qvsed-1.5.4/qvsed/qvsed_dialog.ui` & `qvsed-1.5.5/qvsed/qvsed_dialog.ui`

```diff
@@ -3,15 +3,15 @@
   <class>FileDialog</class>
   <widget class="QDialog" name="FileDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>556</width>
-        <height>181</height>
+        <height>216</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Dialog</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout_2">
       <item>
@@ -43,14 +43,29 @@
               </property>
               <property name="alignment">
                 <set>Qt::AlignCenter</set>
               </property>
             </widget>
           </item>
           <item>
+            <widget class="QLabel" name="cwdLabel">
+              <property name="font">
+                <font>
+                  <pointsize>12</pointsize>
+                </font>
+              </property>
+              <property name="text">
+                <string>Current working directory is &lt;cwd&gt;</string>
+              </property>
+              <property name="alignment">
+                <set>Qt::AlignCenter</set>
+              </property>
+            </widget>
+          </item>
+          <item>
             <widget class="QLineEdit" name="filePathBox">
               <property name="font">
                 <font>
                   <pointsize>11</pointsize>
                 </font>
               </property>
               <property name="styleSheet">
```

### Comparing `qvsed-1.5.4/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.5/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.4
+Version: 1.5.5
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.4/setup.py` & `qvsed-1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.4',
+    version='1.5.5',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

