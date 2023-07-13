# Comparing `tmp/pyautosrt-0.2.8.tar.gz` & `tmp/pyautosrt-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.2.8.tar", last modified: Sat Jul  8 05:00:42 2023, max compression
+gzip compressed data, was "pyautosrt-0.2.9.tar", last modified: Thu Jul 13 02:12:12 2023, max compression
```

## Comparing `pyautosrt-0.2.8.tar` & `pyautosrt-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 05:00:42.755149 pyautosrt-0.2.8/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-07-08 05:00:42.755898 pyautosrt-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 05:00:42.717687 pyautosrt-0.2.8/pyautosrt/
--rw-rw-rw-   0        0        0   228323 2023-07-08 05:00:33.000000 pyautosrt-0.2.8/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 05:00:42.750656 pyautosrt-0.2.8/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-07-08 05:00:42.000000 pyautosrt-0.2.8/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-07-08 05:00:42.000000 pyautosrt-0.2.8/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 05:00:42.000000 pyautosrt-0.2.8/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-08 05:00:42.000000 pyautosrt-0.2.8/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-07-08 05:00:42.000000 pyautosrt-0.2.8/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-08 05:00:42.000000 pyautosrt-0.2.8/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-07-08 05:00:42.759644 pyautosrt-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1772 2023-06-19 03:34:35.000000 pyautosrt-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 05:00:42.752902 pyautosrt-0.2.8/test/
--rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.8/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 02:12:12.834764 pyautosrt-0.2.9/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-07-13 02:12:12.835512 pyautosrt-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 02:12:12.767336 pyautosrt-0.2.9/pyautosrt/
+-rw-rw-rw-   0        0        0   228010 2023-07-13 02:10:31.000000 pyautosrt-0.2.9/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 02:12:12.814536 pyautosrt-0.2.9/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-07-13 02:12:12.000000 pyautosrt-0.2.9/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-13 02:12:12.000000 pyautosrt-0.2.9/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 02:12:12.000000 pyautosrt-0.2.9/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-13 02:12:12.000000 pyautosrt-0.2.9/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-07-13 02:12:12.000000 pyautosrt-0.2.9/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-13 02:12:12.000000 pyautosrt-0.2.9/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-13 02:12:12.838510 pyautosrt-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1772 2023-06-19 03:34:35.000000 pyautosrt-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 02:12:12.832514 pyautosrt-0.2.9/test/
+-rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.9/test/__init__.py
```

### Comparing `pyautosrt-0.2.8/LICENSE` & `pyautosrt-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.8/PKG-INFO` & `pyautosrt-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.8
+Version: 0.2.9
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.8/README.md` & `pyautosrt-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.8/pyautosrt/__init__.py` & `pyautosrt-0.2.9/pyautosrt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 #import warnings
 #warnings.filterwarnings("ignore", category=DeprecationWarning)
 #warnings.filterwarnings("ignore", category=RuntimeWarning)
 #sys.tracebacklimit = 0
 
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -795,18 +795,18 @@
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
@@ -1061,27 +1061,27 @@
                 self.error_messages_callback(e)
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
 
     def __call__(self, data):
         try:
             for i in range(self.retries):
-                url = "http://www.google.com/speech-api/v2/recognize?client=chromium&lang={lang}&key={key}".format(lang=self.language, key=self.api_key)
-                headers = {"Content-Type": "audio/x-flac rate=%d" % self.rate}
+                url = f"http://www.google.com/speech-api/v2/recognize?client=chromium&lang={self.language}&key={self.api_key}"
+                headers = {"Content-Type": "audio/x-flac rate=%d" %self.rate}
 
                 try:
                     resp = requests.post(url, data=data, headers=headers, timeout=self.timeout)
                 except requests.exceptions.ConnectionError:
                     try:
                         resp = httpx.post(url, data=data, headers=headers, timeout=self.timeout)
                     except httpx.exceptions.NetworkError:
@@ -1291,15 +1291,15 @@
         try:
             formatter = SubtitleFormatter(self.format)
             formatted_subtitles = formatter(self.timed_subtitles)
             saved_subtitle_filepath = declared_subtitle_filepath
             if saved_subtitle_filepath:
                 subtitle_file_base, subtitle_file_ext = os.path.splitext(saved_subtitle_filepath)
                 if not subtitle_file_ext:
-                    saved_subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format=self.format)
+                    saved_subtitle_filepath = f"{subtitle_file_base}.{self.format}"
                 else:
                     saved_subtitle_filepath = declared_subtitle_filepath
             with open(saved_subtitle_filepath, 'wb') as f:
                 f.write(formatted_subtitles.encode("utf-8"))
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
@@ -1636,18 +1636,18 @@
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
@@ -1823,18 +1823,18 @@
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
@@ -1846,15 +1846,15 @@
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
@@ -1993,18 +1993,18 @@
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
@@ -2212,18 +2212,18 @@
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
 
@@ -2331,17 +2331,14 @@
     
     # Update the window to show the scroll position
     window.refresh()
 
 
 def set_right_click_menu(element, enabled):
     if enabled:
