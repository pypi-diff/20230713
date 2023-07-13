# Comparing `tmp/conlang_gpt-0.2.0.tar.gz` & `tmp/conlang_gpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlang_gpt-0.2.0.tar", max compression
+gzip compressed data, was "conlang_gpt-0.3.0.tar", max compression
```

## Comparing `conlang_gpt-0.2.0.tar` & `conlang_gpt-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-07-07 15:45:53.300858 conlang_gpt-0.2.0/LICENSE
--rw-r--r--   0        0        0     5021 2023-07-13 16:46:38.235516 conlang_gpt-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-12 15:53:46.232637 conlang_gpt-0.2.0/conlang_gpt/__init__.py
--rw-r--r--   0        0        0       59 2023-07-12 15:54:29.089650 conlang_gpt-0.2.0/conlang_gpt/__main__.py
--rw-r--r--   0        0        0     4286 2023-07-13 16:44:02.667577 conlang_gpt-0.2.0/conlang_gpt/cli.py
--rw-r--r--   0        0        0        0 2023-07-12 15:35:26.763786 conlang_gpt-0.2.0/conlang_gpt/command/__init__.py
--rw-r--r--   0        0        0      470 2023-07-12 15:32:19.988958 conlang_gpt-0.2.0/conlang_gpt/command/create.py
--rw-r--r--   0        0        0     2752 2023-07-12 21:01:19.747487 conlang_gpt-0.2.0/conlang_gpt/command/improve.py
--rw-r--r--   0        0        0     1260 2023-07-12 20:59:32.503313 conlang_gpt-0.2.0/conlang_gpt/command/modify.py
--rw-r--r--   0        0        0     3096 2023-07-13 16:31:16.541309 conlang_gpt-0.2.0/conlang_gpt/command/translate.py
--rw-r--r--   0        0        0    20084 2023-07-13 16:42:24.440107 conlang_gpt-0.2.0/conlang_gpt/language.py
--rw-r--r--   0        0        0     1724 2023-07-09 03:24:32.406355 conlang_gpt-0.2.0/conlang_gpt/openai.py
--rw-r--r--   0        0        0      703 2023-07-13 16:48:28.123082 conlang_gpt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5663 1970-01-01 00:00:00.000000 conlang_gpt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-07 15:45:53.300858 conlang_gpt-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5007 2023-07-13 16:57:15.787399 conlang_gpt-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 15:53:46.232637 conlang_gpt-0.3.0/conlang_gpt/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-12 15:54:29.089650 conlang_gpt-0.3.0/conlang_gpt/__main__.py
+-rw-r--r--   0        0        0     4222 2023-07-13 16:55:57.033421 conlang_gpt-0.3.0/conlang_gpt/cli.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:35:26.763786 conlang_gpt-0.3.0/conlang_gpt/command/__init__.py
+-rw-r--r--   0        0        0      470 2023-07-12 15:32:19.988958 conlang_gpt-0.3.0/conlang_gpt/command/create.py
+-rw-r--r--   0        0        0     2519 2023-07-13 16:56:25.723656 conlang_gpt-0.3.0/conlang_gpt/command/improve.py
+-rw-r--r--   0        0        0     1260 2023-07-12 20:59:32.503313 conlang_gpt-0.3.0/conlang_gpt/command/modify.py
+-rw-r--r--   0        0        0     3096 2023-07-13 16:31:16.541309 conlang_gpt-0.3.0/conlang_gpt/command/translate.py
+-rw-r--r--   0        0        0    20084 2023-07-13 16:42:24.440107 conlang_gpt-0.3.0/conlang_gpt/language.py
+-rw-r--r--   0        0        0     1724 2023-07-09 03:24:32.406355 conlang_gpt-0.3.0/conlang_gpt/openai.py
+-rw-r--r--   0        0        0      703 2023-07-13 16:59:34.955204 conlang_gpt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5649 1970-01-01 00:00:00.000000 conlang_gpt-0.3.0/PKG-INFO
```

### Comparing `conlang_gpt-0.2.0/LICENSE` & `conlang_gpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conlang_gpt-0.2.0/README.md` & `conlang_gpt-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
   Automatically improve the language.
 
 Options:
   --guide TEXT
   --dictionary TEXT             Enter the filename of the dictionary to use in
                                 'example' mode.
-  --text TEXT
   --max-iterations INTEGER      Max number of revisions to perform. Defaults
                                 to 5.
   --similarity-threshold FLOAT  Maximum similarity between two words to be
                                 considered the same. Defaults to 0.98.
   --model TEXT                  OpenAI model to use. Defaults to
                                 gpt-3.5-turbo.
   --embeddings-model TEXT       OpenAI model to use for word embeddings in
