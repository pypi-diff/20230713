# Comparing `tmp/progress parallel-3.1.2.tar.gz` & `tmp/progress parallel-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress parallel-3.1.2.tar", last modified: Sun Jan 22 12:43:31 2023, max compression
+gzip compressed data, was "progress parallel-3.2.1.tar", last modified: Thu Jul 13 12:32:31 2023, max compression
```

## Comparing `progress parallel-3.1.2.tar` & `progress parallel-3.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-22 12:43:31.400270 progress parallel-3.1.2/
--rw-rw-rw-   0        0        0     1092 2023-01-11 02:05:51.000000 progress parallel-3.1.2/LICENSE
--rw-rw-rw-   0        0        0    13178 2023-01-22 12:43:31.400270 progress parallel-3.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-22 12:43:31.363288 progress parallel-3.1.2/progress_parallel.egg-info/
--rw-rw-rw-   0        0        0    13178 2023-01-22 12:43:31.000000 progress parallel-3.1.2/progress_parallel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-01-22 12:43:31.000000 progress parallel-3.1.2/progress_parallel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-22 12:43:31.000000 progress parallel-3.1.2/progress_parallel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-01-22 12:43:31.000000 progress parallel-3.1.2/progress_parallel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-22 12:43:31.398265 progress parallel-3.1.2/prpl/
--rw-rw-rw-   0        0        0      783 2023-01-22 12:28:26.000000 progress parallel-3.1.2/prpl/__init__.py
--rw-rw-rw-   0        0        0     4453 2023-01-22 12:31:21.000000 progress parallel-3.1.2/prpl/prpl.py
--rw-rw-rw-   0        0        0     1909 2023-01-22 12:29:11.000000 progress parallel-3.1.2/prpl/prpl_for_loop_progress.py
--rw-rw-rw-   0        0        0     3741 2023-01-22 12:32:13.000000 progress parallel-3.1.2/prpl/prpl_progress.py
--rw-rw-rw-   0        0        0     2383 2023-01-22 12:32:41.000000 progress parallel-3.1.2/prpl/prpl_progress_simple.py
--rw-rw-rw-   0        0        0       42 2023-01-22 12:43:31.400270 progress parallel-3.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-01-17 16:54:57.000000 progress parallel-3.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:32:31.679802 progress parallel-3.2.1/
+-rw-rw-rw-   0        0        0     1092 2023-01-11 02:05:51.000000 progress parallel-3.2.1/LICENSE
+-rw-rw-rw-   0        0        0    13109 2023-07-13 12:32:31.679802 progress parallel-3.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 12:32:31.662028 progress parallel-3.2.1/progress_parallel.egg-info/
+-rw-rw-rw-   0        0        0    13109 2023-07-13 12:32:31.000000 progress parallel-3.2.1/progress_parallel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-13 12:32:31.000000 progress parallel-3.2.1/progress_parallel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:32:31.000000 progress parallel-3.2.1/progress_parallel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-13 12:32:31.000000 progress parallel-3.2.1/progress_parallel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 12:32:31.678789 progress parallel-3.2.1/prpl/
+-rw-rw-rw-   0        0        0      783 2023-01-22 12:28:26.000000 progress parallel-3.2.1/prpl/__init__.py
+-rw-rw-rw-   0        0        0     4529 2023-07-13 12:18:58.000000 progress parallel-3.2.1/prpl/prpl.py
+-rw-rw-rw-   0        0        0     1909 2023-01-22 12:29:11.000000 progress parallel-3.2.1/prpl/prpl_for_loop_progress.py
+-rw-rw-rw-   0        0        0     3741 2023-01-22 12:32:13.000000 progress parallel-3.2.1/prpl/prpl_progress.py
+-rw-rw-rw-   0        0        0     2383 2023-01-22 12:32:41.000000 progress parallel-3.2.1/prpl/prpl_progress_simple.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 12:32:31.679802 progress parallel-3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2023-01-17 16:54:57.000000 progress parallel-3.2.1/setup.py
```

### Comparing `progress parallel-3.1.2/LICENSE` & `progress parallel-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `progress parallel-3.1.2/PKG-INFO` & `progress parallel-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress parallel
-Version: 3.1.2
+Version: 3.2.1
 Summary: multi threading progress bar
 Home-page: https://github.com/Domzou-kun/prpl
 Download-URL: https://github.com/Domzou-kun/prpl
 Author: Domzou
 License: MIT
 Keywords: Python python progress multi thread threading
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -32,18 +32,17 @@
 </a>
 
 </div>
 
 <div align="center">
    <br>
    
-   # **the latest version of 3.1.2🎉**
-   ## Changes in the new version of **3.1.2**
-   **- Minor modifications to some programs -**  
-   **- Add external link to Japanese readme in readme.md -**
+   # **the latest version of 3.2.1🎉**
+   ## Changes in the new version of **3.2.1**
+   **- Some serious bugs were fixed. -**  
    
    <br>
    <br>
 
    # CAUTION
    **Serious bugs are fixed as hotfixes in v3.1.1.  
    We have discovered a serious flaw in the functionality available in for-loop added in v3.0.1.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: progress parallel Version: 3.1.2 Summary: multi
+Metadata-Version: 2.1 Name: progress parallel Version: 3.2.1 Summary: multi
 threading progress bar Home-page: https://github.com/Domzou-kun/prpl Download-
 URL: https://github.com/Domzou-kun/prpl Author: Domzou License: MIT Keywords:
 Python python progress multi thread threading Classifier: Operating System ::
 Microsoft :: Windows :: Windows 10 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: System ::
@@ -19,17 +19,16 @@
                 img.shields.io/github/issues/Domzou-kun/prpl)
       ![GitHub followers](https://img.shields.io/github/followers/Domzou-
          kun?style=social) [![Twitter](https://badgen.net/badge/icon/
             tweet?icon=twitter&label)](https://twitter.com/intent/
  tweet?text="prpl"%20is%20a%20recommended%20repositoryðð%0a&url=https://
               github.com/Domzou-kun/prpl&hashtags=Github,Python)
 
-    # **the latest version of 3.1.2ð** ## Changes in the new version of
-**3.1.2** **- Minor modifications to some programs -** **- Add external link to
-                       Japanese readme in readme.md -**
+    # **the latest version of 3.2.1ð** ## Changes in the new version of
+               **3.2.1** **- Some serious bugs were fixed. -**
 
 # CAUTION **Serious bugs are fixed as hotfixes in v3.1.1. We have discovered a
  serious flaw in the functionality available in for-loop added in v3.0.1. This
 has been corrected in v3.1.1. Accordingly, v3.0.1 has been removed from PyPI.**
 
 
 --- # prpl `prpl`(progress-parallel) is a library to visualize the progress of
```