-        #print("element = {}".format(element))
-        #print("enabled = {}".format(enabled))
-
         if isinstance(element, sg.Input):
             widget = element.Widget
         elif isinstance(element, sg.Multiline):
             widget = element.Widget
 
         menu = tk.Menu(widget, tearoff=False)
         menu.add_command(label="Copy", command=lambda: element.Widget.event_generate("<<Copy>>"))
@@ -2375,75 +2372,62 @@
 
 
 def is_streaming_url(url, error_messages_callback=None):
 
     streamlink = Streamlink()
 
     if is_valid_url(url):
-        #print("is_valid_url(url) = {}".format(is_valid_url(url)))
         try:
             os.environ['STREAMLINK_DIR'] = './streamlink/'
             os.environ['STREAMLINK_PLUGINS'] = './streamlink/plugins/'
             os.environ['STREAMLINK_PLUGIN_DIR'] = './streamlink/plugins/'
 
             streams = streamlink.streams(url)
             if streams:
-                #print("is_streams = {}".format(True))
                 return True
             else:
-                #print("is_streams = {}".format(False))
                 return False
 
         except OSError:
-            #print("is_streams = OSError")
             if error_messages_callback:
                 error_messages_callback("OSError")
             return False
         except ValueError:
-            #print("is_streams = ValueError")
             if error_messages_callback:
                 error_messages_callback("ValueError")
             return False
         except KeyError:
-            #print("is_streams = KeyError")
             if error_messages_callback:
                 error_messages_callback("KeyError")
             return False
         except RuntimeError:
-            #print("is_streams = RuntimeError")
             if error_messages_callback:
                 error_messages_callback("RuntimeError")
             return False
         except NoPluginError:
-            #print("is_streams = NoPluginError")
             if error_messages_callback:
                 error_messages_callback("NoPluginError")
             return False
         except StreamlinkError:
             return False
-            #print("is_streams = StreamlinkError")
             if error_messages_callback:
                 error_messages_callback("StreamlinkError")
         except StreamError:
             return False
-            #print("is_streams = StreamlinkError")
             if error_messages_callback:
                 error_messages_callback("StreamError")
         except NotImplementedError:
-            #print("is_streams = NotImplementedError")
             if error_messages_callback:
                 error_messages_callback("NotImplementedError")
             return False
         except Exception as e:
-            #print("is_streams = {}".format(e))
             if error_messages_callback:
                 error_messages_callback(e)
             return False
     else:
-        #print("is_valid_url(url) = {}".format(is_valid_url(url)))
         return False
 
 
 def is_valid_url(url, error_messages_callback=None):
     try:
         response = httpx.head(url)
         response.raise_for_status()
@@ -2564,32 +2548,32 @@
 
                 if time_str:
                     time_value = time_str.group(1)
                     #print(f"Time: {time_value}")
 
                     if i == 0:
                         ffmpeg_start_write_time = datetime.now()
-                        #print("ffmpeg_start_write_time = {}".format(ffmpeg_start_write_time))
+                        #print(f"ffmpeg_start_write_time = {ffmpeg_start_write_time}")
 
                         first_streaming_duration_recorded = datetime.strptime(str(time_value), "%H:%M:%S.%f") - datetime(1900, 1, 1)
-                        #print("first_streaming_duration_recorded = {}".format(first_streaming_duration_recorded))
+                        #print(f"first_streaming_duration_recorded = {first_streaming_duration_recorded}")
 
                         # MAKE SURE THAT first_streaming_duration_recorded EXECUTED ONLY ONCE
                         i += 1
 
                         #print("writing time_value")
                         time_value_filename = "time_value"
                         time_value_filepath = os.path.join(tempfile.gettempdir(), time_value_filename)
                         time_value_file = open(time_value_filepath, "w")
                         time_value_file.write(str(time_value))
                         time_value_file.close()
-                        #print("time_value = {}".format(time_value))
+                        #print(f"time_value = {time_value}")
 
                     streaming_duration_recorded = datetime.strptime(str(time_value), "%H:%M:%S.%f") - datetime(1900, 1, 1)
-                    #print("streaming_duration_recorded = {}".format(streaming_duration_recorded))
+                    #print(f"streaming_duration_recorded = {streaming_duration_recorded}")
                     main_window.write_event_value('-EVENT-STREAMING-DURATION-RECORDED-', streaming_duration_recorded)
 
                 # Restart the timer to check for new output
                 timer.cancel()
                 timer = Timer(timeout, lambda: None)
                 if not not_recording: timer.start()
 
@@ -3046,18 +3030,23 @@
                                     pool[media_filepath] = None
                                 return
 
                             ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
 
                             base, ext = os.path.splitext(media_filepath)
 
-                            src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
+                            if ext[1:] == "ts":
+                                media_format = "mp4"
+                            else:
+                                media_format = ext[1:]
+
+                            src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
                             src_tmp_embedded_media_file_display_name = os.path.basename(src_tmp_embedded_media_filepath).split('/')[-1]
 
