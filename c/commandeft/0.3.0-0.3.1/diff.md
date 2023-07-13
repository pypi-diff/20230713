# Comparing `tmp/commandeft-0.3.0.tar.gz` & `tmp/commandeft-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandeft-0.3.0.tar", last modified: Sun Jun 25 17:16:51 2023, max compression
+gzip compressed data, was "commandeft-0.3.1.tar", last modified: Thu Jul 13 18:28:53 2023, max compression
```

## Comparing `commandeft-0.3.0.tar` & `commandeft-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,17 @@
--rw-r--r--   0        0        0     1078 2023-06-04 14:54:11.290505 commandeft-0.3.0/LICENSE
--rw-r--r--   0        0        0     3541 2023-06-25 17:10:36.499026 commandeft-0.3.0/README.md
--rw-r--r--   0        0        0       65 2023-06-12 02:20:42.863520 commandeft-0.3.0/commandeft/.pdm-python
--rw-r--r--   0        0        0       40 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/.gitignore
--rw-r--r--   0        0        0     2201 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate
--rw-r--r--   0        0        0     1493 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate.csh
--rw-r--r--   0        0        0     3078 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate.fish
--rw-r--r--   0        0        0     3397 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate.nu
--rw-r--r--   0        0        0     1782 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate.ps1
--rw-r--r--   0        0        0     1211 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/activate_this.py
-lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/python -> /usr/bin/python3.8
-lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/bin/python3.8 -> python
--rw-r--r--   0        0        0       18 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4311 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.py
--rw-r--r--   0        0        0      233 2023-06-12 02:20:42.855520 commandeft-0.3.0/commandeft/.venv/pyvenv.cfg
--rw-r--r--   0        0        0        0 2023-06-04 15:07:15.290389 commandeft-0.3.0/commandeft/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.3.0/commandeft/constants/__init__.py
--rw-r--r--   0        0        0     3234 2023-06-25 17:15:44.889063 commandeft-0.3.0/commandeft/constants/consts.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.3.0/commandeft/core/__init__.py
--rw-r--r--   0        0        0     3696 2023-06-25 17:15:23.200920 commandeft-0.3.0/commandeft/core/cli.py
--rw-r--r--   0        0        0     1391 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/core/decision.py
--rw-r--r--   0        0        0     4904 2023-06-25 17:15:48.693088 commandeft-0.3.0/commandeft/core/generation.py
--rw-r--r--   0        0        0     2131 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/core/history_cache.py
--rw-r--r--   0        0        0      913 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/main.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.3.0/commandeft/util/__init__.py
--rw-r--r--   0        0        0     3637 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/util/config_util.py
--rw-r--r--   0        0        0      370 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/util/gen_util.py
--rw-r--r--   0        0        0     2349 2023-06-25 17:10:36.499026 commandeft-0.3.0/commandeft/util/interactive_util.py
--rw-r--r--   0        0        0     1995 2023-06-25 17:16:51.673502 commandeft-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5453 1970-01-01 00:00:00.000000 commandeft-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-10 01:12:32.215348 commandeft-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3541 2023-07-13 06:12:07.752921 commandeft-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 23:37:24.840096 commandeft-0.3.1/commandeft/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009549 commandeft-0.3.1/commandeft/constants/__init__.py
+-rw-r--r--   0        0        0     3266 2023-07-13 18:28:25.093811 commandeft-0.3.1/commandeft/constants/consts.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009834 commandeft-0.3.1/commandeft/core/__init__.py
+-rw-r--r--   0        0        0     3103 2023-07-13 18:28:25.095039 commandeft-0.3.1/commandeft/core/cli.py
+-rw-r--r--   0        0        0     1391 2023-07-13 06:12:07.757546 commandeft-0.3.1/commandeft/core/decision.py
+-rw-r--r--   0        0        0     5054 2023-07-13 18:28:25.095963 commandeft-0.3.1/commandeft/core/generation.py
+-rw-r--r--   0        0        0     2131 2023-07-13 06:12:07.759538 commandeft-0.3.1/commandeft/core/history_cache.py
+-rw-r--r--   0        0        0      913 2023-07-13 06:12:07.760737 commandeft-0.3.1/commandeft/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.010171 commandeft-0.3.1/commandeft/util/__init__.py
+-rw-r--r--   0        0        0     4933 2023-07-13 18:28:25.097250 commandeft-0.3.1/commandeft/util/config_util.py
+-rw-r--r--   0        0        0      370 2023-07-13 06:12:07.762484 commandeft-0.3.1/commandeft/util/gen_util.py
+-rw-r--r--   0        0        0     2349 2023-07-13 06:12:07.763340 commandeft-0.3.1/commandeft/util/interactive_util.py
+-rw-r--r--   0        0        0     1995 2023-07-13 18:28:53.081965 commandeft-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5453 1970-01-01 00:00:00.000000 commandeft-0.3.1/PKG-INFO
```

### Comparing `commandeft-0.3.0/LICENSE` & `commandeft-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.0/README.md` & `commandeft-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.0/commandeft/constants/consts.py` & `commandeft-0.3.1/commandeft/constants/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 
 CONFIG_FILE_PATH = os.path.join(os.path.expanduser("~"), ".commandeft", "config")
