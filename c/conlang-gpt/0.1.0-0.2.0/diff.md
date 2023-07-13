# Comparing `tmp/conlang_gpt-0.1.0.tar.gz` & `tmp/conlang_gpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlang_gpt-0.1.0.tar", max compression
+gzip compressed data, was "conlang_gpt-0.2.0.tar", max compression
```

## Comparing `conlang_gpt-0.1.0.tar` & `conlang_gpt-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-07-07 15:45:53.300858 conlang_gpt-0.1.0/LICENSE
--rw-r--r--   0        0        0     3718 2023-07-07 15:46:46.844620 conlang_gpt-0.1.0/README.md
--rw-r--r--   0        0        0     5318 2023-07-07 04:09:21.739099 conlang_gpt-0.1.0/conlang_gpt/__init__.py
--rw-r--r--   0        0        0       56 2023-07-05 19:59:22.676235 conlang_gpt-0.1.0/conlang_gpt/__main__.py
--rw-r--r--   0        0        0     5961 2023-07-07 15:22:03.299400 conlang_gpt-0.1.0/conlang_gpt/language.py
--rw-r--r--   0        0        0     1276 2023-07-07 04:04:47.590111 conlang_gpt-0.1.0/conlang_gpt/openai.py
--rw-r--r--   0        0        0      615 2023-07-07 15:51:31.060224 conlang_gpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 conlang_gpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-07 15:45:53.300858 conlang_gpt-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5021 2023-07-13 16:46:38.235516 conlang_gpt-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 15:53:46.232637 conlang_gpt-0.2.0/conlang_gpt/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-12 15:54:29.089650 conlang_gpt-0.2.0/conlang_gpt/__main__.py
+-rw-r--r--   0        0        0     4286 2023-07-13 16:44:02.667577 conlang_gpt-0.2.0/conlang_gpt/cli.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:35:26.763786 conlang_gpt-0.2.0/conlang_gpt/command/__init__.py
+-rw-r--r--   0        0        0      470 2023-07-12 15:32:19.988958 conlang_gpt-0.2.0/conlang_gpt/command/create.py
+-rw-r--r--   0        0        0     2752 2023-07-12 21:01:19.747487 conlang_gpt-0.2.0/conlang_gpt/command/improve.py
+-rw-r--r--   0        0        0     1260 2023-07-12 20:59:32.503313 conlang_gpt-0.2.0/conlang_gpt/command/modify.py
+-rw-r--r--   0        0        0     3096 2023-07-13 16:31:16.541309 conlang_gpt-0.2.0/conlang_gpt/command/translate.py
+-rw-r--r--   0        0        0    20084 2023-07-13 16:42:24.440107 conlang_gpt-0.2.0/conlang_gpt/language.py
+-rw-r--r--   0        0        0     1724 2023-07-09 03:24:32.406355 conlang_gpt-0.2.0/conlang_gpt/openai.py
+-rw-r--r--   0        0        0      703 2023-07-13 16:48:28.123082 conlang_gpt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5663 1970-01-01 00:00:00.000000 conlang_gpt-0.2.0/PKG-INFO
```

### Comparing `conlang_gpt-0.1.0/LICENSE` & `conlang_gpt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conlang_gpt-0.1.0/README.md` & `conlang_gpt-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # Conlang GPT
 
 Conlang GPT is a command line tool for creating, modifying and using constructed languages, powered by ChatGPT
 
 ## Features
 
+> :warning: This tool is in early development. It is not ready for production use.
+
 | Feature | Status |
 | --- | --- |
-| Automatically generate specifications for written or spoken languages | :white_check_mark: Stable |
-| Automatically or manually improve languages iteratively | :white_check_mark: Stable |
-| Generate vocabulary | :sparkles: Experimental |
-| Translate any text to or from the generated languages | :white_check_mark: Stable |
-| Support for all of OpenAI's chat models | :white_check_mark: Stable |
+| Automatically generate specifications for written or spoken languages | :sparkles: Alpha |
+| Automatically or manually improve language specs iteratively | :sparkles: Alpha |
+| Translate any text to or from the generated languages | :sparkles: Alpha |
+| Generate vocabulary lazily | :sparkles: Alpha |
+| Automatically update vocabulary when language specs change | :sparkles: Alpha |
+| Support for all of OpenAI's chat models | :sparkles: Alpha |
 
 ## Installation
 
 ```
 pip install conlang-gpt
 ```
 
