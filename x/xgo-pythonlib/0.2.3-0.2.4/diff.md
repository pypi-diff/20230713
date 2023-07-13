# Comparing `tmp/xgo-pythonlib-0.2.3.tar.gz` & `tmp/xgo-pythonlib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.2.3.tar", last modified: Tue Jul  4 13:34:53 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.2.4.tar", last modified: Thu Jul 13 03:16:22 2023, max compression
```

## Comparing `xgo-pythonlib-0.2.3.tar` & `xgo-pythonlib-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.670424 xgo-pythonlib-0.2.3/
--rw-rw-rw-   0        0        0     2490 2023-07-04 13:34:53.669424 xgo-pythonlib-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1863 2023-07-04 13:33:41.000000 xgo-pythonlib-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 13:34:53.670424 xgo-pythonlib-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     3744 2023-07-04 13:33:48.000000 xgo-pythonlib-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.660283 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     2490 2023-07-04 13:34:53.000000 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-04 13:34:53.000000 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 13:34:53.000000 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-04 13:34:53.000000 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.661295 xgo-pythonlib-0.2.3/xgoedu/
--rw-rw-rw-   0        0        0    49527 2023-07-04 13:31:39.000000 xgo-pythonlib-0.2.3/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.663295 xgo-pythonlib-0.2.3/xgolib/
--rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.3/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.668424 xgo-pythonlib-0.2.3/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.3/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.3/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.3/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.333249 xgo-pythonlib-0.2.4/
+-rw-rw-rw-   0        0        0     2490 2023-07-13 03:16:22.333249 xgo-pythonlib-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1863 2023-07-04 13:33:41.000000 xgo-pythonlib-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 03:16:22.333249 xgo-pythonlib-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     3744 2023-07-13 03:16:10.000000 xgo-pythonlib-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.323589 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     2490 2023-07-13 03:16:22.000000 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-13 03:16:22.000000 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 03:16:22.000000 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-13 03:16:22.000000 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.325587 xgo-pythonlib-0.2.4/xgoedu/
+-rw-rw-rw-   0        0        0    49547 2023-07-13 03:15:23.000000 xgo-pythonlib-0.2.4/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.326587 xgo-pythonlib-0.2.4/xgolib/
+-rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.4/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.331250 xgo-pythonlib-0.2.4/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.4/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.4/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.4/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.2.3/PKG-INFO` & `xgo-pythonlib-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.3
+Version: 0.2.4
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.2.3/README.md` & `xgo-pythonlib-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.3/setup.py` & `xgo-pythonlib-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.3
+Version: 0.2.4
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.2.3/xgoedu/__init__.py` & `xgo-pythonlib-0.2.4/xgoedu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import json
 import threading
 # from xgolib import XGO
 # from keras.preprocessing import image
 # import _thread  使用_thread会报错，坑！
 
 
-__versinon__ = '1.3.0'
-__last_modified__ = '2023/7/4'
+__versinon__ = '1.3.1'
+__last_modified__ = '2023/7/13'
 
 GPIO.setwarnings(False)
 GPIO.setmode(GPIO.BCM)
 
 camera_still=False
 
 
@@ -188,14 +188,15 @@
     '''
     def lcd_rectangle(self,x1,y1,x2,y2,fill=None,outline="WHITE",width=2):
         self.draw.rectangle((x1,y1,x2,y2),fill=fill,outline=outline,width=width)
         self.display.ShowImage(self.splash)
     #清除屏幕
     def lcd_clear(self):
         self.splash = Image.new("RGB",(320,240),"black")
+        self.draw = ImageDraw.Draw(self.splash)
         self.display.ShowImage(self.splash)
     #显示图片
     '''
     图片的大小为320*240,jpg格式
     '''
     def lcd_picture(self,filename,x=0,y=0):
         path="/home/pi/xgoPictures/"
@@ -752,16 +753,15 @@
 
         path="/home/pi/xgoMusic/"
         save_file = "error.txt" if has_error else 'result.' + FORMAT
         with open(path+save_file, 'wb') as of:
             of.write(result_str)
 
         if has_error:
-            if (IS_PY3):
-                result_str = str(result_str, 'utf-8')
+            result_str = str(result_str, 'utf-8')
             print("tts api  error:" + result_str)
 
         print("result saved as :" + save_file)
 
         self.xgoSpeaker("result.wav")
 
     def cv2AddChineseText(self,img, text, position, textColor=(0, 255, 0), textSize=30):
```

### Comparing `xgo-pythonlib-0.2.3/xgolib/__init__.py` & `xgo-pythonlib-0.2.4/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.3/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.2.4/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.3/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.2.4/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

