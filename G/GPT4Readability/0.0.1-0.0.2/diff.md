# Comparing `tmp/GPT4Readability-0.0.1.tar.gz` & `tmp/GPT4Readability-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPT4Readability-0.0.1.tar", last modified: Thu Jul 13 00:09:48 2023, max compression
+gzip compressed data, was "GPT4Readability-0.0.2.tar", last modified: Thu Jul 13 00:20:53 2023, max compression
```

## Comparing `GPT4Readability-0.0.1.tar` & `GPT4Readability-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:09:48.320941 GPT4Readability-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:09:48.320941 GPT4Readability-0.0.1/GPT4Readability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 00:09:31.000000 GPT4Readability-0.0.1/GPT4Readability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-13 00:09:31.000000 GPT4Readability-0.0.1/GPT4Readability/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-13 00:09:31.000000 GPT4Readability-0.0.1/GPT4Readability/readme_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-13 00:09:31.000000 GPT4Readability-0.0.1/GPT4Readability/suggestions_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-13 00:09:31.000000 GPT4Readability-0.0.1/GPT4Readability/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:09:48.320941 GPT4Readability-0.0.1/GPT4Readability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-13 00:09:48.000000 GPT4Readability-0.0.1/GPT4Readability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-13 00:09:48.000000 GPT4Readability-0.0.1/GPT4Readability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:09:48.000000 GPT4Readability-0.0.1/GPT4Readability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 00:09:48.000000 GPT4Readability-0.0.1/GPT4Readability.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 00:09:48.000000 GPT4Readability-0.0.1/GPT4Readability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 00:09:48.000000 GPT4Readability-0.0.1/GPT4Readability.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 00:09:31.000000 GPT4Readability-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-13 00:09:48.320941 GPT4Readability-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-13 00:09:31.000000 GPT4Readability-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:09:48.320941 GPT4Readability-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-13 00:09:31.000000 GPT4Readability-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/GPT4Readability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/GPT4Readability/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/prompts/readme_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/prompts/refactor_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/readme_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/suggestions_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/GPT4Readability.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/setup.py
```

### Comparing `GPT4Readability-0.0.1/GPT4Readability/__main__.py` & `GPT4Readability-0.0.2/GPT4Readability/__main__.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.1/GPT4Readability/readme_gen.py` & `GPT4Readability-0.0.2/GPT4Readability/readme_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import os
 from getpass import getpass
 from GPT4Readability.utils import *
+from importlib.resources import open_text
+
 
 def generate_readme(root_dir, output_name, model):
     """Generates a README.md file based on the python files in the provided directory
 
     Args:
         root_dir (str): The root directory of the python package to parse and generate a readme for
     """
 
-    prompt_folder_name = os.path.join(os.path.dirname(__file__), "prompts")
-    prompt_path = os.path.join(prompt_folder_name, "readme_prompt.txt")
+    # prompt_folder_name = os.path.join(os.path.dirname(__file__), "prompts")
+    # prompt_path = os.path.join(prompt_folder_name, "readme_prompt.txt")
+
+    with open_text('GPT4Readability.prompts', 'readme_prompt.txt') as f:
+        inb_msg = f.read()
 
-    with open(prompt_path) as f:
-        lines = f.readlines()
-    inb_msg = "".join(lines)
+    # with open(prompt_path) as f:
+    #     lines = f.readlines()
+    # inb_msg = "".join(lines)
 
     file_check_result = check_files_in_directory(root_dir) # Checking for the license and requirements.txt
     inb_msg += file_check_result
     special_file_check_result = check_special_files(root_dir) # Checking for the code of conduct and the style guide
     inb_msg += special_file_check_result
 
     username, reponame = get_github_info_from_local_repo(root_dir)
```

### Comparing `GPT4Readability-0.0.1/GPT4Readability/suggestions_gen.py` & `GPT4Readability-0.0.2/GPT4Readability/suggestions_gen.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import os
 from getpass import getpass
 from GPT4Readability.utils import *
 from tqdm import tqdm 
-import logging
+from importlib.resources import open_text
 
 def generate_suggestions(root_dir, output_name, model):
     """Generates a suggestions.md file with suggested improvements to the code based on the python files in the provided directory
 
     Args:
         root_dir (str): The root directory of the python package to parse and generate a readme for
     """
 
-    prompt_folder_name = os.path.join(os.path.dirname(__file__), "prompts")
-    prompt_path = os.path.join(prompt_folder_name, "refactor_prompt.txt")
+    # prompt_folder_name = os.path.join(os.path.dirname(__file__), "prompts")
+    # prompt_path = os.path.join(prompt_folder_name, "refactor_prompt.txt")
+
+    with open_text('GPT4Readability.prompts', 'refactor_prompt.txt') as f:
+        inb_msg = f.read()
 
     with open(prompt_path) as f:
         lines = f.readlines()
     inb_msg = "".join(lines)
 
     docs = get_docs(root_dir)
     python_files = find_python_files(root_dir)
```

### Comparing `GPT4Readability-0.0.1/GPT4Readability/utils.py` & `GPT4Readability-0.0.2/GPT4Readability/utils.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.1/GPT4Readability.egg-info/PKG-INFO` & `GPT4Readability-0.0.2/GPT4Readability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `GPT4Readability-0.0.1/LICENSE` & `GPT4Readability-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.1/PKG-INFO` & `GPT4Readability-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `GPT4Readability-0.0.1/README.md` & `GPT4Readability-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.1/setup.py` & `GPT4Readability-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 with open('README.md', 'r') as readme:
     # ignore gifs
     description = ''.join([i for i in readme.readlines()
                            if not i.startswith('![')])
 
 setup(
     name='GPT4Readability',
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/loevlie/GPT4Readability',
     author='Dennis Johan Loevlie',
     author_email='loevliedenny@gmail.com',
     description='A tool to automatically generate a README.md and suggest code improvements for any python code repository',
     long_description=description,
     long_description_content_type='text/markdown',
     packages=find_packages(),  # automatically discover all packages and subpackages
+    package_data={"GPT4Readability": ["prompts/*.txt"]},
     python_requires='>=3.6',
     install_requires= [
         "langchain",
         "openai",
         "faiss-cpu",
         "tiktoken",
         "click",
```