### Comparing `progress parallel-3.1.2/progress_parallel.egg-info/PKG-INFO` & `progress parallel-3.2.1/progress_parallel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-parallel
-Version: 3.1.2
+Version: 3.2.1
 Summary: multi threading progress bar
 Home-page: https://github.com/Domzou-kun/prpl
 Download-URL: https://github.com/Domzou-kun/prpl
 Author: Domzou
 License: MIT
 Keywords: Python python progress multi thread threading
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -32,18 +32,17 @@
 </a>
 
 </div>
 
 <div align="center">
    <br>
    
-   # **the latest version of 3.1.2🎉**
-   ## Changes in the new version of **3.1.2**
-   **- Minor modifications to some programs -**  
-   **- Add external link to Japanese readme in readme.md -**
+   # **the latest version of 3.2.1🎉**
+   ## Changes in the new version of **3.2.1**
+   **- Some serious bugs were fixed. -**  
    
    <br>
    <br>
 
    # CAUTION
    **Serious bugs are fixed as hotfixes in v3.1.1.  
    We have discovered a serious flaw in the functionality available in for-loop added in v3.0.1.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: progress-parallel Version: 3.1.2 Summary: multi
+Metadata-Version: 2.1 Name: progress-parallel Version: 3.2.1 Summary: multi
 threading progress bar Home-page: https://github.com/Domzou-kun/prpl Download-
 URL: https://github.com/Domzou-kun/prpl Author: Domzou License: MIT Keywords:
 Python python progress multi thread threading Classifier: Operating System ::
 Microsoft :: Windows :: Windows 10 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: System ::