+## Anatomy of a Language
+
+Languages are represented as two files:
+- **Guide**: The purpose of the language guide is to describe how to use the language, including rules related to grammar and phonetics.
+- **Dictionary**: The dictionary contains the vocabulary for the language. It is built up lazily as more and more text is translated.
+
 ## Commands
 
 ### Overview
 
 Conlang GPT provides several commands:
 
 ```
@@ -42,93 +51,96 @@
 
 ```
  export OPENAI_API_KEY=sk...
 ```
 
 ### `conlang create`
 
-Creates a guide for a new language and writes it to a file.
+Creates the first draft of a guide for a new language and writes it to a file.
 
 ```
 $ conlang create --help
 Usage: conlang create [OPTIONS]
 
   Create a constructed language.
 
 Options:
   --design-goals TEXT
-  --output-guide TEXT
-  --model TEXT         OpenAI model to use. Defaults to gpt-3.5-turbo-16k.
+  --guide TEXT
+  --model TEXT         OpenAI model to use. Defaults to gpt-3.5-turbo.
   --help               Show this message and exit.
 ```
 
 ### `conlang improve`
 
-Attempts to automatically improve the language and saves the resulting guide to a file. Supports two modes - `basic` and `example`. In basic mode, a random flaw with the language is identified and fixed. In example mode, a random English sentence is generated, translated to the conlang and used to identify and fix a problem with the language.
+Attempts to automatically improve the language guide and dictionary. The resulting guide and dictionary are saved to the original input files.
 
 ```
 $ conlang improve --help
 Usage: conlang improve [OPTIONS]
 
   Automatically improve the language.
 
 Options:
-  --input-guide TEXT
-  --output-guide TEXT
-  --mode [basic|example]  Mode to use. Defaults to basic. Set to the
-                          experimental 'example' mode to include a new random
-                          translation in each revision.
-  -n INTEGER              Number of revisions to perform. Defaults to 1.
-  --model TEXT            OpenAI model to use. Defaults to gpt-3.5-turbo-16k.
-  --help                  Show this message and exit.
+  --guide TEXT
+  --dictionary TEXT             Enter the filename of the dictionary to use in
+                                'example' mode.
+  --text TEXT
+  --max-iterations INTEGER      Max number of revisions to perform. Defaults
+                                to 5.
+  --similarity-threshold FLOAT  Maximum similarity between two words to be
+                                considered the same. Defaults to 0.98.
+  --model TEXT                  OpenAI model to use. Defaults to
+                                gpt-3.5-turbo.
+  --embeddings-model TEXT       OpenAI model to use for word embeddings in
+                                'example' mode. Defaults to text-embedding-
+                                ada-002.
+  --help                        Show this message and exit.
 ```
 
 ### `conlang modify`
 
-Makes a specific change to the language and updates the guide.
+Makes a specific change to the language and updates the guide and dictionary.
 
 ```
 $ conlang modify --help
 Usage: conlang modify [OPTIONS]
 
   Make specific changes to the language.
 
 Options:
-  --input-guide TEXT
-  --output-guide TEXT
+  --guide TEXT
+  --dictionary TEXT             Enter the filename of the dictionary to use in
+                                'example' mode.
   --changes TEXT
