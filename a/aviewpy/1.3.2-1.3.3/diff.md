# Comparing `tmp/aviewpy-1.3.2.tar.gz` & `tmp/aviewpy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aviewpy-1.3.2.tar", last modified: Fri Mar  3 21:31:55 2023, max compression
+gzip compressed data, was "aviewpy-1.3.3.tar", last modified: Thu Jul 13 18:57:08 2023, max compression
```

## Comparing `aviewpy-1.3.2.tar` & `aviewpy-1.3.3.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 21:31:55.756883 aviewpy-1.3.2/
--rw-rw-rw-   0        0        0     1091 2022-12-20 23:52:04.000000 aviewpy-1.3.2/LICENSE
--rw-rw-rw-   0        0        0       34 2022-12-20 23:52:04.000000 aviewpy-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      664 2023-03-03 21:31:55.756883 aviewpy-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-03-03 21:26:40.000000 aviewpy-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 21:31:55.731382 aviewpy-1.3.2/aviewpy/
--rw-rw-rw-   0        0        0       66 2022-12-20 23:55:30.000000 aviewpy-1.3.2/aviewpy/__init__.py
--rw-rw-rw-   0        0        0    11133 2023-01-27 13:26:46.000000 aviewpy-1.3.2/aviewpy/contact.py
--rw-rw-rw-   0        0        0     3770 2022-12-21 00:15:59.000000 aviewpy-1.3.2/aviewpy/cs.py
-drwxrwxrwx   0        0        0        0 2023-03-03 21:31:55.741280 aviewpy-1.3.2/aviewpy/files/
--rw-rw-rw-   0        0        0        0 2022-12-21 00:31:35.000000 aviewpy-1.3.2/aviewpy/files/__init__.py
--rw-rw-rw-   0        0        0     1861 2023-02-07 15:57:18.000000 aviewpy-1.3.2/aviewpy/files/bin.py
--rw-rw-rw-   0        0        0     1354 2023-02-24 15:52:22.000000 aviewpy-1.3.2/aviewpy/files/cmd.py
--rw-rw-rw-   0        0        0     7516 2023-01-23 21:28:35.000000 aviewpy-1.3.2/aviewpy/files/shell.py
--rw-rw-rw-   0        0        0     1102 2023-02-01 01:25:09.000000 aviewpy-1.3.2/aviewpy/move.py
--rw-rw-rw-   0        0        0     5232 2023-03-03 21:02:08.000000 aviewpy-1.3.2/aviewpy/objects.py
--rw-rw-rw-   0        0        0     1697 2023-03-03 17:26:22.000000 aviewpy-1.3.2/aviewpy/results.py
--rw-rw-rw-   0        0        0     1676 2023-03-03 01:43:27.000000 aviewpy-1.3.2/aviewpy/sim.py
-drwxrwxrwx   0        0        0        0 2023-03-03 21:31:55.747112 aviewpy-1.3.2/aviewpy/ui/
--rw-rw-rw-   0        0        0        0 2022-12-21 14:52:37.000000 aviewpy-1.3.2/aviewpy/ui/__init__.py
--rw-rw-rw-   0        0        0      850 2023-01-29 15:59:59.000000 aviewpy-1.3.2/aviewpy/ui/alerts.py
--rw-rw-rw-   0        0        0      624 2023-01-29 16:08:26.000000 aviewpy-1.3.2/aviewpy/ui/messages.py
--rw-rw-rw-   0        0        0     2475 2023-02-07 19:36:00.000000 aviewpy-1.3.2/aviewpy/ui/progressbar.py
--rw-rw-rw-   0        0        0      416 2023-02-14 13:55:42.000000 aviewpy-1.3.2/aviewpy/ui/windows.py
-drwxrwxrwx   0        0        0        0 2023-03-03 21:31:55.753843 aviewpy-1.3.2/aviewpy/utils/
--rw-rw-rw-   0        0        0       20 2022-12-21 00:01:02.000000 aviewpy-1.3.2/aviewpy/utils/__init__.py
--rw-rw-rw-   0        0        0     6041 2023-03-03 21:05:07.000000 aviewpy-1.3.2/aviewpy/utils/dereferencer.py
--rw-rw-rw-   0        0        0     1682 2023-03-01 22:31:44.000000 aviewpy-1.3.2/aviewpy/utils/excepthook.py
--rw-rw-rw-   0        0        0     5173 2022-12-20 23:52:04.000000 aviewpy-1.3.2/aviewpy/utils/res_to_csv.py
--rw-rw-rw-   0        0        0     1627 2022-12-21 15:09:59.000000 aviewpy-1.3.2/aviewpy/utils/utils.py
--rw-rw-rw-   0        0        0     4919 2023-03-03 21:00:13.000000 aviewpy-1.3.2/aviewpy/variables.py
-drwxrwxrwx   0        0        0        0 2023-03-03 21:31:55.736424 aviewpy-1.3.2/aviewpy.egg-info/
--rw-rw-rw-   0        0        0      664 2023-03-03 21:31:55.000000 aviewpy-1.3.2/aviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-03-03 21:31:55.000000 aviewpy-1.3.2/aviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 21:31:55.000000 aviewpy-1.3.2/aviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-03-03 21:31:55.000000 aviewpy-1.3.2/aviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-03 21:31:55.000000 aviewpy-1.3.2/aviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-03 21:31:55.756883 aviewpy-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1094 2022-12-21 15:27:19.000000 aviewpy-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-03 21:31:55.754815 aviewpy-1.3.2/test/
--rw-rw-rw-   0        0        0     5501 2023-01-06 20:15:20.000000 aviewpy-1.3.2/test/test_shell.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:57:08.134859 aviewpy-1.3.3/
+-rw-rw-rw-   0        0        0     1091 2022-12-20 23:52:04.000000 aviewpy-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-12-20 23:52:04.000000 aviewpy-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      664 2023-07-13 18:57:08.133862 aviewpy-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-03-03 21:26:40.000000 aviewpy-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 18:57:07.424822 aviewpy-1.3.3/aviewpy/
+-rw-rw-rw-   0        0        0       66 2022-12-20 23:55:30.000000 aviewpy-1.3.3/aviewpy/__init__.py
+-rw-rw-rw-   0        0        0    11000 2023-04-12 16:38:53.000000 aviewpy-1.3.3/aviewpy/contact.py
+-rw-rw-rw-   0        0        0     3770 2022-12-21 00:15:59.000000 aviewpy-1.3.3/aviewpy/cs.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:57:07.736820 aviewpy-1.3.3/aviewpy/files/
+-rw-rw-rw-   0        0        0        0 2022-12-21 00:31:35.000000 aviewpy-1.3.3/aviewpy/files/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-04-28 18:01:01.000000 aviewpy-1.3.3/aviewpy/files/acf.py
+-rw-rw-rw-   0        0        0      309 2023-04-28 18:01:16.000000 aviewpy-1.3.3/aviewpy/files/adm.py
+-rw-rw-rw-   0        0        0     2141 2023-05-01 20:20:51.000000 aviewpy-1.3.3/aviewpy/files/bin.py
+-rw-rw-rw-   0        0        0     1354 2023-02-24 15:52:22.000000 aviewpy-1.3.3/aviewpy/files/cmd.py
+-rw-rw-rw-   0        0        0     7470 2023-05-12 18:33:02.000000 aviewpy-1.3.3/aviewpy/files/shell.py
+-rw-rw-rw-   0        0        0     7063 2023-05-03 15:18:21.000000 aviewpy-1.3.3/aviewpy/files/to.py
+-rw-rw-rw-   0        0        0     3035 2023-04-26 14:59:26.000000 aviewpy-1.3.3/aviewpy/model.py
+-rw-rw-rw-   0        0        0     1102 2023-02-01 01:25:09.000000 aviewpy-1.3.3/aviewpy/move.py
+-rw-rw-rw-   0        0        0     5232 2023-03-03 21:02:08.000000 aviewpy-1.3.3/aviewpy/objects.py
+-rw-rw-rw-   0        0        0     2557 2023-07-07 22:57:12.000000 aviewpy-1.3.3/aviewpy/results.py
+-rw-rw-rw-   0        0        0     8017 2023-07-11 17:41:18.000000 aviewpy-1.3.3/aviewpy/sim.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:57:07.913822 aviewpy-1.3.3/aviewpy/ui/
+-rw-rw-rw-   0        0        0        0 2022-12-21 14:52:37.000000 aviewpy-1.3.3/aviewpy/ui/__init__.py
+-rw-rw-rw-   0        0        0      941 2023-06-06 21:51:39.000000 aviewpy-1.3.3/aviewpy/ui/alerts.py
+-rw-rw-rw-   0        0        0      875 2023-07-10 15:08:16.000000 aviewpy-1.3.3/aviewpy/ui/messages.py
+-rw-rw-rw-   0        0        0     2807 2023-05-12 17:01:09.000000 aviewpy-1.3.3/aviewpy/ui/progressbar.py
+-rw-rw-rw-   0        0        0      416 2023-02-14 13:55:42.000000 aviewpy-1.3.3/aviewpy/ui/windows.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:57:08.129862 aviewpy-1.3.3/aviewpy/utils/
+-rw-rw-rw-   0        0        0       20 2022-12-21 00:01:02.000000 aviewpy-1.3.3/aviewpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     6041 2023-03-03 21:05:07.000000 aviewpy-1.3.3/aviewpy/utils/dereferencer.py
+-rw-rw-rw-   0        0        0     1682 2023-03-18 19:28:15.000000 aviewpy-1.3.3/aviewpy/utils/excepthook.py
+-rw-rw-rw-   0        0        0     5173 2022-12-20 23:52:04.000000 aviewpy-1.3.3/aviewpy/utils/res_to_csv.py
+-rw-rw-rw-   0        0        0     3885 2023-06-06 14:31:27.000000 aviewpy-1.3.3/aviewpy/utils/utils.py
+-rw-rw-rw-   0        0        0     5058 2023-05-31 12:46:11.000000 aviewpy-1.3.3/aviewpy/variables.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:57:07.544820 aviewpy-1.3.3/aviewpy.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-07-13 18:57:05.000000 aviewpy-1.3.3/aviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2023-07-13 18:57:06.000000 aviewpy-1.3.3/aviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 18:57:05.000000 aviewpy-1.3.3/aviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-13 18:57:05.000000 aviewpy-1.3.3/aviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 18:57:06.000000 aviewpy-1.3.3/aviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 18:57:08.136861 aviewpy-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2022-12-21 15:27:19.000000 aviewpy-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:57:08.130861 aviewpy-1.3.3/test/
+-rw-rw-rw-   0        0        0     5501 2023-01-06 20:15:20.000000 aviewpy-1.3.3/test/test_shell.py
```

### Comparing `aviewpy-1.3.2/LICENSE` & `aviewpy-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/PKG-INFO` & `aviewpy-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviewpy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python tools for working with in the Adams View python environment
 Home-page: https://github.com/bthornton191/aviewpy
 Author: Ben Thornton
 Author-email: ben.thornton@hexagon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `aviewpy-1.3.2/aviewpy/contact.py` & `aviewpy-1.3.3/aviewpy/contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,15 @@
 
     Parameters
     ----------
     ans : Analysis
         Adams analysis to
     track_name : str
         Full name of contact track
-    ref_part : Part, optional
-        Part to transform coordinates into, (overridden by `ref_mkr`), by default None
-    ref_mkr : Marker, optional
+    mkr : Marker
         Marker to transform coordinates into, by default None
 
     Returns
     -------
     _type_
         _description_
     """
```

