# Comparing `tmp/autosrt-1.4.4.tar.gz` & `tmp/autosrt-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.4.4.tar", last modified: Sat Jul  8 03:55:41 2023, max compression
+gzip compressed data, was "autosrt-1.4.5.tar", last modified: Wed Jul 12 21:17:21 2023, max compression
```

## Comparing `autosrt-1.4.4.tar` & `autosrt-1.4.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 03:55:41.184198 autosrt-1.4.4/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.4/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-07-08 03:55:41.184947 autosrt-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 03:55:40.895872 autosrt-1.4.4/autosrt/
--rw-rw-rw-   0        0        0   162921 2023-07-08 03:55:07.000000 autosrt-1.4.4/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:55:40.964839 autosrt-1.4.4/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-07-08 03:55:41.203678 autosrt-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:55:41.180452 autosrt-1.4.4/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.4/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.4/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.4/test/test3.py
--rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.4/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:17:21.800546 autosrt-1.4.5/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-07-12 21:17:21.801299 autosrt-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 21:17:21.759583 autosrt-1.4.5/autosrt/
+-rw-rw-rw-   0        0        0   163100 2023-07-12 21:17:04.000000 autosrt-1.4.5/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:17:21.784065 autosrt-1.4.5/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-07-12 21:17:21.000000 autosrt-1.4.5/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-12 21:17:21.000000 autosrt-1.4.5/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 21:17:21.000000 autosrt-1.4.5/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-12 21:17:21.000000 autosrt-1.4.5/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-07-12 21:17:21.000000 autosrt-1.4.5/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 21:17:21.000000 autosrt-1.4.5/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-12 21:17:21.805043 autosrt-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:17:21.799049 autosrt-1.4.5/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.5/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.5/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.5/test/test3.py
+-rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.5/test/test4.py
```

### Comparing `autosrt-1.4.4/LICENSE` & `autosrt-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.4/PKG-INFO` & `autosrt-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.4
+Version: 1.4.5
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.4/README.md` & `autosrt-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.4/autosrt/__init__.py` & `autosrt-1.4.5/autosrt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
 import shlex
 import shutil
 
 
-VERSION = "1.4.4"
+VERSION = "1.4.5"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -956,15 +956,15 @@
                 self.error_messages_callback("Cancelling all tasks")
             else:
                 print("Cancelling all tasks")
             return
 
         except Exception as e:
             if self.error_messages_callback:
-                self.error_messages_callback(e)
+                self.error_messages_callback(f"SpeechRegionFinder: {e}")
             else:
                 print(e)
             return
 
 
 class FLACConverter(object):
     def which(self, program):
@@ -1040,22 +1040,22 @@
                 self.error_messages_callback("Cancelling all tasks")
             else:
                 print("Cancelling all tasks")
             return
 
         except Exception as e:
             if self.error_messages_callback:
-                self.error_messages_callback(e)
+                self.error_messages_callback(f"FLACConverter: {e}")
             else:
                 print(e)
             return
 
 
 class SpeechRecognizer(object):
