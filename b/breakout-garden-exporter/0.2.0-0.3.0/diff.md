# Comparing `tmp/breakout-garden-exporter-0.2.0.tar.gz` & `tmp/breakout-garden-exporter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breakout-garden-exporter-0.2.0.tar", last modified: Tue Jul 11 20:38:39 2023, max compression
+gzip compressed data, was "breakout-garden-exporter-0.3.0.tar", last modified: Thu Jul 13 17:30:52 2023, max compression
```

## Comparing `breakout-garden-exporter-0.2.0.tar` & `breakout-garden-exporter-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-07-11 20:38:39.638414 breakout-garden-exporter-0.2.0/
--rw-r--r--   0 andrew     (501) staff       (20)    35149 2023-06-19 20:41:07.000000 breakout-garden-exporter-0.2.0/LICENSE
--rw-r--r--   0 andrew     (501) staff       (20)     1702 2023-07-11 20:38:39.638606 breakout-garden-exporter-0.2.0/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      957 2023-07-08 10:09:25.000000 breakout-garden-exporter-0.2.0/README.md
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-07-11 20:38:39.624312 breakout-garden-exporter-0.2.0/bin/
--rw-r--r--   0 andrew     (501) staff       (20)     1115 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/bin/breakout-garden-exporter
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-07-11 20:38:39.627588 breakout-garden-exporter-0.2.0/breakout_garden_exporter.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)     1702 2023-07-11 20:38:39.000000 breakout-garden-exporter-0.2.0/breakout_garden_exporter.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      667 2023-07-11 20:38:39.000000 breakout-garden-exporter-0.2.0/breakout_garden_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2023-07-11 20:38:39.000000 breakout-garden-exporter-0.2.0/breakout_garden_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       97 2023-07-11 20:38:39.000000 breakout-garden-exporter-0.2.0/breakout_garden_exporter.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)       29 2023-07-11 20:38:39.000000 breakout-garden-exporter-0.2.0/breakout_garden_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-07-11 20:38:39.633535 breakout-garden-exporter-0.2.0/breakoutgardenexporter/
--rw-r--r--   0 andrew     (501) staff       (20)      947 2023-07-09 12:44:30.000000 breakout-garden-exporter-0.2.0/breakoutgardenexporter/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     1428 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/breakoutgardenexporter/arguments.py
--rw-r--r--   0 andrew     (501) staff       (20)     1730 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/breakoutgardenexporter/icp10125.py
--rw-r--r--   0 andrew     (501) staff       (20)     2340 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/breakoutgardenexporter/metrics.py
--rw-r--r--   0 andrew     (501) staff       (20)      985 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/breakoutgardenexporter/sensor.py
--rw-r--r--   0 andrew     (501) staff       (20)     1835 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/breakoutgardenexporter/sensor_manager.py
--rw-r--r--   0 andrew     (501) staff       (20)     2375 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/breakoutgardenexporter/server.py
--rw-r--r--   0 andrew     (501) staff       (20)      189 2023-07-11 20:38:39.639291 breakout-garden-exporter-0.2.0/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)     1834 2023-07-08 10:06:44.000000 breakout-garden-exporter-0.2.0/setup.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-07-11 20:38:39.637787 breakout-garden-exporter-0.2.0/tests/
--rw-r--r--   0 andrew     (501) staff       (20)      873 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/tests/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     1278 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/tests/test_arguments.py
--rw-r--r--   0 andrew     (501) staff       (20)     1791 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/tests/test_icp10125.py
--rw-r--r--   0 andrew     (501) staff       (20)     1082 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/tests/test_metrics.py
--rw-r--r--   0 andrew     (501) staff       (20)     2161 2023-07-08 09:42:52.000000 breakout-garden-exporter-0.2.0/tests/test_sensor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.691657 breakout-garden-exporter-0.3.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/bin/breakout-garden-exporter
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.691657 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/breakoutgardenexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-13 17:30:47.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/icp10125.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/sensor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/sgp30.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_icp10125.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_sensor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_sgp30.py
```

### Comparing `breakout-garden-exporter-0.2.0/LICENSE` & `breakout-garden-exporter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/PKG-INFO` & `breakout-garden-exporter-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: breakout-garden-exporter
-Version: 0.2.0
+Version: 0.3.0
 Summary: Exposes Prometheus metrics based on data collected from Pimoroni Breakout Garden sensors
 Home-page: https://github.com/andrewjw/breakout-garden-exporter
 Author: Andrew Wilkinson
 Author-email: andrewjwilkinson@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -29,8 +27,7 @@
 Exposes Prometheus metrics from sensors that are part of Pimoroni's Breakout Garden family
 
 optional arguments:
   -h, --help     show this help message and exit
   -q, --quiet    don't log HTTP requests
   --bind [BIND]  the ip address and port to bind to. Default: *:9101
 ```
-
```

