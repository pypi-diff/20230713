# Comparing `tmp/better_rich_prompts-1.0.0.tar.gz` & `tmp/better_rich_prompts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_rich_prompts-1.0.0.tar", max compression
+gzip compressed data, was "better_rich_prompts-1.0.2.tar", max compression
```

## Comparing `better_rich_prompts-1.0.0.tar` & `better_rich_prompts-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-12 16:47:35.207169 better_rich_prompts-1.0.0/better_rich_prompts/__init__.py
--rw-r--r--   0        0        0    11107 2023-07-12 21:51:08.837702 better_rich_prompts-1.0.0/better_rich_prompts/prompt.py
--rw-r--r--   0        0        0     1539 2023-07-12 22:08:26.243507 better_rich_prompts-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2433 2023-07-12 21:55:43.125274 better_rich_prompts-1.0.0/README.md
--rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 better_rich_prompts-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 16:47:35.207169 better_rich_prompts-1.0.2/better_rich_prompts/__init__.py
+-rw-r--r--   0        0        0    11107 2023-07-12 21:51:08.837702 better_rich_prompts-1.0.2/better_rich_prompts/prompt.py
+-rw-r--r--   0        0        0     1539 2023-07-12 22:43:07.955571 better_rich_prompts-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2469 2023-07-12 22:34:45.513991 better_rich_prompts-1.0.2/README.md
+-rw-r--r--   0        0        0     3503 1970-01-01 00:00:00.000000 better_rich_prompts-1.0.2/PKG-INFO
```

### Comparing `better_rich_prompts-1.0.0/better_rich_prompts/prompt.py` & `better_rich_prompts-1.0.2/better_rich_prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `better_rich_prompts-1.0.0/pyproject.toml` & `better_rich_prompts-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "better-rich-prompts"
 homepage = "https://github.com/EwenLo/better-rich-prompts"
 documentation = "https://github.com/EwenLo/better-rich-prompts/"
-version = "1.0.0"
+version = "1.0.2"
 description = "Improved prompts for rich."
 authors = ["Ewen Lorimer <ewen@ewenlorimer.ca>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
```

