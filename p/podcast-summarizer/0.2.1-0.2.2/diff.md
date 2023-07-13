# Comparing `tmp/podcast_summarizer-0.2.1.tar.gz` & `tmp/podcast_summarizer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_summarizer-0.2.1.tar", max compression
+gzip compressed data, was "podcast_summarizer-0.2.2.tar", max compression
```

## Comparing `podcast_summarizer-0.2.1.tar` & `podcast_summarizer-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-07-13 00:12:43.694813 podcast_summarizer-0.2.1/LICENSE
--rw-r--r--   0        0        0     1576 2023-07-13 03:18:53.377475 podcast_summarizer-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-13 00:45:08.553711 podcast_summarizer-0.2.1/podcast_summarizer/__init__.py
--rw-r--r--   0        0        0     3198 2023-07-13 04:56:11.430038 podcast_summarizer-0.2.1/podcast_summarizer/cli.py
--rw-r--r--   0        0        0     1444 2023-07-13 04:51:36.636030 podcast_summarizer-0.2.1/podcast_summarizer/summarizer.py
--rw-r--r--   0        0        0     2128 2023-07-13 04:52:50.401284 podcast_summarizer-0.2.1/podcast_summarizer/youtube.py
--rw-r--r--   0        0        0      571 2023-07-13 04:58:32.488308 podcast_summarizer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2321 1970-01-01 00:00:00.000000 podcast_summarizer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-13 00:12:43.694813 podcast_summarizer-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1576 2023-07-13 03:18:53.377475 podcast_summarizer-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 00:45:08.553711 podcast_summarizer-0.2.2/podcast_summarizer/__init__.py
+-rw-r--r--   0        0        0     3248 2023-07-13 05:02:00.774617 podcast_summarizer-0.2.2/podcast_summarizer/cli.py
+-rw-r--r--   0        0        0     1444 2023-07-13 05:01:26.228320 podcast_summarizer-0.2.2/podcast_summarizer/summarizer.py
+-rw-r--r--   0        0        0     2128 2023-07-13 04:52:50.401284 podcast_summarizer-0.2.2/podcast_summarizer/youtube.py
+-rw-r--r--   0        0        0      571 2023-07-13 05:01:52.422230 podcast_summarizer-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2321 1970-01-01 00:00:00.000000 podcast_summarizer-0.2.2/PKG-INFO
```

### Comparing `podcast_summarizer-0.2.1/LICENSE` & `podcast_summarizer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.2.1/README.md` & `podcast_summarizer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.2.1/podcast_summarizer/cli.py` & `podcast_summarizer-0.2.2/podcast_summarizer/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import click
 import click_spinner
 import podcast_summarizer.youtube as youtube
 import podcast_summarizer.summarizer as summarizer
 from shutil import which
+import warnings
+warnings.filterwarnings("ignore")
 
 @click.command()
 @click.version_option()
 @click.option('--summary-file', '-s', default=None, help="The file to save the summary to.")
 @click.option('--transcription-file', '-t', default=None, help="The file to save the transcription to.")
 @click.option('--audio-format', '-f', default=None, help="The format of the audio file. Defaults to mp3 when it cannot be infered.")
 @click.option('--language', '-l', default="en", help="The language code for the language of the podcast.")
```

### Comparing `podcast_summarizer-0.2.1/podcast_summarizer/summarizer.py` & `podcast_summarizer-0.2.2/podcast_summarizer/summarizer.py`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.2.1/podcast_summarizer/youtube.py` & `podcast_summarizer-0.2.2/podcast_summarizer/youtube.py`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.2.1/pyproject.toml` & `podcast_summarizer-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "podcast-summarizer"
-version = "0.2.1"
+version = "0.2.2"
 description = "Summarizes podcasts."
 authors = ["Diego Quinteiro <diegoquinteiro@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "podcast_summarizer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `podcast_summarizer-0.2.1/PKG-INFO` & `podcast_summarizer-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-summarizer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Summarizes podcasts.
 License: MIT
 Author: Diego Quinteiro
 Author-email: diegoquinteiro@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