@@ -19,17 +19,16 @@
                 img.shields.io/github/issues/Domzou-kun/prpl)
       ![GitHub followers](https://img.shields.io/github/followers/Domzou-
          kun?style=social) [![Twitter](https://badgen.net/badge/icon/
             tweet?icon=twitter&label)](https://twitter.com/intent/
  tweet?text="prpl"%20is%20a%20recommended%20repositoryðð%0a&url=https://
               github.com/Domzou-kun/prpl&hashtags=Github,Python)
 
-    # **the latest version of 3.1.2ð** ## Changes in the new version of
-**3.1.2** **- Minor modifications to some programs -** **- Add external link to
-                       Japanese readme in readme.md -**
+    # **the latest version of 3.2.1ð** ## Changes in the new version of
+               **3.2.1** **- Some serious bugs were fixed. -**
 
 # CAUTION **Serious bugs are fixed as hotfixes in v3.1.1. We have discovered a
  serious flaw in the functionality available in for-loop added in v3.0.1. This
 has been corrected in v3.1.1. Accordingly, v3.0.1 has been removed from PyPI.**
 
 
 --- # prpl `prpl`(progress-parallel) is a library to visualize the progress of
```

### Comparing `progress parallel-3.1.2/prpl/__init__.py` & `progress parallel-3.2.1/prpl/__init__.py`

 * *Files identical despite different names*

### Comparing `progress parallel-3.1.2/prpl/prpl.py` & `progress parallel-3.2.1/prpl/prpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,18 @@
         return list_for_loop_progress(target_list = target_list, checkpoint = checkpoint, title = title, symbol = symbol, symbol_c = symbol_c, c = c_num)
 
     """ Terminal line size """
     terminal_line_size = shutil.get_terminal_size().lines
     print("\n"*terminal_line_size + f"\033[{terminal_line_size}A")  # scroll line
     """ List separate """
     target_list_length = len(target_list)
-    sep_num = int(target_list_length / list_sep)
+    if target_list_length >= list_sep:
+        sep_num = int(target_list_length / list_sep)
+    else:
+        sep_num = 1
     sep_list = [ target_list[sep_ : sep_ + sep_num] for sep_ in range(0, target_list_length, sep_num) ]   # split list along variable list_sep
     """ check variable list_sep """
     if len(sep_list) != list_sep:
         list_sep = len(sep_list)
     """ check arguments dict """
     if args is not None:
         target_function_arguments_list = list(signature(target_function).parameters.keys())
```

### Comparing `progress parallel-3.1.2/prpl/prpl_for_loop_progress.py` & `progress parallel-3.2.1/prpl/prpl_for_loop_progress.py`

 * *Files identical despite different names*

### Comparing `progress parallel-3.1.2/prpl/prpl_progress.py` & `progress parallel-3.2.1/prpl/prpl_progress.py`

 * *Files identical despite different names*

### Comparing `progress parallel-3.1.2/prpl/prpl_progress_simple.py` & `progress parallel-3.2.1/prpl/prpl_progress_simple.py`

 * *Files identical despite different names*

### Comparing `progress parallel-3.1.2/setup.py` & `progress parallel-3.2.1/setup.py`

 * *Files identical despite different names*

