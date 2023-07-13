# Comparing `tmp/threads-api-1.1.4.tar.gz` & `tmp/threads-api-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.1.4.tar", last modified: Wed Jul 12 20:15:23 2023, max compression
+gzip compressed data, was "threads-api-1.1.5.tar", last modified: Thu Jul 13 21:53:15 2023, max compression
```

## Comparing `threads-api-1.1.4.tar` & `threads-api-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.4/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13446 2023-07-12 20:15:23.084892 threads-api-1.1.4/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12916 2023-07-12 20:11:18.000000 threads-api-1.1.4/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      452 2023-07-12 20:11:18.000000 threads-api-1.1.4/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-12 20:15:23.084892 threads-api-1.1.4/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-12 20:11:18.000000 threads-api-1.1.4/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.4/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.4/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    29835 2023-07-12 20:11:18.000000 threads-api-1.1.4/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.4/threads_api/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-12 19:46:32.000000 threads-api-1.1.4/threads_api/tests/get_post_id_test.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      370 2023-07-12 20:11:18.000000 threads-api-1.1.4/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13446 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      404 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.006703 threads-api-1.1.5/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.5/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15004 2023-07-13 21:53:15.006703 threads-api-1.1.5/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    14474 2023-07-13 21:53:08.000000 threads-api-1.1.5/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      472 2023-07-13 21:53:08.000000 threads-api-1.1.5/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-13 21:53:15.006703 threads-api-1.1.5/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-13 21:53:08.000000 threads-api-1.1.5/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.002703 threads-api-1.1.5/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.5/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.006703 threads-api-1.1.5/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.5/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    41169 2023-07-13 21:53:08.000000 threads-api-1.1.5/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.006703 threads-api-1.1.5/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.5/threads_api/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-13 17:43:17.000000 threads-api-1.1.5/threads_api/tests/get_post_id_test.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      592 2023-07-13 21:53:08.000000 threads-api-1.1.5/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.006703 threads-api-1.1.5/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15004 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      404 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.1.4/LICENSE` & `threads-api-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.4/PKG-INFO` & `threads-api-1.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: threads-api
-Version: 1.1.4
-Summary: Unofficial Python client for Meta Threads.net API
-Home-page: https://github.com/danie1/threads-api
-Author: Danie1
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # [<img src="https://raw.githubusercontent.com/danie1/threads-api/main/.github/logo.jpg" width="36" height="36" />](https://github.com/danie1) Meta's Threads.net API
 
 [![Downdloads](https://pepy.tech/badge/threads-api)](https://pypi.org/project/threads-api/)
 [![Version](https://img.shields.io/pypi/v/threads-api.svg?style=flat)](https://pypi.org/project/threads-api/)
 [![Python](https://img.shields.io/pypi/pyversions/threads-api.svg)](https://pypi.org/project/threads-api/) [![MIT License](https://img.shields.io/pypi/l/threads-api.svg?style=flat)](https://github.com/Danie1/threads-api/blob/main/LICENSE) 
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
@@ -33,15 +16,18 @@
 
 > Note: Since v1.1.3 we are using ```instagrapi``` package to login.
 
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
-  * [Installation](#Installation)
+  * [Installation](#installation)
+  * [Set Log Level](#set-desired-log-level)
+* [Contributions](#contributing-to-danie1threads-api)
+* [Supported Features](#supported-features)
 * [Usage Examples](#usage-examples)
 * [Roadmap](#📌-roadmap)
 * [License](#license)
 
 # Demo
 <img src="https://raw.githubusercontent.com/Danie1/threads-api/main/.github/user_example2.jpg" alt="drawing" width="500"/>
 
@@ -49,15 +35,15 @@
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
 or
 ```bash
-poetry install threads-api
+poetry add threads-api
 ```
 
 Example using threads-api to post to Threads.net:
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
 import os
@@ -79,14 +65,100 @@
 async def main():
     await post()
 
 # Create an event loop and run the main function
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
+## Set Desired Log Level
+Threads-API reads the environment variable ```LOG_LEVEL``` and sets the log-level according to its value.
+
+Possible values include: ```DEBUG, INFO, WARNING, ERROR, CRITICAL```
+
+**Log Level defaults to WARNING when not set.**
+
+Useful to know:
+``` bash
+# Set Info (Prints general flow)
+export LOG_LEVEL=INFO
+```
+
+``` bash
+# Set Debug (Prints HTTP Requests + HTTP Responses)
+export LOG_LEVEL=DEBUG
+```
+
+# Contributing to Danie1/threads-api
+## Getting Started
+
+With Poetry (*Recommended*)
+``` bash
+# Step 1: Clone the project
+git clone git@github.com:Danie1/threads-api.git
+
+# Step 2: Install dependencies to virtual environment
+poetry install
+
+# Step 3: Activate virtual environment
+poetry shell
+```
+or
+
+Without Poetry
+
+``` bash
+# Step 1: Clone the project
+git clone git@github.com:Danie1/threads-api.git
+
+# Step 2: Create virtual environment
+python3 -m venv env
+
+# Step 3 (Unix/MacOS): Activate virtual environment
+source env/bin/activate # Unix/MacOS
+
+# Step 3 (Windows): Activate virtual environment
+.\env\Scripts\activate # Windows
+
+# Step 4: Install dependencies
+pip install -r requirements.txt
+```
+
+
+# Supported Features
+- [x] ✅ Login functionality, including 2FA 🔒
+  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
+- [x] ✅ Write Posts (Requires Login 🔒)
+  - [x] ✅ Posts with just text
+  - [x] ✅ Posts with text and an image
+  - [x] ✅ Posts with text that share a url
+  - [x] ✅ Reply to Posts
+- [x] ✅ Perform Actions (Requires Login 🔒)
+  - [x] ✅ Like Posts
+  - [x] ✅ Unlike Posts
+  - [x] ✅ Delete post
+  - [x] ✅ Follow User
+  - [x] ✅ Unfollow User
+  - [x] ✅ Block User
+  - [x] ✅ Unblock User
+  - [x] ✅ Restrict User
+  - [x] ✅ Unrestrict User
+  - [x] ✅ Mute User
+  - [x] ✅ Unmute User
+- [x] ✅ Read Public Data
+  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
+  - [x] ✅ Read a user's profile info
+  - [x] ✅ Read list of a user's Threads
+  - [x] ✅ Read list of a user's Replies
+  - [x] ✅ Read Post and a list of its Replies
+  - [x] ✅ View who liked a post
+- [x] ✅ Read Private Data (Requires Login 🔒)
+  - [x] ✅ Read a user's followers list
+  - [x] ✅ Read a user's following list
+- [x] ✅  CI/CD
+  - [x] ✅  GitHub Actions Pipeline
 
 ## Usage Examples
 View [example.py](https://github.com/Danie1/threads-api/blob/main/example.py) for code examples. 
 At the end of the file you will be able to uncomment and run the individual examples with ease.
 
 Then simply run as:
 ```
@@ -351,41 +423,16 @@
 Example Output:
 ```
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
-
-- [x] ✅ Login functionality 🔒
-  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
-- [x] ✅ Write Posts (Requires Login 🔒)
-  - [x] ✅ Posts with just text
-  - [x] ✅ Posts with text and an image
-  - [x] ✅ Posts with text that share a url
-  - [x] ✅ Reply to Posts
-  - [ ] 🚧 Post with text and share a video
-- [x] ✅ Perform Actions (Requires Login 🔒)
-  - [x] ✅ Like Posts
-  - [x] ✅ Unlike Posts
-  - [x] ✅ Delete post
-  - [x] ✅ Follow User
-  - [x] ✅ Unfollow User
-- [x] ✅ Read Public Data
-  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
-  - [x] ✅ Read a user's profile info
-  - [x] ✅ Read list of a user's Threads
-  - [x] ✅ Read list of a user's Replies
-  - [x] ✅ Read Post and a list of its Replies
-  - [x] ✅ View who liked a post
-- [x] ✅ Read Private Data (Requires Login 🔒)
-  - [x] ✅ Read a user's followers list
-  - [x] ✅ Read a user's following list
-- [x] ✅  CI/CD
-  - [x] ✅  GitHub Actions Pipeline
-  - [ ] 🚧  Pytest
+- [ ] 🚧 Read feed, notifications
+- [ ] 🚧 Post text and share a video
+- [ ] 🚧 Documentation Improvements
+- [ ] 🚧 CI/CD Improvements
+  - [ ] 🚧 Add coverage Pytest
 
 
 # License
 This project is licensed under the MIT license.
-
-
```

### Comparing `threads-api-1.1.4/README.md` & `threads-api-1.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: threads-api
+Version: 1.1.5
+Summary: Unofficial Python client for Meta Threads.net API
+Home-page: https://github.com/danie1/threads-api
+Author: Danie1
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # [<img src="https://raw.githubusercontent.com/danie1/threads-api/main/.github/logo.jpg" width="36" height="36" />](https://github.com/danie1) Meta's Threads.net API
 
 [![Downdloads](https://pepy.tech/badge/threads-api)](https://pypi.org/project/threads-api/)
 [![Version](https://img.shields.io/pypi/v/threads-api.svg?style=flat)](https://pypi.org/project/threads-api/)
 [![Python](https://img.shields.io/pypi/pyversions/threads-api.svg)](https://pypi.org/project/threads-api/) [![MIT License](https://img.shields.io/pypi/l/threads-api.svg?style=flat)](https://github.com/Danie1/threads-api/blob/main/LICENSE) 
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
@@ -16,15 +33,18 @@
 
 > Note: Since v1.1.3 we are using ```instagrapi``` package to login.
 
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
-  * [Installation](#Installation)
+  * [Installation](#installation)
+  * [Set Log Level](#set-desired-log-level)
+* [Contributions](#contributing-to-danie1threads-api)
+* [Supported Features](#supported-features)
 * [Usage Examples](#usage-examples)
 * [Roadmap](#📌-roadmap)
 * [License](#license)
 
 # Demo
 <img src="https://raw.githubusercontent.com/Danie1/threads-api/main/.github/user_example2.jpg" alt="drawing" width="500"/>
 
@@ -32,15 +52,15 @@
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
 or
 ```bash
-poetry install threads-api
+poetry add threads-api
 ```
 
 Example using threads-api to post to Threads.net:
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
 import os
@@ -62,14 +82,100 @@
 async def main():
     await post()
 
 # Create an event loop and run the main function
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
+## Set Desired Log Level
+Threads-API reads the environment variable ```LOG_LEVEL``` and sets the log-level according to its value.
+
+Possible values include: ```DEBUG, INFO, WARNING, ERROR, CRITICAL```
+
+**Log Level defaults to WARNING when not set.**
+
+Useful to know:
+``` bash
+# Set Info (Prints general flow)
+export LOG_LEVEL=INFO
+```
+
+``` bash
+# Set Debug (Prints HTTP Requests + HTTP Responses)
+export LOG_LEVEL=DEBUG
+```
+
+# Contributing to Danie1/threads-api
+## Getting Started
+
+With Poetry (*Recommended*)
+``` bash
+# Step 1: Clone the project
+git clone git@github.com:Danie1/threads-api.git
+
+# Step 2: Install dependencies to virtual environment
+poetry install
+
+# Step 3: Activate virtual environment
+poetry shell
+```
+or
+
+Without Poetry
+
+``` bash
+# Step 1: Clone the project
+git clone git@github.com:Danie1/threads-api.git
+
+# Step 2: Create virtual environment
+python3 -m venv env
+
+# Step 3 (Unix/MacOS): Activate virtual environment
+source env/bin/activate # Unix/MacOS
+
+# Step 3 (Windows): Activate virtual environment
+.\env\Scripts\activate # Windows
+
+# Step 4: Install dependencies
+pip install -r requirements.txt
+```
+
+
+# Supported Features
+- [x] ✅ Login functionality, including 2FA 🔒
+  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
+- [x] ✅ Write Posts (Requires Login 🔒)
+  - [x] ✅ Posts with just text
+  - [x] ✅ Posts with text and an image
+  - [x] ✅ Posts with text that share a url
+  - [x] ✅ Reply to Posts
+- [x] ✅ Perform Actions (Requires Login 🔒)
+  - [x] ✅ Like Posts
+  - [x] ✅ Unlike Posts
+  - [x] ✅ Delete post
+  - [x] ✅ Follow User
+  - [x] ✅ Unfollow User
+  - [x] ✅ Block User
+  - [x] ✅ Unblock User
+  - [x] ✅ Restrict User
+  - [x] ✅ Unrestrict User
+  - [x] ✅ Mute User
+  - [x] ✅ Unmute User
+- [x] ✅ Read Public Data
+  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
+  - [x] ✅ Read a user's profile info
+  - [x] ✅ Read list of a user's Threads
+  - [x] ✅ Read list of a user's Replies
+  - [x] ✅ Read Post and a list of its Replies
+  - [x] ✅ View who liked a post
+- [x] ✅ Read Private Data (Requires Login 🔒)
+  - [x] ✅ Read a user's followers list
+  - [x] ✅ Read a user's following list
+- [x] ✅  CI/CD
+  - [x] ✅  GitHub Actions Pipeline
 
 ## Usage Examples
 View [example.py](https://github.com/Danie1/threads-api/blob/main/example.py) for code examples. 
 At the end of the file you will be able to uncomment and run the individual examples with ease.
 
 Then simply run as:
 ```
@@ -334,39 +440,18 @@
 Example Output:
 ```
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
-
-- [x] ✅ Login functionality 🔒
-  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
-- [x] ✅ Write Posts (Requires Login 🔒)
-  - [x] ✅ Posts with just text
-  - [x] ✅ Posts with text and an image
-  - [x] ✅ Posts with text that share a url
-  - [x] ✅ Reply to Posts
-  - [ ] 🚧 Post with text and share a video
-- [x] ✅ Perform Actions (Requires Login 🔒)
-  - [x] ✅ Like Posts
-  - [x] ✅ Unlike Posts
-  - [x] ✅ Delete post
-  - [x] ✅ Follow User
-  - [x] ✅ Unfollow User
-- [x] ✅ Read Public Data
-  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
-  - [x] ✅ Read a user's profile info
-  - [x] ✅ Read list of a user's Threads
-  - [x] ✅ Read list of a user's Replies
-  - [x] ✅ Read Post and a list of its Replies
-  - [x] ✅ View who liked a post
-- [x] ✅ Read Private Data (Requires Login 🔒)
-  - [x] ✅ Read a user's followers list
-  - [x] ✅ Read a user's following list
-- [x] ✅  CI/CD
-  - [x] ✅  GitHub Actions Pipeline
-  - [ ] 🚧  Pytest
+- [ ] 🚧 Read feed, notifications
+- [ ] 🚧 Post text and share a video
+- [ ] 🚧 Documentation Improvements
+- [ ] 🚧 CI/CD Improvements
+  - [ ] 🚧 Add coverage Pytest
 
 
 # License
 This project is licensed under the MIT license.
+
+
```

### Comparing `threads-api-1.1.4/setup.py` & `threads-api-1.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.1.4',
+    version='1.1.5',
     description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
```

### Comparing `threads-api-1.1.4/threads_api/src/threads_api.py` & `threads-api-1.1.5/threads_api/src/threads_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 
 from instagrapi import Client
 
+import logging
+import sys
+
+from colorama import init, Fore, Style
+
 BASE_URL = "https://i.instagram.com/api/v1"
 LOGIN_URL = BASE_URL + "/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/"
 POST_URL_TEXTONLY = BASE_URL + "/media/configure_text_only_post/"
 POST_URL_IMAGE = BASE_URL + "/media/configure_text_post_app_feed/"
 DEFAULT_HEADERS = {
             'Authority': 'www.threads.net',
             'Accept': '*/*',
@@ -48,17 +53,15 @@
                 'AppleWebKit/605.1.15 (KHTML, like Gecko) Version/11.1.2 Safari/605.1.15'
             ),
             'X-ASBD-ID': '129477',
             'X-FB-LSD': 'NjppQDEgONsU_1LCzrmp6q',
             'X-IG-App-ID': '238260118697367',
         }
 
-class ThreadsAPIOptions:
-    def __init__(self, token: Optional[str] = None):
-        self.token = token
+# This will help debugging flow failures
 
 class SimpleEncDec:
     backend = default_backend()
     iterations = 100_000
 
     @staticmethod
     def _derive_key(password: bytes, salt: bytes, iterations: int = iterations) -> bytes:
@@ -90,37 +93,65 @@
 
 class LoggedOutException(Exception):
      def __init__(self, message):            
         # Call the base class constructor with the parameters it needs
         super().__init__(message)
 
 class ThreadsAPI:
-    def __init__(self, options: Optional[ThreadsAPIOptions] = None):
-        self.token = None
-        self.user_id = None
+    def __init__(self):
+        
+        # Get the log level from the environment variable
+        log_level_env = os.environ.get("LOG_LEVEL", "WARNING")
 
-        if options and options.token:
-            self.token = options.token
+        # Set the log level based on the environment variable
+        log_level = getattr(logging, log_level_env.upper(), None)
+        if not isinstance(log_level, int):
+            raise ValueError(f"Invalid log level: {log_level_env}")
+        
+        self.log_level = log_level
+        
+        self.set_log_level(self.log_level)
+
+        self.logger = logging.getLogger()
+        
 
+        self.token = None
+        self.user_id = None
         self.is_logged_in = False
         self.auth_headers = None
 
         self.FBLSDToken = 'NjppQDEgONsU_1LCzrmp6q'
 
+    def set_log_level(self, log_level):
+        self.log_level = log_level
+        logging.basicConfig(level=self.log_level, format='%(levelname)s:%(message)s')
+
+    def log_request(self, type, url, header, payload=""):
+        self.logger.debug(f'{Fore.GREEN}-\nRequest [{Style.RESET_ALL}{type}{Fore.GREEN}] -> URL: [{Style.RESET_ALL}{url}{Fore.GREEN}]\nHeader: [{Style.RESET_ALL}{header}{Fore.GREEN}]\n Response: [{Style.RESET_ALL}{payload}{Fore.GREEN}]\n-{Style.RESET_ALL}')
+
+    def log_response(self, url, resp):
+        self.logger.debug(f'{Fore.GREEN}-\nResponse -> URL: [{Style.RESET_ALL}{url}{Fore.GREEN}] Response: [{Style.RESET_ALL}{resp}{Fore.GREEN}]\n-{Style.RESET_ALL}')
+        return resp
+
+
     async def _get_public_headers(self) -> str:
         default_headers = copy.deepcopy(DEFAULT_HEADERS)
         default_headers['X-FB-LSD'] = await self._refresh_public_token()
         return default_headers
     
     async def _refresh_public_token(self) -> str:
+        self.logger.info("Refreshing public token")
         modified_default_headers = copy.deepcopy(DEFAULT_HEADERS)
         del modified_default_headers['X-FB-LSD']
+        url = 'https://www.instagram.com/instagram'
         async with aiohttp.ClientSession() as session:
-            async with session.get('https://www.instagram.com/instagram', headers=modified_default_headers) as response:
+            self.log_request('GET', url, modified_default_headers)
+            async with session.get(url, headers=modified_default_headers) as response:
                 data = await response.text()
+                self.log_response(url, data)
                 token_key_value = re.search('LSD",\\[\\],{"token":"(.*?)"},\\d+\\]', data).group()
                 token_key_value = token_key_value.replace('LSD",[],{"token":"', '')
                 token = token_key_value.split('"')[0]
 
         self.FBLSDToken = token
         return self.FBLSDToken
     
@@ -137,50 +168,56 @@
 
         Raises:
             Exception: If the username or password are invalid, or if an error occurs during login.
         """
         def _save_token_to_cache(cached_token_path, token, password):
             with open(cached_token_path, "wb") as fd:
                 fd.write(SimpleEncDec.password_encrypt(token.encode(), password))
+                self.logger.info("Saved token to cache")
             return
 
         def _get_token_from_cache(cached_token_path, password):
             with open(cached_token_path, "rb") as fd:
                 encrypted_token = fd.read()
+                self.logger.info("Loaded token from cache")
+
             return SimpleEncDec.password_decrypt(encrypted_token, password).decode()
         
         async def _set_logged_in_state(username, token):
             self.token = token
             self.auth_headers = {
                 'Authorization': f'Bearer IGT:2:{self.token}',
                 'User-Agent': 'Barcelona 289.0.0.77.109 Android',
                 'Sec-Fetch-Site': 'same-origin',
                 'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
             }
             self.is_logged_in = True
             self.user_id = await self.get_user_id_from_username(username)
+            self.logger.info("Set logged-in state successfully. All set!")
             return
         
         if username is None or password is None:
             raise Exception("Username or password are invalid")
 
         self.username = username
 
         # Look in cache before logging in.
         if cached_token_path is not None and os.path.exists(cached_token_path):
+            self.logger.info(f"Found cache file in {cached_token_path}, attempting to read the token from it.")
             try:
                 await _set_logged_in_state(username, _get_token_from_cache(cached_token_path, password))
                 
                 return True
             except LoggedOutException as e:
                 print(f"[Error] {e}. Attempting to re-login.")
                 pass
 
-        try:      
+        try:
             cl = Client()
+            self.logger.info("Attempting to login")
             cl.login(username, password)
             token = cl.private.headers['Authorization'].split("Bearer IGT:2:")[1]
             
             await _set_logged_in_state(username, token)
                     
             if cached_token_path is not None:
                 _save_token_to_cache(cached_token_path, token, password)
@@ -188,50 +225,64 @@
             print("[ERROR] ", e)
             raise
 
         return True
 
     async def __auth_required_post_request(self, url: str):
         async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, self.auth_headers)
             async with session.post(url, headers=self.auth_headers) as response:
-                return await response.json()
+                resp = await response.json()
+                self.log_response(url, resp)
+                return 
     
     async def __auth_required_get_request(self, url: str):
         async with aiohttp.ClientSession() as session:
+            self.log_request('GET', url, self.auth_headers)
             async with session.get(url, headers=self.auth_headers) as response:
-                return await response.json()
+                resp = await response.json()
+                self.log_response(url, resp)
+                return resp
     
 
     async def get_user_id_from_username(self, username: str) -> str:
         """
         Retrieves the user ID associated with a given username.
         
         Args:
             username (str): The username to retrieve the user ID for.
         
         Returns:
             str: The user ID if found, or None if the user ID is not found.
         """
-        if self.is_logged_in:
+        if self.is_logged_in and self.username == username:
+            self.logger.info(f"Fetching user_id for user [{username}] while logged-in")
             url = BASE_URL + f"/users/{username}/usernameinfo/"
             async with aiohttp.ClientSession() as session:
+                self.log_request('GET', url, self.auth_headers)
                 async with session.get(url, headers=self.auth_headers) as response:
                     data = await response.json()
+                    self.log_response(url, data)
                     
                     if 'message' in data and data['message'] == "login_required" or \
                         'status' in data and data['status'] == 'fail':
                         raise LoggedOutException(str(data))
                     user_id = int(data['user']['pk'])
                     return user_id
         else:
+            self.logger.info(f"Fetching user_id for user [{username}] anonymously")
             url = f"https://www.threads.net/@{username}"
             
+            headers = await self._get_public_headers()
+
             async with aiohttp.ClientSession() as session:
-                async with session.get(url, headers=await self._get_public_headers()) as response:
+                self.log_request('GET', url, headers)
+                async with session.get(url, headers=headers) as response:
                     text = await response.text()
+                    self.log_response(url, text)
 
             text = text.replace('\\s', "").replace('\\n', "")
             user_id = re.search(r'"props":{"user_id":"(\d+)"},', text)
 
             return user_id.group(1) if user_id else None
 
     async def get_user_profile(self, user_id: str):
@@ -267,17 +318,19 @@
                         'userID': user_id,
                     }
                 ),
                 'doc_id': '23996318473300828'
             }
 
         async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, modified_headers, payload)
             async with session.post(url, headers=modified_headers, data=payload) as response:
                 text = await response.text()
                 data = json.loads(text)
+                self.log_response(url, data)
                
         user = data['data']['userData']['user']
         return user
 
     async def get_user_threads(self, user_id: str):
         """
         Retrieves the threads associated with a user with the provided user ID.
@@ -307,22 +360,24 @@
         payload = {
                 'lsd': self.FBLSDToken,
                 'variables': json.dumps(
                     {
                         'userID': user_id,
                     }
                 ),
-                'doc_id': '6307072669391286'
+                'doc_id': '6232751443445612'
             }
         
         async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, modified_headers, payload)
             async with session.post(url, headers=modified_headers, data=payload) as response:
                 try:
                     text = await response.text()
                     data = json.loads(text)
+                    self.log_response(url, data)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['mediaData']['threads']
         return threads
     
     async def get_user_replies(self, user_id: str):
@@ -358,18 +413,20 @@
                         'userID': user_id,
                     }
                 ),
                 'doc_id': '6307072669391286'
             }
 
         async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, modified_headers, payload)
             async with session.post(url, headers=modified_headers, data=payload) as response:
                 try:
                     text = await response.text()
                     data = json.loads(text)
+                    self.log_response(url, data)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['mediaData']['threads']
         return threads
 
     async def get_user_followers(self, user_id: str) -> bool:
@@ -538,18 +595,20 @@
                         'postID': post_id,
                     }
                 ),
                 'doc_id': '5587632691339264',
             }
 
         async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, modified_headers, payload)
             async with session.post(url, headers=modified_headers, data=payload) as response:
                 try:
                     text = await response.text()
                     data = json.loads(text)
+                    self.log_response(url, data)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['data']
         return threads
     
     async def get_post_likes(self, post_id:int):
@@ -585,23 +644,255 @@
                         'mediaID': post_id,
                     }
                 ),
                 'doc_id': '9360915773983802',
             }
 
         async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, modified_headers, payload)
             async with session.post(url, headers=modified_headers, data=payload) as response:
                 try:
                     text = await response.text()
                     data = json.loads(text)
+                    self.log_response(url, data)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         return data['data']['likers']['users']
 
+    async def mute_user(self, user_id):
+        """
+        Mute a user
+
+        Args:
+            user_id (int): The ID of the user to mute.
+
+        Returns:
+            dict: REST API Response in JSON format
+
+        Raises:
+            Exception: If an error occurs during the muting process.
+        """
+        parameters = json.dumps(
+            obj={
+                'target_posts_author_id': user_id,
+                'container_module': 'ig_text_feed_timeline',
+            },
+        )
+
+        encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
+        payload = f'signed_body=SIGNATURE.{encoded_parameters}'
+
+        url = f'{BASE_URL}/friendships/mute_posts_or_story_from_follow/'
+        async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, self.auth_headers, payload)
+            async with session.post(url, 
+                                    headers=self.auth_headers, 
+                                    data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                    self.log_response(url, data)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+        
+        return data
+
+    async def unmute_user(self, user_id):
+        """
+        Unmute a user
+
+        Args:
+            user_id (int): The ID of the user to unmute.
+
+        Returns:
+            dict: REST API Response in JSON format
+
+        Raises:
+            Exception: If an error occurs during the unmuting process.
+        """
+        parameters = json.dumps(
+            obj={
+                'target_posts_author_id': user_id,
+                'container_module': 'ig_text_feed_timeline',
+            },
+        )
+
+        encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
+        payload = f'signed_body=SIGNATURE.{encoded_parameters}'
+
+        url = f'{BASE_URL}/friendships/unmute_posts_or_story_from_follow/'
+
+        async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, self.auth_headers, payload)
+            async with session.post(url, 
+                                    headers=self.auth_headers, 
+                                    data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                    self.log_response(url, data)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+        
+        return data
+    
+    async def restrict_user(self, user_id):
+        """
+        Restrict a user
+
+        Args:
+            user_id (int): The ID of the user to restrict.
+
+        Returns:
+            dict: REST API Response in JSON format
+
+        Raises:
+            Exception: If an error occurs during the restricting process.
+        """
+        parameters = json.dumps(
+            obj={
+                'user_ids': user_id,
+                'container_module': 'ig_text_feed_timeline',
+            },
+        )
+
+        encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
+        payload = f'signed_body=SIGNATURE.{encoded_parameters}'
+
+        url = f'{BASE_URL}/restrict_action/restrict_many/'
+        async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, self.auth_headers, payload)
+            async with session.post(url, 
+                                    headers=self.auth_headers, 
+                                    data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                    self.log_response(url, data)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+        
+        return data
+    
+    async def unrestrict_user(self, user_id):
+        """
+        Unrestrict a user
+
+        Args:
+            user_id (int): The ID of the user to unrestrict.
+
+        Returns:
+            dict: REST API Response in JSON format
+
+        Raises:
+            Exception: If an error occurs during the unrestricting process.
+        """
+        parameters = json.dumps(
+            obj={
+                'user_ids': user_id,
+                'container_module': 'ig_text_feed_timeline',
+            },
+        )
+
+        encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
+        payload = f'signed_body=SIGNATURE.{encoded_parameters}'
+        url = f'{BASE_URL}/restrict_action/unrestrict/'
+        
+        async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, self.auth_headers, payload)
+            async with session.post(url, 
+                                    headers=self.auth_headers, 
+                                    data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                    self.log_response(url, data)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+        
+        return data
+    
+    async def block_user(self, user_id):
+        """
+        Block a user
+
+        Args:
+            user_id (int): The ID of the user to block.
+
+        Returns:
+            dict: REST API Response in JSON format
+
+        Raises:
+            Exception: If an error occurs during the blocking process.
+        """
+        parameters = json.dumps(
+            obj={
+                'user_id': user_id,
+                'surface': 'ig_text_feed_timeline',
+                'is_auto_block_enabled': 'true',
+            },
+        )
+
+        encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
+        payload = f'signed_body=SIGNATURE.{encoded_parameters}'
+        url = f'{BASE_URL}/friendships/block/{user_id}/'
+
+        async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, self.auth_headers, payload)
+            async with session.post(url, 
+                                    headers=self.auth_headers, 
+                                    data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                    self.log_response(url, data)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+        
+        return data
+    
+    async def unblock_user(self, user_id):
+        """
+        Unblock a user
+
+        Args:
+            user_id (int): The ID of the user to unblock.
+
+        Returns:
+            dict: REST API Response in JSON format
+
+        Raises:
+            Exception: If an error occurs during the unblocking process.
+        """
+        parameters = json.dumps(
+            obj={
+                'user_id': user_id,
+                'container_module': 'ig_text_feed_timeline',
+            },
+        )
+
+        encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
+        payload = f'signed_body=SIGNATURE.{encoded_parameters}'
+        url = f'{BASE_URL}/friendships/unblock/{user_id}/'
+
+        async with aiohttp.ClientSession() as session:
+            self.log_request('POST', url, self.auth_headers, payload)
+            async with session.post(url, 
+                                    headers=self.auth_headers, 
+                                    data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                    self.log_response(url, data)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+        
+        return data
+    
     async def post(
         self, caption: str, image_path: str = None, url: str = None, parent_post_id: str = None
     ) -> bool:
         """
         Creates a new post with the given caption, image, URL, and parent post ID.
 
         Args:
@@ -699,17 +990,20 @@
                 "Content-Type": "application/octet-stream",
                 "Content-Length": f"{content_length}",
                 "Accept-Encoding": "gzip",
             }
 
             headers.update(image_headers)
             async with aiohttp.ClientSession() as session:
+                self.log_request('POST', url, headers, content)
                 async with session.post(url, headers=headers, data=content) as response:
                     if response.status == 200:
-                        return await response.json()
+                        resp = await response.json()
+                        self.log_response(url, resp)
+                        return resp
                     else:
                         raise Exception("Failed to upload image")
 
         if not self.is_logged_in:
             raise Exception("You need to login before posting")
         
         now = datetime.now()
@@ -753,18 +1047,20 @@
             params["text_post_app_info"]["reply_id"] = parent_post_id
         params = json.dumps(params)
         payload = f"signed_body=SIGNATURE.{urllib.parse.quote(params)}"
         headers = __get_app_headers().copy()
 
         try:
             async with aiohttp.ClientSession() as session:
+                self.log_request('POST', post_url, headers, payload)
                 async with session.post(post_url, headers=headers, data=payload) as response:
                     data = await response.json()
+                    self.log_response(url, data)
 
                     if 'media' in data and 'pk' in data['media']:
                         # Return the newly created post_id
                         return data['media']['pk']
                     else:
                         raise Exception("Failed to post. Got response:\n" + str(response))
         except Exception as e:
             print("[ERROR] ", e)
-            raise
+            raise
```

### Comparing `threads-api-1.1.4/threads_api.egg-info/PKG-INFO` & `threads-api-1.1.5/threads_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.4
+Version: 1.1.5
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -33,15 +33,18 @@
 
 > Note: Since v1.1.3 we are using ```instagrapi``` package to login.
 
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
-  * [Installation](#Installation)
+  * [Installation](#installation)
+  * [Set Log Level](#set-desired-log-level)
+* [Contributions](#contributing-to-danie1threads-api)
+* [Supported Features](#supported-features)
 * [Usage Examples](#usage-examples)
 * [Roadmap](#📌-roadmap)
 * [License](#license)
 
 # Demo
 <img src="https://raw.githubusercontent.com/Danie1/threads-api/main/.github/user_example2.jpg" alt="drawing" width="500"/>
 
@@ -49,15 +52,15 @@
 
 ### 📦 Installation
 ```bash
 pip install threads-api
 ```
 or
 ```bash
-poetry install threads-api
+poetry add threads-api
 ```
 
 Example using threads-api to post to Threads.net:
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
 import os
@@ -79,14 +82,100 @@
 async def main():
     await post()
 
 # Create an event loop and run the main function
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
+## Set Desired Log Level
+Threads-API reads the environment variable ```LOG_LEVEL``` and sets the log-level according to its value.
+
+Possible values include: ```DEBUG, INFO, WARNING, ERROR, CRITICAL```
+
+**Log Level defaults to WARNING when not set.**
+
+Useful to know:
+``` bash
+# Set Info (Prints general flow)
+export LOG_LEVEL=INFO
+```
+
+``` bash
+# Set Debug (Prints HTTP Requests + HTTP Responses)
+export LOG_LEVEL=DEBUG
+```
+
+# Contributing to Danie1/threads-api
+## Getting Started
+
+With Poetry (*Recommended*)
+``` bash
+# Step 1: Clone the project
+git clone git@github.com:Danie1/threads-api.git
+
+# Step 2: Install dependencies to virtual environment
+poetry install
+
+# Step 3: Activate virtual environment
+poetry shell
+```
+or
+
+Without Poetry
+
+``` bash
+# Step 1: Clone the project
+git clone git@github.com:Danie1/threads-api.git
+
+# Step 2: Create virtual environment
+python3 -m venv env
+
+# Step 3 (Unix/MacOS): Activate virtual environment
+source env/bin/activate # Unix/MacOS
+
+# Step 3 (Windows): Activate virtual environment
+.\env\Scripts\activate # Windows
+
+# Step 4: Install dependencies
+pip install -r requirements.txt
+```
+
+
+# Supported Features
+- [x] ✅ Login functionality, including 2FA 🔒
+  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
+- [x] ✅ Write Posts (Requires Login 🔒)
+  - [x] ✅ Posts with just text
+  - [x] ✅ Posts with text and an image
+  - [x] ✅ Posts with text that share a url
+  - [x] ✅ Reply to Posts
+- [x] ✅ Perform Actions (Requires Login 🔒)
+  - [x] ✅ Like Posts
+  - [x] ✅ Unlike Posts
+  - [x] ✅ Delete post
+  - [x] ✅ Follow User
+  - [x] ✅ Unfollow User
+  - [x] ✅ Block User
+  - [x] ✅ Unblock User
+  - [x] ✅ Restrict User
+  - [x] ✅ Unrestrict User
+  - [x] ✅ Mute User
+  - [x] ✅ Unmute User
+- [x] ✅ Read Public Data
+  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
+  - [x] ✅ Read a user's profile info
+  - [x] ✅ Read list of a user's Threads
+  - [x] ✅ Read list of a user's Replies
+  - [x] ✅ Read Post and a list of its Replies
+  - [x] ✅ View who liked a post
+- [x] ✅ Read Private Data (Requires Login 🔒)
+  - [x] ✅ Read a user's followers list
+  - [x] ✅ Read a user's following list
+- [x] ✅  CI/CD
+  - [x] ✅  GitHub Actions Pipeline
 
 ## Usage Examples
 View [example.py](https://github.com/Danie1/threads-api/blob/main/example.py) for code examples. 
 At the end of the file you will be able to uncomment and run the individual examples with ease.
 
 Then simply run as:
 ```
@@ -351,41 +440,18 @@
 Example Output:
 ```
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
-
-- [x] ✅ Login functionality 🔒
-  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
-- [x] ✅ Write Posts (Requires Login 🔒)
-  - [x] ✅ Posts with just text
-  - [x] ✅ Posts with text and an image
-  - [x] ✅ Posts with text that share a url
-  - [x] ✅ Reply to Posts
-  - [ ] 🚧 Post with text and share a video
-- [x] ✅ Perform Actions (Requires Login 🔒)
-  - [x] ✅ Like Posts
-  - [x] ✅ Unlike Posts
-  - [x] ✅ Delete post
-  - [x] ✅ Follow User
-  - [x] ✅ Unfollow User
-- [x] ✅ Read Public Data
-  - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
-  - [x] ✅ Read a user's profile info
-  - [x] ✅ Read list of a user's Threads
-  - [x] ✅ Read list of a user's Replies
-  - [x] ✅ Read Post and a list of its Replies
-  - [x] ✅ View who liked a post
-- [x] ✅ Read Private Data (Requires Login 🔒)
-  - [x] ✅ Read a user's followers list
-  - [x] ✅ Read a user's following list
-- [x] ✅  CI/CD
-  - [x] ✅  GitHub Actions Pipeline
-  - [ ] 🚧  Pytest
+- [ ] 🚧 Read feed, notifications
+- [ ] 🚧 Post text and share a video
+- [ ] 🚧 Documentation Improvements
+- [ ] 🚧 CI/CD Improvements
+  - [ ] 🚧 Add coverage Pytest
 
 
 # License
 This project is licensed under the MIT license.
```

