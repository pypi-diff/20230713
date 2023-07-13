# Comparing `tmp/tokenmonster-1.1.4.tar.gz` & `tmp/tokenmonster-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenmonster-1.1.4.tar", last modified: Wed Jul 12 14:21:10 2023, max compression
+gzip compressed data, was "tokenmonster-1.1.5.tar", last modified: Thu Jul 13 12:47:52 2023, max compression
```

## Comparing `tokenmonster-1.1.4.tar` & `tokenmonster-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:21:10.009109 tokenmonster-1.1.4/
--rw-r--r--   0 root         (0) root         (0)    16622 2023-07-12 14:21:10.009109 tokenmonster-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16887 2023-07-12 14:01:39.000000 tokenmonster-1.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:21:10.009109 tokenmonster-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      550 2023-07-12 14:19:35.000000 tokenmonster-1.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:21:10.009109 tokenmonster-1.1.4/tokenmonster.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16622 2023-07-12 14:21:09.000000 tokenmonster-1.1.4/tokenmonster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-12 14:21:09.000000 tokenmonster-1.1.4/tokenmonster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:21:09.000000 tokenmonster-1.1.4/tokenmonster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 14:21:09.000000 tokenmonster-1.1.4/tokenmonster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    49041 2023-07-12 14:19:11.000000 tokenmonster-1.1.4/tokenmonster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 12:47:52.938187 tokenmonster-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)    16622 2023-07-13 12:47:52.938187 tokenmonster-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16887 2023-07-12 14:01:39.000000 tokenmonster-1.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 12:47:52.938187 tokenmonster-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-13 12:45:02.000000 tokenmonster-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 12:47:52.938187 tokenmonster-1.1.5/tokenmonster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16622 2023-07-13 12:47:52.000000 tokenmonster-1.1.5/tokenmonster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-13 12:47:52.000000 tokenmonster-1.1.5/tokenmonster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 12:47:52.000000 tokenmonster-1.1.5/tokenmonster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 12:47:52.000000 tokenmonster-1.1.5/tokenmonster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    49113 2023-07-13 12:41:46.000000 tokenmonster-1.1.5/tokenmonster.py
```

### Comparing `tokenmonster-1.1.4/PKG-INFO` & `tokenmonster-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tokenmonster-1.1.4/README.md` & `tokenmonster-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tokenmonster-1.1.4/setup.py` & `tokenmonster-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tokenmonster',
-    version='1.1.4',
+    version='1.1.5',
     py_modules=['tokenmonster'],
     author='Alasdair Forsythe',
     author_email='77910352+alasdairforsythe@users.noreply.github.com',
     description='Tokenize and decode text with TokenMonster vocabularies.',
     url='https://github.com/alasdairforsythe/tokenmonster',
     license='MIT',
     long_description=long_description,
```

### Comparing `tokenmonster-1.1.4/tokenmonster.egg-info/PKG-INFO` & `tokenmonster-1.1.5/tokenmonster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tokenmonster-1.1.4/tokenmonster.py` & `tokenmonster-1.1.5/tokenmonster.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,34 +170,36 @@
                 path = os.path.join(Vocab._dir, path + ".vocab")
             else:
                 clean = path.replace("+", "")
                 if Vocab._file_exists(clean + ".vocab"):
                     path = os.path.join(Vocab._dir, clean + ".vocab")
                 else:
                     if _is_prebuilt(clean):
-                        path = clean
-                        Vocab._download(_TOKENMONSTER_URL + "vocabs/" + path + ".vocab", path + ".vocab")
-                        if not Vocab._file_exists(path + ".vocab"):
+                        path = clean + ".vocab"
+                        Vocab._download(_TOKENMONSTER_URL + "vocabs/" + path, path)
+                        if Vocab._file_exists(path):
+                            path = os.path.join(Vocab._dir, path)
+                        else:
                             raise RuntimeError("TokenMonster: Unable to download the prebuilt vocabulary, please check availability at huggingface.co/alasdairforsythe/tokenmonster")
         elif path.startswith("http://") or path.startswith("https://"):
             fname = os.path.basename(path)
             if Vocab._file_exists(fname):
                 path = os.path.join(Vocab._dir, fname)
             else:
                 Vocab._download(path, fname)
                 if Vocab._file_exists(fname):
                     path = os.path.join(Vocab._dir, fname)
                 else:
                     raise FileNotFoundError("TokenMonster: Unable to download " + path + " to " + Vocab._dir)
         elif os.path.isfile(path):
             pass
-        elif Vocab._file_exists(path + ".vocab"):
-            path = os.path.join(Vocab._dir, path + ".vocab")
         elif Vocab._file_exists(path):
             path = os.path.join(Vocab._dir, path)
+        elif Vocab._file_exists(path + ".vocab"):
+            path = os.path.join(Vocab._dir, path + ".vocab")
         else:
             raise FileNotFoundError("TokenMonster: Unable to locate " + path)
         # Now read the vocabulary header
         with open(path, 'rb') as file:
             vocab_header = file.read(14)
         self._capcode = vocab_header[0]
         self._charset = vocab_header[1]
```

