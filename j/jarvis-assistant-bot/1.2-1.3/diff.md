# Comparing `tmp/jarvis_assistant_bot-1.2.tar.gz` & `tmp/jarvis_assistant_bot-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis_assistant_bot-1.2.tar", last modified: Wed Jul 12 22:02:42 2023, max compression
+gzip compressed data, was "jarvis_assistant_bot-1.3.tar", last modified: Wed Jul 12 22:21:16 2023, max compression
```

## Comparing `jarvis_assistant_bot-1.2.tar` & `jarvis_assistant_bot-1.3.tar`

### file list

```diff
@@ -1,26 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 22:02:42.907852 jarvis_assistant_bot-1.2/
--rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.2/LICENSE
--rw-rw-rw-   0        0        0      784 2023-07-12 20:57:02.000000 jarvis_assistant_bot-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6070 2023-07-12 22:02:42.906852 jarvis_assistant_bot-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 22:02:42.857412 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/
--rw-rw-rw-   0        0        0     6070 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       72 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1081 2023-07-12 22:01:36.000000 jarvis_assistant_bot-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 22:02:42.907852 jarvis_assistant_bot-1.2/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-07-12 22:01:31.000000 jarvis_assistant_bot-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:02:42.905676 jarvis_assistant_bot-1.2/src/
--rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.2/src/__init__.py
--rw-rw-rw-   0        0        0    13189 2023-07-12 21:52:58.000000 jarvis_assistant_bot-1.2/src/commands.py
--rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.2/src/common_functions.py
--rw-rw-rw-   0        0        0    10686 2023-07-12 22:02:01.000000 jarvis_assistant_bot-1.2/src/goose_game.py
--rw-rw-rw-   0        0        0     5736 2023-07-12 21:53:28.000000 jarvis_assistant_bot-1.2/src/main.py
--rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.2/src/memory.py
--rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.2/src/notes_core.py
--rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.2/src/open_ai_input_assistent.py
--rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.2/src/save_load_books.py
--rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.2/src/sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.600770 jarvis_assistant_bot-1.3/
+-rw-rw-rw-   0        0        0     5347 2023-07-05 18:17:59.000000 jarvis_assistant_bot-1.3/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.3/LICENSE
+-rw-rw-rw-   0        0        0      168 2023-07-12 22:19:00.000000 jarvis_assistant_bot-1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6070 2023-07-12 22:21:16.590771 jarvis_assistant_bot-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.384524 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/
+-rw-rw-rw-   0        0        0     6070 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 22:21:16.000000 jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1081 2023-07-12 22:21:09.000000 jarvis_assistant_bot-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 22:21:16.600770 jarvis_assistant_bot-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-07-12 22:21:04.000000 jarvis_assistant_bot-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.451598 jarvis_assistant_bot-1.3/src/
+-rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.3/src/__init__.py
+-rw-rw-rw-   0        0        0    13189 2023-07-12 21:52:58.000000 jarvis_assistant_bot-1.3/src/commands.py
+-rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.3/src/common_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.520592 jarvis_assistant_bot-1.3/src/game/
+-rw-rw-rw-   0        0        0        0 2023-07-12 20:44:02.000000 jarvis_assistant_bot-1.3/src/game/__init__.py
+-rw-rw-rw-   0        0        0   155171 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/background.png
+-rw-rw-rw-   0        0        0  2206416 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/background2.png
+-rw-rw-rw-   0        0        0     4479 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/bomb.png
+-rw-rw-rw-   0        0        0    22447 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/bonus.png
+-rw-rw-rw-   0        0        0    26237 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/bonus2.png
+-rw-rw-rw-   0        0        0    10085 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/enemy.png
+-rw-rw-rw-   0        0        0    11624 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/enemy2.png
+drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.562776 jarvis_assistant_bot-1.3/src/game/goose/
+-rw-rw-rw-   0        0        0     4428 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-1.png
+-rw-rw-rw-   0        0        0     3780 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-2.png
+-rw-rw-rw-   0        0        0     3925 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-3.png
+-rw-rw-rw-   0        0        0     4570 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-4.png
+-rw-rw-rw-   0        0        0     4808 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose/1-5.png
+-rw-rw-rw-   0        0        0    98430 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/goose_doose.jpg
+-rw-rw-rw-   0        0        0     3780 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.3/src/game/player.png
+-rw-rw-rw-   0        0        0    10686 2023-07-12 22:02:01.000000 jarvis_assistant_bot-1.3/src/goose_game.py
+-rw-rw-rw-   0        0        0     5736 2023-07-12 21:53:28.000000 jarvis_assistant_bot-1.3/src/main.py
+-rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/src/memory.py
+-rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/src/notes_core.py
+-rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/src/open_ai_input_assistent.py
+-rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.3/src/save_load_books.py
+-rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.3/src/sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:21:16.589770 jarvis_assistant_bot-1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      906 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/tests/main_tests.py
+-rw-rw-rw-   0        0        0    14082 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/tests/memory_tests.py
+-rw-rw-rw-   0        0        0     7034 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/tests/notes_core_tests.py
+-rw-rw-rw-   0        0        0     4603 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.3/tests/save_load_tests.py
```

### Comparing `jarvis_assistant_bot-1.2/LICENSE` & `jarvis_assistant_bot-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/PKG-INFO` & `jarvis_assistant_bot-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis_assistant_bot
-Version: 1.2
+Version: 1.3
 Summary: Jarvis is a personal assistant application that allows you to manage your address book with contacts. The application provides features to add, remove, change, save, and load contacts, making it easier to organize your personal or professional network. In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
 Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
 Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
 Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jarvis_assistant_bot-1.2/README.md` & `jarvis_assistant_bot-1.3/README.md`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/PKG-INFO` & `jarvis_assistant_bot-1.3/jarvis_assistant_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-assistant-bot
-Version: 1.2
+Version: 1.3
 Summary: Jarvis is a personal assistant application that allows you to manage your address book with contacts. The application provides features to add, remove, change, save, and load contacts, making it easier to organize your personal or professional network. In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
 Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
 Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
 Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jarvis_assistant_bot-1.2/pyproject.toml` & `jarvis_assistant_bot-1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jarvis_assistant_bot"
-version = "1.2"
+version = "1.3"
 authors = [
   { name="Dmytro Filin"},
   { name="Illya Grygoriev"},
   { name="Dmytro Klymenko"},
   { name="Dmytro Paukov"},
   { name="Alexandr "}
 ]
```

