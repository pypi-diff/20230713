# Comparing `tmp/StockStack-0.1.tar.gz` & `tmp/StockStack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StockStack-0.1.tar", last modified: Thu Jul 13 17:25:58 2023, max compression
+gzip compressed data, was "StockStack-0.1.1.tar", last modified: Thu Jul 13 17:32:07 2023, max compression
```

## Comparing `StockStack-0.1.tar` & `StockStack-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-07-13 17:25:58.312419 StockStack-0.1/
--rw-r--r--   0 cb        (1000) cb        (1000)    35149 2023-03-25 22:06:55.000000 StockStack-0.1/LICENSE
--rw-r--r--   0 cb        (1000) cb        (1000)     3826 2023-07-13 17:25:58.312419 StockStack-0.1/PKG-INFO
--rw-r--r--   0 cb        (1000) cb        (1000)     3357 2023-07-13 17:17:12.000000 StockStack-0.1/README.md
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-07-13 17:25:58.312419 StockStack-0.1/StockStack.egg-info/
--rw-r--r--   0 cb        (1000) cb        (1000)     3826 2023-07-13 17:25:58.000000 StockStack-0.1/StockStack.egg-info/PKG-INFO
--rw-r--r--   0 cb        (1000) cb        (1000)      232 2023-07-13 17:25:58.000000 StockStack-0.1/StockStack.egg-info/SOURCES.txt
--rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-07-13 17:25:58.000000 StockStack-0.1/StockStack.egg-info/dependency_links.txt
--rw-r--r--   0 cb        (1000) cb        (1000)       54 2023-07-13 17:25:58.000000 StockStack-0.1/StockStack.egg-info/entry_points.txt
--rw-r--r--   0 cb        (1000) cb        (1000)        9 2023-07-13 17:25:58.000000 StockStack-0.1/StockStack.egg-info/requires.txt
--rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-07-13 17:25:58.000000 StockStack-0.1/StockStack.egg-info/top_level.txt
--rw-r--r--   0 cb        (1000) cb        (1000)       38 2023-07-13 17:25:58.312419 StockStack-0.1/setup.cfg
--rw-r--r--   0 cb        (1000) cb        (1000)      846 2023-07-13 17:25:01.000000 StockStack-0.1/setup.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-07-13 17:32:07.028026 StockStack-0.1.1/
+-rw-r--r--   0 cb        (1000) cb        (1000)    35149 2023-03-25 22:06:55.000000 StockStack-0.1.1/LICENSE
+-rw-r--r--   0 cb        (1000) cb        (1000)     3576 2023-07-13 17:32:07.028026 StockStack-0.1.1/PKG-INFO
+-rw-r--r--   0 cb        (1000) cb        (1000)     3105 2023-07-13 17:30:49.000000 StockStack-0.1.1/README.md
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-07-13 17:32:07.028026 StockStack-0.1.1/StockStack.egg-info/
+-rw-r--r--   0 cb        (1000) cb        (1000)     3576 2023-07-13 17:32:07.000000 StockStack-0.1.1/StockStack.egg-info/PKG-INFO
+-rw-r--r--   0 cb        (1000) cb        (1000)      232 2023-07-13 17:32:07.000000 StockStack-0.1.1/StockStack.egg-info/SOURCES.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-07-13 17:32:07.000000 StockStack-0.1.1/StockStack.egg-info/dependency_links.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)       54 2023-07-13 17:32:07.000000 StockStack-0.1.1/StockStack.egg-info/entry_points.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        9 2023-07-13 17:32:07.000000 StockStack-0.1.1/StockStack.egg-info/requires.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-07-13 17:32:07.000000 StockStack-0.1.1/StockStack.egg-info/top_level.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)       38 2023-07-13 17:32:07.028026 StockStack-0.1.1/setup.cfg
+-rw-r--r--   0 cb        (1000) cb        (1000)      848 2023-07-13 17:32:00.000000 StockStack-0.1.1/setup.py
```

### Comparing `StockStack-0.1/LICENSE` & `StockStack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `StockStack-0.1/PKG-INFO` & `StockStack-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StockStack
-Version: 0.1
+Version: 0.1.1
 Summary: Look up and plot current stock prices from your terminal
 Home-page: https://github.com/carlobortolan/StockStack
 Author: Carlo Bortolan
 Author-email: carlobortolan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,38 +16,28 @@
 Look up and plot current stock prices from your terminal.
 
 This is a Python script for monitoring the current stock prices using the Yahoo Finance API to retrieve the latest
 stock prices and display them in the terminal.
 
 ## INSTALLATION
 
-1. Make sure to have [yfinance](https://pypi.org/project/yfinance/) and other needed dependecies installed
+1. Simply run `pip install StockStack`
 
-```
-$ pip install -r stockstack/requirements.txt
-```
-
-2. Clone this repository to your local machine
-
-```
-$ git clone https://github.com/carlobortolan/StockStack.git ~/stockstack
-```
-
-3. Add <YOUR_ALIAS> as an alias to your _.bashrc_, _.zshrc_, etc.
+2. Add <YOUR_ALIAS> as an alias to your _.bashrc_, _.zshrc_, etc.
 
 ```
 $ echo 'alias <YOUR_ALIAS>="python3 ~/stockstack/caller.py"'>>~/.bashrc
 ```
 
 > _**OPTIONAL**: If you want to have StockStack launch whenever you open a new terminal add:_
 > ```
 > $ echo '<YOUR_ALIAS>'>>~/.bashrc
 > ```
 
-4. Update your _.bashrc_, _.zshrc_, etc.
+3. Update your _.bashrc_, _.zshrc_, etc.
 
 ```
 $ source ~/.bashrc
 ```
 
 ## USAGE
```

