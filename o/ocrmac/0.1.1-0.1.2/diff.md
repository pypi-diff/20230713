# Comparing `tmp/ocrmac-0.1.1.tar.gz` & `tmp/ocrmac-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocrmac-0.1.1.tar", last modified: Fri Dec 30 22:03:22 2022, max compression
+gzip compressed data, was "ocrmac-0.1.2.tar", last modified: Thu Jul 13 08:56:38 2023, max compression
```

## Comparing `ocrmac-0.1.1.tar` & `ocrmac-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 flq567     (502) staff       (20)        0 2022-12-30 22:03:22.664005 ocrmac-0.1.1/
--rw-r--r--   0 flq567     (502) staff       (20)     3523 2022-12-30 21:58:05.000000 ocrmac-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 flq567     (502) staff       (20)     1076 2022-12-30 21:58:05.000000 ocrmac-0.1.1/LICENSE
--rw-r--r--   0 flq567     (502) staff       (20)      262 2022-12-30 21:58:05.000000 ocrmac-0.1.1/MANIFEST.in
--rw-r--r--   0 flq567     (502) staff       (20)     4242 2022-12-30 22:03:22.664107 ocrmac-0.1.1/PKG-INFO
--rw-r--r--   0 flq567     (502) staff       (20)     3349 2022-12-30 21:58:05.000000 ocrmac-0.1.1/README.md
-drwxr-xr-x   0 flq567     (502) staff       (20)        0 2022-12-30 22:03:22.649391 ocrmac-0.1.1/docs/
--rw-r--r--   0 flq567     (502) staff       (20)      607 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/Makefile
--rwxr-xr-x   0 flq567     (502) staff       (20)     4790 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/conf.py
--rw-r--r--   0 flq567     (502) staff       (20)       33 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/contributing.rst
--rw-r--r--   0 flq567     (502) staff       (20)       28 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/history.rst
--rw-r--r--   0 flq567     (502) staff       (20)      303 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/index.rst
--rw-r--r--   0 flq567     (502) staff       (20)     1142 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/installation.rst
--rw-r--r--   0 flq567     (502) staff       (20)      804 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/make.bat
--rw-r--r--   0 flq567     (502) staff       (20)       26 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/readme.rst
--rw-r--r--   0 flq567     (502) staff       (20)       67 2022-12-30 21:58:05.000000 ocrmac-0.1.1/docs/usage.rst
-drwxr-xr-x   0 flq567     (502) staff       (20)        0 2022-12-30 22:03:22.651334 ocrmac-0.1.1/ocrmac/
--rw-r--r--   0 flq567     (502) staff       (20)      139 2022-12-30 21:59:44.000000 ocrmac-0.1.1/ocrmac/__init__.py
--rw-r--r--   0 flq567     (502) staff       (20)      544 2022-12-30 21:58:05.000000 ocrmac-0.1.1/ocrmac/cli.py
--rw-r--r--   0 flq567     (502) staff       (20)     6029 2022-12-30 21:58:05.000000 ocrmac-0.1.1/ocrmac/ocrmac.py
-drwxr-xr-x   0 flq567     (502) staff       (20)        0 2022-12-30 22:03:22.661716 ocrmac-0.1.1/ocrmac.egg-info/
--rw-r--r--   0 flq567     (502) staff       (20)     4242 2022-12-30 22:03:22.000000 ocrmac-0.1.1/ocrmac.egg-info/PKG-INFO
--rw-r--r--   0 flq567     (502) staff       (20)      528 2022-12-30 22:03:22.000000 ocrmac-0.1.1/ocrmac.egg-info/SOURCES.txt
--rw-r--r--   0 flq567     (502) staff       (20)        1 2022-12-30 22:03:22.000000 ocrmac-0.1.1/ocrmac.egg-info/dependency_links.txt
--rw-r--r--   0 flq567     (502) staff       (20)       43 2022-12-30 22:03:22.000000 ocrmac-0.1.1/ocrmac.egg-info/entry_points.txt
--rw-r--r--   0 flq567     (502) staff       (20)        1 2022-12-30 22:03:22.000000 ocrmac-0.1.1/ocrmac.egg-info/not-zip-safe
--rw-r--r--   0 flq567     (502) staff       (20)       42 2022-12-30 22:03:22.000000 ocrmac-0.1.1/ocrmac.egg-info/requires.txt
--rw-r--r--   0 flq567     (502) staff       (20)        7 2022-12-30 22:03:22.000000 ocrmac-0.1.1/ocrmac.egg-info/top_level.txt
--rw-r--r--   0 flq567     (502) staff       (20)      378 2022-12-30 22:03:22.665710 ocrmac-0.1.1/setup.cfg
--rw-r--r--   0 flq567     (502) staff       (20)     1547 2022-12-30 21:59:44.000000 ocrmac-0.1.1/setup.py
-drwxr-xr-x   0 flq567     (502) staff       (20)        0 2022-12-30 22:03:22.663648 ocrmac-0.1.1/tests/
--rw-r--r--   0 flq567     (502) staff       (20)       36 2022-12-30 21:58:05.000000 ocrmac-0.1.1/tests/__init__.py
--rw-r--r--   0 flq567     (502) staff       (20)   436714 2022-12-30 21:58:05.000000 ocrmac-0.1.1/tests/test.png
--rw-r--r--   0 flq567     (502) staff       (20)     1799 2022-12-30 21:58:05.000000 ocrmac-0.1.1/tests/test_ocrmac.py
+drwxr-xr-x   0 flq567     (502) staff       (20)        0 2023-07-13 08:56:38.169760 ocrmac-0.1.2/
+-rw-r--r--   0 flq567     (502) staff       (20)     3523 2022-12-30 21:58:05.000000 ocrmac-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 flq567     (502) staff       (20)     1076 2022-12-30 21:58:05.000000 ocrmac-0.1.2/LICENSE
+-rw-r--r--   0 flq567     (502) staff       (20)      262 2022-12-30 21:58:05.000000 ocrmac-0.1.2/MANIFEST.in
+-rw-r--r--   0 flq567     (502) staff       (20)     4242 2023-07-13 08:56:38.169863 ocrmac-0.1.2/PKG-INFO
+-rw-r--r--   0 flq567     (502) staff       (20)     3349 2022-12-30 21:58:05.000000 ocrmac-0.1.2/README.md
+drwxr-xr-x   0 flq567     (502) staff       (20)        0 2023-07-13 08:56:38.148203 ocrmac-0.1.2/docs/
+-rw-r--r--   0 flq567     (502) staff       (20)      607 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/Makefile
+-rwxr-xr-x   0 flq567     (502) staff       (20)     4790 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/conf.py
+-rw-r--r--   0 flq567     (502) staff       (20)       33 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/contributing.rst
+-rw-r--r--   0 flq567     (502) staff       (20)       28 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/history.rst
+-rw-r--r--   0 flq567     (502) staff       (20)      303 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/index.rst
+-rw-r--r--   0 flq567     (502) staff       (20)     1142 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/installation.rst
+-rw-r--r--   0 flq567     (502) staff       (20)      804 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/make.bat
+-rw-r--r--   0 flq567     (502) staff       (20)       26 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/readme.rst
+-rw-r--r--   0 flq567     (502) staff       (20)       67 2022-12-30 21:58:05.000000 ocrmac-0.1.2/docs/usage.rst
+drwxr-xr-x   0 flq567     (502) staff       (20)        0 2023-07-13 08:56:38.152928 ocrmac-0.1.2/ocrmac/
+-rw-r--r--   0 flq567     (502) staff       (20)      139 2023-07-13 08:43:24.000000 ocrmac-0.1.2/ocrmac/__init__.py
+-rw-r--r--   0 flq567     (502) staff       (20)      544 2022-12-30 21:58:05.000000 ocrmac-0.1.2/ocrmac/cli.py
+-rw-r--r--   0 flq567     (502) staff       (20)     6139 2023-07-13 08:42:17.000000 ocrmac-0.1.2/ocrmac/ocrmac.py
+drwxr-xr-x   0 flq567     (502) staff       (20)        0 2023-07-13 08:56:38.165736 ocrmac-0.1.2/ocrmac.egg-info/
+-rw-r--r--   0 flq567     (502) staff       (20)     4242 2023-07-13 08:56:38.000000 ocrmac-0.1.2/ocrmac.egg-info/PKG-INFO
+-rw-r--r--   0 flq567     (502) staff       (20)      545 2023-07-13 08:56:38.000000 ocrmac-0.1.2/ocrmac.egg-info/SOURCES.txt
+-rw-r--r--   0 flq567     (502) staff       (20)        1 2023-07-13 08:56:38.000000 ocrmac-0.1.2/ocrmac.egg-info/dependency_links.txt
+-rw-r--r--   0 flq567     (502) staff       (20)       43 2023-07-13 08:56:38.000000 ocrmac-0.1.2/ocrmac.egg-info/entry_points.txt
+-rw-r--r--   0 flq567     (502) staff       (20)        1 2022-12-30 22:03:22.000000 ocrmac-0.1.2/ocrmac.egg-info/not-zip-safe
+-rw-r--r--   0 flq567     (502) staff       (20)       42 2023-07-13 08:56:38.000000 ocrmac-0.1.2/ocrmac.egg-info/requires.txt
+-rw-r--r--   0 flq567     (502) staff       (20)        7 2023-07-13 08:56:38.000000 ocrmac-0.1.2/ocrmac.egg-info/top_level.txt
+-rw-r--r--   0 flq567     (502) staff       (20)      378 2023-07-13 08:56:38.170924 ocrmac-0.1.2/setup.cfg
+-rw-r--r--   0 flq567     (502) staff       (20)     1547 2023-07-13 08:43:24.000000 ocrmac-0.1.2/setup.py
+drwxr-xr-x   0 flq567     (502) staff       (20)        0 2023-07-13 08:56:38.169393 ocrmac-0.1.2/tests/
+-rw-r--r--   0 flq567     (502) staff       (20)       36 2022-12-30 21:58:05.000000 ocrmac-0.1.2/tests/__init__.py
+-rw-r--r--   0 flq567     (502) staff       (20)      256 2023-07-13 08:45:18.000000 ocrmac-0.1.2/tests/test.ipynb
+-rw-r--r--   0 flq567     (502) staff       (20)   436714 2022-12-30 21:58:05.000000 ocrmac-0.1.2/tests/test.png
+-rw-r--r--   0 flq567     (502) staff       (20)     1799 2022-12-30 21:58:05.000000 ocrmac-0.1.2/tests/test_ocrmac.py
```

### Comparing `ocrmac-0.1.1/CONTRIBUTING.rst` & `ocrmac-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/LICENSE` & `ocrmac-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/PKG-INFO` & `ocrmac-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrmac
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python wrapper to extract text from images on a mac system. Uses the vision framework from Apple.
 Home-page: https://github.com/straussmaximilian/ocrmac
 Author: Maximilian Strauss
 Author-email: straussmaximilian@gmail.com
 License: MIT license
 Keywords: ocrmac
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ocrmac-0.1.1/README.md` & `ocrmac-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/docs/Makefile` & `ocrmac-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/docs/conf.py` & `ocrmac-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/docs/installation.rst` & `ocrmac-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/docs/make.bat` & `ocrmac-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/ocrmac/cli.py` & `ocrmac-0.1.2/ocrmac/cli.py`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/ocrmac/ocrmac.py` & `ocrmac-0.1.2/ocrmac/ocrmac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Main module."""
 
 import io
-import PIL
+import objc
 
 from PIL import ImageFont, ImageDraw, Image
 
 import Vision
 
 try:
     import matplotlib
@@ -71,42 +71,43 @@
         )
 
     if language_preference is not None and not isinstance(language_preference, list):
         raise ValueError(
             "Invalid language preference format. Language preference must be a list."
         )
 
-    req = Vision.VNRecognizeTextRequest.alloc().init().autorelease()
+    with objc.autorelease_pool():
+        req = Vision.VNRecognizeTextRequest.alloc().init()
 
-    if recognition_level == "fast":
-        req.setRecognitionLevel_(1)
-    else:
-        req.setRecognitionLevel_(0)
-
-    if language_preference is not None:
-        req.setRecognitionLanguages_(language_preference)
-
-    handler = (
-        Vision.VNImageRequestHandler.alloc()
-        .initWithData_options_(pil2buf(image), None)
-        .autorelease()
-    )
-    success = handler.performRequests_error_([req], None)
-
-    res = []
-    if success:
-        for result in req.results():
-
-            bbox = result.boundingBox()
-            w, h = bbox.size.width, bbox.size.height
-            x, y = bbox.origin.x, bbox.origin.y
+        if recognition_level == "fast":
+            req.setRecognitionLevel_(1)
+        else:
+            req.setRecognitionLevel_(0)
 
-            res.append((result.text(), result.confidence(), [x, y, w, h]))
+        if language_preference is not None:
+            req.setRecognitionLanguages_(language_preference)
 
-    return res
+        handler = Vision.VNImageRequestHandler.alloc().initWithData_options_(
+            pil2buf(image), None
+        )
+
+        success = handler.performRequests_error_([req], None)
+        res = []
+        if success:
+            for result in req.results():
+                bbox = result.boundingBox()
+                w, h = bbox.size.width, bbox.size.height
+                x, y = bbox.origin.x, bbox.origin.y
+
+                res.append((result.text(), result.confidence(), [x, y, w, h]))
+
+        req.dealloc()
+        handler.dealloc()
+
+        return res
 
 
 class OCR:
     def __init__(self, image, recognition_level="accurate", language_preference=None):
         """OCR class to extract text from images.
 
         Args:
@@ -125,15 +126,14 @@
 
         self.image = image
         self.recognition_level = recognition_level
         self.language_preference = language_preference
         self.res = None
 
     def recognize(self):
-
         res = text_from_image(
             self.image, self.recognition_level, self.language_preference
         )
         self.res = res
 
         return res
```

