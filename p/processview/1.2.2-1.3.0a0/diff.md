# Comparing `tmp/processview-1.2.2.tar.gz` & `tmp/processview-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processview-1.2.2.tar", last modified: Wed Jun 21 11:54:30 2023, max compression
+gzip compressed data, was "processview-1.3.0a0.tar", last modified: Thu Jul 13 11:01:37 2023, max compression
```

## Comparing `processview-1.2.2.tar` & `processview-1.3.0a0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.2/LICENSE
--rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-06-21 11:54:30.218018 processview-1.2.2/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)      767 2023-06-21 09:33:50.000000 processview-1.2.2/README.md
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.210018 processview-1.2.2/processview/
--rw-r--r--   0 payno     (1001) payno     (1001)       91 2023-06-21 09:33:50.000000 processview-1.2.2/processview/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/core/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3289 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/dataset.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2350 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/helpers.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/core/manager/
--rw-r--r--   0 payno     (1001) payno     (1001)       23 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/manager/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)    13677 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/manager/manager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/core/manager/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1534 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/manager/test/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     4823 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/manager/test/test_manager.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1745 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/setup.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1067 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/sorting.py
--rw-r--r--   0 payno     (1001) payno     (1001)     5128 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/superviseprocess.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/core/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1561 2023-06-21 09:33:50.000000 processview-1.2.2/processview/core/test/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/gui/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)    12926 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/icons.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2296 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/messagebox.py
--rw-r--r--   0 payno     (1001) payno     (1001)    25061 2023-06-21 09:36:58.000000 processview-1.2.2/processview/gui/processmanager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview/gui/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1584 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/test/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3666 2023-06-21 09:33:50.000000 processview-1.2.2/processview/gui/test/test_process_manager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/processview/resources/
--rw-r--r--   0 payno     (1001) payno     (1001)    10757 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.210018 processview-1.2.2/processview/resources/gui/
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/processview/resources/gui/icons/
--rw-r--r--   0 payno     (1001) payno     (1001)      729 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/gui/icons/advancement.png
--rw-r--r--   0 payno     (1001) payno     (1001)     5781 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/gui/icons/advancement.svg
--rw-r--r--   0 payno     (1001) payno     (1001)      926 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/gui/icons/magnifying_glass.png
--rw-r--r--   0 payno     (1001) payno     (1001)     4631 2023-06-21 09:33:50.000000 processview-1.2.2/processview/resources/gui/icons/magnifying_glass.svg
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/processview/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1695 2023-06-21 09:33:50.000000 processview-1.2.2/processview/test/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.218018 processview-1.2.2/processview/utils/
--rw-r--r--   0 payno     (1001) payno     (1001)     2565 2023-06-21 09:33:50.000000 processview-1.2.2/processview/utils/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1559 2023-06-21 09:33:50.000000 processview-1.2.2/processview/utils/singleton.py
--rw-r--r--   0 payno     (1001) payno     (1001)     4411 2023-06-21 11:53:53.000000 processview-1.2.2/processview/version.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 11:54:30.214018 processview-1.2.2/processview.egg-info/
--rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)     1179 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1001) payno     (1001)       94 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/requires.txt
--rw-r--r--   0 payno     (1001) payno     (1001)       12 2023-06-21 11:54:30.000000 processview-1.2.2/processview.egg-info/top_level.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.2.2/processview.egg-info/zip-safe
--rw-r--r--   0 payno     (1001) payno     (1001)     1196 2023-06-21 11:54:30.218018 processview-1.2.2/setup.cfg
--rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-21 09:33:50.000000 processview-1.2.2/setup.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.750609 processview-1.3.0a0/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0a0/LICENSE
+-rw-r--r--   0 payno     (1001) payno     (1001)     1065 2023-07-13 11:01:37.750609 processview-1.3.0a0/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)      767 2023-06-21 09:33:50.000000 processview-1.3.0a0/README.md
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.742609 processview-1.3.0a0/processview/
+-rw-r--r--   0 payno     (1001) payno     (1001)       91 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/core/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3289 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/dataset.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2350 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/helpers.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/core/manager/
+-rw-r--r--   0 payno     (1001) payno     (1001)       23 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/manager/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    13677 2023-07-13 11:00:07.000000 processview-1.3.0a0/processview/core/manager/manager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/core/manager/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1534 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/manager/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4823 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/manager/test/test_manager.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1745 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/setup.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1067 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/sorting.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     5128 2023-07-13 11:00:07.000000 processview-1.3.0a0/processview/core/superviseprocess.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/core/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1561 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/test/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/gui/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    12926 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/icons.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2296 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/messagebox.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    26124 2023-07-13 11:00:09.000000 processview-1.3.0a0/processview/gui/processmanager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/gui/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1584 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3666 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/test/test_process_manager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/resources/
+-rw-r--r--   0 payno     (1001) payno     (1001)    10757 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.738609 processview-1.3.0a0/processview/resources/gui/
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/resources/gui/icons/
+-rw-r--r--   0 payno     (1001) payno     (1001)      729 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/gui/icons/advancement.png
+-rw-r--r--   0 payno     (1001) payno     (1001)     5781 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/gui/icons/advancement.svg
+-rw-r--r--   0 payno     (1001) payno     (1001)      926 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/gui/icons/magnifying_glass.png
+-rw-r--r--   0 payno     (1001) payno     (1001)     4631 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/gui/icons/magnifying_glass.svg
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.750609 processview-1.3.0a0/processview/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1695 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/test/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.750609 processview-1.3.0a0/processview/utils/
+-rw-r--r--   0 payno     (1001) payno     (1001)     2565 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/utils/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1559 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/utils/singleton.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4411 2023-07-13 11:00:41.000000 processview-1.3.0a0/processview/version.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.742609 processview-1.3.0a0/processview.egg-info/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1065 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)     1179 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       94 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/requires.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       12 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.3.0a0/processview.egg-info/zip-safe
+-rw-r--r--   0 payno     (1001) payno     (1001)     1196 2023-07-13 11:01:37.750609 processview-1.3.0a0/setup.cfg
+-rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-21 09:33:50.000000 processview-1.3.0a0/setup.py
```

### Comparing `processview-1.2.2/PKG-INFO` & `processview-1.3.0a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processview
-Version: 1.2.2
+Version: 1.3.0a0
 Summary: Simple helper to provide user feedback about dataset processing
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