### Comparing `better_rich_prompts-1.0.0/README.md` & `better_rich_prompts-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/better-rich-prompts/0.0.1)](https://pypi.org/project/better-rich-prompts/) [![PyPI version](https://badge.fury.io/py/better-rich-prompts.svg)](https://badge.fury.io/py/better-rich-prompts)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/better-rich-prompts/1.0.0)](https://pypi.org/project/better-rich-prompts/) [![PyPI version](https://badge.fury.io/py/better-rich-prompts.svg)](https://badge.fury.io/py/better-rich-prompts)
 
 [![Downloads](https://pepy.tech/badge/better-rich-prompts/month)](https://pepy.tech/project/better-rich-prompts)
 
 
 [English readme](https://github.com/EwenLo/better-rich-prompts/blob/master/README.md)
 
 better-rich-prompts is a Python extension library for [Rich](https://github.com/Textualize/rich).
@@ -25,24 +25,24 @@
 choices = [
     {"name": "english", "language_code": "en"},
     {"name": "spanish", "language_code": "es"},
     {"name":"french","language_code":"fr"},
 ]
 ListPrompt.ask("Select a language", choices, choice_key="name")
 ```
-![ListPrompt Example](https://github.com/EwenLo/better-rich-prompts/raw/master/imgs/list_prompt_ex1.png)
+![ListPrompt Example](https://raw.githubusercontent.com/EwenLo/better-rich-prompts/main/imgs/dict_prompt_ex1.png)
 
 ### Example 2 - Using list of strings
 ```python
 from better_rich_prompts.prompt import ListPrompt
 
 choices = ["en", "es", "fr"]
 ListPrompt.ask("Select a language", choices,default="en")
 ```
-![ListPrompt Example](https://github.com/EwenLo/better-rich-prompts/raw/master/imgs/list_prompt_ex2.png)
+![ListPrompt Example](https://raw.githubusercontent.com/EwenLo/better-rich-prompts/main/imgs/list_prompt_ex2.png)
 
 ### Example 3 - Using list of custom objects
 ```python
 from better_rich_prompts.prompt import ListPrompt
 
 class Language:
     def __init__(self, name, code):
@@ -55,17 +55,17 @@
     Language("spanish", "es"),
     Language("french", "fr"),
 ]
 ListPrompt.ask(
     "Select a language", choices, default="en", choice_key=lambda c: c.code
 )
 ```
-![ListPrompt Example](https://github.com/EwenLo/better-rich-prompts/raw/master/imgs/list_prompt_ex3.png)
+![ListPrompt Example](https://raw.githubusercontent.com/EwenLo/better-rich-prompts/main/imgs/list_prompt_ex3.png)
 
 ## Using Dict Prompt
 ```python
 from better_rich_prompts.prompt import DictPrompt
 
 choices = {"en":"english","es":"spanish","fr":"french"}
 DictPrompt.ask("Select a language", choices)
 ```
-![ListPrompt Example](https://github.com/EwenLo/better-rich-prompts/raw/master/imgs/dict_prompt_ex1.png)
+![ListPrompt Example](https://raw.githubusercontent.com/EwenLo/better-rich-prompts/main/imgs/dict_prompt_ex1.png)
```

### Comparing `better_rich_prompts-1.0.0/PKG-INFO` & `better_rich_prompts-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-rich-prompts
-Version: 1.0.0
+Version: 1.0.2
 Summary: Improved prompts for rich.
 Home-page: https://github.com/EwenLo/better-rich-prompts
 License: MIT
 Author: Ewen Lorimer
 Author-email: ewen@ewenlorimer.ca
 Requires-Python: >=3.7.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Provides-Extra: jupyter
 Requires-Dist: rich (>=3.3.2)
 Project-URL: Documentation, https://github.com/EwenLo/better-rich-prompts/
 Description-Content-Type: text/markdown
 
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/better-rich-prompts/0.0.1)](https://pypi.org/project/better-rich-prompts/) [![PyPI version](https://badge.fury.io/py/better-rich-prompts.svg)](https://badge.fury.io/py/better-rich-prompts)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/better-rich-prompts/1.0.0)](https://pypi.org/project/better-rich-prompts/) [![PyPI version](https://badge.fury.io/py/better-rich-prompts.svg)](https://badge.fury.io/py/better-rich-prompts)
 
 [![Downloads](https://pepy.tech/badge/better-rich-prompts/month)](https://pepy.tech/project/better-rich-prompts)
 
 
 [English readme](https://github.com/EwenLo/better-rich-prompts/blob/master/README.md)
 
 better-rich-prompts is a Python extension library for [Rich](https://github.com/Textualize/rich).
@@ -54,24 +54,24 @@
 choices = [
     {"name": "english", "language_code": "en"},
     {"name": "spanish", "language_code": "es"},
     {"name":"french","language_code":"fr"},
 ]
 ListPrompt.ask("Select a language", choices, choice_key="name")
 ```
-![ListPrompt Example](https://github.com/EwenLo/better-rich-prompts/raw/master/imgs/list_prompt_ex1.png)
+![ListPrompt Example](https://raw.githubusercontent.com/EwenLo/better-rich-prompts/main/imgs/dict_prompt_ex1.png)
 
 ### Example 2 - Using list of strings
 ```python
 from better_rich_prompts.prompt import ListPrompt
 
 choices = ["en", "es", "fr"]
 ListPrompt.ask("Select a language", choices,default="en")
 ```
-![ListPrompt Example](https://github.com/EwenLo/better-rich-prompts/raw/master/imgs/list_prompt_ex2.png)
+![ListPrompt Example](https://raw.githubusercontent.com/EwenLo/better-rich-prompts/main/imgs/list_prompt_ex2.png)
 
 ### Example 3 - Using list of custom objects
 ```python
 from better_rich_prompts.prompt import ListPrompt
 
 class Language:
     def __init__(self, name, code):
@@ -84,18 +84,18 @@
     Language("spanish", "es"),
     Language("french", "fr"),
 ]
 ListPrompt.ask(
     "Select a language", choices, default="en", choice_key=lambda c: c.code
 )
 ```
-![ListPrompt Example](https://github.com/EwenLo/better-rich-prompts/raw/master/imgs/list_prompt_ex3.png)
+![ListPrompt Example](https://raw.githubusercontent.com/EwenLo/better-rich-prompts/main/imgs/list_prompt_ex3.png)
 
 ## Using Dict Prompt
 ```python
 from better_rich_prompts.prompt import DictPrompt
 
 choices = {"en":"english","es":"spanish","fr":"french"}
 DictPrompt.ask("Select a language", choices)
 ```
-![ListPrompt Example](https://github.com/EwenLo/better-rich-prompts/raw/master/imgs/dict_prompt_ex1.png)
+![ListPrompt Example](https://raw.githubusercontent.com/EwenLo/better-rich-prompts/main/imgs/dict_prompt_ex1.png)
```