### Comparing `aviewpy-1.3.2/aviewpy/cs.py` & `aviewpy-1.3.3/aviewpy/cs.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/aviewpy/files/bin.py` & `aviewpy-1.3.3/aviewpy/files/bin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import os
 from pathlib import Path
 import re
 from typing import Union
 import unicodedata
 
 import Adams  # type: ignore # noqa
 from Object import Object  # type: ignore # noqa
@@ -55,7 +56,17 @@
     if len(comps) > 3:
         other = (int(comp) for comp in comps[3:] if len(comp) <= 2)
     else:
         other = ()
 
     return '_'.join(str(val) for val in (year, release, update, build) + other
                     if isinstance(val, int) and val != 0)
+
+def is_compatible(filename: Union[Path, str]):
+    bin_ver = get_bin_version(filename)
+    adams_ver =  os.environ['VERSION']
+
+    for bv, av in zip(bin_ver.split('_'), adams_ver.split('_')):
+        if bv > av:
+            return False
+    
+    return True
```

### Comparing `aviewpy-1.3.2/aviewpy/files/cmd.py` & `aviewpy-1.3.3/aviewpy/files/cmd.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/aviewpy/files/shell.py` & `aviewpy-1.3.3/aviewpy/files/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,16 @@
                     
                     df_facets_new.at[idx, jdx] = new_i_pt
 
         df_points_new = df_points.copy(deep=True).drop_duplicates()
         df_points_new['new_index'] = np.arange(len(df_points_new))
         df_facets_new = df_facets_new.applymap(lambda ipt: df_points_new.loc[ipt]['new_index'].astype(int))
 
