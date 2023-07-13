# Comparing `tmp/codesnipper-0.1.8.tar.gz` & `tmp/codesnipper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codesnipper-0.1.8.tar", last modified: Wed Aug 10 10:36:02 2022, max compression
+gzip compressed data, was "codesnipper-0.1.9.tar", last modified: Sat Aug 13 15:32:55 2022, max compression
```

## Comparing `codesnipper-0.1.8.tar` & `codesnipper-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-08-10 10:36:02.369479 codesnipper-0.1.8/
--rw-rw-rw-   0        0        0     1091 2022-08-10 10:26:23.000000 codesnipper-0.1.8/LICENSE
--rw-rw-rw-   0        0        0        0 2022-08-10 10:26:23.000000 codesnipper-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    16031 2022-08-10 10:36:02.367492 codesnipper-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    15444 2022-08-10 10:26:23.000000 codesnipper-0.1.8/README.md
--rw-rw-rw-   0        0        0      108 2022-08-10 10:26:23.000000 codesnipper-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-10 10:36:02.374479 codesnipper-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1303 2022-08-10 10:32:25.000000 codesnipper-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-10 10:36:02.029382 codesnipper-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-10 10:36:02.121147 codesnipper-0.1.8/src/codesnipper.egg-info/
--rw-rw-rw-   0        0        0    16031 2022-08-10 10:36:01.000000 codesnipper-0.1.8/src/codesnipper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2022-08-10 10:36:02.000000 codesnipper-0.1.8/src/codesnipper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-10 10:36:01.000000 codesnipper-0.1.8/src/codesnipper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-08-10 10:36:01.000000 codesnipper-0.1.8/src/codesnipper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-10 10:36:01.000000 codesnipper-0.1.8/src/codesnipper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-10 10:36:02.364492 codesnipper-0.1.8/src/snipper/
--rw-rw-rw-   0        0        0       84 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/__init__.py
--rw-rw-rw-   0        0        0     3845 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/block_parsing.py
--rw-rw-rw-   0        0        0     7292 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/fix_bf.py
--rw-rw-rw-   0        0        0     2849 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/fix_cite.py
--rw-rw-rw-   0        0        0     3516 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/fix_i.py
--rw-rw-rw-   0        0        0     1304 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/fix_o.py
--rw-rw-rw-   0        0        0      208 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/fix_r.py
--rw-rw-rw-   0        0        0     1830 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/fix_s.py
--rw-rw-rw-   0        0        0     3059 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/legacy.py
--rw-rw-rw-   0        0        0     7546 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/load_citations.py
--rw-rw-rw-   0        0        0     3311 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/snip_dir.py
--rw-rw-rw-   0        0        0     3042 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/snipper_main.py
--rw-rw-rw-   0        0        0       13 2022-08-10 10:26:23.000000 codesnipper-0.1.8/src/snipper/test.py
--rw-rw-rw-   0        0        0       21 2022-08-10 10:26:53.000000 codesnipper-0.1.8/src/snipper/version.py
+drwxrwxrwx   0        0        0        0 2022-08-13 15:32:55.982890 codesnipper-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2022-08-10 10:26:23.000000 codesnipper-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2022-08-10 10:26:23.000000 codesnipper-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    16031 2022-08-13 15:32:55.980895 codesnipper-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15444 2022-08-10 10:26:23.000000 codesnipper-0.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2022-08-10 10:26:23.000000 codesnipper-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-08-13 15:32:55.982890 codesnipper-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1303 2022-08-10 10:32:25.000000 codesnipper-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-13 15:32:55.895124 codesnipper-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2022-08-13 15:32:55.942996 codesnipper-0.1.9/src/codesnipper.egg-info/
+-rw-rw-rw-   0        0        0    16031 2022-08-13 15:32:55.000000 codesnipper-0.1.9/src/codesnipper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2022-08-13 15:32:55.000000 codesnipper-0.1.9/src/codesnipper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-13 15:32:55.000000 codesnipper-0.1.9/src/codesnipper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2022-08-13 15:32:55.000000 codesnipper-0.1.9/src/codesnipper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-08-13 15:32:55.000000 codesnipper-0.1.9/src/codesnipper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-13 15:32:55.978901 codesnipper-0.1.9/src/snipper/
+-rw-rw-rw-   0        0        0       84 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/__init__.py
+-rw-rw-rw-   0        0        0     3845 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/block_parsing.py
+-rw-rw-rw-   0        0        0     7292 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/fix_bf.py
+-rw-rw-rw-   0        0        0     2849 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/fix_cite.py
+-rw-rw-rw-   0        0        0     3516 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/fix_i.py
+-rw-rw-rw-   0        0        0     1304 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/fix_o.py
+-rw-rw-rw-   0        0        0      208 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/fix_r.py
+-rw-rw-rw-   0        0        0     1830 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/fix_s.py
+-rw-rw-rw-   0        0        0     3059 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/legacy.py
+-rw-rw-rw-   0        0        0     7546 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/load_citations.py
+-rw-rw-rw-   0        0        0     3372 2022-08-13 15:32:36.000000 codesnipper-0.1.9/src/snipper/snip_dir.py
+-rw-rw-rw-   0        0        0     3042 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/snipper_main.py
+-rw-rw-rw-   0        0        0       13 2022-08-10 10:26:23.000000 codesnipper-0.1.9/src/snipper/test.py
+-rw-rw-rw-   0        0        0       21 2022-08-13 15:31:48.000000 codesnipper-0.1.9/src/snipper/version.py
```

### Comparing `codesnipper-0.1.8/LICENSE` & `codesnipper-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/PKG-INFO` & `codesnipper-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codesnipper
-Version: 0.1.8
+Version: 0.1.9
 Summary: A lightweight framework for censoring student solutions files and extracting code + output
 Home-page: https://lab.compute.dtu.dk/tuhe/snipper
 Author: Tue Herlau
 Author-email: tuhe@dtu.dk
 License: MIT
 Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/snipper/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `codesnipper-0.1.8/README.md` & `codesnipper-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/setup.py` & `codesnipper-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/codesnipper.egg-info/PKG-INFO` & `codesnipper-0.1.9/src/codesnipper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codesnipper
-Version: 0.1.8
+Version: 0.1.9
 Summary: A lightweight framework for censoring student solutions files and extracting code + output
 Home-page: https://lab.compute.dtu.dk/tuhe/snipper
 Author: Tue Herlau
 Author-email: tuhe@dtu.dk
 License: MIT
 Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/snipper/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `codesnipper-0.1.8/src/codesnipper.egg-info/SOURCES.txt` & `codesnipper-0.1.9/src/codesnipper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/block_parsing.py` & `codesnipper-0.1.9/src/snipper/block_parsing.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/fix_bf.py` & `codesnipper-0.1.9/src/snipper/fix_bf.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/fix_cite.py` & `codesnipper-0.1.9/src/snipper/fix_cite.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/fix_i.py` & `codesnipper-0.1.9/src/snipper/fix_i.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/fix_o.py` & `codesnipper-0.1.9/src/snipper/fix_o.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/fix_s.py` & `codesnipper-0.1.9/src/snipper/fix_s.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/legacy.py` & `codesnipper-0.1.9/src/snipper/legacy.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/load_citations.py` & `codesnipper-0.1.9/src/snipper/load_citations.py`

 * *Files identical despite different names*

### Comparing `codesnipper-0.1.8/src/snipper/snip_dir.py` & `codesnipper-0.1.9/src/snipper/snip_dir.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-import os, shutil
+import os
+import shutil
 from snipper.snipper_main import censor_file
 from pathlib import Path
 import time
 import fnmatch
 import tempfile
