# Comparing `tmp/whisper_autosrt-0.1.7.tar.gz` & `tmp/whisper_autosrt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.1.7.tar", last modified: Sat Jul  8 03:50:34 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.1.8.tar", last modified: Thu Jul 13 01:25:53 2023, max compression
```

## Comparing `whisper_autosrt-0.1.7.tar` & `whisper_autosrt-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 03:50:34.653506 whisper_autosrt-0.1.7/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2056 2023-07-08 03:50:34.653506 whisper_autosrt-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.7/README.md
--rw-rw-rw-   0        0        0      147 2023-07-08 03:50:34.657253 whisper_autosrt-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1749 2023-06-21 11:17:31.000000 whisper_autosrt-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:50:34.614548 whisper_autosrt-0.1.7/whisper_autosrt/
--rw-rw-rw-   0        0        0   168522 2023-07-08 03:50:15.000000 whisper_autosrt-0.1.7/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:50:34.650509 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     2056 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 01:25:53.615467 whisper_autosrt-0.1.8/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2056 2023-07-13 01:25:53.616216 whisper_autosrt-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.8/README.md
+-rw-rw-rw-   0        0        0      147 2023-07-13 01:25:53.618463 whisper_autosrt-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2023-06-21 11:17:31.000000 whisper_autosrt-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:25:53.584000 whisper_autosrt-0.1.8/whisper_autosrt/
+-rw-rw-rw-   0        0        0   169913 2023-07-13 01:25:07.000000 whisper_autosrt-0.1.8/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:25:53.613970 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2056 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.1.7/LICENSE` & `whisper_autosrt-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.7/PKG-INFO` & `whisper_autosrt-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_autosrt
-Version: 0.1.7
+Version: 0.1.8
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `whisper_autosrt-0.1.7/README.md` & `whisper_autosrt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.7/setup.py` & `whisper_autosrt-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.7/whisper_autosrt/__init__.py` & `whisper_autosrt-0.1.8/whisper_autosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import warnings
 warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 from faster_whisper import WhisperModel
 import ctypes
 import shutil
 
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 #marker='█'
 
 
 class WhisperLanguage:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("auto")
@@ -1098,32 +1098,32 @@
     def ffmpeg_check():
         if WavConverter.which("ffmpeg"):
             return "ffmpeg"
         if WavConverter.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
-    def __init__(self, channels=1, rate=16000, progress_callback=None, error_messages_callback=None):
+    def __init__(self, channels=1, rate=48000, progress_callback=None, error_messages_callback=None):
         self.channels = channels
         self.rate = rate
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def __call__(self, media_filepath):
         temp = tempfile.NamedTemporaryFile(suffix='.wav', delete=False)
 
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+                self.error_messages_callback(f"The given file does not exist: '{media_filepath}'")
             else:
-                print(f"The given file does not exist: {media_filepath}")
-                raise Exception(f"Invalid file: {media_filepath}")
+                print(f"The given file does not exist: '{media_filepath}'")
+                raise Exception(f"Invalid file: '{media_filepath}'")
 
         if not self.ffprobe_check():
             if self.error_messages_callback:
                 self.error_messages_callback("Cannot find ffprobe executable")
             else:
                 print("Cannot find ffprobe executable")
                 raise Exception("Dependency not found: ffprobe")
@@ -1691,18 +1691,18 @@
             self.subtitle_path = self.subtitle_path.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+                self.error_messages_callback(f"The given file does not exist: '{media_filepath}'")
             else:
-                print(f"The given file does not exist: {media_filepath}")
-                raise Exception(f"Invalid file: {media_filepath}")
+                print(f"The given file does not exist: '{media_filepath}'")
+                raise Exception(f"Invalid file: '{media_filepath}'")
 
         if not self.ffprobe_check():
             if self.error_messages_callback:
                 self.error_messages_callback("Cannot find ffprobe executable")
             else:
                 print("Cannot find ffprobe executable")
                 raise Exception("Dependency not found: ffprobe")
@@ -1881,18 +1881,18 @@
             self.subtitle_path = self.subtitle_path.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+                self.error_messages_callback(f"The given file does not exist: '{media_filepath}'")
             else:
-                print(f"The given file does not exist: {media_filepath}")
-                raise Exception(f"Invalid file: {media_filepath}")
+                print(f"The given file does not exist: '{media_filepath}'")
+                raise Exception(f"Invalid file: '{media_filepath}'")
 
         if not self.ffprobe_check():
             if self.error_messages_callback:
                 self.error_messages_callback("Cannot find ffprobe executable")
             else:
                 print("Cannot find ffprobe executable")
                 raise Exception("Dependency not found: ffprobe")
@@ -1904,15 +1904,15 @@
                 print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             existing_languages = self.get_existing_subtitle_language(media_filepath)
             if self.language in existing_languages:
                 # THIS 'print' THINGS WILL MAKE progresbar screwed up!
-                #msg = (f"'{self.language}' subtitle stream already existed in {media_filepath}")
+                #msg = (f"'{self.language}' subtitle stream already existed in '{media_filepath}'")
                 #if self.error_messages_callback:
                 #    self.error_messages_callback(msg)
                 #else:
                 #    print(msg)
                 return
 
             else:
@@ -2054,18 +2054,18 @@
             media_filepath = media_filepath.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+                self.error_messages_callback(f"The given file does not exist: '{media_filepath}'")
             else:
-                print(f"The given file does not exist: {media_filepath}")
-                raise Exception(f"Invalid file: {media_filepath}")
+                print(f"The given file does not exist: '{media_filepath}'")
+                raise Exception(f"Invalid file: '{media_filepath}'")
 
         if not self.ffprobe_check():
             if self.error_messages_callback:
                 self.error_messages_callback("Cannot find ffprobe executable")
             else:
                 print("Cannot find ffprobe executable")
                 raise Exception("Dependency not found: ffprobe")
@@ -2332,18 +2332,18 @@
         return None
 
     if "\\" in media_filepath:
         media_filepath = media_filepath.replace("\\", "/")
 
     if not os.path.isfile(media_filepath):
         if error_messages_callback:
-           error_messages_callback(f"The given file does not exist: {media_filepath}")
+           error_messages_callback(f"The given file does not exist: '{media_filepath}'")
         else:
-            print(f"The given file does not exist: {media_filepath}")
-            raise Exception(f"Invalid file: {media_filepath}")
+            print(f"The given file does not exist: '{media_filepath}'")
+            raise Exception(f"Invalid file: '{media_filepath}'")
     if not ffprobe_check():
         if error_messages_callback:
             error_messages_callback("Cannot find ffprobe executable")
         else:
             print("Cannot find ffprobe executable")
             raise Exception("Dependency not found: ffprobe")
 
@@ -2412,18 +2412,18 @@
         return None
 
     if "\\" in media_filepath:
         media_filepath = media_filepath.replace("\\", "/")
 
     if not os.path.isfile(media_filepath):
         if error_messages_callback:
-           error_messages_callback(f"The given file does not exist: {media_filepath}")
+           error_messages_callback(f"The given file does not exist: '{media_filepath}'")
         else:
-            print(f"The given file does not exist: {media_filepath}")
-            raise Exception(f"Invalid file: {media_filepath}")
+            print(f"The given file does not exist: '{media_filepath}'")
+            raise Exception(f"Invalid file: '{media_filepath}'")
     if not ffprobe_check():
         if error_messages_callback:
             error_messages_callback("Cannot find ffprobe executable")
         else:
             print("Cannot find ffprobe executable")
             raise Exception("Dependency not found: ffprobe")
 
@@ -2497,18 +2497,18 @@
         return None
 
     if "\\" in media_filepath:
         media_filepath = media_filepath.replace("\\", "/")
 
     if not os.path.isfile(media_filepath):
         if error_messages_callback:
-           error_messages_callback(f"The given file does not exist: {media_filepath}")
+           error_messages_callback(f"The given file does not exist: '{media_filepath}'")
         else:
-            print(f"The given file does not exist: {media_filepath}")
-            raise Exception(f"Invalid file: {media_filepath}")
+            print(f"The given file does not exist: '{media_filepath}'")
+            raise Exception(f"Invalid file: '{media_filepath}'")
     if not ffprobe_check():
         if error_messages_callback:
             error_messages_callback("Cannot find ffprobe executable")
         else:
             print("Cannot find ffprobe executable")
             raise Exception("Dependency not found: ffprobe")
     if not ffmpeg_check():
@@ -2624,18 +2624,18 @@
         return None
 
     if "\\" in media_filepath:
         media_filepath = media_filepath.replace("\\", "/")
 
     if not os.path.isfile(media_filepath):
         if error_messages_callback:
-           error_messages_callback(f"The given file does not exist: {media_filepath}")
+           error_messages_callback(f"The given file does not exist: '{media_filepath}'")
         else:
-            print(f"The given file does not exist: {media_filepath}")
-            raise Exception(f"Invalid file: {media_filepath}")
+            print(f"The given file does not exist: '{media_filepath}'")
+            raise Exception(f"Invalid file: '{media_filepath}'")
     if not ffmpeg_check():
         if error_messages_callback:
             error_messages_callback("Cannot find ffmpeg executable")
         else:
             print("Cannot find ffmpeg executable")
             raise Exception("Dependency not found: ffmpeg")
 
@@ -2647,15 +2647,15 @@
             subtitle_path = subtitle_path.replace("\\", "/")
 
         if "\\" in output_path:
             output_path = output_path.replace("\\", "/")
 
         existing_languages = get_existing_subtitle_language(media_filepath)
         if language_code in existing_languages:
-            #print(f"'{language_code}' subtitles stream already existed in {media_filepath}")
+            #print(f"'{language_code}' subtitles stream already existed in '{media_filepath}'")
             return
 
         else:
             # Determine the next available subtitles index
             next_index = len(existing_languages)
 
             ffmpeg_command = [
@@ -2760,18 +2760,18 @@
         return None
 
     if "\\" in media_filepath:
         media_filepath = media_filepath.replace("\\", "/")
 
     if not os.path.isfile(media_filepath):
         if error_messages_callback:
-           error_messages_callback(f"The given file does not exist: {media_filepath}")
+           error_messages_callback(f"The given file does not exist: '{media_filepath}'")
         else:
-            print(f"The given file does not exist: {media_filepath}")
-            raise Exception(f"Invalid file: {media_filepath}")
+            print(f"The given file does not exist: '{media_filepath}'")
+            raise Exception(f"Invalid file: '{media_filepath}'")
     if not ffmpeg_check():
         if error_messages_callback:
             error_messages_callback("Cannot find ffmpeg executable")
         else:
             print("Cannot find ffmpeg executable")
             raise Exception("Dependency not found: ffmpeg")
 
@@ -3328,16 +3328,22 @@
                                 if args.force_recognize == False:
                                     removed_media_filepaths.append(media_filepath)
 
                                 if args.embed_src and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                                     base, ext = os.path.splitext(media_filepath)
-                                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
-                                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
+
+                                    if ext[1:] == "ts":
+                                        media_format = "mp4"
+                                    else:
+                                        media_format = ext[1:]
+
+                                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
                                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                     src_tmp_output = subtitle_embedder(media_filepath)
                                     pbar.finish()
 
@@ -3381,16 +3387,22 @@
                                 if args.force_recognize == False:
                                     removed_media_filepaths.append(media_filepath)
 
                                 if args.embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
                                     base, ext = os.path.splitext(media_filepath)
-                                    dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
-                                    embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
+
+                                    if ext[1:] == "ts":
+                                        media_format = "mp4"
+                                    else:
+                                        media_format = ext[1:]
+
+                                    dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                                    embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
                                     widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                     dst_tmp_output = subtitle_embedder(media_filepath)
                                     pbar.finish()
 
@@ -3444,16 +3456,22 @@
     print("=========================================================================================================")
 
     proceed_list = []
     # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to proceed with transcribe
     if args.force_recognize == True:
         for media_filepath in media_filepaths:
             base, ext = os.path.splitext(media_filepath)
-            tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{ext[1:]}"
-            subtitle_removed_media_filepath = f"{base}.force.recognize.{ext[1:]}"
+
+            if ext[1:] == "ts":
+                media_format = "mp4"
+            else:
+                media_format = ext[1:]
+
+            tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{media_format}"
+            subtitle_removed_media_filepath = f"{base}.force.recognize.{media_format}"
 
             #src_tmp_output = remove_subtitles_from_media(media_filepath, tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
 
             widgets = [f"Removing subtitles streams from {media_type} file : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
             tmp_output = subtitle_remover(media_filepath)
@@ -3559,16 +3577,22 @@
             if do_translate == False:
 
                 if args.embed_src == True:
 
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                     base, ext = os.path.splitext(media_filepath)
-                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
-                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
+
+                    if ext[1:] == "ts":
+                        media_format = "mp4"
+                    else:
+                        media_format = ext[1:]
+
+                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     src_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
@@ -3581,17 +3605,23 @@
 
                 if args.embed_src == True and args.embed_dst == True:
 
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
                     base, ext = os.path.splitext(media_filepath)
-                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
-                    src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
-                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
+
+                    if ext[1:] == "ts":
+                        media_format = "mp4"
+                    else:
+                        media_format = ext[1:]
+
+                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                    src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     src_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
@@ -3616,16 +3646,22 @@
 
 
                 elif args.embed_src == True and args.embed_dst == False:
 
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                     base, ext = os.path.splitext(media_filepath)
-                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
-                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
+
+                    if ext[1:] == "ts":
+                        media_format = "mp4"
+                    else:
+                        media_format = ext[1:]
+
+                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     src_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
@@ -3637,16 +3673,22 @@
                         print("Unknown error!")
 
                 elif args.embed_src == False and args.embed_dst == True:
 
                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
                     base, ext = os.path.splitext(media_filepath)
-                    dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
-                    embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
+
+                    if ext[1:] == "ts":
+                        media_format = "mp4"
+                    else:
+                        media_format = ext[1:]
+
+                    dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                    embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
                     widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     dst_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
```

### Comparing `whisper_autosrt-0.1.7/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.1.8/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-autosrt
-Version: 0.1.7
+Version: 0.1.8
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