### Comparing `ocrmac-0.1.1/ocrmac.egg-info/PKG-INFO` & `ocrmac-0.1.2/ocrmac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrmac
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python wrapper to extract text from images on a mac system. Uses the vision framework from Apple.
 Home-page: https://github.com/straussmaximilian/ocrmac
 Author: Maximilian Strauss
 Author-email: straussmaximilian@gmail.com
 License: MIT license
 Keywords: ocrmac
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ocrmac-0.1.1/ocrmac.egg-info/SOURCES.txt` & `ocrmac-0.1.2/ocrmac.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 ocrmac.egg-info/SOURCES.txt
 ocrmac.egg-info/dependency_links.txt
 ocrmac.egg-info/entry_points.txt
 ocrmac.egg-info/not-zip-safe
 ocrmac.egg-info/requires.txt
 ocrmac.egg-info/top_level.txt
 tests/__init__.py
+tests/test.ipynb
 tests/test.png
 tests/test_ocrmac.py
```

### Comparing `ocrmac-0.1.1/setup.py` & `ocrmac-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords="ocrmac",
     name="ocrmac",
     packages=find_packages(include=["ocrmac", "ocrmac.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/straussmaximilian/ocrmac",
-    version="0.1.1",
+    version="0.1.2",
     zip_safe=False,
 )
```

### Comparing `ocrmac-0.1.1/tests/test.png` & `ocrmac-0.1.2/tests/test.png`

 * *Files identical despite different names*

### Comparing `ocrmac-0.1.1/tests/test_ocrmac.py` & `ocrmac-0.1.2/tests/test_ocrmac.py`

 * *Files identical despite different names*

