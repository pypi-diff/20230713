# Comparing `tmp/qvsed-1.5.0.tar.gz` & `tmp/qvsed-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.0.tar", last modified: Thu Jul 13 11:16:44 2023, max compression
+gzip compressed data, was "qvsed-1.5.1.tar", last modified: Thu Jul 13 11:32:20 2023, max compression
```

## Comparing `qvsed-1.5.0.tar` & `qvsed-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 11:16:44.650379 qvsed-1.5.0/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-13 11:16:44.649109 qvsed-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     7228 2023-07-11 10:35:02.000000 qvsed-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 11:16:44.637898 qvsed-1.5.0/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.0/qvsed/__init__.py
--rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.5.0/qvsed/config_default.py
--rw-rw-rw-   0        0        0    25820 2023-07-13 11:15:40.000000 qvsed-1.5.0/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.0/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     3754 2023-07-13 10:44:09.000000 qvsed-1.5.0/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-13 11:16:44.648117 qvsed-1.5.0/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 11:16:44.000000 qvsed-1.5.0/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 11:16:44.650379 qvsed-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-13 11:05:52.000000 qvsed-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:32:20.724235 qvsed-1.5.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-13 11:32:20.722162 qvsed-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6653 2023-07-13 11:27:44.000000 qvsed-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 11:32:20.696414 qvsed-1.5.1/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.1/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.5.1/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    25829 2023-07-13 11:30:44.000000 qvsed-1.5.1/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.1/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     3754 2023-07-13 10:44:09.000000 qvsed-1.5.1/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-13 11:32:20.719955 qvsed-1.5.1/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 11:32:20.000000 qvsed-1.5.1/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 11:32:20.724235 qvsed-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-13 11:31:04.000000 qvsed-1.5.1/setup.py
```

### Comparing `qvsed-1.5.0/LICENSE.txt` & `qvsed-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.0/PKG-INFO` & `qvsed-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.0
+Version: 1.5.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.0/README.md` & `qvsed-1.5.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # QVSED - Qt-based Volatile Small Editor
 
 QVSED is a volatile text editor.
 
 ![QVSED screenshot, showing the help message](qvsed-screenshot.png)
 
-"Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded. Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata. You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
+"Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
+Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 
-QVSED follows the philosophy of ultra-minimalism, with its heavy emphasis on just editing text and nothing more. QVSED's editing style is text-based, not file-based like basically every other editor out there. Text goes in, from a file, and then text later comes out, into another or perhaps the same file.
+QVSED follows the philosophy of ultra-minimalism, with its heavy emphasis on just editing text and nothing more.
+QVSED's editing style is text-based, not file-based like basically every other editor out there.
+Text goes in, from a file, and then text later comes out, into another or perhaps the same file.
 
