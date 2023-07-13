# Comparing `tmp/simalq-0.0.0.tar.gz` & `tmp/simalq-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simalq-0.0.0.tar", last modified: Thu Apr  6 18:51:58 2023, max compression
+gzip compressed data, was "simalq-0.1.0.tar", last modified: Thu Jul 13 17:34:39 2023, max compression
```

## Comparing `simalq-0.0.0.tar` & `simalq-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-04-06 18:51:58.197351 simalq-0.0.0/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5347 2023-04-06 18:51:58.197351 simalq-0.0.0/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4865 2023-04-06 16:47:03.000000 simalq-0.0.0/README.rst
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2023-04-06 18:51:58.197351 simalq-0.0.0/setup.cfg
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      978 2023-04-06 16:59:02.000000 simalq-0.0.0/setup.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-04-06 18:51:58.197351 simalq-0.0.0/simalq/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       10 2023-04-06 16:47:03.000000 simalq-0.0.0/simalq/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1213 2023-04-04 20:06:41.000000 simalq-0.0.0/simalq/game_state.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4821 2023-04-03 20:01:53.000000 simalq-0.0.0/simalq/geometry.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      911 2023-03-30 18:27:45.000000 simalq-0.0.0/simalq/macros.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1659 2023-04-03 19:23:12.000000 simalq-0.0.0/simalq/main.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1570 2023-04-04 18:12:02.000000 simalq-0.0.0/simalq/player_actions.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      539 2023-03-30 17:35:00.000000 simalq-0.0.0/simalq/quest.hy
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-04-06 18:51:58.197351 simalq-0.0.0/simalq/tile/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4894 2023-04-04 18:47:58.000000 simalq-0.0.0/simalq/tile/__init__.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1064 2023-04-04 15:49:17.000000 simalq-0.0.0/simalq/tile/item.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3748 2023-04-04 20:10:22.000000 simalq-0.0.0/simalq/tile/monster.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5524 2023-04-02 18:27:54.000000 simalq-0.0.0/simalq/tile/not_implemented.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4428 2023-04-04 19:54:51.000000 simalq-0.0.0/simalq/tile/scenery.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5818 2023-04-06 18:47:28.000000 simalq-0.0.0/simalq/un_iq.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1293 2023-04-04 18:32:33.000000 simalq-0.0.0/simalq/util.hy
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-04-06 18:51:58.197351 simalq-0.0.0/simalq.egg-info/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5347 2023-04-06 18:51:58.000000 simalq-0.0.0/simalq.egg-info/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      470 2023-04-06 18:51:58.000000 simalq-0.0.0/simalq.egg-info/SOURCES.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2023-04-06 18:51:58.000000 simalq-0.0.0/simalq.egg-info/dependency_links.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      129 2023-04-06 18:51:58.000000 simalq-0.0.0/simalq.egg-info/requires.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       13 2023-04-06 18:51:58.000000 simalq-0.0.0/simalq.egg-info/top_level.txt
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-04-06 18:51:58.197351 simalq-0.0.0/tests/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2023-03-29 13:51:08.000000 simalq-0.0.0/tests/__init__.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-13 17:34:39.958485 simalq-0.1.0/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     6676 2023-07-13 17:34:39.958485 simalq-0.1.0/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     6250 2023-07-13 17:31:08.000000 simalq-0.1.0/README.rst
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2023-07-13 17:34:39.958485 simalq-0.1.0/setup.cfg
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      947 2023-07-13 17:33:39.000000 simalq-0.1.0/setup.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-13 17:34:39.958485 simalq-0.1.0/simalq/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       33 2023-07-13 17:33:55.000000 simalq-0.1.0/simalq/__init__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       76 2023-07-11 20:36:27.000000 simalq-0.1.0/simalq/__main__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2295 2023-07-12 20:19:26.000000 simalq-0.1.0/simalq/cmdline.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1316 2023-06-01 20:01:39.000000 simalq-0.1.0/simalq/color.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    11996 2023-07-11 18:54:38.000000 simalq-0.1.0/simalq/commands.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    10081 2023-07-10 21:08:37.000000 simalq-0.1.0/simalq/display.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     6847 2023-07-03 21:27:25.000000 simalq-0.1.0/simalq/game_state.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     6062 2023-05-29 16:15:53.000000 simalq-0.1.0/simalq/geometry.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1933 2023-04-19 21:08:28.000000 simalq-0.1.0/simalq/macros.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     8279 2023-07-12 20:19:26.000000 simalq-0.1.0/simalq/main.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1811 2023-07-11 20:37:11.000000 simalq-0.1.0/simalq/quest.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-13 17:34:39.958485 simalq-0.1.0/simalq/quest_definition/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4236 2023-07-12 18:59:44.000000 simalq-0.1.0/simalq/quest_definition/__init__.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    19583 2023-07-12 18:59:44.000000 simalq-0.1.0/simalq/quest_definition/tutorial.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3294 2023-07-11 21:34:31.000000 simalq-0.1.0/simalq/save_load.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1970 2023-07-03 21:27:11.000000 simalq-0.1.0/simalq/strings.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-13 17:34:39.958485 simalq-0.1.0/simalq/tile/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    10921 2023-07-09 16:18:07.000000 simalq-0.1.0/simalq/tile/__init__.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    13654 2023-07-03 20:20:15.000000 simalq-0.1.0/simalq/tile/item.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    24271 2023-07-09 16:18:09.000000 simalq-0.1.0/simalq/tile/monster.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1832 2023-07-03 21:27:25.000000 simalq-0.1.0/simalq/tile/player.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    17196 2023-07-09 16:18:09.000000 simalq-0.1.0/simalq/tile/scenery.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2923 2023-07-09 16:18:07.000000 simalq-0.1.0/simalq/tile/tilepedia.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3141 2023-06-23 16:13:46.000000 simalq-0.1.0/simalq/tile/unimplemented.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     7070 2023-07-11 20:37:11.000000 simalq-0.1.0/simalq/un_iq.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     5688 2023-07-08 19:12:08.000000 simalq-0.1.0/simalq/util.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-13 17:34:39.958485 simalq-0.1.0/simalq.egg-info/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     6676 2023-07-13 17:34:39.000000 simalq-0.1.0/simalq.egg-info/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      690 2023-07-13 17:34:39.000000 simalq-0.1.0/simalq.egg-info/SOURCES.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2023-07-13 17:34:39.000000 simalq-0.1.0/simalq.egg-info/dependency_links.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       74 2023-07-13 17:34:39.000000 simalq-0.1.0/simalq.egg-info/requires.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       13 2023-07-13 17:34:39.000000 simalq-0.1.0/simalq.egg-info/top_level.txt
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-13 17:34:39.958485 simalq-0.1.0/tests/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2023-03-29 13:51:08.000000 simalq-0.1.0/tests/__init__.py
```

### Comparing `simalq-0.0.0/PKG-INFO` & `simalq-0.1.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,66 @@
-Metadata-Version: 2.1
-Name: simalq
-Version: 0.0.0
-Summary: Infinitesimal Quest 2 + ε: A turn-based puzzling dungeon crawler
-Home-page: UNKNOWN
-Author: Kodi B. Arfer
-License: UNKNOWN
-Project-URL: Source Code, https://github.com/hylang/simalq
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-
 Infinitesimal Quest 2 + ε
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
-Infinitesimal Quest 2 + ε (or "SQ" for short; Python package name ``simalq``) is an in-progress, not-yet-playable Gauntlet-like turn-based puzzling dungeon crawler written to serve as an official example program for `Hy <http://hylang.org>`_. It's a reimplementation / remake / demake of `Yves Meynard <http://yvesmeynard.com>`_'s 1996 Macintosh game Infinity Quest II, abbreviated "IQ". SQ is planned to feature:
+Infinitesimal Quest 2 + ε (or "SQ" for short; Python package name ``simalq``) is a Gauntlet-like turn-based puzzling dungeon crawler written to serve as an official example program for `Hy <http://hylang.org>`_. It's a reimplementation / remake / demake of `Yves Meynard <http://yvesmeynard.com>`_'s 1996 Macintosh game Infinity Quest II, abbreviated "IQ".
+
+.. figure:: https://hylang.org/simalq/img/screenshot-New_First_Quest-l10-0cf40784f039b08828dc9e2a41bd9544ee646755.png
+  :height: 300
+  :alt: A terminal window with a colorful roguelike-esque map.
+
+  The game running in Konsole on Lubuntu. Here our hero is getting overwhelmed by devils and bats on level 10 of New First Quest.
+
+Features of SQ include:
 
 - Playability on any platform with Python 3 and a compatible terminal emulator
 - Glorious roguelike-like console display, with no distracting graphics, sounds, or mouse support
 - Oodles of monsters, magic items, and tricky terrain
 - Deterministic, full-information gameplay
 - Undo with infinite history
 - Compatibility with quest (level) files in IQ's binary format
 - An extensive test suite
 
 Usage
 ============================================================
 