-    def __init__(self, language="en", rate=44100, retries=3, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", timeout=30, error_messages_callback=None):
+    def __init__(self, language="en", rate=48000, retries=3, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", timeout=30, error_messages_callback=None):
         self.language = language
         self.rate = rate
         self.api_key = api_key
         self.retries = retries
         self.timeout = timeout
         self.error_messages_callback = error_messages_callback
 
@@ -2857,14 +2857,15 @@
     else:
         stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
     remove_temp_files("flac", error_messages_callback=show_error_messages)
     remove_temp_files("wav", error_messages_callback=show_error_messages)
 
     parser = argparse.ArgumentParser()
+
     parser.add_argument('source_path', help="Path to the media files to generate subtitles files (use wildcard for multiple files or separate them with a space character e.g. \"file 1.mp4\" \"file 2.mp4\")", nargs='*')
     parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in media file source_path", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-ll', '--list-languages', help="List all supported languages", action='store_true')
     parser.add_argument('-F', '--format', help="Desired subtitles file format", default="srt")
     parser.add_argument('-lf', '--list-formats', help="List all supported subtitles file formats", action='store_true')
     parser.add_argument('-C', '--concurrency', help="Number of concurrent API requests to make", type=int, default=10)
@@ -2876,16 +2877,14 @@
     args = parser.parse_args()
 
     language = Language()
 
     if args.list_languages:
         print("List of supported languages:")
         for code, language in sorted(language.name_of_code.items()):
-            #print("{code}\t{language}".format(code=code, language=language))
-            #print("%8s\t%s" %(code, language))
             print("%-8s : %s" %(code, language))
         return 0
 
     #if args.src_language not in language.dict:
     if args.src_language not in language.name_of_code.keys():
         print("Source language is not supported. Run with --list-languages to see all supported languages.")
         return 1
@@ -2919,14 +2918,15 @@
     completed_tasks = 0
     media_filepaths = []
     arg_filepaths = []
     invalid_media_filepaths = []
     not_exist_filepaths = []
     argpath = None
     media_type = None
+    media_format = None
 
     #for arg in args.source_path:
     #    print("escape(arg) = %s" %(escape(arg)))
 
     args_source_path = args.source_path
 
     if (not "*" in str(args_source_path)) and (not "?" in str(args_source_path)):
@@ -3159,42 +3159,48 @@
 
                             base, ext = os.path.splitext(media_filepath)
                             src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
 
                             translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             translation_writer.write(src_subtitle_filepath)
 
-                            print("Translated subtitles file saved as      : {}" .format(src_subtitle_filepath))
+                            print(f"Translated subtitles file saved as      : '{src_subtitle_filepath}'")
 
                             # remove media_filepath from transcribe proceed_list because all needed srt files already saved
                             if args.force_recognize == False:
                                 if media_filepath not in removed_media_filepaths:
                                     removed_media_filepaths.append(media_filepath)
 
                             # if args.embed_src is True then we embed the translated srt into media_filepath
                             if args.embed_src == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
 
                                 ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
                                 base, ext = os.path.splitext(media_filepath)
-                                src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                                embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+
+                                if ext[1:] == "ts":
+                                    media_format = "mp4"
+                                else:
+                                    media_format = ext[1:]
+
+                                src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                                embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
                                 widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                 pbar = ProgressBar(widgets=widgets, maxval=100).start()
                                 subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                 src_tmp_output = subtitle_embedder(media_filepath)
                                 pbar.finish()
 
                                 if os.path.isfile(src_tmp_output):
                                     shutil.copy(src_tmp_output, embedded_media_filepath)
                                     os.remove(src_tmp_output)
 
                                 if os.path.isfile(embedded_media_filepath):
-                                    print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                                    print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
 
                             # if args.embed_dst is True we can't embed it because dst subtitles stream already exist
                             if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                                 print(f"No need to embed '{ffmpeg_dst_language_code}' subtitles stream because it's already existed")
 
                     # ffmpeg_src_language_code subtitles stream = exist,
                     # ffmpeg_dst_language_code subtitles stream = not exist
@@ -3211,20 +3217,20 @@
                             translated_subtitle_stream_transcripts = []
                             for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
                                 translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
                                 pbar.update(i)
                             pbar.finish()
 
                             base, ext = os.path.splitext(media_filepath)
-                            dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
+                            dst_subtitle_filepath = f"{base}.{args.dst_language}.{subtitle_format}"
 
                             translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             translation_writer.write(dst_subtitle_filepath)
 
-                            print("Translated subtitles file saved as      : {}" .format(dst_subtitle_filepath))
+                            print(f"Translated subtitles file saved as      : '{dst_subtitle_filepath}'")
 
                             # remove media_filepath from transcribe proceed_list because all needed srt files already saved
                             if args.force_recognize == False:
                                 if media_filepath not in removed_media_filepaths:
                                     removed_media_filepaths.append(media_filepath)
 
                             # if args.embed_src is True we can't embed it because dst subtitles stream already exist
@@ -3233,29 +3239,35 @@
 
                             # if args.embed_dst is True then we embed that translated srt into media_filepath
                             if args.embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
 
                                 ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
                                 base, ext = os.path.splitext(media_filepath)
-                                dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
-                                embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                                if ext[1:] == "ts":
+                                    media_format = "mp4"
+                                else:
+                                    media_format = ext[1:]
+
+                                dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                                embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
                                 widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                 pbar = ProgressBar(widgets=widgets, maxval=100).start()
                                 subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                 dst_tmp_output = subtitle_embedder(media_filepath)
                                 pbar.finish()
 
                                 if os.path.isfile(dst_tmp_output):
                                     shutil.copy(dst_tmp_output, embedded_media_filepath)
                                     os.remove(dst_tmp_output)
 
                                 if os.path.isfile(embedded_media_filepath):
-                                    print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                                    print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
 
                     # ffmpeg_dst_language_code subtitles stream = exist
                     # ffmpeg_src_language_code subtitles stream = exist
                     # remove media_filepath from proceed list
                     elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
                         # remove media_filepath from transcribe proceed_list because all needed srt files already saved
@@ -3297,42 +3309,40 @@
     print("=========================================================================================================")
 
     proceed_list = []
     # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to proceed with transcribe
     if args.force_recognize == True:
         for media_filepath in media_filepaths:
             base, ext = os.path.splitext(media_filepath)
-            tmp_subtitle_removed_media_filepath = "{base}.tmp.subtitles.removed.media_filepath.{format}".format(base=base, format=ext[1:])
-            subtitle_removed_media_filepath = "{base}.force.recognize.{format}".format(base=base, format=ext[1:])
-
-            #src_tmp_output = remove_subtitles_from_media(media_filepath, tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+            tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{ext[1:]}"
+            subtitle_removed_media_filepath = f"{base}.force.recognize.{ext[1:]}"
 
             widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
             tmp_output = subtitle_remover(media_filepath)
             pbar.finish()
 
             if os.path.isfile(tmp_output):
                 shutil.copy(tmp_output, subtitle_removed_media_filepath)
                 os.remove(tmp_output)
 
                 proceed_list.append(subtitle_removed_media_filepath)
 
-            print("Subtitle removed {} file saved as    : {}".format(media_type, subtitle_removed_media_filepath))
+            print(f"Subtitle removed {media_type} file saved as    : '{subtitle_removed_media_filepath}'")
             print("")
 
     # if args.force_recognize is false then we just use modified media_filepaths list
     else:
         proceed_list = media_filepaths
 
 
     # START THE TRANSCRIBE PROCESS
     for media_filepath in proceed_list:
-        print("Processing {}".format(media_filepath))
+        print(f"Processing {media_filepath}")
 
         try:
             widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
             wav_filepath, sample_rate = wav_converter(media_filepath)
             pbar.finish()
@@ -3386,59 +3396,71 @@
                     translated_subtitles = []
                     for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
                         translated_subtitles.append(translated_subtitle)
                         pbar.update(i)
                     pbar.finish()
 
                     base, ext = os.path.splitext(media_filepath)
-                    dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
+                    dst_subtitle_filepath = f"{base}.{args.dst_language}.{subtitle_format}"
                     translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
                     translation_writer.write(dst_subtitle_filepath)
 
                 if do_translate == True:
-                    print("Original subtitles file saved as        : {}".format(src_subtitle_filepath))
-                    print("Translated subtitles file saved as      : {}" .format(dst_subtitle_filepath))
+                    print(f"Original subtitles file saved as        : '{src_subtitle_filepath}'")
+                    print(f"Translated subtitles file saved as      : '{dst_subtitle_filepath}'")
                 else:
-                    print("Subtitles file saved as                 : {}".format(src_subtitle_filepath))
+                    print(f"Subtitles file saved as                 : '{src_subtitle_filepath}'")
 
 
                 # EMBEDDING SUBTITLES FILE
                 embedded_media_filepath = None
                 if do_translate == False:
 
                     if args.embed_src == True:
 
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
                         base, ext = os.path.splitext(media_filepath)
-                        src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                        embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+
+                        if ext[1:] == "ts":
+                            media_format = "mp4"
+                        else:
+                            media_format = ext[1:]
+
+                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
                         widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         src_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if os.path.isfile(src_tmp_output):
                             shutil.copy(src_tmp_output, embedded_media_filepath)
                             os.remove(src_tmp_output)
-                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                            print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
 
                 elif do_translate == True:
 
                     if args.embed_src == True and args.embed_dst == True:
 
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
                         ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
                         base, ext = os.path.splitext(media_filepath)
-                        src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                        src_dst_tmp_embedded_media_filepath = "{base}.{src}.{dst}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
-                        embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                        if ext[1:] == "ts":
+                            media_format = "mp4"
+                        else:
+                            media_format = ext[1:]
+
+                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                        src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
                         '''
                         # USING FUNCTION
                         src_tmp_output = embed_subtitle_into_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, src_tmp_embedded_media_filepath)
                         if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
                             src_dst_tmp_output = embed_subtitle_into_media(src_tmp_embedded_media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, src_dst_tmp_embedded_media_filepath)
                         '''
@@ -3457,62 +3479,74 @@
                             subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                             src_dst_tmp_output = subtitle_embedder(src_tmp_output)
                             pbar.finish()
 
 
                         if os.path.isfile(src_dst_tmp_output):
                             shutil.copy(src_dst_tmp_output, embedded_media_filepath)
-                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                            print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
                         else:
                             print("Unknown error!")
 
                         if os.path.isfile(src_dst_tmp_output):
                             os.remove(src_dst_tmp_output)
                         if os.path.isfile(src_tmp_output):
                             os.remove(src_tmp_output)
 
                     elif args.embed_src == True and args.embed_dst == False:
 
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
                         base, ext = os.path.splitext(media_filepath)
-                        src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                        embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+
+                        if ext[1:] == "ts":
+                            media_format = "mp4"
+                        else:
+                            media_format = ext[1:]
+
+                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
                         widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         src_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if os.path.isfile(src_tmp_output):
                             shutil.copy(src_tmp_output, embedded_media_filepath)
                             os.remove(src_tmp_embedded_media_filepath)
-                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                            print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
                         else:
                             print("Unknown error!")
 
                     elif args.embed_src == False and args.embed_dst == True:
 
                         ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
                         base, ext = os.path.splitext(media_filepath)
-                        dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
-                        embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                        if ext[1:] == "ts":
+                            media_format = "mp4"
+                        else:
+                            media_format = ext[1:]
+
+                        dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                        embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
                         widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         dst_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if os.path.isfile(dst_tmp_output):
                             shutil.copy(dst_tmp_output, embedded_media_filepath)
                             os.remove(dst_tmp_output)
-                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                            print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
                         else:
                             print("Unknown error!")
 
                 if do_translate == False:
                     if args.embed_src == True:
                         if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
                             completed_tasks += 1
```

### Comparing `autosrt-1.4.4/autosrt.egg-info/PKG-INFO` & `autosrt-1.4.5/autosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.4
+Version: 1.4.5
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.4/setup.py` & `autosrt-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.4/test/test1.py` & `autosrt-1.4.5/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.4/test/test2.py` & `autosrt-1.4.5/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.4/test/test3.py` & `autosrt-1.4.5/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.4/test/test4.py` & `autosrt-1.4.5/test/test4.py`

 * *Files identical despite different names*

