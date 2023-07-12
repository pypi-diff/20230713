# Comparing `tmp/jarvis_assistant_bot-1.3.tar.gz` & `tmp/jarvis_assistant_bot-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis_assistant_bot-1.3.tar", last modified: Wed Jul 12 22:21:16 2023, max compression
+gzip compressed data, was "jarvis_assistant_bot-1.4.tar", last modified: Wed Jul 12 23:06:21 2023, max compression
```

## Comparing `jarvis_assistant_bot-1.3.tar` & `jarvis_assistant_bot-1.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.600770 jarvis_assistant_bot-1.3/
--rw-rw-rw-   0        0        0     5347 2023-07-05 18:17:59.000000 jarvis_assistant_bot-1.3/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.3/LICENSE
--rw-rw-rw-   0        0        0      168 2023-07-12 22:19:00.000000 jarvis_assistant_bot-1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6070 2023-07-12 22:21:16.590771 jarvis_assistant_bot-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.384524 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/
--rw-rw-rw-   0        0        0     6070 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       72 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1081 2023-07-12 22:21:09.000000 jarvis_assistant_bot-1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 22:21:16.600770 jarvis_assistant_bot-1.3/setup.cfg
--rw-rw-rw-   0        0        0      794 2023-07-12 22:21:04.000000 jarvis_assistant_bot-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.451598 jarvis_assistant_bot-1.3/src/
--rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.3/src/__init__.py
--rw-rw-rw-   0        0        0    13189 2023-07-12 21:52:58.000000 jarvis_assistant_bot-1.3/src/commands.py
--rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.3/src/common_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.520592 jarvis_assistant_bot-1.3/src/game/
--rw-rw-rw-   0        0        0        0 2023-07-12 20:44:02.000000 jarvis_assistant_bot-1.3/src/game/__init__.py
--rw-rw-rw-   0        0        0   155171 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/background.png
--rw-rw-rw-   0        0        0  2206416 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/background2.png
--rw-rw-rw-   0        0        0     4479 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/bomb.png
--rw-rw-rw-   0        0        0    22447 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/bonus.png
--rw-rw-rw-   0        0        0    26237 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/bonus2.png
--rw-rw-rw-   0        0        0    10085 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/enemy.png
--rw-rw-rw-   0        0        0    11624 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/enemy2.png
-drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.562776 jarvis_assistant_bot-1.3/src/game/goose/
--rw-rw-rw-   0        0        0     4428 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-1.png
--rw-rw-rw-   0        0        0     3780 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-2.png
--rw-rw-rw-   0        0        0     3925 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-3.png
--rw-rw-rw-   0        0        0     4570 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-4.png
--rw-rw-rw-   0        0        0     4808 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-5.png
--rw-rw-rw-   0        0        0    98430 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose_doose.jpg
--rw-rw-rw-   0        0        0     3780 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/player.png
--rw-rw-rw-   0        0        0    10686 2023-07-12 22:02:01.000000 jarvis_assistant_bot-1.3/src/goose_game.py
--rw-rw-rw-   0        0        0     5736 2023-07-12 21:53:28.000000 jarvis_assistant_bot-1.3/src/main.py
--rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/src/memory.py
--rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/src/notes_core.py
--rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/src/open_ai_input_assistent.py
--rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.3/src/save_load_books.py
--rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.3/src/sorter.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.589770 jarvis_assistant_bot-1.3/tests/
--rw-rw-rw-   0        0        0        0 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.3/tests/__init__.py
--rw-rw-rw-   0        0        0      906 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/tests/main_tests.py
--rw-rw-rw-   0        0        0    14082 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/tests/memory_tests.py
--rw-rw-rw-   0        0        0     7034 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/tests/notes_core_tests.py
--rw-rw-rw-   0        0        0     4603 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/tests/save_load_tests.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:06:21.888665 jarvis_assistant_bot-1.4/
+-rw-rw-rw-   0        0        0     5347 2023-07-05 18:17:59.000000 jarvis_assistant_bot-1.4/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.4/LICENSE
+-rw-rw-rw-   0        0        0      168 2023-07-12 22:19:00.000000 jarvis_assistant_bot-1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6070 2023-07-12 23:06:21.888665 jarvis_assistant_bot-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 23:06:21.676649 jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/
+-rw-rw-rw-   0        0        0     6070 2023-07-12 23:06:21.000000 jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-07-12 23:06:21.000000 jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 23:06:21.000000 jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-12 23:06:21.000000 jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-07-12 23:06:21.000000 jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 23:06:21.000000 jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1081 2023-07-12 23:06:13.000000 jarvis_assistant_bot-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 23:06:21.888665 jarvis_assistant_bot-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-07-12 23:06:10.000000 jarvis_assistant_bot-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:06:21.744157 jarvis_assistant_bot-1.4/src/
+-rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.4/src/__init__.py
+-rw-rw-rw-   0        0        0    13189 2023-07-12 21:52:58.000000 jarvis_assistant_bot-1.4/src/commands.py
+-rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.4/src/common_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:06:21.812156 jarvis_assistant_bot-1.4/src/game/
+-rw-rw-rw-   0        0        0        0 2023-07-12 20:44:02.000000 jarvis_assistant_bot-1.4/src/game/__init__.py
+-rw-rw-rw-   0        0        0   155171 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/background.png
+-rw-rw-rw-   0        0        0  2206416 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/background2.png
+-rw-rw-rw-   0        0        0     4479 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/bomb.png
+-rw-rw-rw-   0        0        0    22447 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/bonus.png
+-rw-rw-rw-   0        0        0    26237 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/bonus2.png
+-rw-rw-rw-   0        0        0    10085 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/enemy.png
+-rw-rw-rw-   0        0        0    11624 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/enemy2.png
+drwxrwxrwx   0        0        0        0 2023-07-12 23:06:21.842666 jarvis_assistant_bot-1.4/src/game/goose/
+-rw-rw-rw-   0        0        0     4428 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/goose/1-1.png
+-rw-rw-rw-   0        0        0     3780 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/goose/1-2.png
+-rw-rw-rw-   0        0        0     3925 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/goose/1-3.png
+-rw-rw-rw-   0        0        0     4570 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/goose/1-4.png
+-rw-rw-rw-   0        0        0     4808 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/goose/1-5.png
+-rw-rw-rw-   0        0        0    98430 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/goose_doose.jpg
+-rw-rw-rw-   0        0        0     3780 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.4/src/game/player.png
+-rw-rw-rw-   0        0        0    10885 2023-07-12 23:05:02.000000 jarvis_assistant_bot-1.4/src/goose_game.py
+-rw-rw-rw-   0        0        0     5736 2023-07-12 21:53:28.000000 jarvis_assistant_bot-1.4/src/main.py
+-rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.4/src/memory.py
+-rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.4/src/notes_core.py
+-rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.4/src/open_ai_input_assistent.py
+-rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.4/src/save_load_books.py
+-rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.4/src/sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:06:21.886665 jarvis_assistant_bot-1.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      906 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.4/tests/main_tests.py
+-rw-rw-rw-   0        0        0    14082 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.4/tests/memory_tests.py
+-rw-rw-rw-   0        0        0     7034 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.4/tests/notes_core_tests.py
+-rw-rw-rw-   0        0        0     4603 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.4/tests/save_load_tests.py
```

### Comparing `jarvis_assistant_bot-1.3/CODE_OF_CONDUCT.md` & `jarvis_assistant_bot-1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/LICENSE` & `jarvis_assistant_bot-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/PKG-INFO` & `jarvis_assistant_bot-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis_assistant_bot
-Version: 1.3
+Version: 1.4
 Summary: Jarvis is a personal assistant application that allows you to manage your address book with contacts. The application provides features to add, remove, change, save, and load contacts, making it easier to organize your personal or professional network. In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
 Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
 Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
 Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jarvis_assistant_bot-1.3/README.md` & `jarvis_assistant_bot-1.4/README.md`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/PKG-INFO` & `jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-assistant-bot
-Version: 1.3
+Version: 1.4
 Summary: Jarvis is a personal assistant application that allows you to manage your address book with contacts. The application provides features to add, remove, change, save, and load contacts, making it easier to organize your personal or professional network. In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
 Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
 Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
 Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/SOURCES.txt` & `jarvis_assistant_bot-1.4/jarvis_assistant_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/pyproject.toml` & `jarvis_assistant_bot-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jarvis_assistant_bot"
-version = "1.3"
+version = "1.4"
 authors = [
   { name="Dmytro Filin"},
   { name="Illya Grygoriev"},
   { name="Dmytro Klymenko"},
   { name="Dmytro Paukov"},
   { name="Alexandr "}
 ]
```