-        new_points = [tuple(r) for _, r in df_points_new[['x', 'y', 'z']].iterrows()]
-        new_facets = [tuple(r) for _, r in df_facets_new.iterrows()]
+        new_points = df_points_new[['x', 'y', 'z']].to_numpy()
+        new_facets = df_facets_new.to_numpy()
 
     else:
         new_points, new_facets = points, facets
 
     return new_points, new_facets
 
 # @lru_cache(maxsize=1)
```

### Comparing `aviewpy-1.3.2/aviewpy/move.py` & `aviewpy-1.3.3/aviewpy/move.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/aviewpy/objects.py` & `aviewpy-1.3.3/aviewpy/objects.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/aviewpy/ui/alerts.py` & `aviewpy-1.3.3/aviewpy/ui/alerts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from contextlib import contextmanager
 
 import Adams  # type: ignore # noqa
 
 
 @contextmanager
 def adams_errors_suppressed():
+
+    level = Adams.evaluate_exp('user_string(".system_defaults.graphic_window_level")')
     Adams.execute_cmd('interface message graphic_window_level=quiet')
     try:
         yield
     finally:
-        Adams.execute_cmd('interface message graphic_window_level=Verbose')
+        Adams.execute_cmd(f'interface message graphic_window_level={level}')
 
 
 def alert_box(msg: str, alert_type: str = 'info', exc_type: Exception = None):
     """Adams View alert box
 
     Parameters
     ----------
```

### Comparing `aviewpy-1.3.2/aviewpy/ui/progressbar.py` & `aviewpy-1.3.3/aviewpy/ui/progressbar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,60 @@
+from __future__ import annotations
 from contextlib import contextmanager
+from typing import Callable
 
 from PyQt4.QtGui import QApplication
 
-import Adams  # type: ignore # noqa # isort: skip
+import Adams  # type: ignore
 
 PROGRESS_BAR_NAME = '.gui.main.status_toolbar.__PROGRESSBAR__status'
 STATUS_LABEL_NAME = '.gui.main.status_toolbar.status_label'
 
+STATUS_CALLBACK: Callable[[str], None] = None
+PROGRESS_CALLBACK: Callable[[float], None] = None
 
 class Label:
     def __set_name__(self, owner, name):
         self.storage_name = name # pylint: disable=all
 
     def __set__(self, instance, value: str):
         value = str(value)
         Adams.evaluate_exp(f'status_print("{value}")')
         app = QApplication.instance()
         if isinstance(app, QApplication):
             app.processEvents()
         instance.__dict__[self.storage_name] = value
 
+        if STATUS_CALLBACK is not None:
+            STATUS_CALLBACK(value)
+
     def __get__(self, instance, owner):
         return instance.__dict__[self.storage_name]
 
 
 class Progress:
     def __set_name__(self, owner, name):
         self.storage_name = name # pylint: disable=all
         self._value = None
 
-    def __set__(self, instance, value: float):
+    def __set__(self, instance: ProgressBarUpdater, value: float):
         instance.__dict__[self.storage_name] = value
         if any([self.storage_name not in instance.__dict__,
                 not Adams.evaluate_exp(f'{PROGRESS_BAR_NAME}.displayed'),
                 (not isinstance(value, (float, int))) or self._value != int(value)]):
             self._value = value
             Adams.execute_cmd(f'int slider display slider_name={PROGRESS_BAR_NAME}')
             Adams.execute_cmd(f'int slider set slider_name={PROGRESS_BAR_NAME} value={int(value)}')
             app = QApplication.instance()
             if isinstance(app, QApplication):
                 app.processEvents()
             instance.show_label()
+
+            if PROGRESS_CALLBACK is not None:
+                PROGRESS_CALLBACK(value)
     
     def __get__(self, instance, owner):
         return instance.__dict__[self.storage_name]
 
 
 class ProgressBarUpdater():
     progress = Progress()
```

### Comparing `aviewpy-1.3.2/aviewpy/utils/dereferencer.py` & `aviewpy-1.3.3/aviewpy/utils/dereferencer.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/aviewpy/utils/excepthook.py` & `aviewpy-1.3.3/aviewpy/utils/excepthook.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/aviewpy/utils/res_to_csv.py` & `aviewpy-1.3.3/aviewpy/utils/res_to_csv.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/aviewpy/variables.py` & `aviewpy-1.3.3/aviewpy/variables.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import Adams  # type: ignore # noqa # isort: skip
 from Object import ObjectBase as Object  # type: ignore # noqa # isort: skip
 
 
 def set_dv(parent, name: str, value, append=False, **kwargs):
     """Sets the value of a design variable. If the design variable does not exist, it is created.
     
