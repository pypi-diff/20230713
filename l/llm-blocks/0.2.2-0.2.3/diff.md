# Comparing `tmp/llm-blocks-0.2.2.tar.gz` & `tmp/llm-blocks-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-blocks-0.2.2.tar", last modified: Wed Jun  7 16:29:56 2023, max compression
+gzip compressed data, was "llm-blocks-0.2.3.tar", last modified: Wed Jul 12 23:29:27 2023, max compression
```

## Comparing `llm-blocks-0.2.2.tar` & `llm-blocks-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 16:29:56.925255 llm-blocks-0.2.2/
--rw-rw-rw-   0        0        0     2771 2023-06-07 16:29:56.924250 llm-blocks-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2327 2023-06-07 15:34:54.000000 llm-blocks-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 16:29:56.912248 llm-blocks-0.2.2/llm_blocks/
--rw-rw-rw-   0        0        0        0 2023-06-06 22:53:28.000000 llm-blocks-0.2.2/llm_blocks/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-06-07 15:34:54.000000 llm-blocks-0.2.2/llm_blocks/chat_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:29:56.922251 llm-blocks-0.2.2/llm_blocks.egg-info/
--rw-rw-rw-   0        0        0     2771 2023-06-07 16:29:56.000000 llm-blocks-0.2.2/llm_blocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-07 16:29:56.000000 llm-blocks-0.2.2/llm_blocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 16:29:56.000000 llm-blocks-0.2.2/llm_blocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-07 16:29:56.000000 llm-blocks-0.2.2/llm_blocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 16:29:56.000000 llm-blocks-0.2.2/llm_blocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 16:29:56.925255 llm-blocks-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-06-07 16:29:11.000000 llm-blocks-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:29:27.789849 llm-blocks-0.2.3/
+-rw-rw-rw-   0        0        0     2771 2023-07-12 23:29:27.788848 llm-blocks-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2327 2023-06-07 15:34:54.000000 llm-blocks-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 23:29:27.782613 llm-blocks-0.2.3/llm_blocks/
+-rw-rw-rw-   0        0        0        0 2023-06-06 22:53:28.000000 llm-blocks-0.2.3/llm_blocks/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-06-07 15:34:54.000000 llm-blocks-0.2.3/llm_blocks/chat_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:29:27.787852 llm-blocks-0.2.3/llm_blocks.egg-info/
+-rw-rw-rw-   0        0        0     2771 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 23:29:27.789849 llm-blocks-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-07-12 23:29:10.000000 llm-blocks-0.2.3/setup.py
```

### Comparing `llm-blocks-0.2.2/PKG-INFO` & `llm-blocks-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-blocks
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple interface for creating and managing LLM chains
 Home-page: https://github.com/voynow/llm-blocks
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm-blocks-0.2.2/README.md` & `llm-blocks-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `llm-blocks-0.2.2/llm_blocks/chat_utils.py` & `llm-blocks-0.2.3/llm_blocks/chat_utils.py`

 * *Files identical despite different names*

### Comparing `llm-blocks-0.2.2/llm_blocks.egg-info/PKG-INFO` & `llm-blocks-0.2.3/llm_blocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-blocks
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple interface for creating and managing LLM chains
 Home-page: https://github.com/voynow/llm-blocks
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm-blocks-0.2.2/setup.py` & `llm-blocks-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="llm-blocks",
-    version="0.2.2",
+    version="0.2.3",
     author="Jamie Voynow",
     author_email="voynow99@gmail.com",
     description="Simple interface for creating and managing LLM chains",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/voynow/llm-blocks",
     packages=find_packages(),
     install_requires=[
         'langchain',
-        'pandas',
-        'matplotlib',
-        'numpy',
-        'ipywidgets',
         'python-dotenv',
-        'git2vec'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
+
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
```