-                            src_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
+                            src_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
                             src_embedded_media_file_display_name = os.path.basename(src_embedded_media_filepath).split('/')[-1]
 
                             window_key = '-PROGRESS-LOG-'
                             msg = f"Embedding '{ffmpeg_src_language_code}' subtitles file '{src_subtitle_file_display_name}' into '{media_file_display_name}'"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
@@ -3234,18 +3223,23 @@
                                     pool[media_filepath] = None
                                 return
 
                             ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
 
                             base, ext = os.path.splitext(media_filepath)
 
-                            dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                            if ext[1:] == "ts":
+                                media_format = "mp4"
+                            else:
+                                media_format = ext[1:]
+
+                            dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
                             dst_tmp_embedded_media_file_display_name = os.path.basename(dst_tmp_embedded_media_filepath).split('/')[-1]
 
-                            dst_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
+                            dst_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
                             dst_embedded_media_file_display_name = os.path.basename(dst_embedded_media_filepath).split('/')[-1]
 
                             window_key = '-PROGRESS-LOG-'
                             msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles file '{dst_subtitle_file_display_name}' into '{media_file_display_name}'"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
@@ -3718,30 +3712,35 @@
 
                 # EMBEDDING subtitles file
                 ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
                 ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
 
                 base, ext = os.path.splitext(media_filepath)
 
-                src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
+                if ext[1:] == "ts":
+                    media_format = "mp4"
+                else:
+                    media_format = ext[1:]
+
+                src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
                 src_tmp_embedded_media_file_display_name = os.path.basename(src_tmp_embedded_media_filepath).split('/')[-1]
 
-                dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
                 dst_tmp_embedded_media_file_display_name = os.path.basename(dst_tmp_embedded_media_filepath).split('/')[-1]
 
-                src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
                 src_dst_tmp_embedded_media_file_display_name = os.path.basename(src_dst_tmp_embedded_media_filepath).split('/')[-1]
 
-                src_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
+                src_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
                 src_embedded_media_file_display_name = os.path.basename(src_embedded_media_filepath).split('/')[-1]
 
-                dst_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
+                dst_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
                 dst_embedded_media_file_display_name = os.path.basename(dst_embedded_media_filepath).split('/')[-1]
 
-                src_dst_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
+                src_dst_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{media_format}"
                 src_dst_embedded_media_file_display_name = os.path.basename(src_dst_embedded_media_filepath).split('/')[-1]
                 
 
                 if is_same_language(src, dst, error_messages_callback=show_error_messages):
 
                     if embed_src == True:
                         try:
@@ -4136,15 +4135,15 @@
     parser.add_argument('-v', '--version', action='version', version=VERSION)
 
     args = parser.parse_args()
 
     if args.list_formats:
         print("Supported subtitle formats :")
         for subtitle_format in SubtitleFormatter.supported_formats:
-            print("{format}".format(format=subtitle_format))
+            print(f"{subtitle_format}")
         parser.exit(0)
 
     if args.list_languages:
         print("Supported languages :")
         for code, language in sorted(language.name_of_code.items()):
             print("%-8s : %s" %(code, language))
         parser.exit(0)
@@ -4825,19 +4824,19 @@
                             msg = "Invalid URL, please enter a valid URL"
                             sg.Popup(msg, title="Info", line_width=50, any_key_closes=True)
                             not_recording = True
                             main_window['-RECORD-STREAMING-'].update(('Stop Record Streaming','Start Record Streaming')[not_recording], button_color=(('white', ('red', '#283b5b')[not_recording])))
 
                     else:
                         if sys.platform == "win32":
-                            #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
+                            #print(f"thread_record_streaming.is_alive() = {thread_record_streaming.is_alive()}")
                             stop_record_streaming_windows()
 
                         elif sys.platform == "linux":
-                            #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
+                            #print(f"thread_record_streaming.is_alive() = {thread_record_streaming.is_alive()}")
                             stop_record_streaming_linux()
 
 
         elif event == '-SAVE-RECORDED-STREAMING-':
 
             tmp_recorded_streaming_filename = "record.mp4"
             tmp_recorded_streaming_filepath = os.path.join(tempfile.gettempdir(), tmp_recorded_streaming_filename)
@@ -4851,16 +4850,16 @@
 
             else:
                 sg.set_options(font=FONT)
                 msg = "No streaming was recorded"
                 sg.Popup(msg, title="Info", line_width=50, any_key_closes=True)
 
 
-        #print("event = {}".format(event))
-        #print("values = {}".format(values))
+        #print(f"event = {event}")
+        #print(f"values = {values}")
 
     if thread_transcribe and thread_transcribe.is_alive():
         stop_thread(thread_transcribe)
 
     if thread_transcribe_starter and thread_transcribe_starter.is_alive():
         stop_thread(thread_transcribe_starter)
```

### Comparing `pyautosrt-0.2.8/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.2.9/pyautosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.8
+Version: 0.2.9
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.8/setup.py` & `pyautosrt-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.8/test/__init__.py` & `pyautosrt-0.2.9/test/__init__.py`

 * *Files identical despite different names*