### Comparing `jarvis_assistant_bot-1.2/setup.py` & `jarvis_assistant_bot-1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name='jarvis_assistant_bot',
-    version='1.2',
+    version='1.3',
     description='Welcome to Jarvis, your personal assistant! Jarvis is here to help you stay organized and manage your contacts, reminders, notes, and files efficiently.',
     author='Python Forces',
     url='https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654',
-    packages=['src'],
+    packages=find_packages(),
+    include_package_data=True,
     
     entry_points={
         'console_scripts': [
             'Jarvis=src.main:main',
         ],
     },
     install_requires=[
```

### Comparing `jarvis_assistant_bot-1.2/src/commands.py` & `jarvis_assistant_bot-1.3/src/commands.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/src/common_functions.py` & `jarvis_assistant_bot-1.3/src/common_functions.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/src/goose_game.py` & `jarvis_assistant_bot-1.3/src/goose_game.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/src/main.py` & `jarvis_assistant_bot-1.3/src/main.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/src/memory.py` & `jarvis_assistant_bot-1.3/src/memory.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/src/notes_core.py` & `jarvis_assistant_bot-1.3/src/notes_core.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/src/open_ai_input_assistent.py` & `jarvis_assistant_bot-1.3/src/open_ai_input_assistent.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/src/save_load_books.py` & `jarvis_assistant_bot-1.3/src/save_load_books.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.2/src/sorter.py` & `jarvis_assistant_bot-1.3/src/sorter.py`

 * *Files identical despite different names*