-  --model TEXT         OpenAI model to use. Defaults to gpt-3.5-turbo-16k.
-  --help               Show this message and exit.
+  --similarity-threshold FLOAT  Maximum similarity between two words to be
+                                considered the same. Defaults to 0.98.
+  --model TEXT                  OpenAI model to use. Defaults to
+                                gpt-3.5-turbo.
+  --embeddings-model TEXT       OpenAI model to use for word embeddings in
+                                'example' mode. Defaults to text-embedding-
+                                ada-002.
+  --help                        Show this message and exit.
 ```
 
 ### `conlang translate`
 
-Translates text between any language ChatGPT was trained on to and the conlang. The language of the input text is automatically detected and used to dermine which language to translate to.
+Translates text between any language ChatGPT was trained on to and the conlang. The language of the input text is automatically detected and used to dermine which language to translate to. If any problems are encountered while translating, the guide and dictionary will be repeatedly fixed until `--max-improvements` is reached.
 
 ```
 $ conlang translate --help
 Usage: conlang translate [OPTIONS]
 
   Translate text to or from a constructed language.
 
 Options:
   --guide TEXT
+  --dictionary TEXT
   --text TEXT
-  --model TEXT  OpenAI model to use
-  --help        Show this message and exit.
-```
-
-### `conlang words` (experimental)
-
-```
-$ conlang words --help
-Usage: conlang words [OPTIONS]
-
-  Generate words in the language (experimental).
-
-Options:
-  --guide TEXT
-  --output TEXT
-  -n INTEGER     Number of words to generate. Defaults to 15.
-  --model TEXT   OpenAI model to use. Defaults to gpt-3.5-turbo-16k.
-  --help         Show this message and exit.
+  --max-improvements INTEGER    Max number of relevant improvements to make to
+                                the guide and dictionary. Defaults to 5.
+  --similarity-threshold FLOAT  Maximum similarity between two words to be
+                                considered the same. Defaults to 0.98.
+  --model TEXT                  OpenAI model to use
+  --embedding-model TEXT        OpenAI model to use for word embeddings
+  --help                        Show this message and exit.
 ```
```

### Comparing `conlang_gpt-0.1.0/conlang_gpt/openai.py` & `conlang_gpt-0.2.0/conlang_gpt/openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,34 +5,58 @@
 import dotenv
 import openai
 
 
 dotenv.load_dotenv()
 
 if "OPENAI_API_KEY" not in os.environ:
-    raise Exception("OpenAI API key not found. Please set the OPENAI_API_KEY environment variable to your API key.")
+    raise Exception(
+        "OpenAI API key not found. Please set the OPENAI_API_KEY environment variable to your API key."
+    )
 openai.api_key = os.environ["OPENAI_API_KEY"]
 
 
 def complete_chat(**kwargs):
     """Complete a chat with the OpenAI API."""
 
     delay = 1
     while True:
         try:
             completion = openai.ChatCompletion.create(**kwargs)
             break
         except openai.error.APIError as e:
-            click.echo(click.style(f"OpenAI API error: {e}. Retrying in {delay} second(s)...", fg="red"))
+            click.echo(
+                click.style(
+                    f"OpenAI API error: {e}. Retrying in {delay} second(s)...", fg="red"
+                )
+            )
             time.sleep(delay)
         except openai.error.RateLimitError:
-            click.echo(click.style(f"OpenAI API rate limit exceeded. Retrying in {delay} second(s)...", fg="red"))
+            click.echo(
+                click.style(
+                    f"OpenAI API rate limit exceeded. Retrying in {delay} second(s)...",
+                    fg="red",
+                )
+            )
             time.sleep(delay)
             delay *= 2
         except openai.error.ServiceUnavailableError:
-            click.echo(click.style(f"OpenAI API service unavailable. Retrying in {delay} second(s)...", fg="red"))
+            click.echo(
+                click.style(
+                    f"OpenAI API service unavailable. Retrying in {delay} second(s)...",
+                    fg="red",
+                )
+            )
             time.sleep(delay)
         except openai.error.Timeout:
-            click.echo(click.style(f"OpenAI API timeout. Retrying in {delay} second(s)...", fg="red"))
+            click.echo(
+                click.style(
+                    f"OpenAI API timeout. Retrying in {delay} second(s)...", fg="red"
+                )
+            )
             time.sleep(delay)
 
     return completion
