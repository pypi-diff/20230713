# Comparing `tmp/chatarena-0.1.8.dev0.tar.gz` & `tmp/chatarena-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatarena-0.1.8.dev0.tar", last modified: Fri Apr 14 21:18:39 2023, max compression
+gzip compressed data, was "chatarena-0.1.9.tar", last modified: Tue May  9 19:59:29 2023, max compression
```

## Comparing `chatarena-0.1.8.dev0.tar` & `chatarena-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.783217 chatarena-0.1.8.dev0/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11404 2023-04-03 15:56:48.000000 chatarena-0.1.8.dev0/LICENSE
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    12435 2023-04-14 21:18:39.782875 chatarena-0.1.8.dev0/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11837 2023-04-14 21:15:02.000000 chatarena-0.1.8.dev0/README.md
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.774672 chatarena-0.1.8.dev0/chatarena/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        0 2023-04-03 15:56:48.000000 chatarena-0.1.8.dev0/chatarena/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4899 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/agent.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     6690 2023-04-14 21:14:59.000000 chatarena-0.1.8.dev0/chatarena/arena.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.779924 chatarena-0.1.8.dev0/chatarena/backends/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      749 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/backends/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3869 2023-04-14 21:14:59.000000 chatarena-0.1.8.dev0/chatarena/backends/anthropic.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1337 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/backends/base.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4088 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/backends/cohere.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3613 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/backends/hf_transformers.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      669 2023-04-04 12:55:00.000000 chatarena-0.1.8.dev0/chatarena/backends/human.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3656 2023-04-14 21:14:59.000000 chatarena-0.1.8.dev0/chatarena/backends/openai.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4839 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/config.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4671 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/database.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.782457 chatarena-0.1.8.dev0/chatarena/environments/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      700 2023-04-06 00:43:37.000000 chatarena-0.1.8.dev0/chatarena/environments/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2647 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/environments/base.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11463 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/environments/chameleon.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     6153 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/environments/conversation.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4757 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/environments/pettingzoo_chess.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2794 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/message.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      827 2023-04-03 15:56:48.000000 chatarena-0.1.8.dev0/chatarena/utils.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.776788 chatarena-0.1.8.dev0/chatarena.egg-info/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    12435 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      745 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/SOURCES.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/dependency_links.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      111 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/requires.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       10 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/top_level.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      608 2023-04-14 21:17:28.000000 chatarena-0.1.8.dev0/pyproject.toml
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2023-04-14 21:18:39.783301 chatarena-0.1.8.dev0/setup.cfg
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      871 2023-04-14 21:18:19.000000 chatarena-0.1.8.dev0/setup.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-05-09 19:59:29.861000 chatarena-0.1.9/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11404 2023-04-20 11:55:19.000000 chatarena-0.1.9/LICENSE
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    13411 2023-05-09 19:59:29.860458 chatarena-0.1.9/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    12818 2023-05-09 19:52:17.000000 chatarena-0.1.9/README.md
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-05-09 19:59:29.846066 chatarena-0.1.9/chatarena/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        0 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     5800 2023-05-09 19:52:17.000000 chatarena-0.1.9/chatarena/agent.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     6730 2023-05-09 19:52:17.000000 chatarena-0.1.9/chatarena/arena.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-05-09 19:59:29.854480 chatarena-0.1.9/chatarena/backends/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      749 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/backends/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3888 2023-05-09 19:52:17.000000 chatarena-0.1.9/chatarena/backends/anthropic.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1626 2023-05-09 19:52:17.000000 chatarena-0.1.9/chatarena/backends/base.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4088 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/backends/cohere.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3613 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/backends/hf_transformers.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      669 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/backends/human.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     5980 2023-05-09 19:52:17.000000 chatarena-0.1.9/chatarena/backends/openai.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4839 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/config.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4671 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/database.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-05-09 19:59:29.859664 chatarena-0.1.9/chatarena/environments/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      779 2023-05-09 19:52:17.000000 chatarena-0.1.9/chatarena/environments/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2647 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/environments/base.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11463 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/environments/chameleon.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     6153 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/environments/conversation.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4757 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/environments/pettingzoo_chess.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4197 2023-05-09 19:52:17.000000 chatarena-0.1.9/chatarena/environments/pettingzoo_tictactoe.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2843 2023-05-09 19:52:17.000000 chatarena-0.1.9/chatarena/message.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      827 2023-04-20 11:55:19.000000 chatarena-0.1.9/chatarena/utils.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-05-09 19:59:29.849341 chatarena-0.1.9/chatarena.egg-info/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    13411 2023-05-09 19:59:29.000000 chatarena-0.1.9/chatarena.egg-info/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      792 2023-05-09 19:59:29.000000 chatarena-0.1.9/chatarena.egg-info/SOURCES.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2023-05-09 19:59:29.000000 chatarena-0.1.9/chatarena.egg-info/dependency_links.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      166 2023-05-09 19:59:29.000000 chatarena-0.1.9/chatarena.egg-info/requires.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       10 2023-05-09 19:59:29.000000 chatarena-0.1.9/chatarena.egg-info/top_level.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      603 2023-05-09 19:52:17.000000 chatarena-0.1.9/pyproject.toml
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2023-05-09 19:59:29.861130 chatarena-0.1.9/setup.cfg
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      943 2023-05-09 19:52:17.000000 chatarena-0.1.9/setup.py
```

### Comparing `chatarena-0.1.8.dev0/LICENSE` & `chatarena-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/PKG-INFO` & `chatarena-0.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: chatarena
-Version: 0.1.8.dev0
-Summary: Multi-Agent Language Game Environments for LLMs
-Home-page: https://github.com/chatarena/chatarena
-Author: Yuxiang Wu
-Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
-Project-URL: Homepage, https://github.com/chatarena/chatarena
-Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!--
   Title: Chat Arena
   Description: Chat Arena (or ChatArena) is a language game environment for Large Language Models (LLMs) like GPT-3, GPT-4, ChatGPT, etc.
   Author: Yuxiang Wu
   -->
 
 <h1 align="center"> 🏟 <span style="color:orange">ChatArena</span> </h1>
