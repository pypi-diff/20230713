# Comparing `tmp/freeGPT-1.2.2.tar.gz` & `tmp/freeGPT-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.2.2.tar", last modified: Sat Jul  1 09:45:48 2023, max compression
+gzip compressed data, was "freeGPT-1.2.3.tar", last modified: Thu Jul 13 11:19:43 2023, max compression
```

## Comparing `freeGPT-1.2.2.tar` & `freeGPT-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 09:45:48.898915 freeGPT-1.2.2/
--rw-rw-rw-   0        0        0    35149 2023-07-01 09:45:08.000000 freeGPT-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3648 2023-07-01 09:45:48.897917 freeGPT-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2355 2023-07-01 09:45:08.000000 freeGPT-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 09:45:48.870911 freeGPT-1.2.2/freeGPT/
--rw-rw-rw-   0        0        0      120 2023-07-01 09:45:08.000000 freeGPT-1.2.2/freeGPT/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-07-01 09:45:08.000000 freeGPT-1.2.2/freeGPT/alpaca_7b.py
--rw-rw-rw-   0        0        0     1955 2023-07-01 09:45:08.000000 freeGPT-1.2.2/freeGPT/gpt3.py
--rw-rw-rw-   0        0        0     4647 2023-07-01 09:45:08.000000 freeGPT-1.2.2/freeGPT/gpt4.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:45:48.896912 freeGPT-1.2.2/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3648 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 09:45:48.899912 freeGPT-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1676 2023-07-01 09:45:08.000000 freeGPT-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:19:43.392366 freeGPT-1.2.3/
+-rw-rw-rw-   0        0        0    18092 2023-07-13 11:17:19.000000 freeGPT-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3637 2023-07-13 11:19:43.391366 freeGPT-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2356 2023-07-13 11:17:19.000000 freeGPT-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 11:19:43.345396 freeGPT-1.2.3/freeGPT/
+-rw-rw-rw-   0        0        0      120 2023-07-13 11:17:20.000000 freeGPT-1.2.3/freeGPT/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-07-13 11:17:20.000000 freeGPT-1.2.3/freeGPT/alpaca_7b.py
+-rw-rw-rw-   0        0        0     2087 2023-07-13 11:17:20.000000 freeGPT-1.2.3/freeGPT/gpt3.py
+-rw-rw-rw-   0        0        0     4647 2023-07-13 11:17:20.000000 freeGPT-1.2.3/freeGPT/gpt4.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:19:43.389368 freeGPT-1.2.3/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3637 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 11:19:43.000000 freeGPT-1.2.3/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 11:19:43.393366 freeGPT-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1670 2023-07-13 11:17:19.000000 freeGPT-1.2.3/setup.py
```

### Comparing `freeGPT-1.2.2/PKG-INFO` & `freeGPT-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.2
+Version: 1.2.3
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
-License: GPLv3
+License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
-Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
-Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt4,gpt3,gpt,ai
+Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
@@ -34,49 +34,50 @@
 
 ## Get started:
 
 ```
 py -m pip install --upgrade freeGPT
 ```
 
-**Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)!**
+**Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
 | gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
 
 ## Support this repository:
 
 - Star this repository :D
-- Add the [freeGPT Discord bot](https://dsc.gg/freeGPT).
+- Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## TODO List:
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
 - [x] Make the overall library easier to understand.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
+- [x] Make a ChatUI.
 - [ ] Add an image generation model.
 
 ## Discord bot:
 
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - This bot has all the models in this repository available.
 - It's interactive, overall fast, and easy to use.
-- And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot).
+- And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
 ```python
 import freeGPT
 import asyncio
```

### Comparing `freeGPT-1.2.2/README.md` & `freeGPT-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,49 +8,50 @@
 
 ## Get started:
 
 ```
 py -m pip install --upgrade freeGPT
 ```
 
-**Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)!**
+**Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
 | gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
 
 ## Support this repository:
 
 - Star this repository :D
-- Add the [freeGPT Discord bot](https://dsc.gg/freeGPT).
+- Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## TODO List:
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
 - [x] Make the overall library easier to understand.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
+- [x] Make a ChatUI.
 - [ ] Add an image generation model.
 
 ## Discord bot:
 
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - This bot has all the models in this repository available.
 - It's interactive, overall fast, and easy to use.
-- And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot).
+- And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
 ```python
 import freeGPT
 import asyncio
```

### Comparing `freeGPT-1.2.2/freeGPT/alpaca_7b.py` & `freeGPT-1.2.3/freeGPT/alpaca_7b.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests
+from requests import post, exceptions
 from fake_useragent import UserAgent
 
 
 class Completion:
     """
     A class for generating text completions using an API.
 
@@ -23,15 +23,15 @@
         Returns:
             str: The generated text completion.
 
         Raises:
             Exception: If there is an error fetching the response from the API.
         """
         try:
-            resp = requests.post(
+            resp = post(
                 "https://us-central1-arched-keyword-306918.cloudfunctions.net/run-inference-1",
                 headers={
                     "Origin": "https://chatllama.baseten.co",
                     "Referer": "https://chatllama.baseten.co/",
                     "Accept": "application/json, text/plain, */*",
                     "Accept-Encoding": "gzip, deflate, br",
                     "Accept-Language": "en-US,en;q=0.9",
@@ -42,12 +42,13 @@
                     "Sec-Ch-Ua-Platform": "Windows",
                     "Sec-Fetch-Dest": "empty",
                     "Sec-Fetch-Mode": "cors",
                     "Sec-Fetch-Site": "cross-site",
                     "User-Agent": UserAgent().random,
                 },
                 json={"prompt": prompt},
+                timeout=30,
             ).json()
-        except requests.exceptions.RequestException:
+        except exceptions.RequestException:
             raise Exception("Unable to fetch the response.")
 
         return resp["completion"]
```

### Comparing `freeGPT-1.2.2/freeGPT/gpt3.py` & `freeGPT-1.2.3/freeGPT/gpt3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,60 @@
-import json
-import requests
+from json import loads, JSONDecodeError
+from requests import post, exceptions
 
 
 class Completion:
+    """
+    This class provides methods for generating completions based on prompts.
+    """
+
     async def create(prompt):
         """
         Create a new completion based on the given prompt.
 
         Args:
             prompt (str): The prompt to generate a completion for.
 
         Returns:
             str: The generated completion.
 
         Raises:
             Exception: If unable to fetch the response.
         """
         try:
-            session = requests.Session()
-            resp_obj = session.post(
+            resp_obj = post(
                 "https://ava-alpha-api.codelink.io/api/chat",
                 headers={"Content-Type": "application/json"},
                 json={
                     "model": "gpt-4",
                     "temperature": 0.6,
                     "stream": True,
                     "messages": [
                         {"role": "system", "content": "You are Ava, an AI assistant."},
                         {"role": "user", "content": prompt},
                     ],
                 },
+                timeout=30,
             )
-        except Exception:
+        except exceptions.RequestException:
             raise Exception("Unable to fetch the response.")
+
         resp = ""
         for line in resp_obj.iter_lines():
             line_text = line.decode("utf-8").strip()
             if line_text.startswith("data:"):
                 data = line_text.split("data:")[1]
                 try:
-                    data_json = json.loads(data)
+                    data_json = loads(data)
                     if "choices" in data_json:
                         choices = data_json["choices"]
                         for choice in choices:
                             if (
                                 "finish_reason" in choice
                                 and choice["finish_reason"] == "stop"
                             ):
                                 break
                             if "delta" in choice and "content" in choice["delta"]:
                                 resp += choice["delta"]["content"]
-                except json.JSONDecodeError:
+                except JSONDecodeError:
                     pass
         return resp
```

### Comparing `freeGPT-1.2.2/freeGPT/gpt4.py` & `freeGPT-1.2.3/freeGPT/gpt4.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.2/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.2.3/freeGPT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.2
+Version: 1.2.3
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
-License: GPLv3
+License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
-Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
-Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt4,gpt3,gpt,ai
+Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
@@ -34,49 +34,50 @@
 
 ## Get started:
 
 ```
 py -m pip install --upgrade freeGPT
 ```
 
-**Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)!**
+**Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
 | gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
 
 ## Support this repository:
 
 - Star this repository :D
-- Add the [freeGPT Discord bot](https://dsc.gg/freeGPT).
+- Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## TODO List:
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
 - [x] Make the overall library easier to understand.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
+- [x] Make a ChatUI.
 - [ ] Add an image generation model.
 
 ## Discord bot:
 
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - This bot has all the models in this repository available.
 - It's interactive, overall fast, and easy to use.
-- And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot).
+- And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
 ```python
 import freeGPT
 import asyncio
```

### Comparing `freeGPT-1.2.2/setup.py` & `freeGPT-1.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.2.2",
+    version="1.2.3",
     description="freeGPT provides free access to GPT3, GPT4 and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
-    license="GPLv3",
+    license="GPLv2",
     keywords=[
         "artificial-intelligence",
         "machine-learning",
         "deep-learning",
         "gpt4free",
+        "gpt4all",
         "chatbot",
         "freegpt",
         "chatgpt",
         "python",
         "openai",
         "llama",
         "free",
-        "gpt4",
-        "gpt3",
         "gpt",
         "ai",
     ],
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    packages=find_packages(),
+    packages=find_packages(exclude=[".github"]),
     install_requires=[
         "requests",
         "fake-useragent",
     ],
     project_urls={
         "Source": "https://github.com/Ruu3f/freeGPT",
-        "Issues": "https://github.com/Ruu3f/freeGPT/issues",
         "Discord": "https://discord.gg/XH6pUGkwRr",
     },
 )
```