### Comparing `jarvis_assistant_bot-1.3/setup.py` & `jarvis_assistant_bot-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jarvis_assistant_bot',
-    version='1.3',
+    version='1.4',
     description='Welcome to Jarvis, your personal assistant! Jarvis is here to help you stay organized and manage your contacts, reminders, notes, and files efficiently.',
     author='Python Forces',
     url='https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654',
     packages=find_packages(),
     include_package_data=True,
     
     entry_points={
```

### Comparing `jarvis_assistant_bot-1.3/src/commands.py` & `jarvis_assistant_bot-1.4/src/commands.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/common_functions.py` & `jarvis_assistant_bot-1.4/src/common_functions.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/background.png` & `jarvis_assistant_bot-1.4/src/game/background.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/background2.png` & `jarvis_assistant_bot-1.4/src/game/background2.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/bomb.png` & `jarvis_assistant_bot-1.4/src/game/bomb.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/bonus.png` & `jarvis_assistant_bot-1.4/src/game/bonus.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/bonus2.png` & `jarvis_assistant_bot-1.4/src/game/bonus2.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/enemy.png` & `jarvis_assistant_bot-1.4/src/game/enemy.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/enemy2.png` & `jarvis_assistant_bot-1.4/src/game/enemy2.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/goose/1-1.png` & `jarvis_assistant_bot-1.4/src/game/goose/1-1.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/goose/1-2.png` & `jarvis_assistant_bot-1.4/src/game/goose/1-2.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/goose/1-3.png` & `jarvis_assistant_bot-1.4/src/game/goose/1-3.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/goose/1-4.png` & `jarvis_assistant_bot-1.4/src/game/goose/1-4.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/goose/1-5.png` & `jarvis_assistant_bot-1.4/src/game/goose/1-5.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/goose_doose.jpg` & `jarvis_assistant_bot-1.4/src/game/goose_doose.jpg`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/game/player.png` & `jarvis_assistant_bot-1.4/src/game/player.png`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/goose_game.py` & `jarvis_assistant_bot-1.4/src/goose_game.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from os import listdir
+import pkg_resources
 import pygame
 from pygame.constants import QUIT, K_DOWN, K_UP, K_LEFT, K_RIGHT, K_SPACE, K_s, K_w, K_a, K_d, K_ESCAPE
 import random
+import os
 
 def play():
 
     pygame.init()
 
     WHITE = 255, 255, 255
     BLACK = 0, 0, 0
@@ -19,53 +21,54 @@
 
     FPS = pygame.time.Clock()
 
     screen = width, height = 1280, 720
 
     main_surface = pygame.display.set_mode(screen)
 
-    IMGS_PATH = 'src/game/goose'
+    IMGS_PATH_GOOSE =  pkg_resources.resource_filename('src', 'game/goose/')
+    IMGS_PATH_GAME = pkg_resources.resource_filename('src', 'game/')
 
     # player = pygame.Surface((20, 20))
     # player.fill((WHITE))
-    player_imgs = [pygame.image.load(IMGS_PATH + '/' + file).convert_alpha() for file in listdir(IMGS_PATH)]
+    player_imgs = [pygame.image.load(IMGS_PATH_GOOSE + file).convert_alpha() for file in listdir(IMGS_PATH_GOOSE)]
     player = player_imgs[0]
     player_rect = player.get_rect()
     player_speed = 10
 
     def create_enemy():
         # enemy = pygame.Surface((20, 20))
         # enemy.fill((RED))
-        enemy = pygame.image.load('src/game/enemy2.png').convert_alpha()
+        enemy = pygame.image.load(IMGS_PATH_GAME + 'enemy2.png').convert_alpha()
         enemy_rect = pygame.Rect(width + enemy.get_width(), random.randint(0, height - enemy.get_height()), *enemy.get_size())
         enemy_speed = random.randint(6,10)
         return [enemy, enemy_rect, enemy_speed]
 
     def create_bonus():
         # bonus = pygame.Surface((20, 20))
         # bonus.fill((GREEN))
-        bonus = pygame.image.load('src/game/bonus2.png').convert_alpha()
+        bonus = pygame.image.load(IMGS_PATH_GAME + 'bonus2.png').convert_alpha()
         bonus_rect = pygame.Rect(random.randint(0, width - bonus.get_width()), -bonus.get_height(), *bonus.get_size())
         bonus_speed = random.randint(4,7)
         return [bonus, bonus_rect, bonus_speed]
 
     def create_bomb():
-        bomb = pygame.image.load('src/game/bomb.png').convert_alpha()
+        bomb = pygame.image.load(IMGS_PATH_GAME+'bomb.png').convert_alpha()
         bomb_rect = player_rect
         bomb_speed = random.randint(5,8)
         return [bomb, bomb_rect, bomb_speed]
 
     def handle_events():
         for event in pygame.event.get():
             if event.type == pygame.KEYDOWN:
                 if event.key == pygame.K_SPACE and bombs != 0:
                     bombss.append(create_bomb())
                     bombs -= 1
 
-    bg = pygame.transform.scale(pygame.image.load('src/game/background2.png').convert(), screen)
+    bg = pygame.transform.scale(pygame.image.load(IMGS_PATH_GAME + 'background2.png').convert(), screen)
     bgX = 0
     bgX2 = bg.get_width()
     bg_speed = 5
 
     CREATE_ENEMY = pygame.USEREVENT + 1 
     pygame.time.set_timer(CREATE_ENEMY, 1000)
 
@@ -100,15 +103,15 @@
 
                 elif event.type == pygame.KEYDOWN:
                     if event.key == pygame.K_ESCAPE:
                         game_over = False
 
             # keyboard.wait('esc')
 
-            custom_image = pygame.image.load('src/game/goose_doose.jpg').convert_alpha()
+            custom_image = pygame.image.load(IMGS_PATH_GAME + 'goose_doose.jpg').convert_alpha()
             custom_image_rect = custom_image.get_rect(center=(width // 2, height // 2))
             main_surface.blit(custom_image, custom_image_rect)
                     
             game_over_text = font.render("Гра закінчена!", True, WHITE)
             game_over_rect = game_over_text.get_rect(center=(width // 2 + 150, height // 2 - 100))
             main_surface.blit(game_over_text, game_over_rect)
                     
@@ -127,15 +130,15 @@
         
     while start_screen:
         
         # Код для відображення початкового екрану
         main_surface.blit(bg, (0, 0))
         
         # Власна картинка та напис
-        custom_image = pygame.image.load('src/game/background.png').convert_alpha()
+        custom_image = pygame.image.load(IMGS_PATH_GAME + 'background.png').convert_alpha()
         custom_image_rect = custom_image.get_rect(center=(width // 2, height // 2))
         main_surface.blit(custom_image, custom_image_rect)
 
         text = font.render("Натисніть будь-яку клавішу, щоб грати", True, BLACK)
         text_rect = text.get_rect(center=(width // 2, height // 2 + 100))
         main_surface.blit(text, text_rect)
```

### Comparing `jarvis_assistant_bot-1.3/src/main.py` & `jarvis_assistant_bot-1.4/src/main.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/memory.py` & `jarvis_assistant_bot-1.4/src/memory.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/notes_core.py` & `jarvis_assistant_bot-1.4/src/notes_core.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/open_ai_input_assistent.py` & `jarvis_assistant_bot-1.4/src/open_ai_input_assistent.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/save_load_books.py` & `jarvis_assistant_bot-1.4/src/save_load_books.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/src/sorter.py` & `jarvis_assistant_bot-1.4/src/sorter.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/tests/main_tests.py` & `jarvis_assistant_bot-1.4/tests/main_tests.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/tests/memory_tests.py` & `jarvis_assistant_bot-1.4/tests/memory_tests.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/tests/notes_core_tests.py` & `jarvis_assistant_bot-1.4/tests/notes_core_tests.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.3/tests/save_load_tests.py` & `jarvis_assistant_bot-1.4/tests/save_load_tests.py`

 * *Files identical despite different names*