+    Note
+    ----
+    Return value is `None` if `parent' is a string.
+
     Parameters
     ----------
     parent : Object or str
         Parent object of the design variable
     name : str
         Name of the design variable
     value : Number, str, or Object (or list of any of these)
@@ -26,15 +30,15 @@
     value = [value] if not isinstance(value, Iterable) or isinstance(value, str) else value
 
     if isinstance(parent, Object):
         dv = _set_dv_obj(parent, name, value, append, **kwargs)
     elif isinstance(parent, str):
         dv = _set_dv_str(parent, name, value, append)                                               # pylint: disable=assignment-from-no-return
     else:
-        raise TypeError(f'Invalid type for value: {type(parent)}')
+        raise TypeError(f'Invalid type for value: {type(value)}')
 
     return dv
 
 
 def _set_dv_obj(parent: Object, name: str, value: List[Union[Number, str, Object]], append=False, **kwargs):
     """Function to handle setting a design variable when the parent is an Object"""
     if name in parent.DesignVariables:
@@ -52,15 +56,15 @@
     return dv
 
 
 def _set_dv_str(parent: str, name: str, value: List[Union[Number, str, Object]], append=False):
     """Function to handle setting a design variable when the parent is a string"""
     if Adams.evaluate_exp(f'db_exists("{parent}.{name}")') and append:
         value_ = Adams.evaluate_exp(f'{parent}.{name}')
-        value_ = [value_] if not isinstance(value_, (tuple, list)) else value_
+        value_ = [value_] if not isinstance(value_, (tuple, list)) else list(value_)
         value = value_ + value
 
     _cmd_set_dv(value, parent, name)
 
 
 def _create_dv(value: list, parent: Object, name: str, **kwargs):
     """Creates a design variable with the given value.
@@ -101,25 +105,26 @@
     value : Number, str, or Object (or list of any of these)
         Value(s) to set the design variable to
     parent : str
         Parent object of the design variable
     name : str
         Name of the design variable
     """
+    
     if isinstance(value, list) and all(isinstance(v, str) for v in value):
         val_text = ', '.join([f'"{v}"' for v in value])
         Adams.execute_cmd(f'var set var={parent}.{name} str={val_text}')
 
     elif isinstance(value, list) and all(isinstance(v, Number) for v in value):
-        val_text = ', '.join(value)
+        val_text = ', '.join([f'{v}' for v in value])
         Adams.execute_cmd(f'var set var={parent}.{name} real={val_text}')
 
     elif isinstance(value, list) and all(isinstance(v, int) for v in value):
-        val_text = ', '.join(value)
+        val_text = ', '.join([f'{v}' for v in value])
         Adams.execute_cmd(f'var set var={parent}.{name} int={val_text}')
 
     elif isinstance(value, list) and all(isinstance(v, Object) for v in value):
-        val_text = ', '.join(value)
+        val_text = ', '.join([f'{v}' for v in value])
         Adams.execute_cmd(f'var set var={parent}.{name} obj={val_text}')
 
     else:
-        raise TypeError(f'Invalid type for value: {type(parent)}')
+        raise TypeError(f'Invalid type for value: {type(value)}')
```