```

### Comparing `conlang_gpt-0.2.0/conlang_gpt/cli.py` & `conlang_gpt-0.3.0/conlang_gpt/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 )
 @click.option(
     "--dictionary",
     "dictionary_path",
     required=False,
     help="Enter the filename of the dictionary to use in 'example' mode.",
 )
-@click.option("--text", required=False)
 @click.option(
     "--max-iterations",
     default=5,
     help="Max number of revisions to perform. Defaults to 5.",
 )
 @click.option(
     "--similarity-threshold",
@@ -100,26 +99,24 @@
     "--embeddings-model",
     default="text-embedding-ada-002",
     help="OpenAI model to use for word embeddings in 'example' mode. Defaults to text-embedding-ada-002.",
 )
 def improve(
     guide_path,
     dictionary_path,
-    text,
     max_iterations,
     similarity_threshold,
     model,
     embeddings_model,
 ):
     """Automatically improve the language."""
 
     improve_(
         guide_path,
         dictionary_path,
-        text,
         max_iterations,
         similarity_threshold,
         model,
         embeddings_model,
     )
```

### Comparing `conlang_gpt-0.2.0/conlang_gpt/command/improve.py` & `conlang_gpt-0.3.0/conlang_gpt/command/improve.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,43 +8,32 @@
     modify_language,
 )
 
 
 def improve(
     guide_path,
     dictionary_path,
-    text,
     max_iterations,
     similarity_threshold,
     model,
     embeddings_model,
 ):
     """Automatically improve the language."""
 
-    if text:
-        click.echo(
-            click.style(
-                "The --text option is experimental. It may not work as expected.",
-                fg="yellow",
-            )
-        )
-
     # Load the beginner's guide
     with open(guide_path, "r") as file:
         guide = file.read()
 
     # Load the dictionary
     dictionary = load_dictionary(dictionary_path)
 
     # Revise the language guide
     for i in range(max_iterations):
         # Try to improve the language guide
-        improved_guide = improve_language(
-            guide, dictionary, model, embeddings_model, text
-        )
+        improved_guide = improve_language(guide, dictionary, model, embeddings_model)
 
         # Stop if no problems were found
         if improved_guide is None:
             break
 
         # Update the language guide
         guide = improved_guide
```

### Comparing `conlang_gpt-0.2.0/conlang_gpt/command/modify.py` & `conlang_gpt-0.3.0/conlang_gpt/command/modify.py`

 * *Files identical despite different names*

### Comparing `conlang_gpt-0.2.0/conlang_gpt/command/translate.py` & `conlang_gpt-0.3.0/conlang_gpt/command/translate.py`

 * *Files identical despite different names*

### Comparing `conlang_gpt-0.2.0/conlang_gpt/language.py` & `conlang_gpt-0.3.0/conlang_gpt/language.py`

 * *Files identical despite different names*

### Comparing `conlang_gpt-0.2.0/conlang_gpt/openai.py` & `conlang_gpt-0.3.0/conlang_gpt/openai.py`

 * *Files identical despite different names*

### Comparing `conlang_gpt-0.2.0/pyproject.toml` & `conlang_gpt-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "conlang-gpt"
-version = "0.2.0"
+version = "0.3.0"
 description = "ChatGPT language generator and translator"
 authors = ["Caleb Sacks <16855387+clabe45@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/clabe45/conlang-gpt"
 keywords = ["conlang", "chatgpt", "gpt 4", "openai"]
 license = "MIT"
 packages = [{include = "conlang_gpt"}]
```

### Comparing `conlang_gpt-0.2.0/PKG-INFO` & `conlang_gpt-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conlang-gpt
-Version: 0.2.0
+Version: 0.3.0
 Summary: ChatGPT language generator and translator
 Home-page: https://github.com/clabe45/conlang-gpt
 License: MIT
 Keywords: conlang,chatgpt,gpt 4,openai
 Author: Caleb Sacks
 Author-email: 16855387+clabe45@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -98,15 +98,14 @@
 
   Automatically improve the language.
 
 Options:
   --guide TEXT
   --dictionary TEXT             Enter the filename of the dictionary to use in
                                 'example' mode.
-  --text TEXT
   --max-iterations INTEGER      Max number of revisions to perform. Defaults
                                 to 5.
   --similarity-threshold FLOAT  Maximum similarity between two words to be
                                 considered the same. Defaults to 0.98.
   --model TEXT                  OpenAI model to use. Defaults to
                                 gpt-3.5-turbo.
   --embeddings-model TEXT       OpenAI model to use for word embeddings in
```

