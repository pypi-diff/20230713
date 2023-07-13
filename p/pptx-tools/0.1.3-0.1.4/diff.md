# Comparing `tmp/pptx-tools-0.1.3.tar.gz` & `tmp/pptx-tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx-tools-0.1.3.tar", last modified: Tue Jul 11 08:59:23 2023, max compression
+gzip compressed data, was "pptx-tools-0.1.4.tar", last modified: Thu Jul 13 01:56:42 2023, max compression
```

## Comparing `pptx-tools-0.1.3.tar` & `pptx-tools-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.742346 pptx-tools-0.1.3/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/pptx_tools/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/apps/slide_add_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/audio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/pptx_tools/data/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/data/hello.pptx
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/data/transparent.png
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/slide_transition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/pptx_tools/tts/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/azure_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/azure_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/google_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/google_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/pptx_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/tests/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/tests/pptx_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/tests/pptx_tools/test_slide_add_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/apps/slide_add_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/audio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/data/hello.pptx
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/data/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/slide_transition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools/tts/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/azure_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/azure_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/google_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/tts/google_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/pptx_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/pptx_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-13 01:56:42.000000 pptx-tools-0.1.4/pptx_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:42.375689 pptx-tools-0.1.4/tests/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/tests/pptx_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-13 01:56:32.000000 pptx-tools-0.1.4/tests/pptx_tools/test_slide_add_voice.py
```

### Comparing `pptx-tools-0.1.3/LICENSE` & `pptx-tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/pptx_tools/apps/slide_add_voice.py` & `pptx-tools-0.1.4/pptx_tools/apps/slide_add_voice.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 import argparse
 from pathlib import Path
 import sys
 
 from eos import make_fancy_output_dir
 import termcolor
 
-from pptx_tools.tts.azure_tts_voice import \
-    voice_name_to_language_code as azure_voice
-from pptx_tools.tts.google_tts_voice import \
-    voice_name_to_language_code as google_voice
 from pptx_tools.utils import add_synthesize_audio
 
 
 def main():
     tts_engines = ['google', 'azure']
     parser = argparse.ArgumentParser(description='Add voice to presentation.')
     parser.add_argument("input", help="The input pptx file.")
@@ -26,24 +22,30 @@
                         default='google',
                         help='select the text-to-speech engine. '
                         'You can choose {}.'.format(tts_engines))
     parser.add_argument("--slide-duration-offset", type=float,
                         default=1.0)
     args = parser.parse_args()
     if args.voice_name is not None:
-        if args.tts == 'google' and args.voice_name not in google_voice:
-            print('Invalid voice_name. Avaliable voices are:')
-            print([voice for voice in google_voice.keys()])
-            print("You can check the sample audio here: "
-                  "https://cloud.google.com/text-to-speech/docs/voices")
-            sys.exit(0)
-        elif args.tts == 'azure' and args.voice_name not in azure_voice:
-            print('Invalid voice_name. Avaliable voices are:')
-            print([voice for voice in azure_voice.keys()])
-            sys.exit(0)
+        if args.tts == 'google':
+            from pptx_tools.tts.google_tts_voice import \
+                voice_name_to_language_code as google_voice
+            if args.voice_name not in google_voice:
+                print('Invalid voice_name. Avaliable voices are:')
+                print([voice for voice in google_voice.keys()])
+                print("You can check the sample audio here: "
+                      "https://cloud.google.com/text-to-speech/docs/voices")
+                sys.exit(0)
+        elif args.tts == 'azure':
+            from pptx_tools.tts.azure_tts_voice import \
+                voice_name_to_language_code as azure_voice
+            if args.voice_name not in azure_voice:
+                print('Invalid voice_name. Avaliable voices are:')
+                print([voice for voice in azure_voice.keys()])
+                sys.exit(0)
     output_dir = Path(make_fancy_output_dir(
         args.out, no_save=True))
     output_slide_path = add_synthesize_audio(
         args.input, output_dir, voice_name=args.voice_name,
         slide_duration_offset=args.slide_duration_offset)
     termcolor.cprint('=> Saved to {}'.format(output_slide_path), 'green')
```

### Comparing `pptx-tools-0.1.3/pptx_tools/data/hello.pptx` & `pptx-tools-0.1.4/pptx_tools/data/hello.pptx`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/pptx_tools/slide_transition.py` & `pptx-tools-0.1.4/pptx_tools/slide_transition.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/pptx_tools/tts/azure_tts.py` & `pptx-tools-0.1.4/pptx_tools/tts/azure_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/pptx_tools/tts/azure_tts_voice.py` & `pptx-tools-0.1.4/pptx_tools/tts/azure_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/pptx_tools/tts/google_tts.py` & `pptx-tools-0.1.4/pptx_tools/tts/google_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/pptx_tools/tts/google_tts_voice.py` & `pptx-tools-0.1.4/pptx_tools/tts/google_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/pptx_tools/utils.py` & `pptx-tools-0.1.4/pptx_tools/utils.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/pptx_tools.egg-info/SOURCES.txt` & `pptx-tools-0.1.4/pptx_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.3/setup.py` & `pptx-tools-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "0.1.3"
+version = "0.1.4"
 
 
 if sys.argv[-1] == "release":
     # Release via github-actions.
     commands = [
         'git tag v{:s}'.format(version),
         'git push origin master --tag',
@@ -39,14 +39,21 @@
 
 with open('requirements.txt') as f:
     install_requires = []
     for line in f:
         req = line.split('#')[0].strip()
         install_requires.append(req)
 
+azure_install_requires = []
+with open('requirements_azure.txt') as f:
+    azure_install_requires = []
+    for line in f:
+        req = line.split('#')[0].strip()
+        azure_install_requires.append(req)
+
 setup(
     name="pptx-tools",
     version=version,
     description="A power point tools",
     author="iory",
     author_email="ab.ioryz@gmail.com",
     url="https://github.com/iory/pptx-tools",
@@ -65,13 +72,18 @@
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=find_packages(),
     package_data={'pptx_tools': listup_package_data()},
     zip_safe=False,
     setup_requires=setup_requires,
     install_requires=install_requires,
+    extras_require={
+        'azure': azure_install_requires,
+        'all': (install_requires
+                + azure_install_requires),
+    },
     entry_points={
         "console_scripts": [
             "slide-add-voice=pptx_tools.apps.slide_add_voice:main",
         ]
     },
 )
```

### Comparing `pptx-tools-0.1.3/tests/pptx_tools/test_slide_add_voice.py` & `pptx-tools-0.1.4/tests/pptx_tools/test_slide_add_voice.py`

 * *Files identical despite different names*

