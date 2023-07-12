# Comparing `tmp/jarvis_assistant_bot-1.1.tar.gz` & `tmp/jarvis_assistant_bot-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis_assistant_bot-1.1.tar", last modified: Wed Jul 12 21:02:55 2023, max compression
+gzip compressed data, was "jarvis_assistant_bot-1.2.tar", last modified: Wed Jul 12 22:02:42 2023, max compression
```

## Comparing `jarvis_assistant_bot-1.1.tar` & `jarvis_assistant_bot-1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 21:02:55.255920 jarvis_assistant_bot-1.1/
--rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.1/LICENSE
--rw-rw-rw-   0        0        0      784 2023-07-12 20:57:02.000000 jarvis_assistant_bot-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6070 2023-07-12 21:02:55.251913 jarvis_assistant_bot-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 21:02:55.216309 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/
--rw-rw-rw-   0        0        0     6070 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       72 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-07-12 21:00:06.000000 jarvis_assistant_bot-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 21:02:55.255920 jarvis_assistant_bot-1.1/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-07-12 21:02:45.000000 jarvis_assistant_bot-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 21:02:55.250820 jarvis_assistant_bot-1.1/src/
--rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.1/src/__init__.py
--rw-rw-rw-   0        0        0    13213 2023-07-12 20:56:24.000000 jarvis_assistant_bot-1.1/src/commands.py
--rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.1/src/common_functions.py
--rw-rw-rw-   0        0        0    10652 2023-07-12 20:51:04.000000 jarvis_assistant_bot-1.1/src/goose_game.py
--rw-rw-rw-   0        0        0     5590 2023-07-12 12:45:11.000000 jarvis_assistant_bot-1.1/src/main.py
--rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.1/src/memory.py
--rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.1/src/notes_core.py
--rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.1/src/open_ai_input_assistent.py
--rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.1/src/save_load_books.py
--rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.1/src/sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:02:42.907852 jarvis_assistant_bot-1.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.2/LICENSE
+-rw-rw-rw-   0        0        0      784 2023-07-12 20:57:02.000000 jarvis_assistant_bot-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6070 2023-07-12 22:02:42.906852 jarvis_assistant_bot-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 22:02:42.857412 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/
+-rw-rw-rw-   0        0        0     6070 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-12 22:02:42.000000 jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1081 2023-07-12 22:01:36.000000 jarvis_assistant_bot-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 22:02:42.907852 jarvis_assistant_bot-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-07-12 22:01:31.000000 jarvis_assistant_bot-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:02:42.905676 jarvis_assistant_bot-1.2/src/
+-rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.2/src/__init__.py
+-rw-rw-rw-   0        0        0    13189 2023-07-12 21:52:58.000000 jarvis_assistant_bot-1.2/src/commands.py
+-rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.2/src/common_functions.py
+-rw-rw-rw-   0        0        0    10686 2023-07-12 22:02:01.000000 jarvis_assistant_bot-1.2/src/goose_game.py
+-rw-rw-rw-   0        0        0     5736 2023-07-12 21:53:28.000000 jarvis_assistant_bot-1.2/src/main.py
+-rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.2/src/memory.py
+-rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.2/src/notes_core.py
+-rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.2/src/open_ai_input_assistent.py
+-rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.2/src/save_load_books.py
+-rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.2/src/sorter.py
```

### Comparing `jarvis_assistant_bot-1.1/LICENSE` & `jarvis_assistant_bot-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.1/MANIFEST.in` & `jarvis_assistant_bot-1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.1/PKG-INFO` & `jarvis_assistant_bot-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis_assistant_bot
-Version: 1.1
+Version: 1.2
 Summary: Jarvis is a personal assistant application that allows you to manage your address book with contacts. The application provides features to add, remove, change, save, and load contacts, making it easier to organize your personal or professional network. In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
 Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
 Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
 Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jarvis_assistant_bot-1.1/README.md` & `jarvis_assistant_bot-1.2/README.md`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/PKG-INFO` & `jarvis_assistant_bot-1.2/jarvis_assistant_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-assistant-bot
-Version: 1.1
+Version: 1.2
 Summary: Jarvis is a personal assistant application that allows you to manage your address book with contacts. The application provides features to add, remove, change, save, and load contacts, making it easier to organize your personal or professional network. In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
 Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
 Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
 Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jarvis_assistant_bot-1.1/pyproject.toml` & `jarvis_assistant_bot-1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jarvis_assistant_bot"
-version = "1.001"
+version = "1.2"
 authors = [
   { name="Dmytro Filin"},
   { name="Illya Grygoriev"},
   { name="Dmytro Klymenko"},
   { name="Dmytro Paukov"},
   { name="Alexandr "}
 ]
```