@@ -31,24 +15,24 @@
 [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
 [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
 [![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 
 ---
 
-ChatArena is a Python library designed to facilitate communication and collaboration between multiple Large Language
-Models (LLMs).
+ChatArena is a library that provides multi-agent language game environments and facilitates research about autonomous
+LLM agents and their social interactions.
 It provides the following features:
 
-- **Language Game Environments**: it provides a framework for creating multi-agent language game environments and a set
-  of general-purposed language-driven environments.
-- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents and
-  enables seamless communication between them.
-- **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
-  engineer) your LLM players to succeed in the environment.
+- **Abstraction**: it provides a flexible framework to define multiple players, environments and the interactions
+  between them, based on Markov Decision Process.
+- **Language Game Environments**: it provides a set of environments that can help understanding, benchmarking or
+  training agent LLMs.
+- **User-friendly Interfaces**: it provides both Web UI and CLI to develop/prompt engineer your LLM agents to act in
+  environments.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
 **Try our online demo:**
 [![demo](https://img.shields.io/badge/Demo-Huggingface%F0%9F%A4%97%20Space-orange?style=flat)](https://chatarena-chatarena-demo.hf.space)
@@ -85,36 +69,36 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena, and you can access it from your browser.
+This will launch a demo server for ChatArena, and you can access it from your browser (port 8080).
 
 [//]: # (The interface looks like this:)
 
 [//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
 
 Check out this video to learn how to use Web
 UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ## Basic Usage
 
 ### Key Concepts
 
-- **Player**: a player is an agent that can interact with other players in a game environment. A player is defined by
-  its name, its backend, and its role description.
-    - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
-      backend can be a human, a remote or local LLM, or any program you create.
-- **Environment**: an environment is a class that defines the rules of a game and the game state transition.
-    - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
-      define game environments using an LLM.
-- **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
-  run the game and save the game history, and interact with the game via the Web UI or CLI.
+1. **Arena**: Arena encapsulates an environment and a collection of players. It drives the main loop of the game and
+   provides HCI utilities like webUI, CLI, configuration loading and data storage.
+2. **Environment**: The environment stores the game state and executes game logics to make transitions between game
+   states. It also renders observations for players, the observations are natural languages.
+    1. The game state is not directly visible to the players. Players can only see the observations.
+3. **Language Backend**: Language backends are the source of language intelligence. It takes text (or collection of
+   text) as input and returns text in response.
+4. **Player**: The player is an agent that plays the game. In RL terminology, it’s a policy, a stateless function
+   mapping from observations to actions.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -208,26 +192,38 @@
 # Tic-tac-toe example
 Arena.from_config("examples/tic-tac-toe.json").launch_cli()
 
 # Rock-paper-scissors example
 Arena.from_config("examples/rock-paper-scissors.json").launch_cli()
 ```
 
+### General Custimization Guide
+
+1. **Arena**: Overriding Arena basically means one is going to write their own main loop. This can allow different
+   interaction interfaces or drive games in a more automated manner, for example, running an online RL training loop
+2. **Environment**: A new environment corresponds to a new game, one can define the game dynamics here with hard-coded
+   rules or a mixture of rules and language backend.
+3. **Backend**: If one needs to change the way of formatting observations (in terms of messages) into queries for the
+   language model, the backend should be overridden.
+4. **Player**: By default, when a new observation is fed, players will query the language backend and return the
+   response as actions. But one can also customize the way that players are interacting with the language backend.
+
 ### Creating your Custom Environment
 
 You can define your own environment by extending the `Environment` class. Here are the general steps:
 
 1. Define the class by inheriting from a base class and setting `type_name`, then add the class
    to [`ALL_ENVIRONMENTS`](chatarena/environments/__init__.py#L17)
 2. Initialize the class by defining `__init__` method (its arguments will define the corresponding config) and
    initializing class attributes
 3. Implement game mechanics in methods `step`
 4. Handle game states and rewards by implementing methods such as `reset`, `get_observation`, `is_terminal`,
    and `get_rewards`
-5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to a
+5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to
+   a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
 If you want to port an existing library's environment to ChatArena, check
@@ -294,27 +290,34 @@
 Please ensure your code follows the existing style and structure.
 
 ## Citation
 
 If you find ChatArena useful for your research, please cite our repository (our arxiv paper is coming soon):
 
 ```bibtex
-@misc{ChatArena,
+@software{ChatArena,
   author = {Yuxiang Wu, Zhengyao Jiang, Akbir Khan, Yao Fu, Laura Ruis, Edward Grefenstette, and Tim Rocktäschel},
   title = {ChatArena: Multi-Agent Language Game Environments for Large Language Models},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
+  version = {0.1},
   howpublished = {\url{https://github.com/chatarena/chatarena}},
 }
 ```
 
 ## Contact
 
 If you have any questions or suggestions, feel free to open an issue or submit a pull request.
 You can also follow us on [Twitter](https://twitter.com/_chatarena) or
 join [our Slack channel](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 to get the latest updates.
 
 Happy chatting!
 
+## Sponsors
+
+We would like to thank our sponsors for supporting this project:
+
+- [SEQUOIA](https://www.sequoiacap.com/)
+- [Shixiang Capital](https://sx.shixiangcap.com/home)
```

### Comparing `chatarena-0.1.8.dev0/README.md` & `chatarena-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: chatarena
+Version: 0.1.9
+Summary: Multi-Agent Language Game Environments for LLMs
+Home-page: https://github.com/chatarena/chatarena
+Author: Yuxiang Wu
+Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
+Project-URL: Homepage, https://github.com/chatarena/chatarena
+Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!--
   Title: Chat Arena
   Description: Chat Arena (or ChatArena) is a language game environment for Large Language Models (LLMs) like GPT-3, GPT-4, ChatGPT, etc.
   Author: Yuxiang Wu
   -->
 
 <h1 align="center"> 🏟 <span style="color:orange">ChatArena</span> </h1>
@@ -15,24 +31,24 @@
 [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
 [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
 [![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 
 ---
 
-ChatArena is a Python library designed to facilitate communication and collaboration between multiple Large Language
-Models (LLMs).
+ChatArena is a library that provides multi-agent language game environments and facilitates research about autonomous
+LLM agents and their social interactions.
 It provides the following features:
 
-- **Language Game Environments**: it provides a framework for creating multi-agent language game environments and a set
-  of general-purposed language-driven environments.
-- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents and
-  enables seamless communication between them.
-- **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
-  engineer) your LLM players to succeed in the environment.
+- **Abstraction**: it provides a flexible framework to define multiple players, environments and the interactions
+  between them, based on Markov Decision Process.
+- **Language Game Environments**: it provides a set of environments that can help understanding, benchmarking or
+  training agent LLMs.
+- **User-friendly Interfaces**: it provides both Web UI and CLI to develop/prompt engineer your LLM agents to act in
+  environments.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
 **Try our online demo:**
 [![demo](https://img.shields.io/badge/Demo-Huggingface%F0%9F%A4%97%20Space-orange?style=flat)](https://chatarena-chatarena-demo.hf.space)
@@ -69,36 +85,36 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena, and you can access it from your browser.
+This will launch a demo server for ChatArena, and you can access it from your browser (port 8080).
 
 [//]: # (The interface looks like this:)
 
 [//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
 
 Check out this video to learn how to use Web
 UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ## Basic Usage
 
 ### Key Concepts
 
-- **Player**: a player is an agent that can interact with other players in a game environment. A player is defined by
-  its name, its backend, and its role description.
-    - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
-      backend can be a human, a remote or local LLM, or any program you create.
-- **Environment**: an environment is a class that defines the rules of a game and the game state transition.
-    - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
-      define game environments using an LLM.
-- **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
-  run the game and save the game history, and interact with the game via the Web UI or CLI.
+1. **Arena**: Arena encapsulates an environment and a collection of players. It drives the main loop of the game and
+   provides HCI utilities like webUI, CLI, configuration loading and data storage.
+2. **Environment**: The environment stores the game state and executes game logics to make transitions between game
+   states. It also renders observations for players, the observations are natural languages.
+    1. The game state is not directly visible to the players. Players can only see the observations.
+3. **Language Backend**: Language backends are the source of language intelligence. It takes text (or collection of
+   text) as input and returns text in response.
+4. **Player**: The player is an agent that plays the game. In RL terminology, it’s a policy, a stateless function
+   mapping from observations to actions.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -192,26 +208,38 @@
 # Tic-tac-toe example
 Arena.from_config("examples/tic-tac-toe.json").launch_cli()
 
 # Rock-paper-scissors example
 Arena.from_config("examples/rock-paper-scissors.json").launch_cli()
 ```
 
+### General Custimization Guide
+
+1. **Arena**: Overriding Arena basically means one is going to write their own main loop. This can allow different
+   interaction interfaces or drive games in a more automated manner, for example, running an online RL training loop
+2. **Environment**: A new environment corresponds to a new game, one can define the game dynamics here with hard-coded
+   rules or a mixture of rules and language backend.
+3. **Backend**: If one needs to change the way of formatting observations (in terms of messages) into queries for the
+   language model, the backend should be overridden.
+4. **Player**: By default, when a new observation is fed, players will query the language backend and return the
+   response as actions. But one can also customize the way that players are interacting with the language backend.
+
 ### Creating your Custom Environment
 
 You can define your own environment by extending the `Environment` class. Here are the general steps:
 
 1. Define the class by inheriting from a base class and setting `type_name`, then add the class
    to [`ALL_ENVIRONMENTS`](chatarena/environments/__init__.py#L17)
 2. Initialize the class by defining `__init__` method (its arguments will define the corresponding config) and
    initializing class attributes
 3. Implement game mechanics in methods `step`
 4. Handle game states and rewards by implementing methods such as `reset`, `get_observation`, `is_terminal`,
    and `get_rewards`
-5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to a
+5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to
+   a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
 If you want to port an existing library's environment to ChatArena, check
@@ -278,27 +306,34 @@
 Please ensure your code follows the existing style and structure.
 
 ## Citation
 
 If you find ChatArena useful for your research, please cite our repository (our arxiv paper is coming soon):
 
 ```bibtex
-@misc{ChatArena,
+@software{ChatArena,
   author = {Yuxiang Wu, Zhengyao Jiang, Akbir Khan, Yao Fu, Laura Ruis, Edward Grefenstette, and Tim Rocktäschel},
   title = {ChatArena: Multi-Agent Language Game Environments for Large Language Models},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
+  version = {0.1},
   howpublished = {\url{https://github.com/chatarena/chatarena}},
 }
 ```
 
 ## Contact
 
 If you have any questions or suggestions, feel free to open an issue or submit a pull request.
 You can also follow us on [Twitter](https://twitter.com/_chatarena) or
 join [our Slack channel](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 to get the latest updates.
 
 Happy chatting!
 
+## Sponsors
+
+We would like to thank our sponsors for supporting this project:
+
+- [SEQUOIA](https://www.sequoiacap.com/)
+- [Shixiang Capital](https://sx.shixiangcap.com/home)
```

### Comparing `chatarena-0.1.8.dev0/chatarena/agent.py` & `chatarena-0.1.9/chatarena/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Union
 import re
 from tenacity import RetryError
 import logging
 import uuid
 from abc import abstractmethod
+import asyncio
 
 from .backends import IntelligenceBackend, load_backend
 from .message import Message, SYSTEM_NAME
 from .config import AgentConfig, Configurable, BackendConfig
 
 # A special signal sent by the player to indicate that it is not possible to continue the conversation, and it requests to end the conversation.
 # It contains a random UUID string to avoid being exploited by any of the players.
@@ -52,29 +53,48 @@
         return AgentConfig(
             name=self.name,
             role_desc=self.role_desc,
             backend=self.backend.to_config(),
             global_prompt=self.global_prompt,
         )
 
-    def __call__(self, observation: List[Message]) -> str:
+    def act(self, observation: List[Message]) -> str:
         """
         Call the agents to generate a response (equivalent to taking an action).
         """
         try:
             response = self.backend.query(agent_name=self.name, role_desc=self.role_desc,
                                           history_messages=observation, global_prompt=self.global_prompt,
                                           request_msg=None)
         except RetryError as e:
             logging.warning(f"Agent {self.name} failed to generate a response. "
                             f"Error: {e.last_attempt.exception()}. "
                             f"Sending signal to end the conversation.")
             response = SIGNAL_END_OF_CONVERSATION
 
         return response
+
+    def __call__(self, observation: List[Message]) -> str:
+        return self.act(observation)
+
+    async def async_act(self, observation: List[Message]) -> str:
+        """
+        Async call the agents to generate a response (equivalent to taking an action).
+        """
+        try:
+            response = self.backend.async_query(agent_name=self.name, role_desc=self.role_desc,
+                                                history_messages=observation, global_prompt=self.global_prompt,
+                                                request_msg=None)
+        except RetryError as e:
+            logging.warning(f"Agent {self.name} failed to generate a response. "
+                            f"Error: {e.last_attempt.exception()}. "
+                            f"Sending signal to end the conversation.")
+            response = SIGNAL_END_OF_CONVERSATION
+
+        return response
 
     def reset(self):
         self.backend.reset()
 
 
 class Moderator(Player):
     """
```

### Comparing `chatarena-0.1.8.dev0/chatarena/arena.py` & `chatarena-0.1.9/chatarena/arena.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,18 @@
         player_name = self.environment.get_next_player()
         player = self.name_to_player[player_name]  # get the player object
         observation = self.environment.get_observation(player_name)  # get the observation for the player
 
         timestep = None
         for i in range(self.invalid_actions_retry):  # try to take an action for a few times
             action = player(observation)  # take an action
-            if self.environment.check_action(action, player_name):
+            if self.environment.check_action(action, player_name):  # action is valid
                 timestep = self.environment.step(player_name, action)  # update the environment
                 break
-            else:
+            else:  # action is invalid
                 logging.warning(f"{player_name} made an invalid action {action}")
                 continue
 
         if timestep is None:  # if the player made invalid actions for too many times, terminate the game
             warning_msg = f"{player_name} has made invalid actions for {self.invalid_actions_retry} times. Terminating the game."
             logging.warning(warning_msg)
             raise TooManyInvalidActions(warning_msg)
```

### Comparing `chatarena-0.1.8.dev0/chatarena/backends/__init__.py` & `chatarena-0.1.9/chatarena/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/backends/anthropic.py` & `chatarena-0.1.9/chatarena/backends/anthropic.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,22 +57,22 @@
         """
         format the input and call the Claude API
         args:
             agent_name: the name of the agent
             role_desc: the description of the role of the agent
             env_desc: the description of the environment
             history_messages: the history of the conversation, or the observation for the agent
-            request_msg: the request for the chatGPT
+            request_msg: the request from the system to guide the agent's next response
         """
         all_messages = [(SYSTEM, global_prompt), (SYSTEM, role_desc)] if global_prompt else [(SYSTEM, role_desc)]
 
         for message in history_messages:
             all_messages.append((message.agent_name, message.content))
         if request_msg:
-            all_messages.append((request_msg.agent_name, request_msg.content))
+            all_messages.append((SYSTEM, request_msg.content))
 
         prompt = ""
         prev_is_human = False  # Whether the previous message is from human (in anthropic, the human is the user)
         for i, message in enumerate(all_messages):
             if i == 0:
                 assert message[0] == SYSTEM  # The first message should be from the system
```

### Comparing `chatarena-0.1.8.dev0/chatarena/backends/base.py` & `chatarena-0.1.9/chatarena/backends/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,13 +26,19 @@
         return BackendConfig(**self._config_dict)
 
     @abstractmethod
     def query(self, agent_name: str, role_desc: str, history_messages: List[Message], global_prompt: str = None,
               request_msg: Message = None, *args, **kwargs) -> str:
         raise NotImplementedError
 
+    @abstractmethod
+    async def async_query(self, agent_name: str, role_desc: str, history_messages: List[Message],
+                          global_prompt: str = None, request_msg: Message = None, *args, **kwargs) -> str:
+        """Async querying"""
+        raise NotImplementedError
+
     # reset the state of the backend
     def reset(self):
         if self.stateful:
             raise NotImplementedError
         else:
             pass
```

### Comparing `chatarena-0.1.8.dev0/chatarena/backends/cohere.py` & `chatarena-0.1.9/chatarena/backends/cohere.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/backends/hf_transformers.py` & `chatarena-0.1.9/chatarena/backends/hf_transformers.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/backends/human.py` & `chatarena-0.1.9/chatarena/backends/human.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/config.py` & `chatarena-0.1.9/chatarena/config.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/database.py` & `chatarena-0.1.9/chatarena/database.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/environments/__init__.py` & `chatarena-0.1.9/chatarena/environments/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from .base import Environment, TimeStep
 from .conversation import Conversation, ModeratedConversation
 from .chameleon import Chameleon
 from .pettingzoo_chess import PettingzooChess
+from .pettingzoo_tictactoe import PettingzooTicTacToe
 
 from ..config import EnvironmentConfig
 
 ALL_ENVIRONMENTS = [
     Conversation,
     ModeratedConversation,
     Chameleon,
     PettingzooChess,
+    PettingzooTicTacToe,
 ]
 
 ENV_REGISTRY = {env.type_name: env for env in ALL_ENVIRONMENTS}
 
 
 # Load an environment from a config dictionary
 def load_environment(config: EnvironmentConfig):
```

### Comparing `chatarena-0.1.8.dev0/chatarena/environments/base.py` & `chatarena-0.1.9/chatarena/environments/base.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/environments/chameleon.py` & `chatarena-0.1.9/chatarena/environments/chameleon.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/environments/conversation.py` & `chatarena-0.1.9/chatarena/environments/conversation.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/environments/pettingzoo_chess.py` & `chatarena-0.1.9/chatarena/environments/pettingzoo_chess.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena/message.py` & `chatarena-0.1.9/chatarena/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import List, Union
 from dataclasses import dataclass
 import time
 from uuid import uuid1
 import hashlib
 
+# Preserved roles
+SYSTEM_NAME = "System"
+MODERATOR_NAME = "Moderator"
 
-SYSTEM_NAME="System"
 
 def _hash(input: str):
     hex_dig = hashlib.sha256(input.encode()).hexdigest()
     return hex_dig
 
 
 @dataclass
```

### Comparing `chatarena-0.1.8.dev0/chatarena/utils.py` & `chatarena-0.1.9/chatarena/utils.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8.dev0/chatarena.egg-info/PKG-INFO` & `chatarena-0.1.9/chatarena.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatarena
-Version: 0.1.8.dev0
+Version: 0.1.9
 Summary: Multi-Agent Language Game Environments for LLMs
 Home-page: https://github.com/chatarena/chatarena
 Author: Yuxiang Wu
 Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
 Project-URL: Homepage, https://github.com/chatarena/chatarena
 Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
 Classifier: Programming Language :: Python :: 3
@@ -31,24 +31,24 @@
 [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
 [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
 [![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 
 ---
 
-ChatArena is a Python library designed to facilitate communication and collaboration between multiple Large Language
-Models (LLMs).
+ChatArena is a library that provides multi-agent language game environments and facilitates research about autonomous
+LLM agents and their social interactions.
 It provides the following features:
 
-- **Language Game Environments**: it provides a framework for creating multi-agent language game environments and a set
-  of general-purposed language-driven environments.
-- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents and
-  enables seamless communication between them.
-- **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
-  engineer) your LLM players to succeed in the environment.
+- **Abstraction**: it provides a flexible framework to define multiple players, environments and the interactions
+  between them, based on Markov Decision Process.
+- **Language Game Environments**: it provides a set of environments that can help understanding, benchmarking or
+  training agent LLMs.
+- **User-friendly Interfaces**: it provides both Web UI and CLI to develop/prompt engineer your LLM agents to act in
+  environments.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
 **Try our online demo:**
 [![demo](https://img.shields.io/badge/Demo-Huggingface%F0%9F%A4%97%20Space-orange?style=flat)](https://chatarena-chatarena-demo.hf.space)
@@ -85,36 +85,36 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena, and you can access it from your browser.
+This will launch a demo server for ChatArena, and you can access it from your browser (port 8080).
 
 [//]: # (The interface looks like this:)
 
 [//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
 
 Check out this video to learn how to use Web
 UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ## Basic Usage
 
 ### Key Concepts
 
-- **Player**: a player is an agent that can interact with other players in a game environment. A player is defined by
-  its name, its backend, and its role description.
-    - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
-      backend can be a human, a remote or local LLM, or any program you create.
-- **Environment**: an environment is a class that defines the rules of a game and the game state transition.
-    - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
-      define game environments using an LLM.
-- **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
-  run the game and save the game history, and interact with the game via the Web UI or CLI.
+1. **Arena**: Arena encapsulates an environment and a collection of players. It drives the main loop of the game and
+   provides HCI utilities like webUI, CLI, configuration loading and data storage.
+2. **Environment**: The environment stores the game state and executes game logics to make transitions between game
+   states. It also renders observations for players, the observations are natural languages.
+    1. The game state is not directly visible to the players. Players can only see the observations.
+3. **Language Backend**: Language backends are the source of language intelligence. It takes text (or collection of
+   text) as input and returns text in response.
+4. **Player**: The player is an agent that plays the game. In RL terminology, it’s a policy, a stateless function
+   mapping from observations to actions.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -208,26 +208,38 @@
 # Tic-tac-toe example
 Arena.from_config("examples/tic-tac-toe.json").launch_cli()
 
 # Rock-paper-scissors example
 Arena.from_config("examples/rock-paper-scissors.json").launch_cli()
 ```
 
+### General Custimization Guide
+
+1. **Arena**: Overriding Arena basically means one is going to write their own main loop. This can allow different
+   interaction interfaces or drive games in a more automated manner, for example, running an online RL training loop
+2. **Environment**: A new environment corresponds to a new game, one can define the game dynamics here with hard-coded
+   rules or a mixture of rules and language backend.
+3. **Backend**: If one needs to change the way of formatting observations (in terms of messages) into queries for the
+   language model, the backend should be overridden.
+4. **Player**: By default, when a new observation is fed, players will query the language backend and return the
+   response as actions. But one can also customize the way that players are interacting with the language backend.
+
 ### Creating your Custom Environment
 
 You can define your own environment by extending the `Environment` class. Here are the general steps:
 
 1. Define the class by inheriting from a base class and setting `type_name`, then add the class
    to [`ALL_ENVIRONMENTS`](chatarena/environments/__init__.py#L17)
 2. Initialize the class by defining `__init__` method (its arguments will define the corresponding config) and
    initializing class attributes
 3. Implement game mechanics in methods `step`
 4. Handle game states and rewards by implementing methods such as `reset`, `get_observation`, `is_terminal`,
    and `get_rewards`
-5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to a
+5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to
+   a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
 If you want to port an existing library's environment to ChatArena, check
@@ -294,27 +306,34 @@
 Please ensure your code follows the existing style and structure.
 
 ## Citation
 
 If you find ChatArena useful for your research, please cite our repository (our arxiv paper is coming soon):
 
 ```bibtex
-@misc{ChatArena,
+@software{ChatArena,
   author = {Yuxiang Wu, Zhengyao Jiang, Akbir Khan, Yao Fu, Laura Ruis, Edward Grefenstette, and Tim Rocktäschel},
   title = {ChatArena: Multi-Agent Language Game Environments for Large Language Models},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
+  version = {0.1},
   howpublished = {\url{https://github.com/chatarena/chatarena}},
 }
 ```
 
 ## Contact
 
 If you have any questions or suggestions, feel free to open an issue or submit a pull request.
 You can also follow us on [Twitter](https://twitter.com/_chatarena) or
 join [our Slack channel](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 to get the latest updates.
 
 Happy chatting!
 
+## Sponsors
+
+We would like to thank our sponsors for supporting this project:
+
+- [SEQUOIA](https://www.sequoiacap.com/)
+- [Shixiang Capital](https://sx.shixiangcap.com/home)
```

### Comparing `chatarena-0.1.8.dev0/chatarena.egg-info/SOURCES.txt` & `chatarena-0.1.9/chatarena.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 chatarena/backends/hf_transformers.py
 chatarena/backends/human.py
 chatarena/backends/openai.py
 chatarena/environments/__init__.py
 chatarena/environments/base.py
 chatarena/environments/chameleon.py
 chatarena/environments/conversation.py
-chatarena/environments/pettingzoo_chess.py
+chatarena/environments/pettingzoo_chess.py
+chatarena/environments/pettingzoo_tictactoe.py
```

### Comparing `chatarena-0.1.8.dev0/pyproject.toml` & `chatarena-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatarena"
-version = "0.1.8.dev0"
+version = "0.1.9"
 authors = [
     { name = "Yuxiang Wu", email = "yuxiang.cs@gmail.com" },
 ]
 description = "Multi-Agent Language Game Environments for LLMs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chatarena-0.1.8.dev0/setup.py` & `chatarena-0.1.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from setuptools import setup, find_packages
 
 _deps = [
-    "cohere>=4.1.0",
-    "openai>=0.27.0",
-    "gradio>=3.20.0",
-    "transformers>=4.0",
+    "openai==0.27.2",
+    "anthropic==0.2.6",
+    "cohere==4.3.1",
+    "transformers>=4.27.4",
     "tenacity==8.2.2",
-    "rich>=13.3.1",
-    "prompt_toolkit>=3.0"
+    "gradio==3.20.0",
+    "rich==13.3.3",
+    "prompt_toolkit==3.0.38",
+    "pettingzoo==1.22.3",
+    "chess==1.9.4",
 ]
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 requirements = _deps
 
 setup(
     name="chatarena",
-    version="0.1.8.dev0",
+    version="0.1.9",
     author="Yuxiang Wu",
     author_email="yuxiang.cs@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/chatarena/chatarena",
     packages=find_packages(),
```