+
+
+def get_embedding(text, model):
+    return openai.Embedding.create(input=[text], model=model)["data"][0]["embedding"]
```

### Comparing `conlang_gpt-0.1.0/pyproject.toml` & `conlang_gpt-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "conlang-gpt"
-version = "0.1.0"
+version = "0.2.0"
 description = "ChatGPT language generator and translator"
 authors = ["Caleb Sacks <16855387+clabe45@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/clabe45/conlang-gpt"
 keywords = ["conlang", "chatgpt", "gpt 4", "openai"]
 license = "MIT"
 packages = [{include = "conlang_gpt"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-openai = "^0.27.8"
+openai = {extras = ["embeddings"], version = "^0.27.8"}
 python-dotenv = "^1.0.0"
 click = "^8.1.3"
 
 
 [tool.poetry.scripts]
-conlang = "conlang_gpt.__init__:cli"
+conlang = "conlang_gpt.cli:cli"
 
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `conlang_gpt-0.1.0/PKG-INFO` & `conlang_gpt-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: conlang-gpt
-Version: 0.1.0
+Version: 0.2.0
 Summary: ChatGPT language generator and translator
 Home-page: https://github.com/clabe45/conlang-gpt
 License: MIT
 Keywords: conlang,chatgpt,gpt 4,openai
 Author: Caleb Sacks
 Author-email: 16855387+clabe45@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: openai[embeddings] (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Conlang GPT
 
 Conlang GPT is a command line tool for creating, modifying and using constructed languages, powered by ChatGPT
 
 ## Features
 
+> :warning: This tool is in early development. It is not ready for production use.
+
 | Feature | Status |
 | --- | --- |
-| Automatically generate specifications for written or spoken languages | :white_check_mark: Stable |
-| Automatically or manually improve languages iteratively | :white_check_mark: Stable |
-| Generate vocabulary | :sparkles: Experimental |
-| Translate any text to or from the generated languages | :white_check_mark: Stable |
-| Support for all of OpenAI's chat models | :white_check_mark: Stable |
+| Automatically generate specifications for written or spoken languages | :sparkles: Alpha |
+| Automatically or manually improve language specs iteratively | :sparkles: Alpha |
+| Translate any text to or from the generated languages | :sparkles: Alpha |
+| Generate vocabulary lazily | :sparkles: Alpha |
+| Automatically update vocabulary when language specs change | :sparkles: Alpha |
+| Support for all of OpenAI's chat models | :sparkles: Alpha |
 
 ## Installation
 
 ```
 pip install conlang-gpt
 ```
 
+## Anatomy of a Language
+
+Languages are represented as two files:
+- **Guide**: The purpose of the language guide is to describe how to use the language, including rules related to grammar and phonetics.
+- **Dictionary**: The dictionary contains the vocabulary for the language. It is built up lazily as more and more text is translated.
+
 ## Commands
 
 ### Overview
 
 Conlang GPT provides several commands:
 
 ```
@@ -60,94 +69,97 @@
 
 ```
  export OPENAI_API_KEY=sk...
 ```
 
 ### `conlang create`
 
-Creates a guide for a new language and writes it to a file.
+Creates the first draft of a guide for a new language and writes it to a file.
 
 ```
 $ conlang create --help
 Usage: conlang create [OPTIONS]
 
   Create a constructed language.
 
 Options:
   --design-goals TEXT
-  --output-guide TEXT
-  --model TEXT         OpenAI model to use. Defaults to gpt-3.5-turbo-16k.
+  --guide TEXT
+  --model TEXT         OpenAI model to use. Defaults to gpt-3.5-turbo.
   --help               Show this message and exit.
 ```
 
 ### `conlang improve`
 
-Attempts to automatically improve the language and saves the resulting guide to a file. Supports two modes - `basic` and `example`. In basic mode, a random flaw with the language is identified and fixed. In example mode, a random English sentence is generated, translated to the conlang and used to identify and fix a problem with the language.
+Attempts to automatically improve the language guide and dictionary. The resulting guide and dictionary are saved to the original input files.
 
 ```
 $ conlang improve --help
 Usage: conlang improve [OPTIONS]
 
   Automatically improve the language.
 
 Options:
-  --input-guide TEXT
-  --output-guide TEXT
-  --mode [basic|example]  Mode to use. Defaults to basic. Set to the
-                          experimental 'example' mode to include a new random
-                          translation in each revision.
-  -n INTEGER              Number of revisions to perform. Defaults to 1.
-  --model TEXT            OpenAI model to use. Defaults to gpt-3.5-turbo-16k.
-  --help                  Show this message and exit.
+  --guide TEXT
+  --dictionary TEXT             Enter the filename of the dictionary to use in
+                                'example' mode.
+  --text TEXT
+  --max-iterations INTEGER      Max number of revisions to perform. Defaults
+                                to 5.
+  --similarity-threshold FLOAT  Maximum similarity between two words to be
+                                considered the same. Defaults to 0.98.
+  --model TEXT                  OpenAI model to use. Defaults to
+                                gpt-3.5-turbo.
+  --embeddings-model TEXT       OpenAI model to use for word embeddings in
+                                'example' mode. Defaults to text-embedding-
+                                ada-002.
+  --help                        Show this message and exit.
 ```
 
 ### `conlang modify`
 
-Makes a specific change to the language and updates the guide.
+Makes a specific change to the language and updates the guide and dictionary.
 
 ```
 $ conlang modify --help
 Usage: conlang modify [OPTIONS]
 
   Make specific changes to the language.
 
 Options:
-  --input-guide TEXT
-  --output-guide TEXT
+  --guide TEXT
+  --dictionary TEXT             Enter the filename of the dictionary to use in
+                                'example' mode.
   --changes TEXT
-  --model TEXT         OpenAI model to use. Defaults to gpt-3.5-turbo-16k.
-  --help               Show this message and exit.
+  --similarity-threshold FLOAT  Maximum similarity between two words to be
+                                considered the same. Defaults to 0.98.
+  --model TEXT                  OpenAI model to use. Defaults to
+                                gpt-3.5-turbo.
+  --embeddings-model TEXT       OpenAI model to use for word embeddings in
+                                'example' mode. Defaults to text-embedding-
+                                ada-002.
+  --help                        Show this message and exit.
 ```
 
 ### `conlang translate`
 
-Translates text between any language ChatGPT was trained on to and the conlang. The language of the input text is automatically detected and used to dermine which language to translate to.
+Translates text between any language ChatGPT was trained on to and the conlang. The language of the input text is automatically detected and used to dermine which language to translate to. If any problems are encountered while translating, the guide and dictionary will be repeatedly fixed until `--max-improvements` is reached.
 
 ```
 $ conlang translate --help
 Usage: conlang translate [OPTIONS]
 
   Translate text to or from a constructed language.
 
 Options:
   --guide TEXT
+  --dictionary TEXT
   --text TEXT
-  --model TEXT  OpenAI model to use
-  --help        Show this message and exit.
-```
-
-### `conlang words` (experimental)
-
-```
-$ conlang words --help
-Usage: conlang words [OPTIONS]
-
-  Generate words in the language (experimental).
-
-Options:
-  --guide TEXT
-  --output TEXT
-  -n INTEGER     Number of words to generate. Defaults to 15.
-  --model TEXT   OpenAI model to use. Defaults to gpt-3.5-turbo-16k.
-  --help         Show this message and exit.
+  --max-improvements INTEGER    Max number of relevant improvements to make to
+                                the guide and dictionary. Defaults to 5.
+  --similarity-threshold FLOAT  Maximum similarity between two words to be
+                                considered the same. Defaults to 0.98.
+  --model TEXT                  OpenAI model to use
+  --embedding-model TEXT        OpenAI model to use for word embeddings
+  --help                        Show this message and exit.
 ```
```

