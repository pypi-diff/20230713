# Comparing `tmp/git2doc-0.2.3.tar.gz` & `tmp/git2doc-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2doc-0.2.3.tar", last modified: Sun Jun 25 20:19:16 2023, max compression
+gzip compressed data, was "git2doc-0.2.4.tar", last modified: Thu Jul 13 00:12:09 2023, max compression
```

## Comparing `git2doc-0.2.3.tar` & `git2doc-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 20:19:16.913595 git2doc-0.2.3/
--rw-rw-rw-   0        0        0     2942 2023-06-25 20:19:16.912599 git2doc-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2273 2023-06-25 20:06:36.000000 git2doc-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 20:19:16.898362 git2doc-0.2.3/git2doc/
--rw-rw-rw-   0        0        0        0 2023-06-19 20:38:01.000000 git2doc-0.2.3/git2doc/__init__.py
--rw-rw-rw-   0        0        0    12271 2023-06-25 19:48:30.000000 git2doc-0.2.3/git2doc/loader.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:19:16.908600 git2doc-0.2.3/git2doc.egg-info/
--rw-rw-rw-   0        0        0     2942 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 20:19:16.914599 git2doc-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-06-25 20:18:56.000000 git2doc-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 00:12:09.721788 git2doc-0.2.4/
+-rw-rw-rw-   0        0        0     2942 2023-07-13 00:12:09.720789 git2doc-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2273 2023-06-25 20:06:36.000000 git2doc-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 00:12:09.713792 git2doc-0.2.4/git2doc/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:38:01.000000 git2doc-0.2.4/git2doc/__init__.py
+-rw-rw-rw-   0        0        0    12438 2023-07-13 00:09:51.000000 git2doc-0.2.4/git2doc/loader.py
+drwxrwxrwx   0        0        0        0 2023-07-13 00:12:09.719792 git2doc-0.2.4/git2doc.egg-info/
+-rw-rw-rw-   0        0        0     2942 2023-07-13 00:12:09.000000 git2doc-0.2.4/git2doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-07-13 00:12:09.000000 git2doc-0.2.4/git2doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 00:12:09.000000 git2doc-0.2.4/git2doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-13 00:12:09.000000 git2doc-0.2.4/git2doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 00:12:09.000000 git2doc-0.2.4/git2doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 00:12:09.721788 git2doc-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-07-13 00:11:41.000000 git2doc-0.2.4/setup.py
```

### Comparing `git2doc-0.2.3/PKG-INFO` & `git2doc-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.2.3
+Version: 0.2.4
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2doc-0.2.3/README.md` & `git2doc-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `git2doc-0.2.3/git2doc/loader.py` & `git2doc-0.2.4/git2doc/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from datetime import datetime, timedelta
 import dotenv
 from git import Blob, Repo
 from git.exc import InvalidGitRepositoryError, GitCommandError
 import os
 import math
 from pathlib import Path
-import polars as pl
 import requests
 import shutil
 import stat
 import time
 from typing import List, Optional, Dict
 
 
@@ -331,28 +330,28 @@
         except GitCommandError:
             shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
             retries += 1
     print(f"Failed to pull data from {repo_key} after {max_retries} attempts.")
     return None
 
 
-def write_to_parquet(filedata, metadata, base_filename, write_batch_counter):
-    """Write data to parquet files and clear the data"""
-    print(f"Writing batch {write_batch_counter} containing {len(filedata)} files..")
-
-    folder = "output_data"
-    if not os.path.exists(folder):
-        os.makedirs(folder)
-
-    pl.DataFrame(filedata).write_parquet(
-        f"{folder}/filedata_{base_filename}_{write_batch_counter}.parquet"
-    )
-    pl.DataFrame(metadata).write_parquet(
-        f"{folder}/metadata_{base_filename}_{write_batch_counter}.parquet"
-    )
+# def write_to_parquet(filedata, metadata, base_filename, write_batch_counter):
+#     """Write data to parquet files and clear the data"""
+#     print(f"Writing batch {write_batch_counter} containing {len(filedata)} files..")
+
+#     folder = "output_data"
+#     if not os.path.exists(folder):
+#         os.makedirs(folder)
+
+#     pl.DataFrame(filedata).write_parquet(
+#         f"{folder}/filedata_{base_filename}_{write_batch_counter}.parquet"
+#     )
+#     pl.DataFrame(metadata).write_parquet(
+#         f"{folder}/metadata_{base_filename}_{write_batch_counter}.parquet"
+#     )
 
 
 def process_repo(i, repo, metadata, filedata, delete=True):
     """Process a repository and add its data to the metadata and filedata lists."""
 
     if repo["size"]:
         repo_key = repo["html_url"]
@@ -399,20 +398,22 @@
         for i, repo in enumerate(repos):
             metadata, filedata = process_repo(
                 i, repo, metadata, filedata
             )
 
             # If the batch size is reached, write the data to parquet files and clear the lists
             if not (i + 1) % write_batch_size:
-                write_to_parquet(filedata, metadata, base_filename, write_batch_counter)
+                print("WARNING: write_to_parquet has been temporarily disabled")
+                # write_to_parquet(filedata, metadata, base_filename, write_batch_counter)
                 metadata.clear()
                 filedata.clear()
                 write_batch_counter += 1
 
         # Write the remaining data to parquet files
         if metadata and filedata:
-            write_to_parquet(filedata, metadata, base_filename, write_batch_counter)
+            print("WARNING: write_to_parquet has been temporarily disabled")
+            # write_to_parquet(filedata, metadata, base_filename, write_batch_counter)
 
     finally:
         # Always clean up the repo data folder
         if os.path.exists(REPODATA_FOLDER):
             shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
```

### Comparing `git2doc-0.2.3/git2doc.egg-info/PKG-INFO` & `git2doc-0.2.4/git2doc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.2.3
+Version: 0.2.4
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2doc-0.2.3/setup.py` & `git2doc-0.2.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2doc',
-    version='0.2.3',
+    version='0.2.4',
     description='A tool for converting git repositories into documents',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2doc',
     packages=find_packages(),
     install_requires=[
         'langchain',
```

