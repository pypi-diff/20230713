# Comparing `tmp/qvsed-1.5.5.tar.gz` & `tmp/qvsed-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.5.tar", last modified: Thu Jul 13 15:27:04 2023, max compression
+gzip compressed data, was "qvsed-1.5.6.tar", last modified: Thu Jul 13 16:10:37 2023, max compression
```

## Comparing `qvsed-1.5.5.tar` & `qvsed-1.5.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 15:27:04.502818 qvsed-1.5.5/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.5/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-13 15:27:04.501825 qvsed-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     6653 2023-07-13 12:44:21.000000 qvsed-1.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 15:27:04.474974 qvsed-1.5.5/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.5/qvsed/__init__.py
--rw-rw-rw-   0        0        0      729 2023-07-13 13:56:47.000000 qvsed-1.5.5/qvsed/config_default.py
--rw-rw-rw-   0        0        0    26381 2023-07-13 15:26:19.000000 qvsed-1.5.5/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.5/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     4175 2023-07-13 15:16:38.000000 qvsed-1.5.5/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-13 15:27:04.499795 qvsed-1.5.5/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 15:27:04.000000 qvsed-1.5.5/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 15:27:04.502818 qvsed-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-13 15:26:45.000000 qvsed-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:10:37.523616 qvsed-1.5.6/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-13 16:10:37.523616 qvsed-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6818 2023-07-13 15:58:25.000000 qvsed-1.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 16:10:37.499352 qvsed-1.5.6/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.6/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-07-13 15:51:04.000000 qvsed-1.5.6/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    26528 2023-07-13 15:54:00.000000 qvsed-1.5.6/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.6/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     4175 2023-07-13 15:16:38.000000 qvsed-1.5.6/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-13 16:10:37.521089 qvsed-1.5.6/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 16:10:37.523616 qvsed-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-13 16:10:15.000000 qvsed-1.5.6/setup.py
```

### Comparing `qvsed-1.5.5/LICENSE.txt` & `qvsed-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.5/PKG-INFO` & `qvsed-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.5
+Version: 1.5.6
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.5/README.md` & `qvsed-1.5.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 ## Usage
 
 QVSED is broken up into three parts - the Action Deck, the Text Area and the Echo Area.
 
 The Action Deck contains editing commands, the Text Area is where the text content goes, and the Echo Area is where messages will be printed.
 
+There's also the File Picker, for whenever QVSED prompts you to open or save a file. It provides a simple text entry and a button to open your system's file picker.
+
 ## Keyboard Shortcuts
 
 QVSED contains a mix of bindings from the original ASMED, Vim-style bindings and Emacs-style bindings.
 
 ### Key Prefixes
 
 + `C-` - `Ctrl` (Windows, Linux), `⌘` (macOS)
@@ -63,15 +65,15 @@
 + **Full Screen** - `<A-f>` - Toggle full screen mode.
 + **Get Help** - `<C-h>` - Show a help message in the Text Area. This will overwrite your current work.
 + **Quit QVSED**  - `<A-q>` - Quit QVSED on the spot with no confirmation dialog.
 
 ### File Picker bindings
 
 + **Open/Save** - `<RET>` - Load from/save to the specified file path.
-+ **Cancel** - `<ESC>` - Cancel and go back to QVSED.
++ **Cancel** - `<ESC>` or `<A-q>` - Cancel and go back to QVSED.
 + **System File Picker**  - `<C-d>` - Launch your OS file picker.
 
 ### Motion bindings
 
 These bindings are for the most part inspired by Vim, if not Emacs.
 
 + `<A-h>` - Move left a character. Inspired by Vim's `h`.
@@ -106,42 +108,30 @@
 
 The Echo Area is the small bar at the bottom of the QVSED window that prints information.
 
 For example, when a file is opened, it prints its file name. If a config file was not found, it'll generate one and give you the path.
 
 QVSED inherited the name from Emacs. Well, less "inherited" and more "stolen from."
 
-## Configuration
-
-When QVSED is started, it looks for a configuration file. If it can't find one, it creates one and populates it with defaults.
+## File Picker
 
-On Windows, the configuration file will be stored at `C:\Users\<username>\AppData\Roaming\QVSED\config.py`, where `<username>` is your Windows username.
+The File Picker is displayed when you use the **Open File** or **Save File** Action Deck commands.
 
-On *nix systems, the configuration file will be stored at `~/.config/QVSED/config.py`, where `~` is your home directory (`/home/<username>`).
+It consists of the following elements:
 
