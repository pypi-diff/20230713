# Comparing `tmp/seaplayer-0.5.5.post1.tar.gz` & `tmp/seaplayer-0.5.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.5.post1.tar", max compression
+gzip compressed data, was "seaplayer-0.5.5.post2.tar", max compression
```

## Comparing `seaplayer-0.5.5.post1.tar` & `seaplayer-0.5.5.post2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.5.post1/LICENSE
--rw-r--r--   0        0        0     1698 2023-06-13 21:20:39.923937 seaplayer-0.5.5.post1/pyproject.toml
--rw-r--r--   0        0        0     1324 2023-05-28 16:32:50.014284 seaplayer-0.5.5.post1/README.md
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.5.post1/seaplayer/__init__.py
--rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.5.post1/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.5.post1/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0      316 2023-05-31 18:55:35.145071 seaplayer-0.5.5.post1/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-31 21:59:01.640445 seaplayer-0.5.5.post1/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0     2916 2023-05-31 18:55:35.143083 seaplayer-0.5.5.post1/seaplayer/codecs/AnySound.py
--rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.5.post1/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     1160 2023-05-31 18:55:35.144073 seaplayer-0.5.5.post1/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      487 2023-05-31 18:55:35.144073 seaplayer-0.5.5.post1/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      475 2023-05-30 22:33:59.986095 seaplayer-0.5.5.post1/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0     2419 2023-06-13 21:20:39.925946 seaplayer-0.5.5.post1/seaplayer/codecs/URLS.py
--rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.5.post1/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.5.post1/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6188 2023-05-27 18:01:34.042639 seaplayer-0.5.5.post1/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.5.post1/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.5.post1/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.5.post1/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.5.post1/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.5.post1/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1460 2023-05-31 18:55:35.146073 seaplayer-0.5.5.post1/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.5.post1/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-27 17:36:06.594476 seaplayer-0.5.5.post1/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.5.post1/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.5.post1/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.5.post1/seaplayer/objects/DataOptions.py
--rw-r--r--   0        0        0     3073 2023-06-13 21:20:39.926942 seaplayer-0.5.5.post1/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.5.post1/seaplayer/objects/Input.py
--rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.5.post1/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5701 2023-05-27 17:49:37.836036 seaplayer-0.5.5.post1/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.5.post1/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.5.post1/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.5.post1/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.5.post1/seaplayer/plug/__main__.py
--rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.5.post1/seaplayer/plug/cli/__init__.py
--rw-r--r--   0        0        0     5259 2023-05-27 12:11:55.197047 seaplayer-0.5.5.post1/seaplayer/plug/cli/cli.py
--rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.5.post1/seaplayer/plug/cli/exceptions.py
--rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.5.post1/seaplayer/plug/cli/functions.py
--rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.5.post1/seaplayer/plug/cli/vars.py
--rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.5.post1/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.5.post1/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     8688 2023-05-28 16:09:52.376773 seaplayer-0.5.5.post1/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.5.post1/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.5.post1/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.5.post1/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.5.post1/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0    21058 2023-05-31 18:55:35.146073 seaplayer-0.5.5.post1/seaplayer/seaplayer.py
--rw-r--r--   0        0        0       91 2023-05-27 09:37:18.022755 seaplayer-0.5.5.post1/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     1576 2023-05-27 12:03:27.045912 seaplayer-0.5.5.post1/seaplayer/types/Cache.py
--rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.5.post1/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1599 2023-06-13 21:20:39.926942 seaplayer-0.5.5.post1/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0     1526 2023-06-13 21:20:39.927941 seaplayer-0.5.5.post1/seaplayer/units.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 seaplayer-0.5.5.post1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.5.post2/LICENSE
+-rw-r--r--   0        0        0     1698 2023-07-13 12:53:06.838374 seaplayer-0.5.5.post2/pyproject.toml
+-rw-r--r--   0        0        0     1324 2023-05-28 16:32:50.014284 seaplayer-0.5.5.post2/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.5.post2/seaplayer/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.5.post2/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.5.post2/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0      316 2023-05-31 18:55:35.145071 seaplayer-0.5.5.post2/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-31 21:59:01.640445 seaplayer-0.5.5.post2/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0     2916 2023-05-31 18:55:35.143083 seaplayer-0.5.5.post2/seaplayer/codecs/AnySound.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.5.post2/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     1160 2023-05-31 18:55:35.144073 seaplayer-0.5.5.post2/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      487 2023-05-31 18:55:35.144073 seaplayer-0.5.5.post2/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      475 2023-05-30 22:33:59.986095 seaplayer-0.5.5.post2/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0     2419 2023-06-13 21:20:39.925946 seaplayer-0.5.5.post2/seaplayer/codecs/URLS.py
+-rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.5.post2/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.5.post2/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6188 2023-05-27 18:01:34.042639 seaplayer-0.5.5.post2/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.5.post2/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.5.post2/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.5.post2/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.5.post2/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.5.post2/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1460 2023-05-31 18:55:35.146073 seaplayer-0.5.5.post2/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.5.post2/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-27 17:36:06.594476 seaplayer-0.5.5.post2/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.5.post2/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.5.post2/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.5.post2/seaplayer/objects/DataOptions.py
+-rw-r--r--   0        0        0     3073 2023-06-13 21:20:39.926942 seaplayer-0.5.5.post2/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.5.post2/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.5.post2/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5701 2023-05-27 17:49:37.836036 seaplayer-0.5.5.post2/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.5.post2/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.5.post2/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.5.post2/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.5.post2/seaplayer/plug/__main__.py
+-rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.5.post2/seaplayer/plug/cli/__init__.py
+-rw-r--r--   0        0        0     5259 2023-05-27 12:11:55.197047 seaplayer-0.5.5.post2/seaplayer/plug/cli/cli.py
+-rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.5.post2/seaplayer/plug/cli/exceptions.py
+-rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.5.post2/seaplayer/plug/cli/functions.py
+-rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.5.post2/seaplayer/plug/cli/vars.py
+-rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.5.post2/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.5.post2/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     8688 2023-05-28 16:09:52.376773 seaplayer-0.5.5.post2/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.5.post2/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.5.post2/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.5.post2/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.5.post2/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0    21058 2023-05-31 18:55:35.146073 seaplayer-0.5.5.post2/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0       91 2023-05-27 09:37:18.022755 seaplayer-0.5.5.post2/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-27 12:03:27.045912 seaplayer-0.5.5.post2/seaplayer/types/Cache.py
+-rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.5.post2/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1599 2023-06-13 21:20:39.926942 seaplayer-0.5.5.post2/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0     1526 2023-07-13 12:53:21.850881 seaplayer-0.5.5.post2/seaplayer/units.py
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 seaplayer-0.5.5.post2/PKG-INFO
```

### Comparing `seaplayer-0.5.5.post1/LICENSE` & `seaplayer-0.5.5.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/pyproject.toml` & `seaplayer-0.5.5.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.5.post1"
+version = "0.5.5.post2"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `seaplayer-0.5.5.post1/README.md` & `seaplayer-0.5.5.post2/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.5.post2/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/codecs/Any.py` & `seaplayer-0.5.5.post2/seaplayer/codecs/Any.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/codecs/AnySound.py` & `seaplayer-0.5.5.post2/seaplayer/codecs/AnySound.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.5.post2/seaplayer/codecs/MIDI.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/codecs/URLS.py` & `seaplayer-0.5.5.post2/seaplayer/codecs/URLS.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/codecs/WAV.py` & `seaplayer-0.5.5.post2/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/codeсbase.py` & `seaplayer-0.5.5.post2/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/config.py` & `seaplayer-0.5.5.post2/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/css/objects.css` & `seaplayer-0.5.5.post2/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/css/seaplayer.css` & `seaplayer-0.5.5.post2/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/functions.py` & `seaplayer-0.5.5.post2/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/modules/colorizer.py` & `seaplayer-0.5.5.post2/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/objects/Configurate.py` & `seaplayer-0.5.5.post2/seaplayer/objects/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/objects/DataOptions.py` & `seaplayer-0.5.5.post2/seaplayer/objects/DataOptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/objects/Image.py` & `seaplayer-0.5.5.post2/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/objects/Input.py` & `seaplayer-0.5.5.post2/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/objects/Log.py` & `seaplayer-0.5.5.post2/seaplayer/objects/Log.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/objects/MusicList.py` & `seaplayer-0.5.5.post2/seaplayer/objects/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/objects/Notification.py` & `seaplayer-0.5.5.post2/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.5.post2/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/plug/cli/cli.py` & `seaplayer-0.5.5.post2/seaplayer/plug/cli/cli.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/plug/cli/exceptions.py` & `seaplayer-0.5.5.post2/seaplayer/plug/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/plug/cli/functions.py` & `seaplayer-0.5.5.post2/seaplayer/plug/cli/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.5.post2/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.5.post2/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.5.post2/seaplayer/plug/pluginloader.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.5.post2/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/screens/Configurate.py` & `seaplayer-0.5.5.post2/seaplayer/screens/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/screens/Unknown.py` & `seaplayer-0.5.5.post2/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/seaplayer.py` & `seaplayer-0.5.5.post2/seaplayer/seaplayer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/types/Cache.py` & `seaplayer-0.5.5.post2/seaplayer/types/Cache.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/types/Convert.py` & `seaplayer-0.5.5.post2/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/types/MusicList.py` & `seaplayer-0.5.5.post2/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.5.post1/seaplayer/units.py` & `seaplayer-0.5.5.post2/seaplayer/units.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.5.post1"
+__version__ = "0.5.5.post2"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.5.5.post1/PKG-INFO` & `seaplayer-0.5.5.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.5.post1
+Version: 0.5.5.post2
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
```