### Comparing `aviewpy-1.3.2/aviewpy.egg-info/PKG-INFO` & `aviewpy-1.3.3/aviewpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviewpy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python tools for working with in the Adams View python environment
 Home-page: https://github.com/bthornton191/aviewpy
 Author: Ben Thornton
 Author-email: ben.thornton@hexagon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `aviewpy-1.3.2/aviewpy.egg-info/SOURCES.txt` & `aviewpy-1.3.3/aviewpy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 aviewpy/__init__.py
 aviewpy/contact.py
 aviewpy/cs.py
+aviewpy/model.py
 aviewpy/move.py
 aviewpy/objects.py
 aviewpy/results.py
 aviewpy/sim.py
 aviewpy/variables.py
 aviewpy.egg-info/PKG-INFO
 aviewpy.egg-info/SOURCES.txt
 aviewpy.egg-info/dependency_links.txt
 aviewpy.egg-info/requires.txt
 aviewpy.egg-info/top_level.txt
 aviewpy/files/__init__.py
+aviewpy/files/acf.py
+aviewpy/files/adm.py
 aviewpy/files/bin.py
 aviewpy/files/cmd.py
 aviewpy/files/shell.py
+aviewpy/files/to.py
 aviewpy/ui/__init__.py
 aviewpy/ui/alerts.py
 aviewpy/ui/messages.py
 aviewpy/ui/progressbar.py
 aviewpy/ui/windows.py
 aviewpy/utils/__init__.py
 aviewpy/utils/dereferencer.py
```

### Comparing `aviewpy-1.3.2/setup.py` & `aviewpy-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.2/test/test_shell.py` & `aviewpy-1.3.3/test/test_shell.py`

 * *Files identical despite different names*