-As of QVSED 1.3.0, you can customise the colour scheme in addition to the font. For a list of sample colour schemes, [go here](COLOURS.md).
++ A label instructing you to enter the file path, relative or absolute.
++ Another label that shows the current working directory.
++ A text box where you can enter the file path.
++ Three buttons:
+  + **System File Picker** opens your operating system's file picker, so you can select the file you want without having to type in its path, just like in pre-1.5.0 QVSED versions. This can also be accessed with the `<C-d>` key binding.
+  + **Open** or **Save** (depending on the Action Deck command you used) opens or saves the file at the specified path.
+  + **Cancel** closes the dialog without saving any changes.
 
-```python
-# The default QVSED config.
+The File Picker makes it simple to load the file you want, simply by typing in its path.
 
-# Font
-font_family = ["JetBrains Mono", "Cascadia Code", "Consolas", "Menlo", "monospace"]
-font_size = 11
+If this is too oversimplified for you, or you just need to use your system file picker for whatever reason, you can always use the System File Picker option.
 
-# Colours
-text_color = "#FFFFFF"
-background_color = "#282C34"
-
-button_color = "#393F4A"
-button_hover_color = "#31353F"
-button_pressed_color = "#282C34"
-
-text_area_color = "#31353F"
-echo_area_color = "#393F4A"
+## Configuration
 
-scroll_bar_color = "#363D49"
-scroll_bar_background_color = "#282F3B"
-scroll_bar_hover_color = "#4F5664"
-scroll_bar_pressed_color = "#262B34"
-```
+For configuration documentation, see [CONFIG.md](CONFIG.md).
 
-Keep in mind that `font_family` *must* be a list. If you want only one font, specify `font_family = ["My Font"]`.
+For colour scheme configuration, see [COLOURS.md](COLOURS.md) for a list of sample colour schemes.
```

### Comparing `qvsed-1.5.5/qvsed/config_default.py` & `qvsed-1.5.6/qvsed/config_default.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# This config file serves as a template and should not be modified directly; please make any necessary changes in config.py.
+# This is QVSED's config file template and should not be modified directly; please make any necessary changes in config.py.
 # pylint: disable=all
 
 # Font
 font_family = ["JetBrains Mono", "Cascadia Code", "Consolas", "Menlo", "monospace"]
 font_size = 11
 
+# Options
+echo_area_timeout = 3000
+
 # Colours
 text_color = "#FFFFFF"
 background_color = "#282C34"
 
 button_text_color = "#FFFFFF"
 button_color = "#393F4A"
 button_hover_color = "#31353F"
```

### Comparing `qvsed-1.5.5/qvsed/qvsed.py` & `qvsed-1.5.6/qvsed/qvsed.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
         super().__init__()
         self.load_ui_file()
         self.focus_text_area()
         self.install_event_filter()
         self.set_text_area_encoding("UTF-8")
         self.set_up_text_area_handlers()
         self.set_up_action_deck()
-        self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         self.load_config()
+        self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         self.set_up_fonts()
         if self.check_if_file_parameter():
             self.load_from_file(sys.argv[1])
 
     def apply_style_sheet(self, text_color, background_color, button_color, button_text_color,
                             button_hover_color, button_pressed_color, text_area_color,
                             text_area_text_color, echo_area_color, echo_area_text_color,
@@ -244,15 +244,16 @@
     def echo_area_update(self, message):
         """
         Update the Echo Area with the given message.
         """
         echo_area = self.echoArea
         echo_area.setText(message)
         echo_area.setCursorPosition(0)
-        self.echo_area_timeout_clear(3000)
+        if self.echo_area_timeout > 0:
+            self.echo_area_timeout_clear(self.echo_area_timeout)
 
     def focus_text_area(self):
         """
         Set the Text Area to have focus.
         """
         text_area = self.textArea
         text_area.setFocus()
@@ -322,14 +323,16 @@
         spec = importlib.util.spec_from_file_location("qvsed_config", user_config_file)
         qvsed_config = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(qvsed_config)
 
         self.font_family = qvsed_config.font_family
         self.font_size = qvsed_config.font_size
 
+        self.echo_area_timeout = getattr(qvsed_config, 'echo_area_timeout', 3000)
+
         # Load the colour scheme settings from the config file
         # We use the shorter American spellings because it's standard, I guess
         text_color = getattr(qvsed_config, 'text_color', None)
         background_color = getattr(qvsed_config, 'background_color', None)
 
         button_color = getattr(qvsed_config, 'button_color', None)
         button_text_color = getattr(qvsed_config, 'button_text_color', text_color)
```

### Comparing `qvsed-1.5.5/qvsed/qvsed.ui` & `qvsed-1.5.6/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.5/qvsed/qvsed_dialog.ui` & `qvsed-1.5.6/qvsed/qvsed_dialog.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.5/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.6/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.5
+Version: 1.5.6
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.5/setup.py` & `qvsed-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.5',
+    version='1.5.6',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

