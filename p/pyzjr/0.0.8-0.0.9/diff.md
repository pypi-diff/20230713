# Comparing `tmp/pyzjr-0.0.8.tar.gz` & `tmp/pyzjr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-0.0.8.tar", last modified: Tue Jul  4 16:18:29 2023, max compression
+gzip compressed data, was "dist\pyzjr-0.0.9.tar", last modified: Fri Jul  7 11:36:33 2023, max compression
```

## Comparing `pyzjr-0.0.8.tar` & `pyzjr-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 16:18:29.000000 pyzjr-0.0.8/
--rw-rw-rw-   0        0        0     1515 2023-07-04 16:18:29.000000 pyzjr-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-07-04 16:18:21.000000 pyzjr-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr/
--rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-0.0.8/pyzjr/ColorModule.py
--rw-rw-rw-   0        0        0    18267 2023-07-04 09:37:15.000000 pyzjr-0.0.8/pyzjr/Enimage.py
--rw-rw-rw-   0        0        0     3624 2023-06-10 05:53:05.000000 pyzjr-0.0.8/pyzjr/PIC.py
--rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-0.0.8/pyzjr/TrackBar.py
--rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.8/pyzjr/Z.py
--rw-rw-rw-   0        0        0     1330 2023-07-04 16:03:33.000000 pyzjr-0.0.8/pyzjr/__init__.py
--rw-rw-rw-   0        0        0     5028 2023-07-04 09:36:12.000000 pyzjr-0.0.8/pyzjr/definition.py
--rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.8/pyzjr/utils.py
--rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.8/pyzjr/video.py
--rw-rw-rw-   0        0        0     2334 2023-07-04 09:41:55.000000 pyzjr-0.0.8/pyzjr/zmath.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     1515 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 16:18:29.000000 pyzjr-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1734 2023-07-04 09:41:57.000000 pyzjr-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:36:33.000000 pyzjr-0.0.9/
+-rw-rw-rw-   0        0        0     1591 2023-07-07 11:36:33.000000 pyzjr-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      664 2023-07-07 11:35:18.000000 pyzjr-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr/
+-rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-0.0.9/pyzjr/ColorModule.py
+-rw-rw-rw-   0        0        0    18267 2023-07-04 09:37:15.000000 pyzjr-0.0.9/pyzjr/Enimage.py
+-rw-rw-rw-   0        0        0     9091 2023-07-07 11:28:19.000000 pyzjr-0.0.9/pyzjr/MinIO.py
+-rw-rw-rw-   0        0        0     3624 2023-06-10 05:53:05.000000 pyzjr-0.0.9/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-0.0.9/pyzjr/TrackBar.py
+-rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.9/pyzjr/Z.py
+-rw-rw-rw-   0        0        0     1357 2023-07-07 11:29:39.000000 pyzjr-0.0.9/pyzjr/__init__.py
+-rw-rw-rw-   0        0        0     5028 2023-07-07 11:31:29.000000 pyzjr-0.0.9/pyzjr/definition.py
+-rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.9/pyzjr/utils.py
+-rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.9/pyzjr/video.py
+-rw-rw-rw-   0        0        0     2334 2023-07-04 09:41:55.000000 pyzjr-0.0.9/pyzjr/zmath.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     1591 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:36:33.000000 pyzjr-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1734 2023-07-07 11:29:41.000000 pyzjr-0.0.9/setup.py
```

### Comparing `pyzjr-0.0.8/PKG-INFO` & `pyzjr-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 0.0.8
+Version: 0.0.9
 Summary:  a computer vision library that supports both Win and Mac 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
@@ -21,14 +21,16 @@
         
         https://pypi.org/project/pyzjr/
         
         https://github.com/Auorui/pyzjr (I want stars ⭐ hhh)
         
         ## Update log
         
+        `0.0.9` Added mini module, can perform bucket operations
+        
         `0.0.8` Can be used normally, added zmath file
         
         `0.0.7` fix bug
         
         `0.0.1` first release
         
         ## Upload of Library
```

### Comparing `pyzjr-0.0.8/README.md` & `pyzjr-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 https://pypi.org/project/pyzjr/
 
 https://github.com/Auorui/pyzjr (I want stars ⭐ hhh)
 
 ## Update log
 
+`0.0.9` Added mini module, can perform bucket operations
+
 `0.0.8` Can be used normally, added zmath file
 
 `0.0.7` fix bug
 
 `0.0.1` first release
 
 ## Upload of Library
```

### Comparing `pyzjr-0.0.8/pyzjr/ColorModule.py` & `pyzjr-0.0.9/pyzjr/ColorModule.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.8/pyzjr/Enimage.py` & `pyzjr-0.0.9/pyzjr/Enimage.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.8/pyzjr/PIC.py` & `pyzjr-0.0.9/pyzjr/PIC.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.8/pyzjr/TrackBar.py` & `pyzjr-0.0.9/pyzjr/TrackBar.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.8/pyzjr/__init__.py` & `pyzjr-0.0.9/pyzjr/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 """
 from pyzjr import pyps as ps  # Using Image Processing
 from pyzjr import pysift as sift  # Using SIFT matching algorithm
 from pyzjr import Color as color
 """
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import cv2
 
 
 from pyzjr.PIC import download_file,getPhotopath,Pic_rename,read_resize_image,\
                       load_images_from_folder,save_images
 from pyzjr.Enimage import Filter,Enhance,Random_Enhance,Retinex,\
@@ -28,14 +28,15 @@
 from pyzjr.ColorModule import *
 from pyzjr.definition import *
 from pyzjr.TrackBar import *
 from pyzjr.utils import *
 from pyzjr.video import *
 from pyzjr.Z import * 
 from pyzjr.zmath import *
+from pyzjr.MinIO import *
 
 repair_TELEA=cv2.INPAINT_TELEA
 repair_NS=cv2.INPAINT_NS
 Lap_64F=cv2.CV_64F
 
 # print("test successful")  #仅仅在测试时候使用，其他时候不用
```

### Comparing `pyzjr-0.0.8/pyzjr/definition.py` & `pyzjr-0.0.9/pyzjr/definition.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.8/pyzjr/utils.py` & `pyzjr-0.0.9/pyzjr/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.8/pyzjr/video.py` & `pyzjr-0.0.9/pyzjr/video.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.8/pyzjr/zmath.py` & `pyzjr-0.0.9/pyzjr/zmath.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.8/pyzjr.egg-info/PKG-INFO` & `pyzjr-0.0.9/pyzjr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 0.0.8
+Version: 0.0.9
 Summary:  a computer vision library that supports both Win and Mac 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
@@ -21,14 +21,16 @@
         
         https://pypi.org/project/pyzjr/
         
         https://github.com/Auorui/pyzjr (I want stars ⭐ hhh)
         
         ## Update log
         
+        `0.0.9` Added mini module, can perform bucket operations
+        
         `0.0.8` Can be used normally, added zmath file
         
         `0.0.7` fix bug
         
         `0.0.1` first release
         
         ## Upload of Library
```

### Comparing `pyzjr-0.0.8/setup.py` & `pyzjr-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = ' a computer vision library that supports both Win and Mac '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports both Win and Mac'
 
 setup(
     name="pyzjr",
     version=VERSION,
     author="Auorui",
```

