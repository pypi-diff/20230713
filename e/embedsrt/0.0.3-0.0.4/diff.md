# Comparing `tmp/embedsrt-0.0.3.tar.gz` & `tmp/embedsrt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedsrt-0.0.3.tar", last modified: Sat Jul  8 13:20:32 2023, max compression
+gzip compressed data, was "embedsrt-0.0.4.tar", last modified: Thu Jul 13 19:32:33 2023, max compression
```

## Comparing `embedsrt-0.0.3.tar` & `embedsrt-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:20:32.790245 embedsrt-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 embedsrt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 embedsrt-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1560 2023-07-08 13:20:32.790992 embedsrt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3199 2023-06-07 14:26:01.000000 embedsrt-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 13:20:32.755030 embedsrt-0.0.3/embedsrt/
--rw-rw-rw-   0        0        0    73365 2023-07-08 13:17:54.000000 embedsrt-0.0.3/embedsrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:20:32.788746 embedsrt-0.0.3/embedsrt.egg-info/
--rw-rw-rw-   0        0        0     1560 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-07-08 13:20:32.793991 embedsrt-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1355 2023-06-07 14:21:47.000000 embedsrt-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:32:33.617063 embedsrt-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 embedsrt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 embedsrt-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1560 2023-07-13 19:32:33.617063 embedsrt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3199 2023-06-07 14:26:01.000000 embedsrt-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 19:32:33.578104 embedsrt-0.0.4/embedsrt/
+-rw-rw-rw-   0        0        0    73725 2023-07-13 19:32:08.000000 embedsrt-0.0.4/embedsrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:32:33.614817 embedsrt-0.0.4/embedsrt.egg-info/
+-rw-rw-rw-   0        0        0     1560 2023-07-13 19:32:33.000000 embedsrt-0.0.4/embedsrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-07-13 19:32:33.000000 embedsrt-0.0.4/embedsrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 19:32:33.000000 embedsrt-0.0.4/embedsrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-13 19:32:33.000000 embedsrt-0.0.4/embedsrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-13 19:32:33.000000 embedsrt-0.0.4/embedsrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 19:32:33.000000 embedsrt-0.0.4/embedsrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-13 19:32:33.620060 embedsrt-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2023-06-07 14:21:47.000000 embedsrt-0.0.4/setup.py
```

### Comparing `embedsrt-0.0.3/LICENSE` & `embedsrt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `embedsrt-0.0.3/PKG-INFO` & `embedsrt-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedsrt
-Version: 0.0.3
+Version: 0.0.4
 Summary: a utility for embedding subtitle file into video file
 Home-page: https://github.com/botbahlul/embedsrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `embedsrt-0.0.3/README.md` & `embedsrt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `embedsrt-0.0.3/embedsrt/__init__.py` & `embedsrt-0.0.4/embedsrt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 import pysrt
 from pathlib import Path
 from datetime import datetime, timedelta
 import time
 
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -1034,18 +1034,18 @@
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
@@ -1057,15 +1057,15 @@
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
@@ -1195,18 +1195,18 @@
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
@@ -1226,15 +1226,15 @@
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
@@ -1338,18 +1338,18 @@
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
 
@@ -1434,18 +1434,18 @@
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
 
@@ -1516,14 +1516,15 @@
 
     media_filepaths = []
     not_exist_media_filepaths = []
     invalid_media_filepaths = []
     media_filepaths = []
     media_filepath_str = ""
     media_type = None
+    media_format = None
 
     ffmpeg_src_language_code = None
     ffmpeg_dst_language_code = None
 
     language = Language()
 
     if args.list_languages:
@@ -1536,14 +1537,21 @@
 
     if args.media_filepath and args.subtitle_file_path and args.language and args.output_file_path:
 
         media_filepath = args.media_filepath
         subtitle_path = args.subtitle_file_path
         language_code = args.language
         output_path = args.output_file_path
+        base, ext = os.path.splitext(output_path)
+        if ext[1:] == "ts":
+            print("Subtitles embedded media file cannot be saved in '.ts' format, will save it in '.mp4' format instead")
+            media_format = "mp4"
+        else:
+            media_format = ext[1:]
+        output_path = f"{base}.{media_format}"
 
         if args.language not in language.name_of_ffmpeg_code.keys():
             print("language code is not supported. Run with --list-languages to see all supported languages.")
             sys.exit(1)
 
         if (not ("*" and "?") in str(args.media_filepath)):
             fpath = Path(args.media_filepath)
@@ -1585,20 +1593,20 @@
                     media_type = None
 
             else:
                 not_exist_media_filepaths.append(media_filepaths[0])
                 media_type = None
 
         if invalid_media_filepaths:
-            msg = "{} is not valid video or audio file".format(invalid_media_filepaths[0])
+            msg = f"'{invalid_media_filepaths[0]}' is not valid video or audio file"
             print(msg)
             sys.exit(0)
 
         if not_exist_media_filepaths:
-            msg = "{} is not exist".format(not_exist_media_filepaths[0])
+            msg = f"'{not_exist_media_filepaths[0]}' is not exist"
             print(msg)
             sys.exit(0)
 
         if not media_filepaths and not not_exist_media_filepaths:
             print("No any video file matching filename you typed")
             sys.exit(0)
 
@@ -1643,28 +1651,29 @@
                     valid_subtitle_paths.append(subtitle_paths[0])
                 else:
                     invalid_subtitle_paths.append(subtitle_paths[0])
             else:
                 not_exist_subtitle_paths.append(subtitle_paths[0])
 
         if invalid_subtitle_paths:
-            msg = "{} is not a valid SRT subtitle file".format(invalid_subtitle_paths[0])
+            msg = f"'{invalid_subtitle_paths[0]}' is not a valid SRT subtitle file"
             print(msg)
 
         if not_exist_subtitle_paths:
-            msg = "{} is not exist".format(not_exist_subtitle_paths[0])
+            msg = f"'{not_exist_subtitle_paths[0]}' is not exist"
             print(msg)
 
         if not valid_subtitle_paths and not not_exist_subtitle_paths:
             print("No any SRT subtitle file matching filename you typed")
 
         if media_filepaths and valid_subtitle_paths and output_path:
             base, ext = os.path.splitext(media_filepaths[0])
             ffmpeg_src_language_code = args.language
-            print("Checking %s" %media_filepaths[0])
+
+            print(f"Checking '{media_filepaths[0]}'")
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepaths[0])
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
@@ -1679,15 +1688,15 @@
                     widgets = [f"Embeding \'{language_code}\' subtitles with {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=valid_subtitle_paths[0], language=language_code, output_path=output_path, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     result = subtitle_embedder(media_filepaths[0])
                     pbar.finish()
 
         if result and os.path.isfile(result):
-            print("Subtitles embedded {} created at : {}".format(media_type, output_path))
+            print(f"Subtitles embedded {media_type} created at : '{output_path}'")
 
     else:
         parser.print_help()
         exit(1)
 
 
 if __name__ == '__main__':
```

### Comparing `embedsrt-0.0.3/embedsrt.egg-info/PKG-INFO` & `embedsrt-0.0.4/embedsrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedsrt
-Version: 0.0.3
+Version: 0.0.4
 Summary: a utility for embedding subtitle file into video file
 Home-page: https://github.com/botbahlul/embedsrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `embedsrt-0.0.3/setup.py` & `embedsrt-0.0.4/setup.py`

 * *Files identical despite different names*