-MAX_TOKENS = 4096
+GPT_3_5_MAX_TOKENS = 4096
+GPT_4_MAX_TOKENS = 8192
 
 init_messages = [
     "What mischief are we up to now?\n Describe the command you're concocting:\n",
     "Oh no, caught in another coding conundrum?\n Share the details:\n",
     "Here to save the day!\n Enlighten me with the command you're grappling with:\n",
     "When your coding journey hits a snag,\n Describe the task that makes you sag:\n",
     "No shame in seeking guidance.\n What command do you need a helping hand with?:\n",
```

### Comparing `commandeft-0.3.0/commandeft/core/decision.py` & `commandeft-0.3.1/commandeft/core/decision.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.0/commandeft/core/generation.py` & `commandeft-0.3.1/commandeft/core/generation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import sys
 import re
 import click
 import openai
 
 
-from commandeft.constants.consts import MAX_TOKENS
 from commandeft.core.history_cache import HistoryCache
 from commandeft.util.config_util import get_configuration
 
+if get_configuration("model") == "gpt-4":
+    from commandeft.constants.consts import GPT_4_MAX_TOKENS as MAX_TOKENS
+else:
+    from commandeft.constants.consts import GPT_3_5_MAX_TOKENS as MAX_TOKENS
+
 
 class Generation:
     def __init__(self, config):
         self.__session_gen_count = 0
         self.__config = config
         self.__history_cache: HistoryCache = config.get("history_cache", HistoryCache(model=self.model))
```

### Comparing `commandeft-0.3.0/commandeft/core/history_cache.py` & `commandeft-0.3.1/commandeft/core/history_cache.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.0/commandeft/main.py` & `commandeft-0.3.1/commandeft/main.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.0/commandeft/util/config_util.py` & `commandeft-0.3.1/commandeft/util/config_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,53 @@
 import os
 import sys
 import json
 from InquirerPy import prompt
 import click
 
-from commandeft.constants.consts import CONFIG_FILE_PATH, MAX_TOKENS
+from commandeft.constants.consts import CONFIG_FILE_PATH
+from commandeft.core.history_cache import HistoryCache
+from commandeft.util.gen_util import get_current_os, get_current_shell
 
 
 def get_configuration(config_property, config_file_path: str = CONFIG_FILE_PATH):
     if os.path.exists(config_file_path):
         with open(config_file_path, "r", encoding="utf-8") as config_file:
             configuration = json.load(config_file)
             return configuration.get(config_property)
     return None
 
 
+def create_generation_config():
+    model = get_configuration("model")
+    current_os = get_current_os()
+    current_shell = get_current_shell()
+    temperature = get_configuration("temperature")
+    max_tokens = get_configuration("max_tokens")
+    interactive_history = get_configuration("interactive_history")
+
+    generation_config = {
+        "model": model,
+        "temperature": temperature,
+        "max_tokens": max_tokens,
+        "interactive_history": interactive_history,
+        "current_os": current_os,
+        "current_shell": current_shell,
+        "history_cache": HistoryCache(model=model),
+    }
+
+    return generation_config
+
+
+if get_configuration("model") == "gpt-4":
+    from commandeft.constants.consts import GPT_4_MAX_TOKENS as MAX_TOKENS
+else:
+    from commandeft.constants.consts import GPT_3_5_MAX_TOKENS as MAX_TOKENS
+
+
 def validate_configuration(config_file_path: str = CONFIG_FILE_PATH):
     required_keys = ["model", "temperature", "max_tokens", "accept_command_behavior"]
 
     if not os.path.exists(config_file_path):
         click.echo(click.style("Configuration file not found.", fg="red"))
         sys.exit(1)
 
@@ -26,73 +55,86 @@
         configuration = json.load(config_file)
 
     for key in required_keys:
         if key not in configuration or configuration[key] is None or configuration[key] == "":
             click.echo(click.style(f"Config Error: Missing or empty value for configuration key: '{key}'", fg="red"))
             sys.exit(1)
 
-    if configuration["temperature"] < 0 or configuration["temperature"] > 1:
+    if configuration["temperature"] < 0 or configuration["temperature"] > 2:
         click.echo(click.style("Config Error: Invalid temperature value in configuration.", fg="red"))
         sys.exit(1)
 
     if not 1 <= configuration["max_tokens"] <= MAX_TOKENS:
         click.echo(click.style("Config Error: Invalid max_tokens value in configuration.", fg="red"))
         sys.exit(1)
 
-    if configuration["model"] not in ["gpt-3.5-turbo", "gpt4"]:
+    if configuration["model"] not in ["gpt-3.5-turbo", "gpt-4"]:
         click.echo(click.style("Config Error: Invalid model value in configuration.", fg="red"))
         sys.exit(1)
 
     if configuration["accept_command_behavior"] not in ["run", "copy"]:
         click.echo(click.style("Config Error: Invalid model value in configuration.", fg="red"))
         sys.exit(1)
 
     return configuration
 
 
+def validate_max_tokens(answers, curr_val):
+    if curr_val == "":
+        return False
+
+    if answers["model"] == "gpt-4":
+        return 1 <= int(curr_val) <= 8192
+
+    return 1 <= int(curr_val) <= 4096
+
+
 def get_configuration_answers():
     # pylint: disable=unnecessary-lambda
-    questions = [
+    model_question = [
         {
             "type": "list",
             "name": "model",
             "message": "Choose the model to be used:\n",
             "choices": ["gpt-3.5-turbo", "gpt-4"],
         },
+    ]
+    model_answer = prompt(model_question)
+    questions = [
         {
             "type": "input",
             "name": "temperature",
-            "message": "Enter the temperature (0-1 with max 2 decimal places):\n",
-            "validate": lambda val: 0 <= float(val) <= 1,
-            "filter": lambda val: float(val),
+            "message": "Enter the temperature (0-2 with max 2 decimal places):\n",
+            "validate": lambda val: False if val == "" else 0 <= float(val) <= 2,
+            "filter": lambda val: False if val == "" else float(val),
+        },
+        {
+            "type": "input",
+            "name": "max_tokens",
+            "message": "Enter max_tokens (gpt-3.5-turbo:[1-4,096], gpt-4:[1-8,192]).:\n",
+            "validate": lambda val: validate_max_tokens(model_answer, val),
+            "filter": lambda val: False if val == "" else int(val),
         },
         {
             "type": "confirm",
             "name": "interactive_history",
             "message": "Would you like interactive mode to keep generation history?\n)",
             "default": True,
         },
         {
-            "type": "input",
-            "name": "max_tokens",
-            "message": "Enter max_tokens [1-4,096].:\n(in interactive mode with history enabled, this value is ignored)\n",
-            "validate": lambda val: 1 <= float(val) <= MAX_TOKENS,
-            "filter": lambda val: int(val),
-        },
-        {
             "type": "password",
             "name": "api_key",
             "message": "Enter your OpenAI API key:\n",
         },
         {
             "type": "list",
             "name": "accept_command_behavior",
             "message": "When accepting a command in interactive mode, would you like to:\n",
             "choices": [
                 {"name": "Copy it to clipboard?", "value": "copy", "short": "copy?"},
                 {"name": "Run it?", "value": "run", "short": "run?"},
             ],
-        }
-        # Add more questions as needed
+        },
     ]
     answers = prompt(questions)
+    answers = {**model_answer, **answers}
     return answers
```

### Comparing `commandeft-0.3.0/commandeft/util/interactive_util.py` & `commandeft-0.3.1/commandeft/util/interactive_util.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.0/pyproject.toml` & `commandeft-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "commandeft"
-version = "0.3.0"
+version = "0.3.1"
 description = "CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models."
 readme = "README.md"
 authors = [
     { name = "Petros Sidirokastritis", email = "sidirope@gmail.com" },
 ]
 requires-python = ">=3.8.1, <=3.11.4"
 dependencies = [
```

### Comparing `commandeft-0.3.0/PKG-INFO` & `commandeft-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandeft
-Version: 0.3.0
+Version: 0.3.1
 Summary: CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models.
 Keywords: commandeft cli tool shell commands prompt-based command generation natural language prompts shell commands shell scripts shell command generation intelligent code generation language-to-code conversion developer-friendly simplified scripting code efficiency streamline workflow intelligent suggestions efficient command composition gpt-3.5-turbo gpt-4 shell command suggestion interactive mode guided prompt command execution
 Author-Email: Petros Sidirokastritis <sidirope@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Ferrum-Citadel/commandeft
 Requires-Python: <=3.11.4,>=3.8.1
 Requires-Dist: PyJWT==2.7.0
```

