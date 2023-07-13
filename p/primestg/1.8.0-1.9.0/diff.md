# Comparing `tmp/primestg-1.8.0.tar.gz` & `tmp/primestg-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/primestg-1.8.0.tar", last modified: Thu May 31 10:00:46 2018, max compression
+gzip compressed data, was "dist/primestg-1.9.0.tar", last modified: Fri Nov  2 12:22:45 2018, max compression
```

## Comparing `primestg-1.8.0.tar` & `primestg-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2018-05-31 10:00:46.000000 primestg-1.8.0/
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2018-05-31 10:00:46.000000 primestg-1.8.0/primestg/
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2018-05-31 10:00:46.000000 primestg-1.8.0/primestg/report/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)    15266 2018-05-31 10:00:40.000000 primestg-1.8.0/primestg/report/base.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       57 2016-12-21 11:32:22.000000 primestg-1.8.0/primestg/report/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)    41616 2018-05-31 10:00:40.000000 primestg-1.8.0/primestg/report/reports.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     4834 2017-09-08 08:01:04.000000 primestg-1.8.0/primestg/service.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      349 2017-11-07 07:50:11.000000 primestg-1.8.0/primestg/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      899 2017-11-07 07:50:11.000000 primestg-1.8.0/primestg/message.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      743 2018-05-31 10:00:46.000000 primestg-1.8.0/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2018-05-31 10:00:46.000000 primestg-1.8.0/setup.cfg
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      885 2018-05-31 10:00:40.000000 primestg-1.8.0/setup.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2129 2018-05-31 09:59:39.000000 primestg-1.8.0/README.rst
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2018-05-31 10:00:46.000000 primestg-1.8.0/primestg.egg-info/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        9 2018-05-31 10:00:46.000000 primestg-1.8.0/primestg.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      743 2018-05-31 10:00:46.000000 primestg-1.8.0/primestg.egg-info/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      318 2018-05-31 10:00:46.000000 primestg-1.8.0/primestg.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       10 2018-05-31 10:00:46.000000 primestg-1.8.0/primestg.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2018-05-31 10:00:46.000000 primestg-1.8.0/primestg.egg-info/dependency_links.txt
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2018-11-02 12:22:45.000000 primestg-1.9.0/
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2018-11-02 12:22:45.000000 primestg-1.9.0/primestg/
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2018-11-02 12:22:45.000000 primestg-1.9.0/primestg/report/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)    15266 2018-05-31 10:00:40.000000 primestg-1.9.0/primestg/report/base.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       57 2016-12-21 11:32:22.000000 primestg-1.9.0/primestg/report/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)    43652 2018-11-02 12:21:58.000000 primestg-1.9.0/primestg/report/reports.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     4834 2017-09-08 08:01:04.000000 primestg-1.9.0/primestg/service.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      349 2017-11-07 07:50:11.000000 primestg-1.9.0/primestg/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      899 2017-11-07 07:50:11.000000 primestg-1.9.0/primestg/message.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      743 2018-11-02 12:22:45.000000 primestg-1.9.0/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2018-11-02 12:22:45.000000 primestg-1.9.0/setup.cfg
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      885 2018-11-02 12:22:15.000000 primestg-1.9.0/setup.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2129 2018-05-31 09:59:39.000000 primestg-1.9.0/README.rst
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2018-11-02 12:22:45.000000 primestg-1.9.0/primestg.egg-info/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        9 2018-11-02 12:22:45.000000 primestg-1.9.0/primestg.egg-info/top_level.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      743 2018-11-02 12:22:45.000000 primestg-1.9.0/primestg.egg-info/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      318 2018-11-02 12:22:45.000000 primestg-1.9.0/primestg.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       10 2018-11-02 12:22:45.000000 primestg-1.9.0/primestg.egg-info/requires.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2018-11-02 12:22:45.000000 primestg-1.9.0/primestg.egg-info/dependency_links.txt
```

### Comparing `primestg-1.8.0/primestg/report/base.py` & `primestg-1.9.0/primestg/report/base.py`

 * *Files identical despite different names*

### Comparing `primestg-1.8.0/primestg/report/reports.py` & `primestg-1.9.0/primestg/report/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     MeasureActiveReactive, Parameter, MeterWithMagnitude,
     ConcentratorWithMetersWithConcentratorName, Concentrator, Measure,
     MeterWithConcentratorName,
 )
 from primestg.message import MessageS
 
 SUPPORTED_REPORTS = ['S02', 'S04', 'S05', 'S06', 'S09', 'S12', 'S13', 'S15',
-                     'S17', 'S24']
+                     'S17', 'S24', 'S27']
 
 
 def is_supported(report_code):
     return report_code in SUPPORTED_REPORTS
 
 
 def get_integer_value(param):
