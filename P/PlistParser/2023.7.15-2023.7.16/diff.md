# Comparing `tmp/PlistParser-2023.7.15.tar.gz` & `tmp/PlistParser-2023.7.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlistParser-2023.7.15.tar", last modified: Thu Jul 13 13:55:20 2023, max compression
+gzip compressed data, was "PlistParser-2023.7.16.tar", last modified: Thu Jul 13 14:45:45 2023, max compression
```

## Comparing `PlistParser-2023.7.15.tar` & `PlistParser-2023.7.16.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 13:55:20.604655 PlistParser-2023.7.15/
--rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.15/LICENSE.txt
--rw-rw-rw-   0        0        0    15431 2023-07-13 13:55:20.604655 PlistParser-2023.7.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 13:55:20.580562 PlistParser-2023.7.15/PlistParser/
--rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.15/PlistParser/Base64.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:55:20.603667 PlistParser-2023.7.15/PlistParser/DisplaceTemplate/
--rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.15/PlistParser/DisplaceTemplate/__init__.py
--rw-rw-rw-   0        0        0       47 2023-07-11 15:47:49.000000 PlistParser-2023.7.15/PlistParser/Extend.py
--rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.15/PlistParser/Info.py
--rw-rw-rw-   0        0        0     5984 2023-07-13 11:36:05.000000 PlistParser-2023.7.15/PlistParser/Plist.py
--rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.15/PlistParser/PlistParser.py
--rw-rw-rw-   0        0        0      174 2023-07-13 13:39:15.000000 PlistParser-2023.7.15/PlistParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:55:20.602670 PlistParser-2023.7.15/PlistParser.egg-info/
--rw-rw-rw-   0        0        0    15431 2023-07-13 13:55:20.000000 PlistParser-2023.7.15/PlistParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-13 13:55:20.000000 PlistParser-2023.7.15/PlistParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 13:55:20.000000 PlistParser-2023.7.15/PlistParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-13 13:55:20.000000 PlistParser-2023.7.15/PlistParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14729 2023-07-13 13:29:30.000000 PlistParser-2023.7.15/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 13:55:20.604655 PlistParser-2023.7.15/setup.cfg
--rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:45:45.235370 PlistParser-2023.7.16/
+-rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.16/LICENSE.txt
+-rw-rw-rw-   0        0        0    15431 2023-07-13 14:45:45.235370 PlistParser-2023.7.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 14:45:45.225238 PlistParser-2023.7.16/PlistParser/
+-rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.16/PlistParser/Base64.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:45:45.234130 PlistParser-2023.7.16/PlistParser/DisplaceTemplate/
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.16/PlistParser/DisplaceTemplate/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-07-11 15:47:49.000000 PlistParser-2023.7.16/PlistParser/Extend.py
+-rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.16/PlistParser/Info.py
+-rw-rw-rw-   0        0        0     6001 2023-07-13 14:41:47.000000 PlistParser-2023.7.16/PlistParser/Plist.py
+-rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.16/PlistParser/PlistParser.py
+-rw-rw-rw-   0        0        0      174 2023-07-13 14:45:31.000000 PlistParser-2023.7.16/PlistParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:45:45.234130 PlistParser-2023.7.16/PlistParser.egg-info/
+-rw-rw-rw-   0        0        0    15431 2023-07-13 14:45:45.000000 PlistParser-2023.7.16/PlistParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-13 14:45:45.000000 PlistParser-2023.7.16/PlistParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 14:45:45.000000 PlistParser-2023.7.16/PlistParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-13 14:45:45.000000 PlistParser-2023.7.16/PlistParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14729 2023-07-13 13:29:30.000000 PlistParser-2023.7.16/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 14:45:45.235370 PlistParser-2023.7.16/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.16/setup.py
```

### Comparing `PlistParser-2023.7.15/LICENSE.txt` & `PlistParser-2023.7.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.15/PKG-INFO` & `PlistParser-2023.7.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.15
+Version: 2023.7.16
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
```

### Comparing `PlistParser-2023.7.15/PlistParser/Info.py` & `PlistParser-2023.7.16/PlistParser/Info.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.15/PlistParser/Plist.py` & `PlistParser-2023.7.16/PlistParser/Plist.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         return self.dict_index
 
     def __neg__(self):
         """
         重载 单目运算符 -
         :return:
         """
-        return self.dict
+        return self.simplification_dict()
 
     def __invert__(self):
         """
         重载 单目运算符 ~
         :return:
         """
         return self.path_tuple
```

### Comparing `PlistParser-2023.7.15/PlistParser/PlistParser.py` & `PlistParser-2023.7.16/PlistParser/PlistParser.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.15/PlistParser.egg-info/PKG-INFO` & `PlistParser-2023.7.16/PlistParser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.15
+Version: 2023.7.16
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
```

### Comparing `PlistParser-2023.7.15/README.md` & `PlistParser-2023.7.16/README.md`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.15/setup.py` & `PlistParser-2023.7.16/setup.py`

 * *Files identical despite different names*