-QVSED can be used as a simple scratchpad or throwaway editor, as well as a general editing software application, since it won't prompt you if you do anything destructive, It stays out of your way on many occasions. Whether or not that's a good thing is up to you.
+QVSED works well as a simple scratchpad, but it's also quite useful for more involved editing operations, providing a seamless experience without posing prompts for potentially destructive actions.
+It's not as powerful as something like Vim or even ed, but it provides a unique editing experience you won't find anywhere else. Whether or not this is a good thing is up to you.
 
 QVSED is a PyQt5 rewrite of my older project, [ASMED (Another SMol EDitor)](https://github.com/That1M8Head/ASMED), which was written using Windows Forms, and was quite obviously only for Windows.
 
 QVSED aims to replace ASMED by offering cross-platform support and the advantages of a lightweight editor without the overhead of .NET, as well as provide features that I never thought to add to ASMED because it was .NET only.
 
 ## Installing
 
 QVSED [is available on PyPI](https://pypi.org/project/QVSED/). You can install it using the following command:
 
 ```bash
 pip install --upgrade qvsed
 ```
 
-To run QVSED, use the `qvsed` command. If you find it convenient to have a clickable icon to launch QVSED with, scroll down to find out how to make a shortcut/alias/symlink/whatever.
+To run QVSED, use the `qvsed` command. Feel free to make a shortcut/alias/symlink to it if you find that convenient.
 
 ## License
 
 QVSED is free software, licensed under the GNU General Public License version 3 or later.
 
 ## Usage
 
 QVSED is broken up into three parts - the Action Deck, the Text Area and the Echo Area.
 
-The Action Deck contains editing commands, the Text Area is a text area, and the Echo Area is where messages will be printed.
+The Action Deck contains editing commands, the Text Area is where the text content goes, and the Echo Area is where messages will be printed.
 
 ## Keyboard Shortcuts
 
 QVSED contains a mix of bindings from the original ASMED, Vim-style bindings and Emacs-style bindings.
 
 ### Key Prefixes
 
@@ -56,14 +60,20 @@
 + **Clear Text** - `<C-n>` - Clear the Text Area. Think of it like New File.
 + **Open File** - `<C-f>` - Launch a file picker and load the chosen file's contents into the Text Area.
 + **Save File** - `<C-s>` - Launch a file picker and save the contents of the Text Area to the chosen file name.
 + **Full Screen** - `<A-f>` - Toggle full screen mode.
 + **Get Help** - `<C-h>` - Show a help message in the Text Area. This will overwrite your current work.
 + **Quit QVSED**  - `<A-q>` - Quit QVSED on the spot with no confirmation dialog.
 
+### File Picker bindings
+
++ **Open/Save** - `<RET>` - Load from/save to the specified file path.
++ **Cancel** - `<ESC>` - Cancel and go back to QVSED.
++ **System File Picker**  - `<C-d>` - Launch your OS file picker.
+
 ### Motion bindings
 
 These bindings are for the most part inspired by Vim, if not Emacs.
 
 + `<A-h>` - Move left a character. Inspired by Vim's `h`.
 + `<A-j>` - Move down a character. Inspired by Vim's `j`.
 + `<A-k>` - Move up a character. Inspired by Vim's `k`.
@@ -131,19 +141,7 @@
 scroll_bar_color = "#363D49"
 scroll_bar_background_color = "#282F3B"
 scroll_bar_hover_color = "#4F5664"
 scroll_bar_pressed_color = "#262B34"
 ```
 
 Keep in mind that `font_family` *must* be a list. If you want only one font, specify `font_family = ["My Font"]`.
-
-## Making Shortcuts
-
-### Windows
-
-1. Locate the QVSED executable file, usually located at `C:\Users\<username>\AppData\Local\Programs\Python\Python3xx\Scripts\qvsed.exe`. Substitute `<username>` with your Windows username and `xx` with whatever Python version you use, for example `Python311`.
-2. Right-click on the executable file and select "Create Shortcut."
-3. Move the shortcut to your desired location, such as the desktop or the Start Menu folder.
-4. Double-click on the shortcut to launch QVSED directly.
-5. If you want, supply your own icon, because QVSED doesn't have its own icon yet.
-
-There aren't instructions for macOS or Linux because I didn't have access to either system at the time to check, but I'll update it in the future sometime maybe.
```

### Comparing `qvsed-1.5.0/qvsed/config_default.py` & `qvsed-1.5.1/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.0/qvsed/qvsed.py` & `qvsed-1.5.1/qvsed/qvsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                           echo_area_color, scroll_bar_color, scroll_bar_background_color,
                           scroll_bar_hover_color, scroll_bar_pressed_color):
         """
         Generate and apply a style sheet based on the config.py file.
         """
 
         stylesheet = f"""
-QMainWindow {{
+QMainWindow, QDialog {{
     color: {text_color};
     background: {background_color};
 }}
 
 QPlainTextEdit, QLineEdit {{
     padding: 8px;
     border: none;
```

### Comparing `qvsed-1.5.0/qvsed/qvsed.ui` & `qvsed-1.5.1/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.0/qvsed/qvsed_dialog.ui` & `qvsed-1.5.1/qvsed/qvsed_dialog.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.0/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.1/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.0
+Version: 1.5.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.0/setup.py` & `qvsed-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.0',
+    version='1.5.1',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