### Comparing `jarvis_assistant_bot-1.1/setup.py` & `jarvis_assistant_bot-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='jarvis_assistant_bot',
-    version='1.01',
+    version='1.2',
     description='Welcome to Jarvis, your personal assistant! Jarvis is here to help you stay organized and manage your contacts, reminders, notes, and files efficiently.',
     author='Python Forces',
     url='https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654',
     packages=['src'],
     
     entry_points={
         'console_scripts': [
```

### Comparing `jarvis_assistant_bot-1.1/src/commands.py` & `jarvis_assistant_bot-1.2/src/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from prompt_toolkit.completion import WordCompleter
 from colorama import Fore,Style
 from prettytable import PrettyTable
 from src.common_functions import STR_EPIC_COMMANDS
 from src.memory import Record,SetterValueIncorrect,AddressBook,Phone
 from src.notes_core import *
 from src.sorter import sort_files_in_this_path
-from src.goose_game import *
-import keyboard
 
 CHECK_SECOND_ARG_CHANGE_CONTACT = ("phone","email","birthday","address")
 CHECK_SECOND_ARG_CHANGE_NOTE = ("title","tag","description")
 
 def get_command_input_agree(Input_message=''):
     Input_value = None
     while True:
@@ -219,15 +217,15 @@
     return "Notes sorted by tags."
 
 def show_all_notes(*arg, a_book=AddressBook,n_book=Notebook):
     table = n_book.show_notes()
     return table
 
 def start_game(*arg,a_book = AddressBook,n_book = Notebook):
-    play()
+    return "Starting the game..."
 
 def ending(*arg,a_book = AddressBook,n_book = Notebook):
     return 'Goodbye!'
 
 input_variants = ['hello','hi','start','add contact','new contact','create contact','change contact','change phone','change contact details',"sort","sort files","need sort",
                   'get contact', 'show contact','show person','show contacts','show address book','show all book','goodbye','close','end','search user','find contact','find user', "help","commands",
                   "need help",'remove note','delete note','get note out','add note', 'new note','create note','find notes', 'search notes','remove contact','delete contact','take out contact'
```

### Comparing `jarvis_assistant_bot-1.1/src/common_functions.py` & `jarvis_assistant_bot-1.2/src/common_functions.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.1/src/goose_game.py` & `jarvis_assistant_bot-1.2/src/goose_game.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from os import listdir
 import pygame
 from pygame.constants import QUIT, K_DOWN, K_UP, K_LEFT, K_RIGHT, K_SPACE, K_s, K_w, K_a, K_d, K_ESCAPE
 import random
-import time
-# from src.main import *
 
 def play():
 
     pygame.init()
 
     WHITE = 255, 255, 255
     BLACK = 0, 0, 0
@@ -91,42 +89,45 @@
     start_screen = True
     is_working = False
     can_create_bomb = True
     game_over = False
 
     def show_game_over_screen():
         game_over = True
-        while game_over:
-            
+        while game_over:           
             for event in pygame.event.get():
                 if event.type == pygame.QUIT:
-                    pygame.quit()
+                    game_over = False
 
                 elif event.type == pygame.KEYDOWN:
                     if event.key == pygame.K_ESCAPE:
-                        pygame.quit()
+                        game_over = False
+
+            # keyboard.wait('esc')
 
-                        
             custom_image = pygame.image.load('src/game/goose_doose.jpg').convert_alpha()
             custom_image_rect = custom_image.get_rect(center=(width // 2, height // 2))
             main_surface.blit(custom_image, custom_image_rect)
-            
+                    
             game_over_text = font.render("Гра закінчена!", True, WHITE)
             game_over_rect = game_over_text.get_rect(center=(width // 2 + 150, height // 2 - 100))
             main_surface.blit(game_over_text, game_over_rect)
-            
+                    
             extra_text = font.render("Гусак пішов на лікарняний", True, WHITE)
             extra_rect = extra_text.get_rect(center=(width // 2 + 150, height // 2 - 50))
             main_surface.blit(extra_text, extra_rect)
 
             score_text = font.render("Ваш рахунок: " + str(scores), True, WHITE)
             score_rect = score_text.get_rect(center=(width // 2 + 150, height // 2 ))
             main_surface.blit(score_text, score_rect)
-            
+                    
             pygame.display.flip()
+        print('The End. Thank for attention.')
+        pygame.quit()
+
         
     while start_screen:
         
         # Код для відображення початкового екрану
         main_surface.blit(bg, (0, 0))
         
         # Власна картинка та напис
@@ -157,15 +158,14 @@
                     show_game_over_screen()
                     is_working == False
                 
             if event.type == CREATE_ENEMY:
                 enemies.append(create_enemy())
                 if len(enemies) <= 2:
                     enemies.append(create_enemy())
-                    print(len(enemies))
                 if scores !=0 and scores % 10 == 0:
                     enemies.append(create_enemy())
                     enemies.append(create_enemy())
                 
             if event.type == CREATE_BONUS:
                 bonuses.append(create_bonus())
```

### Comparing `jarvis_assistant_bot-1.1/src/main.py` & `jarvis_assistant_bot-1.2/src/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from src.commands import find_closest_command, get_command_input,get_command_input_agree
 from src.save_load_books import *
 from src.open_ai_input_assistent import *
 from src.memory import *
 from src.notes_core import Notebook,Tag
 from src.common_functions import STR_EPIC_ASSISTANT
 from colorama import init
+from src.goose_game import *
 import keyboard
 import os
 
 Use_Open_Ai = False
 work_books = None
 
 def use_open_ai():
@@ -135,14 +136,18 @@
             result = command_exe(command, a_book, n_book)
             if isinstance(result, list):
                 # Print each item in the result listc
                 for i in result:
                     print(i)
             else:
                 print(result) if result else None
+                if result == "Starting the game...":
+                    play()
+                    end_work()
+
             # End of app
             if command["name"] == 'ending':
                 break
         elif Use_Open_Ai:
             print(Fore.MAGENTA + input_answer_from_ai(input_string) + Style.RESET_ALL)
         else:
             print("Sorry, i don't understand this your command. Please try again.")
```

### Comparing `jarvis_assistant_bot-1.1/src/memory.py` & `jarvis_assistant_bot-1.2/src/memory.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.1/src/notes_core.py` & `jarvis_assistant_bot-1.2/src/notes_core.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.1/src/open_ai_input_assistent.py` & `jarvis_assistant_bot-1.2/src/open_ai_input_assistent.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.1/src/save_load_books.py` & `jarvis_assistant_bot-1.2/src/save_load_books.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.1/src/sorter.py` & `jarvis_assistant_bot-1.2/src/sorter.py`

 * *Files identical despite different names*

