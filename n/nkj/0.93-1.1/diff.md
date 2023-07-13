# Comparing `tmp/nkj-0.93.tar.gz` & `tmp/nkj-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkj-0.93.tar", last modified: Thu Jul 13 08:26:56 2023, max compression
+gzip compressed data, was "nkj-1.1.tar", last modified: Thu Jul 13 08:26:16 2023, max compression
```

## Comparing `nkj-0.93.tar` & `nkj-1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-13 08:26:56.438977 nkj-0.93/
--rw-r--r--   0 nakajima   (501) staff       (20)      151 2023-07-13 08:26:56.438780 nkj-0.93/PKG-INFO
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-13 08:26:56.435621 nkj-0.93/nkj/
--rw-r--r--   0 nakajima   (501) staff       (20)      190 2023-05-22 09:16:20.000000 nkj-0.93/nkj/__init__.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1760 2023-05-02 17:38:40.000000 nkj-0.93/nkj/arg.py
--rw-r--r--   0 nakajima   (501) staff       (20)    16357 2023-07-04 12:22:38.000000 nkj-0.93/nkj/cam.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1232 2023-05-03 06:08:21.000000 nkj-0.93/nkj/core.py
--rw-r--r--   0 nakajima   (501) staff       (20)     6795 2023-06-12 14:04:44.000000 nkj-0.93/nkj/curvefit.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3593 2023-05-02 18:05:13.000000 nkj-0.93/nkj/cv.py
--rw-r--r--   0 nakajima   (501) staff       (20)    23284 2023-06-08 08:47:20.000000 nkj-0.93/nkj/cwt.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2284 2023-06-19 16:47:05.000000 nkj-0.93/nkj/ea.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2393 2023-05-02 17:46:49.000000 nkj-0.93/nkj/fa.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2325 2023-05-02 17:50:02.000000 nkj-0.93/nkj/file.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3857 2023-05-19 07:00:21.000000 nkj-0.93/nkj/filter.py
--rw-r--r--   0 nakajima   (501) staff       (20)    14923 2023-07-13 01:15:56.000000 nkj-0.93/nkj/func.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1150 2023-05-02 17:34:25.000000 nkj-0.93/nkj/json.py
--rw-r--r--   0 nakajima   (501) staff       (20)    80728 2023-07-07 01:47:09.000000 nkj-0.93/nkj/math.py
--rw-r--r--   0 nakajima   (501) staff       (20)      502 2023-05-02 15:36:15.000000 nkj-0.93/nkj/np.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1638 2023-05-02 17:37:18.000000 nkj-0.93/nkj/os.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2149 2023-05-02 15:36:15.000000 nkj-0.93/nkj/plot.py
--rw-r--r--   0 nakajima   (501) staff       (20)      701 2023-05-02 17:17:27.000000 nkj-0.93/nkj/prob.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3326 2023-05-03 03:21:09.000000 nkj-0.93/nkj/pygame.py
--rw-r--r--   0 nakajima   (501) staff       (20)     9145 2023-05-03 03:23:05.000000 nkj-0.93/nkj/serial.py
--rw-r--r--   0 nakajima   (501) staff       (20)      186 2023-05-02 17:55:10.000000 nkj-0.93/nkj/socket.py
--rw-r--r--   0 nakajima   (501) staff       (20)     5356 2023-05-02 17:41:44.000000 nkj-0.93/nkj/stat.py
--rw-r--r--   0 nakajima   (501) staff       (20)     5941 2023-06-27 07:05:16.000000 nkj-0.93/nkj/str.py
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-13 08:26:56.438475 nkj-0.93/nkj.egg-info/
--rw-r--r--   0 nakajima   (501) staff       (20)      151 2023-07-13 08:26:56.000000 nkj-0.93/nkj.egg-info/PKG-INFO
--rw-r--r--   0 nakajima   (501) staff       (20)      394 2023-07-13 08:26:56.000000 nkj-0.93/nkj.egg-info/SOURCES.txt
--rw-r--r--   0 nakajima   (501) staff       (20)        1 2023-07-13 08:26:56.000000 nkj-0.93/nkj.egg-info/dependency_links.txt
--rw-r--r--   0 nakajima   (501) staff       (20)        4 2023-07-13 08:26:56.000000 nkj-0.93/nkj.egg-info/top_level.txt
--rw-r--r--   0 nakajima   (501) staff       (20)       38 2023-07-13 08:26:56.439045 nkj-0.93/setup.cfg
--rw-r--r--   0 nakajima   (501) staff       (20)      285 2023-07-13 08:26:49.000000 nkj-0.93/setup.py
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-13 08:26:16.674574 nkj-1.1/
+-rw-r--r--   0 nakajima   (501) staff       (20)      150 2023-07-13 08:26:16.674361 nkj-1.1/PKG-INFO
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-13 08:26:16.672783 nkj-1.1/nkj/
+-rw-r--r--   0 nakajima   (501) staff       (20)      190 2023-05-22 09:16:20.000000 nkj-1.1/nkj/__init__.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1760 2023-05-02 17:38:40.000000 nkj-1.1/nkj/arg.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    16357 2023-07-04 12:22:38.000000 nkj-1.1/nkj/cam.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1232 2023-05-03 06:08:21.000000 nkj-1.1/nkj/core.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     6795 2023-06-12 14:04:44.000000 nkj-1.1/nkj/curvefit.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3593 2023-05-02 18:05:13.000000 nkj-1.1/nkj/cv.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    23284 2023-06-08 08:47:20.000000 nkj-1.1/nkj/cwt.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2284 2023-06-19 16:47:05.000000 nkj-1.1/nkj/ea.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2393 2023-05-02 17:46:49.000000 nkj-1.1/nkj/fa.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2325 2023-05-02 17:50:02.000000 nkj-1.1/nkj/file.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3857 2023-05-19 07:00:21.000000 nkj-1.1/nkj/filter.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    14923 2023-07-13 01:15:56.000000 nkj-1.1/nkj/func.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1150 2023-05-02 17:34:25.000000 nkj-1.1/nkj/json.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    80728 2023-07-07 01:47:09.000000 nkj-1.1/nkj/math.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      502 2023-05-02 15:36:15.000000 nkj-1.1/nkj/np.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1638 2023-05-02 17:37:18.000000 nkj-1.1/nkj/os.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2149 2023-05-02 15:36:15.000000 nkj-1.1/nkj/plot.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      701 2023-05-02 17:17:27.000000 nkj-1.1/nkj/prob.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3326 2023-05-03 03:21:09.000000 nkj-1.1/nkj/pygame.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     9145 2023-05-03 03:23:05.000000 nkj-1.1/nkj/serial.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      186 2023-05-02 17:55:10.000000 nkj-1.1/nkj/socket.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     5356 2023-05-02 17:41:44.000000 nkj-1.1/nkj/stat.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     5941 2023-06-27 07:05:16.000000 nkj-1.1/nkj/str.py
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-13 08:26:16.674009 nkj-1.1/nkj.egg-info/
+-rw-r--r--   0 nakajima   (501) staff       (20)      150 2023-07-13 08:26:16.000000 nkj-1.1/nkj.egg-info/PKG-INFO
+-rw-r--r--   0 nakajima   (501) staff       (20)      394 2023-07-13 08:26:16.000000 nkj-1.1/nkj.egg-info/SOURCES.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)        1 2023-07-13 08:26:16.000000 nkj-1.1/nkj.egg-info/dependency_links.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)        4 2023-07-13 08:26:16.000000 nkj-1.1/nkj.egg-info/top_level.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)       38 2023-07-13 08:26:16.674647 nkj-1.1/setup.cfg
+-rw-r--r--   0 nakajima   (501) staff       (20)      285 2023-07-13 08:25:47.000000 nkj-1.1/setup.py
```

### Comparing `nkj-0.93/nkj/arg.py` & `nkj-1.1/nkj/arg.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/cam.py` & `nkj-1.1/nkj/cam.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/core.py` & `nkj-1.1/nkj/core.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/curvefit.py` & `nkj-1.1/nkj/curvefit.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/cv.py` & `nkj-1.1/nkj/cv.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/cwt.py` & `nkj-1.1/nkj/cwt.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/ea.py` & `nkj-1.1/nkj/ea.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/fa.py` & `nkj-1.1/nkj/fa.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/file.py` & `nkj-1.1/nkj/file.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/filter.py` & `nkj-1.1/nkj/filter.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/func.py` & `nkj-1.1/nkj/func.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/json.py` & `nkj-1.1/nkj/json.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/math.py` & `nkj-1.1/nkj/math.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/os.py` & `nkj-1.1/nkj/os.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/plot.py` & `nkj-1.1/nkj/plot.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/prob.py` & `nkj-1.1/nkj/prob.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/pygame.py` & `nkj-1.1/nkj/pygame.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/serial.py` & `nkj-1.1/nkj/serial.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/stat.py` & `nkj-1.1/nkj/stat.py`

 * *Files identical despite different names*

### Comparing `nkj-0.93/nkj/str.py` & `nkj-1.1/nkj/str.py`

 * *Files identical despite different names*

