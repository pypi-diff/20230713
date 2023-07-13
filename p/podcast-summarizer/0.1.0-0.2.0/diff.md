# Comparing `tmp/podcast_summarizer-0.1.0.tar.gz` & `tmp/podcast_summarizer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_summarizer-0.1.0.tar", max compression
+gzip compressed data, was "podcast_summarizer-0.2.0.tar", max compression
```

## Comparing `podcast_summarizer-0.1.0.tar` & `podcast_summarizer-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-07-13 00:12:43.694813 podcast_summarizer-0.1.0/LICENSE
--rw-r--r--   0        0        0     1065 2023-07-13 02:56:26.565999 podcast_summarizer-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-13 00:45:08.553711 podcast_summarizer-0.1.0/podcast_summarizer/__init__.py
--rw-r--r--   0        0        0     2733 2023-07-13 02:37:57.911087 podcast_summarizer-0.1.0/podcast_summarizer/cli.py
--rw-r--r--   0        0        0     1433 2023-07-13 02:42:35.524886 podcast_summarizer-0.1.0/podcast_summarizer/summarizer.py
--rw-r--r--   0        0        0      566 2023-07-13 03:07:11.348949 podcast_summarizer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 podcast_summarizer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-13 00:12:43.694813 podcast_summarizer-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1576 2023-07-13 03:18:53.377475 podcast_summarizer-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 00:45:08.553711 podcast_summarizer-0.2.0/podcast_summarizer/__init__.py
+-rw-r--r--   0        0        0     3198 2023-07-13 04:56:11.430038 podcast_summarizer-0.2.0/podcast_summarizer/cli.py
+-rw-r--r--   0        0        0     1444 2023-07-13 04:51:36.636030 podcast_summarizer-0.2.0/podcast_summarizer/summarizer.py
+-rw-r--r--   0        0        0     2128 2023-07-13 04:52:50.401284 podcast_summarizer-0.2.0/podcast_summarizer/youtube.py
+-rw-r--r--   0        0        0      608 2023-07-13 04:56:40.260232 podcast_summarizer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2352 1970-01-01 00:00:00.000000 podcast_summarizer-0.2.0/PKG-INFO
```

### Comparing `podcast_summarizer-0.1.0/LICENSE` & `podcast_summarizer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.1.0/podcast_summarizer/cli.py` & `podcast_summarizer-0.2.0/podcast_summarizer/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 import os
 import click
 import click_spinner
+import podcast_summarizer.youtube as youtube
 import podcast_summarizer.summarizer as summarizer
 from shutil import which
 
 @click.command()
 @click.version_option()
 @click.option('--summary-file', '-s', default=None, help="The file to save the summary to.")
 @click.option('--transcription-file', '-t', default=None, help="The file to save the transcription to.")
 @click.option('--audio-format', '-f', default=None, help="The format of the audio file. Defaults to mp3 when it cannot be infered.")
+@click.option('--language', '-l', default="en", help="The language code for the language of the podcast.")
 @click.argument('podcast_url_or_path')
-def cli(podcast_url_or_path, summary_file, transcription_file, audio_format):
+def cli(podcast_url_or_path, summary_file, transcription_file, audio_format, language):
     """Summarizes the podcast provided by the PODCAST_URL_OR_PATH.
     
     - PODCAST_URL_OR_PATH can be a URL or a path to a local audio file.
+    
+    - PODCAST_URL_OR_PATH can be a YouTube URL (https://www.youtube.com/watch?v=...)
 
     - PODCAST_URL_OR_PATH can also be a path to a local ".txt" file containing the transcription.
     """
 
     if not which("ffmpeg"):
         raise Exception("ffmpeg is not installed. Please install ffmpeg.")
 
     if not os.getenv("OPENAI_API_KEY"):
         raise Exception("OPENAI_API_KEY is not set. Please add your API key to your environment variables.")
     
+    if podcast_url_or_path.startswith("https://www.youtube.com/watch?v="):
+        podcast_url_or_path = youtube.extract_from_youtube(podcast_url_or_path, transcription_file, language)
+    
     if podcast_url_or_path.lower().endswith(".txt") and os.path.isfile(podcast_url_or_path):
         transcription = open(podcast_url_or_path, "r").read()
     else:
         with summarizer.openAudio(podcast_url_or_path, audio_format) as file:
-            click.echo("Transcribing...", nl=False)
+            click.echo("🎙️ Transcribing...", nl=False)
             with click_spinner.spinner():
                 transcription = summarizer.transcribe(file.name)
             click.echo("\r", nl=False)
             click.secho("🎙️ Transcription complete!", fg="green")
 
         if transcription_file:
             with open(transcription_file, "w") as transcription_file:
                 transcription_file.write(transcription)
                 click.secho("💾 Transcription saved to transcription.txt")
         
-    click.echo("Summarizing...", nl=False)
+    click.echo("📝 Summarizing...", nl=False)
     with click_spinner.spinner():
