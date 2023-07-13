# Comparing `tmp/pptx-tools-0.1.4.tar.gz` & `tmp/pptx-tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx-tools-0.1.4.tar", last modified: Thu Jul 13 01:56:42 2023, max compression
+gzip compressed data, was "pptx-tools-0.1.5.tar", last modified: Thu Jul 13 04:47:10 2023, max compression
```

## Comparing `pptx-tools-0.1.4.tar` & `pptx-tools-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/apps/slide_add_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/audio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools/data/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/data/hello.pptx
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/data/transparent.png
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/slide_transition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools/tts/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/azure_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/azure_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/google_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/google_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/tests/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/tests/pptx_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/tests/pptx_tools/test_slide_add_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-13 04:47:10.209297 pptx-tools-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/apps/slide_add_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/audio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/data/hello.pptx
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/data/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/slide_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/slide_transition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools/tts/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/azure_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/azure_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/google_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/google_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/video_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-13 04:47:10.209297 pptx-tools-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/tests/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/tests/pptx_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/tests/pptx_tools/test_slide_add_voice.py
```

### Comparing `pptx-tools-0.1.4/LICENSE` & `pptx-tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/PKG-INFO` & `pptx-tools-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: A power point tools
 Home-page: https://github.com/iory/pptx-tools
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pptx-tools-0.1.4/README.md` & `pptx-tools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/pptx_tools/apps/slide_add_voice.py` & `pptx-tools-0.1.5/pptx_tools/apps/slide_add_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/pptx_tools/data/hello.pptx` & `pptx-tools-0.1.5/pptx_tools/data/hello.pptx`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/pptx_tools/slide_transition.py` & `pptx-tools-0.1.5/pptx_tools/slide_transition.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/pptx_tools/tts/azure_tts.py` & `pptx-tools-0.1.5/pptx_tools/tts/azure_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/pptx_tools/tts/azure_tts_voice.py` & `pptx-tools-0.1.5/pptx_tools/tts/azure_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/pptx_tools/tts/google_tts.py` & `pptx-tools-0.1.5/pptx_tools/tts/google_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/pptx_tools/tts/google_tts_voice.py` & `pptx-tools-0.1.5/pptx_tools/tts/google_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.4/pptx_tools/utils.py` & `pptx-tools-0.1.5/pptx_tools/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from lxml import etree
 from pptx import Presentation
 from pptx.util import Inches
 from tqdm import tqdm
 
 from pptx_tools.audio_utils import get_wave_duration
 from pptx_tools.data import get_transparent_img_path
+from pptx_tools.slide_info import get_slide_infos
+from pptx_tools.slide_info import slide_info_to_dict
 from pptx_tools.slide_transition import set_slide_duration
+from pptx_tools.video_utils import add_video_duration
+from pptx_tools.video_utils import max_video_duration
 
 
 base_logger = logging.getLogger(__name__)
 
 
 def xpath(el, query):
     nsmap = {'p': 'http://schemas.openxmlformats.org/presentationml/2006/main'}
@@ -51,14 +55,18 @@
     else:
         raise ValueError("Not supported tts {}".format(tts))
 
     output_path = Path(outdir)
     makedirs(output_path)
 
     presentation = Presentation(slide_path)
+    slide_infos = get_slide_infos(presentation)
+    add_video_duration(slide_path, slide_infos)
+    slide_info_dict = slide_info_to_dict(slide_infos)
+
     total_time = 0.0
     for page, slide in tqdm(enumerate(presentation.slides, start=1),
                             total=len(presentation.slides)):
         if slide.has_notes_slide and slide.notes_slide.notes_text_frame.text:
             note_txt = slide.notes_slide.notes_text_frame.text
             note_txt = note_txt.replace('\n', ' ')
             wave_path = output_path / '{}.wav'.format(page)
@@ -82,14 +90,16 @@
                     elif tts == 'azure':
                         voice_name = 'ja-JP-NanamiNeural'
                     else:
                         raise RuntimeError('invalid tts')
             text_to_speech(wave_path, note_txt,
                            voice_name=voice_name)
             duration = get_wave_duration(wave_path)
+            video_duration = max_video_duration(slide_info_dict[page])
+            duration = max(duration, video_duration)
             set_slide_duration(slide, duration + slide_duration_offset)
             total_time += duration + slide_duration_offset
             try:
                 movie = slide.shapes.add_movie(
                     str(wave_path),
                     Inches(0), Inches(0), Inches(1.0), Inches(1.0),
                     poster_frame_image=str(get_transparent_img_path()),
```

### Comparing `pptx-tools-0.1.4/pptx_tools.egg-info/PKG-INFO` & `pptx-tools-0.1.5/pptx_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: A power point tools
 Home-page: https://github.com/iory/pptx-tools
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pptx-tools-0.1.4/pptx_tools.egg-info/SOURCES.txt` & `pptx-tools-0.1.5/pptx_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 pptx_tools/__init__.py
 pptx_tools/audio_utils.py
+pptx_tools/slide_info.py
 pptx_tools/slide_transition.py
 pptx_tools/utils.py
+pptx_tools/video_utils.py
 pptx_tools.egg-info/PKG-INFO
 pptx_tools.egg-info/SOURCES.txt
 pptx_tools.egg-info/dependency_links.txt
 pptx_tools.egg-info/entry_points.txt
 pptx_tools.egg-info/not-zip-safe
 pptx_tools.egg-info/requires.txt
 pptx_tools.egg-info/top_level.txt
```

### Comparing `pptx-tools-0.1.4/setup.py` & `pptx-tools-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "0.1.4"
+version = "0.1.5"
 
 
 if sys.argv[-1] == "release":
     # Release via github-actions.
     commands = [
         'git tag v{:s}'.format(version),
         'git push origin master --tag',
```

### Comparing `pptx-tools-0.1.4/tests/pptx_tools/test_slide_add_voice.py` & `pptx-tools-0.1.5/tests/pptx_tools/test_slide_add_voice.py`

 * *Files identical despite different names*