-from line_profiler_pycharm import profile
+# from line_profiler_pycharm import profile
 
-@profile
+# @profile
 def snip_dir(source_dir,  # Sources
              dest_dir=None,  # Will write to this directory
              output_dir=None, # Where snippets are going to be stored
              references=None, # Reference database
              exclude=None, clean_destination_dir=True,
              run_files=True,  # Run #!o tags and #!i tags
              cut_files=True,   # censor files.
              license_head=None,
              censor_files=True,
+             verbose=True,
              ):
 
     print("Snipper fixing", source_dir)
-
     if dest_dir == None:
         dest_dir = tempfile.mkdtemp()
         print("[snipper]", "no destination dir was specified so using nonsense destination:", dest_dir)
 
     if references == None:
         references = dict(aux=None, bibtex=None,  commands=[])
 
@@ -45,16 +46,16 @@
 
     if clean_destination_dir:
         shutil.rmtree(dest_dir)
 
     os.makedirs(dest_dir)
     out = dest_dir
     hw = {'base': source_dir}
-
-    print(f"[snipper]: {hw['base']} -> {out}")
+    if verbose:
+        print(f"[snipper]: {hw['base']} -> {out}")
     if os.path.exists(dest_dir):
         shutil.rmtree(dest_dir)
 
     shutil.copytree(source_dir, dest_dir)
     time.sleep(0.02)
 
     ls = list(Path(dest_dir).glob('**/*'))
@@ -68,27 +69,28 @@
     cutouts = {}
     for f, accept in acceptable:
         if os.path.isdir(f) or not str(f).endswith(".py") or  str(f).endswith("_grade.py"):
             continue
         if accept:
             solution_list = []
             kwargs = {}
-            print("Snipper processing", f)
+            if verbose:
+                print("Snipper processing", f)
             nrem, cut = censor_file(f, run_files=run_files, run_out_dirs=output_dir, cut_files=cut_files,
                                # solution_list=solution_list,
                                base_path=dest_dir,
                                references=references,
                                license_head=license_head,
                                censor_files=censor_files,
                                **kwargs)
-            if nrem > 0:
+            if nrem > 0 and verbose:
                 print(f"{nrem}> {f}")
             cutouts[str(f)] = cut
             n += nrem
-    # print("[snipper]", "removing")
+
     for rm_file, accept in acceptable:
         rm_file = os.path.abspath(rm_file)
         if not accept:
             if os.path.isfile(rm_file):
                 os.remove(rm_file)
             else:
                 if os.path.isdir(rm_file+"/"):
```

### Comparing `codesnipper-0.1.8/src/snipper/snipper_main.py` & `codesnipper-0.1.9/src/snipper/snipper_main.py`

 * *Files identical despite different names*