### Comparing `breakout-garden-exporter-0.2.0/README.md` & `breakout-garden-exporter-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/bin/breakout-garden-exporter` & `breakout-garden-exporter-0.3.0/bin/breakout-garden-exporter`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/breakout_garden_exporter.egg-info/PKG-INFO` & `breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: breakout-garden-exporter
-Version: 0.2.0
+Version: 0.3.0
 Summary: Exposes Prometheus metrics based on data collected from Pimoroni Breakout Garden sensors
 Home-page: https://github.com/andrewjw/breakout-garden-exporter
 Author: Andrew Wilkinson
 Author-email: andrewjwilkinson@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -29,8 +27,7 @@
 Exposes Prometheus metrics from sensors that are part of Pimoroni's Breakout Garden family
 
 optional arguments:
   -h, --help     show this help message and exit
   -q, --quiet    don't log HTTP requests
   --bind [BIND]  the ip address and port to bind to. Default: *:9101
 ```
-
```

### Comparing `breakout-garden-exporter-0.2.0/breakout_garden_exporter.egg-info/SOURCES.txt` & `breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,12 +11,14 @@
 breakoutgardenexporter/__init__.py
 breakoutgardenexporter/arguments.py
 breakoutgardenexporter/icp10125.py
 breakoutgardenexporter/metrics.py
 breakoutgardenexporter/sensor.py
 breakoutgardenexporter/sensor_manager.py
 breakoutgardenexporter/server.py
+breakoutgardenexporter/sgp30.py
 tests/__init__.py
 tests/test_arguments.py
 tests/test_icp10125.py
 tests/test_metrics.py
-tests/test_sensor_manager.py
+tests/test_sensor_manager.py
+tests/test_sgp30.py
```

### Comparing `breakout-garden-exporter-0.2.0/breakoutgardenexporter/__init__.py` & `breakout-garden-exporter-0.3.0/breakoutgardenexporter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 from .arguments import get_arguments
 from .icp10125 import ICP10125Sensor
 from .metrics import Metrics, MetricType, COUNTER, GAUGE
 from .sensor_manager import SensorManager
 from .server import serve
+from .sgp30 import SGP30Sensor
```

### Comparing `breakout-garden-exporter-0.2.0/breakoutgardenexporter/arguments.py` & `breakout-garden-exporter-0.3.0/breakoutgardenexporter/arguments.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/breakoutgardenexporter/icp10125.py` & `breakout-garden-exporter-0.3.0/breakoutgardenexporter/icp10125.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/breakoutgardenexporter/metrics.py` & `breakout-garden-exporter-0.3.0/breakoutgardenexporter/metrics.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/breakoutgardenexporter/sensor.py` & `breakout-garden-exporter-0.3.0/breakoutgardenexporter/sensor.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/breakoutgardenexporter/sensor_manager.py` & `breakout-garden-exporter-0.3.0/breakoutgardenexporter/sensor_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 import time
 import threading
 from typing import Dict
 
 from .icp10125 import ICP10125Sensor
 from .metrics import Metrics
 from .sensor import Sensor
+from .sgp30 import SGP30Sensor
 
-SENSORS = [ICP10125Sensor]
+SENSORS = [ICP10125Sensor, SGP30Sensor]
 
 
 class SensorManager(threading.Thread):
     def __init__(self, metrics: Metrics) -> None:
         threading.Thread.__init__(self)
         self.daemon = True
         self.sensors: Dict[Sensor, float] = {}
```

### Comparing `breakout-garden-exporter-0.2.0/breakoutgardenexporter/server.py` & `breakout-garden-exporter-0.3.0/breakoutgardenexporter/server.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/setup.py` & `breakout-garden-exporter-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/tests/__init__.py` & `breakout-garden-exporter-0.3.0/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from .test_arguments import TestArguments
 from .test_icp10125 import TestICP10125
 from .test_metrics import TestMetrics
 from .test_sensor_manager import TestSensorManager
+from .test_sgp30 import TestSGP30
```

### Comparing `breakout-garden-exporter-0.2.0/tests/test_arguments.py` & `breakout-garden-exporter-0.3.0/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/tests/test_icp10125.py` & `breakout-garden-exporter-0.3.0/tests/test_icp10125.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/tests/test_metrics.py` & `breakout-garden-exporter-0.3.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.2.0/tests/test_sensor_manager.py` & `breakout-garden-exporter-0.3.0/tests/test_sensor_manager.py`

 * *Files identical despite different names*