### Comparing `processview-1.2.2/README.md` & `processview-1.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/dataset.py` & `processview-1.3.0a0/processview/core/dataset.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/helpers.py` & `processview-1.3.0a0/processview/core/helpers.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/manager/manager.py` & `processview-1.3.0a0/processview/core/manager/manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/manager/test/__init__.py` & `processview-1.3.0a0/processview/core/manager/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/manager/test/test_manager.py` & `processview-1.3.0a0/processview/core/manager/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/setup.py` & `processview-1.3.0a0/processview/core/setup.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/sorting.py` & `processview-1.3.0a0/processview/core/sorting.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/superviseprocess.py` & `processview-1.3.0a0/processview/core/superviseprocess.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/core/test/__init__.py` & `processview-1.3.0a0/processview/core/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/gui/icons.py` & `processview-1.3.0a0/processview/gui/icons.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/gui/messagebox.py` & `processview-1.3.0a0/processview/gui/messagebox.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/gui/processmanager.py` & `processview-1.3.0a0/processview/gui/processmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,30 +73,35 @@
     Redefinition of QTableView for datasets and processes
     """
 
     def __init__(self, parent):
         qt.QTableView.__init__(self, parent)
         self.verticalHeader().setSectionsClickable(True)
 
+        # QMenu for the dataset name
+        self.dataset_menu = qt.QMenu()
+        self._copyAction = qt.QAction("copy")
+        self.dataset_menu.addAction(self._copyAction)
+        self._clearAction = qt.QAction("clear")
+        self.dataset_menu.addAction(self._clearAction)
+
         # QMenu for cell from on dataset and one process
         self.menu_dataset_vs_process = qt.QMenu()
         self._reprocessAction = qt.QAction("reprocess")
         self.menu_dataset_vs_process.addAction(self._reprocessAction)
         self._infoAction = qt.QAction("info")
         self.menu_dataset_vs_process.addAction(self._infoAction)
+        self.menu_dataset_vs_process.addAction(self._clearAction)
 
         self._target = (None, None)
         # register target of the last menu (process, DatasetIdentifier)
 
-        self.copy_menu = qt.QMenu()
-        self._copyAction = qt.QAction("copy")
-        self.copy_menu.addAction(self._copyAction)
-
         # connect signal / slot
         self._copyAction.triggered.connect(self._requestDatasetIdCopy)
+        self._clearAction.triggered.connect(self._requestClearDataset)
         self._reprocessAction.triggered.connect(self._requestReprocessing)
         self._infoAction.triggered.connect(self._requestInfo)
 
     def _processAt(self, x_pos):
         column = self.columnAt(x_pos)
         if column >= 1:
             processes = self.model()._processes
@@ -113,15 +118,15 @@
 
     def contextMenuEvent(self, event):
         row = self.columnAt(event.pos().x())
         dataset = self._datasetAt(event.pos().y())
         if row == 0:
             # handle column column
             self._target = (None, dataset)
-            self.copy_menu.exec_(event.globalPos())
+            self.dataset_menu.exec_(event.globalPos())
         else:
             # handle processes column
             process = self._processAt(event.pos().x())
             if (
                 process is not None
                 and dataset is not None
                 and _ProcessManager().met(process=process, dataset=dataset)
@@ -130,25 +135,37 @@
                 self.menu_dataset_vs_process.exec_(event.globalPos())
             else:
                 self._target = (None, None)
         super().contextMenuEvent(event)
 
     def _requestReprocessing(self, *args, **kwargs):
         process, dataset = self._target
+
         if process is not None and dataset is not None:
             assert isinstance(process, SuperviseProcess)
             assert isinstance(dataset, DatasetIdentifier)
             process.reprocess(dataset.recreate_dataset())
 
     def _requestDatasetIdCopy(self, *args, **kwargs):
         _, dataset = self._target
         if dataset is not None:
             clipboard = qt.QGuiApplication.clipboard()
             clipboard.setText(dataset.to_str())
 
+    def _requestClearDataset(self, *args, **kwargs):
+        def get_dataset_at(row: int):
+            datasets = self.model()._sorted_datasets
+            return datasets.get(
+                list(datasets.keys())[row],
+                None,
+            )
+
+        datasets = [get_dataset_at(index.row()) for index in self.selectedIndexes()]
+        self.model().remove_datasets(datasets)
+
     def _requestInfo(self, *args, **kwargs):
         process, dataset = self._target
         if process is not None and dataset is not None:
             infos = ProcessManager().get_dataset_details(
                 dataset=dataset, process=process
             )
             if infos in (None, ""):
@@ -157,14 +174,20 @@
             msg = MessageBox(self)
             msg.setInfos(infos=infos)
             extra_info = "{} processing {}".format(process.name, dataset)
             msg.setWindowTitle(extra_info)
             msg.setWindowModality(qt.Qt.NonModal)
             msg.show()
 
+    def sizeHintForColumn(self, column):
+        if column == 0:
+            return 350
+        else:
+            return super().sizeHintForColumn(column)
+
 
 class ProcessManagerWidget(qt.QWidget):
     """
     Main widget to dispaly dataset vs process metadata
     """
 
     def __init__(self, parent):
@@ -227,14 +250,15 @@
 
 
 class _DatasetProcessModel(qt.QAbstractTableModel):
     def __init__(self, parent, header, *args):
         qt.QAbstractTableModel.__init__(self, parent, *args)
         self.header = header
         self._processes = OrderedDict()
+        # processes with order as key and Process as value
         self._sorted_datasets = OrderedDict()
         self._unsorted_datasets = OrderedDict()
         self._processPatterns = tuple()
         # is there some process name pattern to follow ?
         self._datasetPatterns = tuple()
         # is there some dataset id pattern to follow ?
         self._sort_type = SortType.FIRST_APPEARANCE
@@ -269,25 +293,27 @@
     def dataset_patterns(self):
         return self._datasetPatterns
 
     @dataset_patterns.setter
     def dataset_patterns(self, patterns):
         self._datasetPatterns = patterns
 
-    def add(self, dataset, status):
-        self._processes[dataset] = status
-        self.endResetModel()
-
-    def remove(self, dataset):
-        if dataset in self._processes:
-            del self._processes[dataset]
-        self.endResetModel()
+    def remove_datasets(self, datasets):
+        remaining_datasets = list(self._unsorted_datasets)
+        for dataset in datasets:
+            if not isinstance(dataset, DatasetIdentifier):
+                raise ValueError(
+                    f"dataset is expected to be a dataset identifier. Get {type(dataset)} instead"
+                )
+            try:
+                remaining_datasets.remove(dataset)
+            except Exception:
+                pass
 
-    def update_dataset(self, dataset, status):
-        self._processes[dataset] = status
+        self.setDatasets(remaining_datasets)
         self.endResetModel()
 
     def clear(self):
         self._processes = OrderedDict()
         self.endResetModel()
 
     def rowCount(self, parent=None):
```

### Comparing `processview-1.2.2/processview/gui/test/__init__.py` & `processview-1.3.0a0/processview/gui/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/gui/test/test_process_manager.py` & `processview-1.3.0a0/processview/gui/test/test_process_manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/resources/__init__.py` & `processview-1.3.0a0/processview/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/resources/gui/icons/advancement.png` & `processview-1.3.0a0/processview/resources/gui/icons/advancement.png`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/resources/gui/icons/advancement.svg` & `processview-1.3.0a0/processview/resources/gui/icons/advancement.svg`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/resources/gui/icons/magnifying_glass.png` & `processview-1.3.0a0/processview/resources/gui/icons/magnifying_glass.png`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/resources/gui/icons/magnifying_glass.svg` & `processview-1.3.0a0/processview/resources/gui/icons/magnifying_glass.svg`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/test/__init__.py` & `processview-1.3.0a0/processview/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/utils/__init__.py` & `processview-1.3.0a0/processview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/utils/singleton.py` & `processview-1.3.0a0/processview/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/processview/version.py` & `processview-1.3.0a0/processview/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,17 @@
     "beta": 11,
     "gamma": 11,
     "rc": 12,
     "final": 15,
 }
 
 MAJOR = 1
-MINOR = 2
-MICRO = 2
-RELEV = "final"  # <16
+MINOR = 3
+MICRO = 0
+RELEV = "alpha"  # <16
 SERIAL = 0  # <16
 
 date = __date__
 
 from collections import namedtuple
 
 _version_info = namedtuple(
```

### Comparing `processview-1.2.2/processview.egg-info/PKG-INFO` & `processview-1.3.0a0/processview.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processview
-Version: 1.2.2
+Version: 1.3.0a0
 Summary: Simple helper to provide user feedback about dataset processing
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

### Comparing `processview-1.2.2/processview.egg-info/SOURCES.txt` & `processview-1.3.0a0/processview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processview-1.2.2/setup.cfg` & `processview-1.3.0a0/setup.cfg`

 * *Files identical despite different names*