-There's no user interface yet, but you can run the tests with the command ``pytest``.
+You can install SQ via `pip <https://packaging.python.org/en/latest/tutorials/installing-packages/>`__ from the Python Package Index (PyPI) with the command ``pip install simalq``, or from source with  ``pip install .``. For the best display, you should use a terminal emulator that supports 24-bit color (I'm a fan of `Konsole <https://konsole.kde.org>`__), but SQ should be able to cope with less color support and use the best approximations available via its dependency `blessed <https://pypi.org/project/blessed/>`__.
+
+Run SQ with ``python3 -m simalq``, or run the tests with ``pytest``. Use ``python3 -m simalq --help`` for options. A good way to start is Tutorial Quest: ``python3 -m simalq Tutorial_Quest``.
 
 The first time that SQ requires IQ's original quests, it will download them automatically. The download is cached, so no Internet connection is needed afterwards.
 
+See the `tilepedia <http://hylang.org/simalq/doc/tilepedia>`__ for an HTML compendium of tile info pages.
+
 The story so far
 ============================================================
 
-Her Royal Highness Princess Triskaidecagonn XIII (whose friends call her "Tris"), tiring of her studies, shut the heavy grimoire of nonstandard analysis. "For too long I have been obliged to concern myself with tedious scholarship," she lamented aloud, "while my older brother Argonn has sallied forth on many an heroic quest. Here I sit, idling, with nary an opportunity to test my own skills in the sword, the bow, and the sliding-block puzzle."
+Her Royal Highness Princess Triskaidecagonn XIII (whose friends call her "Tris"), tiring of her studies, shut the heavy grimoire of nonstandard analysis. "For too long I have been obliged to concern myself with tedious scholarship" she lamented aloud "while my older brother Argonn has sallied forth on many an heroic quest. Here I sit, idling, with nary an opportunity to test my own skills in the sword, the bow, and the sliding-block puzzle."
 
 "Aha!" cried the fell wizard Idok, deep in his underground laboratory, who had been spying on the princess through his mystical Macintosh LC so he could copy her homework answers. "Here is an opportunity to teach you, young princess, to be careful what you wish for." He typed a dread incantation in Hy, the long-dead language of squids born of snakes, and in a swarm of foul parentheses, Tris was carried off to a vast dungeon deep beneath the faraway elven land of Québec. The place looked familiar, and Tris realized that Idok had plagiarized pretty much the whole thing from the thesis of his doctoral advisor, the wicked sorcerer Karvarel. Her brother had braved these very dungeons years ago. She didn't have his memoirs handy, but she did know one really good magic spell, which allowed her to predict the future. Now, with this clairvoyance, her trusty sword and bow, and anything handy she happens to find lying around, Tris must escape the dungeon or die in the attempt. And if she can stuff her pockets with loot on the way, that would really help with her kingdom's latest financial crisis.
 
 Differences from IQ
 ============================================================
 
-Apart from cosmetic and other interface differences, the chief way SQ differs from IQ in its design is its commitment to determinism. SQ replaces IQ's random mechanics, such as monster pathfinding, with deterministic equivalents, sometimes making aspects of the game stateful that were previously stateless. SQ also deliberately omits interface hijinks like darkness and confusion. SQ adds mid-game saving and loading, undo, visibility of the map outside the hero's shooting radius, fixes to bugs and weird behavior (e.g., winning with a "you have died message" if you win the game and die to poison on the same turn), removal of many engine limits (e.g., max and min level size), and the ability to adjust some core game rules (e.g., whether monsters can walk on items).
+Apart from cosmetic and other interface differences, the chief way SQ differs from IQ in its design is its commitment to determinism. SQ replaces IQ's random mechanics, such as monster pathfinding, with deterministic equivalents, sometimes making aspects of the game stateful that were previously stateless. SQ also deliberately omits interface hijinks like darkness and confusion. SQ adds flavor text for tiles, mid-game saving and loading, undo, visibility of the map outside the hero's shooting radius, fixes to bugs and weird behavior (e.g., winning with a "you have died" message if you win the game and die to poison on the same turn), removal of many engine limits (e.g., max and min level size), and the ability to adjust some core game rules (e.g., whether monsters can walk on items).
 
 While the author of IQ kindly provided me with its source code for reference, SQ is an original work that doesn't substantively copy IQ at the code level, and has many fine differences (deliberate, and probably also accidental) in behavior.
 
-Contributing
+Development status
 ============================================================
 
-At this stage of development, bugs and feature requests are unlikely to be useful, so the GitHub issues list is disabled. If you'd like to get involved, get in touch with me directly.
+SQ is reasonably polished and allows playing through several complete quests. The primary thing that's missing is the implementation of more tile types, to support more of IQ's original quests. I also plan to do some larger-scale code cleanup and document some of the interesting parts of the implementation, so that SQ better serves its purpose as an instructive example Hy program.
+
+Version history
+============================================================
+
+- 0.1.0 (2023-07-13): First playable release.
 
 License
 ============================================================
 
 This program is copyright 2023 Kodi B. Arfer.
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the `GNU General Public License`_ for more details.
 
 .. _`GNU General Public License`: http://www.gnu.org/licenses/
-
-
```

### Comparing `simalq-0.0.0/setup.py` & `simalq-0.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+dependencies = [
+    'hy == 0.27.0',
+    'hyrule == 0.4.0',
+    'toolz >= 0.12.0',
+    'construct >= 2.10.68',
+    'blessed >= 1.20.0']
+
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name = 'simalq',
-    version = '0.0.0',
+    version = '0.1.0',
     author = 'Kodi B. Arfer',
     description = 'Infinitesimal Quest 2 + ε: A turn-based puzzling dungeon crawler',
     long_description = Path('README.rst').read_text(),
     long_description_content_type = 'text/x-rst',
     project_urls = {
         'Source Code': 'https://github.com/hylang/simalq'},
-    install_requires = [
-        'hy @ git+https://github.com/hylang/hy@master',
-        'hyrule @ git+https://github.com/hylang/hyrule@master',
-        'toolz >= 0.12.0',
-        'construct >= 2.10.68'],
+    install_requires = dependencies,
     packages = setuptools.find_packages(),
     package_data = dict(simalq = [
         str(p.relative_to('simalq'))
         for p in Path('simalq').rglob('*.hy')]),
     classifiers = [
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent',
```

### Comparing `simalq-0.0.0/simalq/geometry.hy` & `simalq-0.1.0/simalq/geometry.hy`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 (require
-  hyrule [unless]
+  hyrule [unless do-n]
   simalq.macros [defdataclass])
 (import
   itertools [chain]
   toolz [unique]
-  simalq.util [seq sign])
+  simalq.util [seq sign]
+  simalq.game-state [G])
 (setv  T True  F False)
 
 
 (defdataclass Map []
   "A level layout."
 
   [wrap-x wrap-y data]
@@ -39,23 +40,28 @@
 ((fn []
   ; Define the direction constants (`Direction.N`, `.NE`, etc.)
   ; and collections thereof (`Direction.orths`, `.diags`, `.all`).
   (setv Direction.orths (tuple (map Direction
     ["north" "east" "south" "west"]
     [0       1       0      -1]
     [1       0      -1       0])))
+  (setv arrows
+    ["↑"     "→"    "↓"     "←"])
   (for [d Direction.orths]
     (setattr Direction (.upper (get d.name 0)) d))
+  (setv Direction.arrows (dict (zip Direction.orths arrows)))
   (setv Direction.diags (tuple (gfor
     d1 [Direction.N Direction.S]
     d2 [Direction.E Direction.W]
     :setv new (Direction (+ d1.name d2.name) (+ d1.x d2.x) (+ d1.y d2.y))
     :do (setattr Direction (.upper (+ (get d1.name 0) (get d2.name 0))) new)
     new)))
-  (setv Direction.all (+ Direction.orths Direction.diags))
+  (setv Direction.all #(
+     Direction.N Direction.NE Direction.E Direction.SE
+     Direction.S Direction.SW Direction.W Direction.NW))
   (setv Direction.from-coords (dfor
     d Direction.all
     #(d.x d.y) d))
   ; Define opposite directions.
   (setv opposites (dfor
     d1 Direction.all
     d2 Direction.all
@@ -67,35 +73,55 @@
 
 (defdataclass Pos []
   "A position; a point on a map."
 
   [map x y]
   :frozen T
 
-  (defn __init__ [self m x y]
-    (when m.wrap-x
-      (%= x m.width))
-    (when m.wrap-y
-      (%= y m.height))
-    (unless (and (<= 0 x (- m.width 1)) (<= 0 y (- m.height 1)))
+  (defn __init__ [self map x y]
+    (when map.wrap-x
+      (%= x map.width))
+    (when map.wrap-y
+      (%= y map.height))
+    (unless (and (<= 0 x (- map.width 1)) (<= 0 y (- map.height 1)))
       (raise (GeometryError f"Illegal position: {x}, {y}")))
-    (for [[k v] (.items (dict  :map m  :x x  :y y))]
+    (for [[k v] (.items (dict  :map map  :x x  :y y))]
       ; Call `object.__setattr__` to bypass `dataclass`'s frozen
       ; checks.
       (object.__setattr__ self k v)))
 
   (defn __str__ [self]
     "Provide a concise representation, without the linked map."
     f"<Pos {self.x},{self.y}>")
 
   (defn __hash__ [self]
-    (hash #(self.x self.y (id self.map)))))
+    (hash #(self.x self.y (id self.map))))
+
+  (defn [property] xy [self]
+    #(self.x self.y)))
+
+(hy.repr-register Pos str)
 
 (defn pos+ [pos direction]
-  (Pos pos.map (+ direction.x pos.x) (+ direction.y pos.y)))
+  (try
+    (Pos pos.map (+ direction.x pos.x) (+ direction.y pos.y))
+    (except [GeometryError])))
+
+(defn ray [pos direction length]
+  "Return a line of `length` points in `direction` from `pos`, not
+  including `pos`. If it wraps far enough that it would get to `pos`,
+  it stops just before it."
+
+  (setv out [pos])
+  (do-n length
+    (setv new (pos+ (get out -1) direction))
+    (when (or (is new None) (= new pos))
+      (break))
+    (.append out new))
+  (tuple (cut out 1 None)))
 
 (defn at [pos]
   (get pos.map.data pos.x pos.y))
 
 (defn adjacent? [p1 p2]
   (= (dist p1 p2) 1))
 
@@ -126,40 +152,52 @@
   (when (and m.wrap-x (> (abs dx) (/ m.width 2)))
     (*= dx -1))
   (setv dy (- p2.y p1.y))
   (when (and m.wrap-y (> (abs dy) (/ m.height 2)))
     (*= dy -1))
   (get Direction.from-coords #((sign dx) (sign dy))))
 
+(defn pos-seed [pos]
+  "Using a `Pos`, get a number you could use as an RNG seed. Nearby
+  `Pos`es should return different values."
+  (+
+    (* G.level-n 1,000,003)
+      ; The multiplier is chosen to be (a) prime and (b) bigger
+      ; than the area of most levels.
+    pos.x
+    (* G.map.width pos.y)))
 
-(defn burst [center size]
+
+(defn burst [center size [exclude-center False]]
   "Return a generator of all distinct points within distance `size` of
-  `center`. Thus the points form a square that's `size + 1` squares
-  wide. The order in which they're generated spirals outwards like
-  this (with size = 2):
+  `center`. Thus the points form a square that's `2 * size + 1`
+  squares wide. The order in which they're generated spirals outwards
+  like this (with size = 2):
 
       21 20 19 18 17
       22  7  6  5 16
       23  8  0  4 15
       24  1  2  3 14
        9 10 11 12 13
 
   This follows `SpiralX` and `SpiralY` in IQ (but upside-down). An
   important property of it is that activating monsters in this order
   allows monsters closer to the player to move first, so a line of
-  monsters can march toward the player without creating gaps."
+  monsters can march toward the player without creating gaps.
+
+  If `exclude-center` is true, the center position isn't returned."
 
   (unique (gfor
-    c (seq 0 size)
+    c (seq 0 (min size (max center.map.width center.map.height)))
     [x y] (py "chain(
       (( x, -c) for x in seq(    -c,      c,  1)),
       (( c,  y) for y in seq(-c + 1,      c,  1)),
       (( x,  c) for x in seq( c - 1,     -c, -1)),
       ((-c,  y) for y in seq( c - 1, -c + 1, -1)))")
     :setv p (try
       (Pos center.map (+ center.x x) (+ center.y y))
       (except [GeometryError]))
-    :if p
+    :if (and p (not (and exclude-center (= p center))))
     p)))
 
 
 (defclass GeometryError [Exception])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `simalq-0.0.0/simalq/un_iq.hy` & `simalq-0.1.0/simalq/un_iq.hy`

 * *Files 20% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 ;; --------------------------------------------------------------
 ;; * Imports
 ;; --------------------------------------------------------------
 
 (require
   hyrule [unless])
 (import
+  types [FunctionType]
   fractions [Fraction]
-  os
-  pathlib [Path]
   zipfile [ZipFile]
+  functools [cache]
   construct
   toolz [partition]
+  simalq.util [cache-dir]
   simalq.geometry [Map Pos]
   simalq.quest [Quest Level]
   simalq.tile [Tile])
 (setv  T True  F False)
 
 ;; --------------------------------------------------------------
 ;; * Helpers
@@ -118,79 +119,111 @@
     'map (Bytes (* this.width this.height))
     'tile-extras (Array this.n-tile-extras (sym-struct
       'pos iq-pos
       'data (Bytes 2)))))
   Terminated)))
 
 ;; --------------------------------------------------------------
-;; * `read-quest`, `iq-quest`
+;; * `iq-quest`
 ;; --------------------------------------------------------------
 
-(defn read-quest [inp]
-  "Parse `bytes` into a `Quest`."
+(defn iq-quest [quest-name]
+  "Get the given original quest IQ, as a `Quest`. Or use the symbol
+  `all` to get all quests as a dictionary."
+  (if (= quest-name 'all)
+    (dfor
+      [k v] (.items (iq-quests-raw))
+      k (read-quest k v))
+    (read-quest quest-name (get (iq-quests-raw) quest-name))))
 
-  (setv data (.parse quest-fmt inp))
+(defn [cache] iq-quests-raw []
+  "Get a dictionary of raw IQ quests as `bytes` objects."
 
-  (defn mk-pos [m xy]
-    "Convert from IQ coordinates (1-based indices, y = 1 on top, 0
-    means missing) to SQ coordinates (0-based indices with y = 0 on
-    bottom, None means missing)."
-    (if (and #* xy)
-      (Pos m (- (get xy 0) 1) (- m.height (get xy 1)))
-      None))
+  ; Download the quests if needed.
+  (.mkdir cache-dir :exist-ok T)
+  (setv path (/ cache-dir "infinity_quests_2.zip"))
+  (unless (.exists path)
+    (import http.client contextlib)
+    (with [con (contextlib.closing (http.client.HTTPConnection "arfer.net"))]
+      (.request con "GET" "/downloads/infinity_quests_2.zip"
+        :headers {"User-Agent" "Infinitesimal Quest 2 + epsilon"})
+      (setv r (.getresponse con))
+      (assert (= r.status 200))
+      (.write-bytes path (.read r))))
+
+  ; Read the files from the archive.
+  (setv prefix "infinity_quests_2/")
+  (with [z (ZipFile path "r")] (dfor
+    q (.namelist z)
+    :setv v (.read z q)
+    :if v
+    (.removeprefix q prefix) v)))
 
+(defn read-quest [name inp]
+  "Parse `bytes` into a `Quest`."
+
+  (setv data (.parse quest-fmt inp))
   (Quest
+    :name name
     :title data.title
+    :authors (if (= name "New DeathQuest")
+      "Yves and Serge Meynard"
+      "Yves Meynard")
     :starting-hp data.starting-hp
     :levels (tuple (gfor
       [i l] (enumerate data.levels)
+
       :setv m (Map.make l.wrap-x l.wrap-y l.width l.height)
+      :setv mk-pos (fn [xy]
+        "Convert from IQ coordinates (1-based indices, y = 1 on top, 0
+        means missing) to SQ coordinates (0-based indices with y = 0 on
+        bottom, None means missing)."
+        (if (and #* xy)
+          (Pos m (- (get xy 0) 1) (- m.height (get xy 1)))
+          None))
       :setv tile-extras (dfor
         c l.tile-extras
-        (mk-pos m c.pos) (tuple c.data))
+        (mk-pos c.pos) (tuple c.data))
+
       :do (for [x (range l.width)  y (range l.height)]
         ; Fill in `m`.
         (setv iq-ix (get l.map (+ (* x l.height) (- l.height y 1))))
           ; We have to reverse y-coordinates to get y = 0 as the
           ; bottom row.
         (unless (= iq-ix FLOOR)
           (setv p (Pos m x y))
-          (setv cls (get Tile.types-by-iq-ix iq-ix))
-          (.append (get m.data x y) (cls :pos p #**
+          (setv result (get Tile.types-by-iq-ix iq-ix))
+          (defn te [cls]
             (if (in p tile-extras)
-              (.read-tile-extras cls #* (get tile-extras p))
-              {})))))
+              (.read-tile-extras cls mk-pos
+                #* (get tile-extras p))
+              {}))
+          (.extend (get m.data x y) (cond
+            (is (type result) type)
+              ; The usual case: the `iq-ix` specifies the type, and no
+              ; more.
+              [(result :pos p #** (te result))]
+            (is (type result) dict)
+              ; This `iq-ix` specifies the type and a certain value of
+              ; a slot.
+              [((get result "cls") :pos p
+                #** {(get result "slot") (get result "value")}
+                #** (te (get result "cls")))]
+            (callable (type result))
+              ; A special case where a callback makes the tiles
+              ; itself. It can return any number of them.
+              (result p #* (get tile-extras p))
+            T
+              (raise (ValueError (+ "Bad `Tile.types-by-iq-ix` entry: " (repr result))))))))
+
       (Level
         :n (+ i 1)
         :title l.title
-        :player-start (mk-pos m l.player-start)
+        :player-start (mk-pos l.player-start)
         :next-level l.next-level
         :poison-intensity (if (= l.poison-interval 0)
           (Fraction 0)
           (Fraction 1 l.poison-interval))
         :time-limit l.time-limit
         :exit-speed l.exit-speed
-        :moving-exit-start (mk-pos m l.moving-exit-start)
+        :moving-exit-start (mk-pos l.moving-exit-start)
         :map m)))))
-
-
-(defn iq-quest [quest-name]
-  "Get the given original quest file from IQ, as a raw `bytes`
-  object."
-
-  ; Download the quests if needed.
-  (assert (get os.environ "XDG_CACHE_HOME"))
-  (setv path (/ (Path (get os.environ "XDG_CACHE_HOME")) "simalq"))
-  (.mkdir path :exist-ok T)
-  (setv path (/ path "infinity_quests_2.zip"))
-  (unless (.exists path)
-    (import http.client contextlib)
-    (with [con (contextlib.closing (http.client.HTTPConnection "arfer.net"))]
-      (.request con "GET" "/downloads/infinity_quests_2.zip"
-        :headers {"User-Agent" "Infinitesimal Quest 2 + epsilon"})
-      (setv r (.getresponse con))
-      (assert (= r.status 200))
-      (.write-bytes path (.read r))))
-
-  ; Get the requested quest (heh).
-  (with [z (ZipFile path "r")]
-    (.read z (+ "infinity_quests_2/" quest-name))))
```

### Comparing `simalq-0.0.0/simalq.egg-info/PKG-INFO` & `simalq-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 Metadata-Version: 2.1
 Name: simalq
-Version: 0.0.0
+Version: 0.1.0
 Summary: Infinitesimal Quest 2 + ε: A turn-based puzzling dungeon crawler
-Home-page: UNKNOWN
 Author: Kodi B. Arfer
-License: UNKNOWN
 Project-URL: Source Code, https://github.com/hylang/simalq
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 
 Infinitesimal Quest 2 + ε
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
-Infinitesimal Quest 2 + ε (or "SQ" for short; Python package name ``simalq``) is an in-progress, not-yet-playable Gauntlet-like turn-based puzzling dungeon crawler written to serve as an official example program for `Hy <http://hylang.org>`_. It's a reimplementation / remake / demake of `Yves Meynard <http://yvesmeynard.com>`_'s 1996 Macintosh game Infinity Quest II, abbreviated "IQ". SQ is planned to feature:
+Infinitesimal Quest 2 + ε (or "SQ" for short; Python package name ``simalq``) is a Gauntlet-like turn-based puzzling dungeon crawler written to serve as an official example program for `Hy <http://hylang.org>`_. It's a reimplementation / remake / demake of `Yves Meynard <http://yvesmeynard.com>`_'s 1996 Macintosh game Infinity Quest II, abbreviated "IQ".
+
+.. figure:: https://hylang.org/simalq/img/screenshot-New_First_Quest-l10-0cf40784f039b08828dc9e2a41bd9544ee646755.png
+  :height: 300
+  :alt: A terminal window with a colorful roguelike-esque map.
+
+  The game running in Konsole on Lubuntu. Here our hero is getting overwhelmed by devils and bats on level 10 of New First Quest.
+
+Features of SQ include:
 
 - Playability on any platform with Python 3 and a compatible terminal emulator
 - Glorious roguelike-like console display, with no distracting graphics, sounds, or mouse support
 - Oodles of monsters, magic items, and tricky terrain
 - Deterministic, full-information gameplay
 - Undo with infinite history
 - Compatibility with quest (level) files in IQ's binary format
 - An extensive test suite
 
 Usage
 ============================================================
 
-There's no user interface yet, but you can run the tests with the command ``pytest``.
+You can install SQ via `pip <https://packaging.python.org/en/latest/tutorials/installing-packages/>`__ from the Python Package Index (PyPI) with the command ``pip install simalq``, or from source with  ``pip install .``. For the best display, you should use a terminal emulator that supports 24-bit color (I'm a fan of `Konsole <https://konsole.kde.org>`__), but SQ should be able to cope with less color support and use the best approximations available via its dependency `blessed <https://pypi.org/project/blessed/>`__.
+
+Run SQ with ``python3 -m simalq``, or run the tests with ``pytest``. Use ``python3 -m simalq --help`` for options. A good way to start is Tutorial Quest: ``python3 -m simalq Tutorial_Quest``.
 
 The first time that SQ requires IQ's original quests, it will download them automatically. The download is cached, so no Internet connection is needed afterwards.
 
+See the `tilepedia <http://hylang.org/simalq/doc/tilepedia>`__ for an HTML compendium of tile info pages.
+
 The story so far
 ============================================================
 
-Her Royal Highness Princess Triskaidecagonn XIII (whose friends call her "Tris"), tiring of her studies, shut the heavy grimoire of nonstandard analysis. "For too long I have been obliged to concern myself with tedious scholarship," she lamented aloud, "while my older brother Argonn has sallied forth on many an heroic quest. Here I sit, idling, with nary an opportunity to test my own skills in the sword, the bow, and the sliding-block puzzle."
+Her Royal Highness Princess Triskaidecagonn XIII (whose friends call her "Tris"), tiring of her studies, shut the heavy grimoire of nonstandard analysis. "For too long I have been obliged to concern myself with tedious scholarship" she lamented aloud "while my older brother Argonn has sallied forth on many an heroic quest. Here I sit, idling, with nary an opportunity to test my own skills in the sword, the bow, and the sliding-block puzzle."
 
 "Aha!" cried the fell wizard Idok, deep in his underground laboratory, who had been spying on the princess through his mystical Macintosh LC so he could copy her homework answers. "Here is an opportunity to teach you, young princess, to be careful what you wish for." He typed a dread incantation in Hy, the long-dead language of squids born of snakes, and in a swarm of foul parentheses, Tris was carried off to a vast dungeon deep beneath the faraway elven land of Québec. The place looked familiar, and Tris realized that Idok had plagiarized pretty much the whole thing from the thesis of his doctoral advisor, the wicked sorcerer Karvarel. Her brother had braved these very dungeons years ago. She didn't have his memoirs handy, but she did know one really good magic spell, which allowed her to predict the future. Now, with this clairvoyance, her trusty sword and bow, and anything handy she happens to find lying around, Tris must escape the dungeon or die in the attempt. And if she can stuff her pockets with loot on the way, that would really help with her kingdom's latest financial crisis.
 
 Differences from IQ
 ============================================================
 
-Apart from cosmetic and other interface differences, the chief way SQ differs from IQ in its design is its commitment to determinism. SQ replaces IQ's random mechanics, such as monster pathfinding, with deterministic equivalents, sometimes making aspects of the game stateful that were previously stateless. SQ also deliberately omits interface hijinks like darkness and confusion. SQ adds mid-game saving and loading, undo, visibility of the map outside the hero's shooting radius, fixes to bugs and weird behavior (e.g., winning with a "you have died message" if you win the game and die to poison on the same turn), removal of many engine limits (e.g., max and min level size), and the ability to adjust some core game rules (e.g., whether monsters can walk on items).
+Apart from cosmetic and other interface differences, the chief way SQ differs from IQ in its design is its commitment to determinism. SQ replaces IQ's random mechanics, such as monster pathfinding, with deterministic equivalents, sometimes making aspects of the game stateful that were previously stateless. SQ also deliberately omits interface hijinks like darkness and confusion. SQ adds flavor text for tiles, mid-game saving and loading, undo, visibility of the map outside the hero's shooting radius, fixes to bugs and weird behavior (e.g., winning with a "you have died" message if you win the game and die to poison on the same turn), removal of many engine limits (e.g., max and min level size), and the ability to adjust some core game rules (e.g., whether monsters can walk on items).
 
 While the author of IQ kindly provided me with its source code for reference, SQ is an original work that doesn't substantively copy IQ at the code level, and has many fine differences (deliberate, and probably also accidental) in behavior.
 
-Contributing
+Development status
 ============================================================
 
-At this stage of development, bugs and feature requests are unlikely to be useful, so the GitHub issues list is disabled. If you'd like to get involved, get in touch with me directly.
+SQ is reasonably polished and allows playing through several complete quests. The primary thing that's missing is the implementation of more tile types, to support more of IQ's original quests. I also plan to do some larger-scale code cleanup and document some of the interesting parts of the implementation, so that SQ better serves its purpose as an instructive example Hy program.
+
+Version history
+============================================================
+
+- 0.1.0 (2023-07-13): First playable release.
 
 License
 ============================================================
 
 This program is copyright 2023 Kodi B. Arfer.
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the `GNU General Public License`_ for more details.
 
 .. _`GNU General Public License`: http://www.gnu.org/licenses/
-
-
```

