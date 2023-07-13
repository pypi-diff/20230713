# Comparing `tmp/aicodebot-0.9.5.tar.gz` & `tmp/aicodebot-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.9.5.tar", last modified: Wed Jul 12 05:07:38 2023, max compression
+gzip compressed data, was "aicodebot-0.9.6.tar", last modified: Wed Jul 12 05:07:49 2023, max compression
```

## Comparing `aicodebot-0.9.5.tar` & `aicodebot-0.9.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:07:38.088542 aicodebot-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-12 05:07:13.000000 aicodebot-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-12 05:07:38.088542 aicodebot-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-12 05:07:13.000000 aicodebot-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:07:38.088542 aicodebot-0.9.5/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 05:07:13.000000 aicodebot-0.9.5/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-12 05:07:13.000000 aicodebot-0.9.5/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-12 05:07:13.000000 aicodebot-0.9.5/aicodebot/coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 05:07:13.000000 aicodebot-0.9.5/aicodebot/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-12 05:07:13.000000 aicodebot-0.9.5/aicodebot/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-07-12 05:07:13.000000 aicodebot-0.9.5/aicodebot/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:07:38.088542 aicodebot-0.9.5/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-12 05:07:38.000000 aicodebot-0.9.5/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 05:07:38.000000 aicodebot-0.9.5/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:07:38.000000 aicodebot-0.9.5/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 05:07:38.000000 aicodebot-0.9.5/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 05:07:38.000000 aicodebot-0.9.5/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 05:07:38.000000 aicodebot-0.9.5/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 05:07:13.000000 aicodebot-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 05:07:38.088542 aicodebot-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-12 05:07:13.000000 aicodebot-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:07:49.983347 aicodebot-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-12 05:07:17.000000 aicodebot-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-12 05:07:49.983347 aicodebot-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-12 05:07:17.000000 aicodebot-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:07:49.983347 aicodebot-0.9.6/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 05:07:17.000000 aicodebot-0.9.6/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-12 05:07:17.000000 aicodebot-0.9.6/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-12 05:07:17.000000 aicodebot-0.9.6/aicodebot/coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-12 05:07:17.000000 aicodebot-0.9.6/aicodebot/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-12 05:07:17.000000 aicodebot-0.9.6/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-07-12 05:07:17.000000 aicodebot-0.9.6/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:07:49.983347 aicodebot-0.9.6/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-12 05:07:49.000000 aicodebot-0.9.6/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 05:07:49.000000 aicodebot-0.9.6/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:07:49.000000 aicodebot-0.9.6/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 05:07:49.000000 aicodebot-0.9.6/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 05:07:49.000000 aicodebot-0.9.6/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 05:07:49.000000 aicodebot-0.9.6/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 05:07:17.000000 aicodebot-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 05:07:49.983347 aicodebot-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-12 05:07:17.000000 aicodebot-0.9.6/setup.py
```

### Comparing `aicodebot-0.9.5/LICENSE` & `aicodebot-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.5/PKG-INFO` & `aicodebot-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.5
+Version: 0.9.6
 Summary: AI-powered tool for developers, simplifying coding tasks and improving workflow efficiency.
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aicodebot-0.9.5/README.md` & `aicodebot-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.5/aicodebot/cli.py` & `aicodebot-0.9.6/aicodebot/cli.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.5/aicodebot/coder.py` & `aicodebot-0.9.6/aicodebot/coder.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         """Get a text representation of the git diff for the current commit or staged files, including new files"""
         base_git_diff = ["git", "diff", "-U10"]  # Tell diff to provide 10 lines of context
 
         if commit:
             # If a commit is provided, just get the diff for that commit
             logger.debug(f"Getting diff for commit {commit}")
             show = exec_and_get_output(["git", "show", commit])
-            logger.debug(f"Diff for commit {commit}: {show}")
+            logger.opt(raw=True).debug(f"Diff for commit {commit}: {show}")
             return show
         else:
             # Otherwise, get the diff for the staged files, or if there are none, the diff for the unstaged files
             staged_files = exec_and_get_output(["git", "diff", "--cached", "--name-only"]).splitlines()
             if staged_files:
                 logger.debug(f"Getting diff for staged files: {staged_files}")
                 diff_type = "--cached"
```

### Comparing `aicodebot-0.9.5/aicodebot/config.py` & `aicodebot-0.9.6/aicodebot/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from aicodebot.helpers import logger
 from pathlib import Path
 import functools, os, yaml
 
 
-@functools.lru_cache
 def get_config_file():
     if "AICODEBOT_CONFIG_FILE" in os.environ:
         config_file = Path(os.getenv("AICODEBOT_CONFIG_FILE"))
     else:
         config_file = Path(Path.home() / ".aicodebot.yaml")
-    logger.debug(f"Using config file {config_file}")
     return config_file
 
 
 @functools.lru_cache
 def read_config():
     """Read the config file and return its contents as a dictionary."""
     config_file = get_config_file()
+    logger.debug(f"Using config file {config_file}")
     if config_file.exists():
         logger.debug(f"Config file {config_file} exists")
         with Path(config_file).open("r") as f:
             return yaml.safe_load(f)
     else:
         logger.debug(f"Config file {config_file} does not exist")
         return None
```

### Comparing `aicodebot-0.9.5/aicodebot/helpers.py` & `aicodebot-0.9.6/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.5/aicodebot/prompts.py` & `aicodebot-0.9.6/aicodebot/prompts.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.5/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.9.6/aicodebot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.5
+Version: 0.9.6
 Summary: AI-powered tool for developers, simplifying coding tasks and improving workflow efficiency.
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aicodebot-0.9.5/pyproject.toml` & `aicodebot-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.5/setup.py` & `aicodebot-0.9.6/setup.py`

 * *Files identical despite different names*