### Comparing `StockStack-0.1/README.md` & `StockStack-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,28 @@
 Look up and plot current stock prices from your terminal.
 
 This is a Python script for monitoring the current stock prices using the Yahoo Finance API to retrieve the latest
 stock prices and display them in the terminal.
 
 ## INSTALLATION
 
-1. Make sure to have [yfinance](https://pypi.org/project/yfinance/) and other needed dependecies installed
+1. Simply run `pip install StockStack`
 
-```
-$ pip install -r stockstack/requirements.txt
-```
-
-2. Clone this repository to your local machine
-
-```
-$ git clone https://github.com/carlobortolan/StockStack.git ~/stockstack
-```
-
-3. Add <YOUR_ALIAS> as an alias to your _.bashrc_, _.zshrc_, etc.
+2. Add <YOUR_ALIAS> as an alias to your _.bashrc_, _.zshrc_, etc.
 
 ```
 $ echo 'alias <YOUR_ALIAS>="python3 ~/stockstack/caller.py"'>>~/.bashrc
 ```
 
 > _**OPTIONAL**: If you want to have StockStack launch whenever you open a new terminal add:_
 > ```
 > $ echo '<YOUR_ALIAS>'>>~/.bashrc
 > ```
 
-4. Update your _.bashrc_, _.zshrc_, etc.
+3. Update your _.bashrc_, _.zshrc_, etc.
 
 ```
 $ source ~/.bashrc
 ```
 
 ## USAGE
```

### Comparing `StockStack-0.1/StockStack.egg-info/PKG-INFO` & `StockStack-0.1.1/StockStack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StockStack
-Version: 0.1
+Version: 0.1.1
 Summary: Look up and plot current stock prices from your terminal
 Home-page: https://github.com/carlobortolan/StockStack
 Author: Carlo Bortolan
 Author-email: carlobortolan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,38 +16,28 @@
 Look up and plot current stock prices from your terminal.
 
 This is a Python script for monitoring the current stock prices using the Yahoo Finance API to retrieve the latest
 stock prices and display them in the terminal.
 
 ## INSTALLATION
 
-1. Make sure to have [yfinance](https://pypi.org/project/yfinance/) and other needed dependecies installed
+1. Simply run `pip install StockStack`
 
-```
-$ pip install -r stockstack/requirements.txt
-```
-
-2. Clone this repository to your local machine
-
-```
-$ git clone https://github.com/carlobortolan/StockStack.git ~/stockstack
-```
-
-3. Add <YOUR_ALIAS> as an alias to your _.bashrc_, _.zshrc_, etc.
+2. Add <YOUR_ALIAS> as an alias to your _.bashrc_, _.zshrc_, etc.
 
 ```
 $ echo 'alias <YOUR_ALIAS>="python3 ~/stockstack/caller.py"'>>~/.bashrc
 ```
 
 > _**OPTIONAL**: If you want to have StockStack launch whenever you open a new terminal add:_
 > ```
 > $ echo '<YOUR_ALIAS>'>>~/.bashrc
 > ```
 
-4. Update your _.bashrc_, _.zshrc_, etc.
+3. Update your _.bashrc_, _.zshrc_, etc.
 
 ```
 $ source ~/.bashrc
 ```
 
 ## USAGE
```

### Comparing `StockStack-0.1/setup.py` & `StockStack-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='StockStack',
-    version='0.1',
+    version='0.1.1',
     author='Carlo Bortolan',
     author_email='carlobortolan@gmail.com',
     description='Look up and plot current stock prices from your terminal',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/carlobortolan/StockStack',
     packages=find_packages(),
```