-        summary = summarizer.summarize(transcription)
+        summary = summarizer.summarize(transcription, language)
     click.echo("\r", nl=False)
     click.secho("📝 Summary complete!", fg="green")
 
     if summary_file:
         with open(summary_file, "w") as summary_file:
             summary_file.write(summary)
             click.secho("💾 Summary saved to summary.txt", fg="green")
```

### Comparing `podcast_summarizer-0.1.0/podcast_summarizer/summarizer.py` & `podcast_summarizer-0.2.0/podcast_summarizer/summarizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import openai
 import urllib.request
 import tempfile
 import whisper
 
+
 messages = []
 SUPPORTED_AUDIO_FORMATS = ["m4a","mp3","webm","mp4","mpga","wav","mpeg"]
 
 def openAudio(url_or_path, audio_format):
     if os.path.isfile(url_or_path):
         return open(url_or_path, "rb")
     try:
@@ -25,16 +26,16 @@
 
 def transcribe(mp3_path):
     model = whisper.load_model("tiny")
     result = model.transcribe(mp3_path, fp16=False)
 
     return result["text"]
 
-def summarize(text):
-    return askLLM(f'Please summarize the following podcast transcription in its original language: {text}')
+def summarize(text, language):
+    return askLLM(f'Please summarize the following podcast transcription, respond in "{language}": {text}')
 
 def askLLM(message):
     openai.api_key = os.getenv("OPENAI_API_KEY")
     
     global messages
 
     messages += [{
```

### Comparing `podcast_summarizer-0.1.0/pyproject.toml` & `podcast_summarizer-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "podcast-summarizer"
-version = "0.1.0"
+version = "0.2.0"
 description = "Summarizes podcasts."
 authors = ["Diego Quinteiro <diegoquinteiro@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "podcast_summarizer"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^0.27.8"
 click = "^8.1.4"
 openai-whisper = {git = "https://github.com/openai/whisper.git"}
 click-spinner = "^0.1.10"
+yt-dlp = "^2023.7.6"
+webvtt-py = "^0.4.6"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `podcast_summarizer-0.1.0/PKG-INFO` & `podcast_summarizer-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,77 @@
 Metadata-Version: 2.1
 Name: podcast-summarizer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Summarizes podcasts.
 License: MIT
 Author: Diego Quinteiro
 Author-email: diegoquinteiro@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: click-spinner (>=0.1.10,<0.2.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: openai-whisper @ git+https://github.com/openai/whisper.git
+Requires-Dist: webvtt-py (>=0.4.6,<0.5.0)
+Requires-Dist: yt-dlp (>=2023.7.6,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # podcast-summarizer
 ![Version](https://img.shields.io/pypi/v/podcast-summarizer)
 ![Python Version Support](https://img.shields.io/pypi/pyversions/podcast-summarizer)
 
 Summarizes a podcast from an audio or transcription using ChatGPT.
 
+## Instalation
+```bash
+pip install podcast-summarizer
+```
+
 ## Usage
 ```bash
 # Summarize a podcast audio from an URL.
 podcast-summarizer http://.../audio.mp3
 
+# Summarize a podcast audio from an YouTube video.
+podcast-summarizer https://www.youtube.com/watch?v=...
+
 # Summarize a podcast audio from local file.
 podcast-summarizer audio.mp3
 
 # Summarize a podcast audio and save transcription and summary to files.
-podcast-summarizer -t transcription.txt -s summary.txt http://.../audio.mp3
+podcast-summarizer -t transcription.txt -s summary.txt audio.mp3
 
 # Summarize an already transcribed podcast
 podcast-summarizer transcription.txt
 ```
 
-## Instalation
-```bash
-pip install podcast-summarizer
-```
-
+## Setup
 You'll need to install `ffmpeg` before running the script.
 
 ```bash
 # on Ubuntu or Debian
 sudo apt update && sudo apt install ffmpeg
 
 # on Arch Linux
 sudo pacman -S ffmpeg
 
 # on MacOS using Homebrew (https://brew.sh/)
 brew install ffmpeg
 ```
 
-You'll also need to set the `OPENAI_API_KEY` environment variable.
+The script expects an environment variable called `OPEN_API_KEY`.
+
+1. Get an [OpenAI API Key](https://github.com/Significant-Gravitas/Auto-GPT#:~:text=Get%20an%20OpenAI-,API%20Key,-Download%20the%20latest)
+2. Add the key to your `OPEN_API_KEY` environment variable:
+  - If you use `bash`:
+    ```bash
+    echo 'export OPENAI_API_KEY={your api key}' >> ~/.bash_profile && source ~/.bash_profile
+    ```
+  - If yu use `zsh`:
+    ```bash
+    echo 'export OPENAI_API_KEY={your api key}' >> ~/.zshenv && source ~/.zshenv
+    ```
 
-```bash
-export OPENAI_API_KEY=<YOUR_API_KEY..>
-```
```