@@ -116,14 +116,50 @@
                 values.append(v)
         except Exception as e:
             self._warnings.append('ERROR: Thrown exception: {}'.format(e))
 
         return values
 
 
+class MeasureS27(MeasureActiveReactive):
+    """
+    Class for a set of measures of report S27.
+    """
+
+    @property
+    def values(self):
+        """
+        Set of measures of report S27.
+
+        :return: a dict with a set of measures of report S27
+        """
+        values = []
+        try:
+            timestamp = self._get_timestamp('Fh')
+            timestamp_max = self._get_timestamp('Fx')
+            v = {
+                'type': 'manual',
+                'value': 'a',
+                'date_begin': timestamp,
+                'date_end': timestamp,
+                'contract': int(self.objectified.get('Ctr')),
+                'period': int(self.objectified.get('Pt')),
+                'max': int(self.objectified.get('Mx')),
+                'date_max': timestamp_max
+            }
+
+            for s27_values in self.objectified.Value:
+                v.update(self.active_reactive(s27_values, 'a'))
+                values.append(v)
+        except Exception as e:
+            self._warnings.append('ERROR: Thrown exception: {}'.format(e))
+
+        return values
+
+
 class MeasureEvents(Measure):
     """
     Class for a set of measures of report S09.
     """
 
     @property
     def values(self):
@@ -689,14 +725,39 @@
         The class used to instance measure sets for report S05.
 
         :return: a class to instance measure sets of report S05
         """
         return MeasureS05
 
 
+class MeterS27(MeterWithMagnitude):
+    """
+    Class for a meter of report S27.
+    """
+
+    @property
+    def report_type(self):
+        """
+        The type of report for report S27.
+
+        :return: a string with 'S27'
+        """
+
+        return 'S27'
+
+    @property
+    def measure_class(self):
+        """
+        The class used to instance measure sets for report S27.
+
+        :return: a class to instance measure sets of report S27
+        """
+        return MeasureS27
+
+
 class MeterS06(MeterWithMagnitude):
     """
     Class for a meter of report S06.
     """
 
     def __init__(
             self,
@@ -894,14 +955,29 @@
         The class used to instance meters for report S05.
 
         :return: a class to instance meters of report S05
         """
         return MeterS05
 
 
+class ConcentratorS27(ConcentratorWithMetersWithConcentratorName):
+    """
+    Class for a concentrator of report S27.
+    """
+
+    @property
+    def meter_class(self):
+        """
+        The class used to instance meters for report S27.
+
+        :return: a class to instance meters of report S27
+        """
+        return MeterS27
+
+
 class ConcentratorS06(ConcentratorWithMetersWithConcentratorName):
     """
     Class for a concentrator of report S06.
     """
 
     def __init__(self, objectified_concentrator, report_version, request_id):
         """
@@ -1377,14 +1453,18 @@
                 'args': [
                     objectified_concentrator,
                     self.report_version,
                     self.request_id,
                     self.report_type
                 ]
             },
+            'S27': {
+                'class': ConcentratorS27,
+                'args': [objectified_concentrator]
+            },
         }
 
         if self.report_type not in report_type_class:
             raise NotImplementedError('Report type not implemented!')
 
         get = report_type_class.get(self.report_type).get
         concentrator_class = get('class')
```

### Comparing `primestg-1.8.0/primestg/service.py` & `primestg-1.9.0/primestg/service.py`

 * *Files identical despite different names*

### Comparing `primestg-1.8.0/primestg/message.py` & `primestg-1.9.0/primestg/message.py`

 * *Files identical despite different names*

### Comparing `primestg-1.8.0/PKG-INFO` & `primestg-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: primestg
-Version: 1.8.0
+Version: 1.9.0
 Summary: Prime STG-DC Interface Specification
 Home-page: https://github.com/gisce/primestg
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: GNU Affero General Public License v3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `primestg-1.8.0/setup.py` & `primestg-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='primestg',
-    version='1.8.0',
+    version='1.9.0',
     packages=find_packages(),
     url='https://github.com/gisce/primestg',
     license='GNU Affero General Public License v3',
     author='GISCE-TI, S.L.',
     author_email='devel@gisce.net',
     install_requires=[
         'lxml',
```

### Comparing `primestg-1.8.0/README.rst` & `primestg-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `primestg-1.8.0/primestg.egg-info/PKG-INFO` & `primestg-1.9.0/primestg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: primestg
-Version: 1.8.0
+Version: 1.9.0
 Summary: Prime STG-DC Interface Specification
 Home-page: https://github.com/gisce/primestg
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: GNU Affero General Public License v3
 Description: UNKNOWN
 Platform: UNKNOWN
```

