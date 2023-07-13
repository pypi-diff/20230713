# Comparing `tmp/midas-weather-1.0.1.tar.gz` & `tmp/midas-weather-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-weather-1.0.1.tar", last modified: Mon Sep 19 11:06:46 2022, max compression
+gzip compressed data, was "midas-weather-1.1.0.tar", last modified: Thu Jul 13 14:06:03 2023, max compression
```

## Comparing `midas-weather-1.0.1.tar` & `midas-weather-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-09-19 11:06:46.680321 midas-weather-1.0.1/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     7648 2022-04-01 11:58:46.000000 midas-weather-1.0.1/LICENSE
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1002 2022-09-19 11:06:46.680321 midas-weather-1.0.1/PKG-INFO
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       15 2022-04-01 11:58:46.000000 midas-weather-1.0.1/README.md
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-09-19 11:06:46.680321 midas-weather-1.0.1/midas/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-09-19 11:06:46.680321 midas-weather-1.0.1/midas/modules/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-09-19 11:06:46.680321 midas-weather-1.0.1/midas/modules/weather/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2022-05-09 06:34:11.000000 midas-weather-1.0.1/midas/modules/weather/__init__.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8050 2022-04-06 06:12:01.000000 midas-weather-1.0.1/midas/modules/weather/download.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1305 2022-04-01 11:58:46.000000 midas-weather-1.0.1/midas/modules/weather/meta.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-09-19 11:06:46.680321 midas-weather-1.0.1/midas/modules/weather/model/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-04-01 11:58:46.000000 midas-weather-1.0.1/midas/modules/weather/model/__init__.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3933 2022-04-01 11:58:46.000000 midas-weather-1.0.1/midas/modules/weather/model/current.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7156 2022-04-01 11:58:46.000000 midas-weather-1.0.1/midas/modules/weather/model/forecast.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5382 2022-05-09 06:34:11.000000 midas-weather-1.0.1/midas/modules/weather/model/provider.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6447 2022-09-19 11:05:32.000000 midas-weather-1.0.1/midas/modules/weather/module.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8857 2022-05-09 06:34:11.000000 midas-weather-1.0.1/midas/modules/weather/simulator.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-09-19 11:06:46.680321 midas-weather-1.0.1/midas_weather.egg-info/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1002 2022-09-19 11:06:46.000000 midas-weather-1.0.1/midas_weather.egg-info/PKG-INFO
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      534 2022-09-19 11:06:46.000000 midas-weather-1.0.1/midas_weather.egg-info/SOURCES.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2022-09-19 11:06:46.000000 midas-weather-1.0.1/midas_weather.egg-info/dependency_links.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      114 2022-09-19 11:06:46.000000 midas-weather-1.0.1/midas_weather.egg-info/requires.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2022-09-19 11:06:46.000000 midas-weather-1.0.1/midas_weather.egg-info/top_level.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2022-09-19 11:06:46.680321 midas-weather-1.0.1/setup.cfg
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1666 2022-04-04 10:37:12.000000 midas-weather-1.0.1/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-13 14:06:03.266454 midas-weather-1.1.0/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     7648 2023-07-13 13:26:00.000000 midas-weather-1.1.0/LICENSE
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      983 2023-07-13 14:06:03.266454 midas-weather-1.1.0/PKG-INFO
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       15 2023-07-13 13:26:00.000000 midas-weather-1.1.0/README.md
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-13 14:06:03.263121 midas-weather-1.1.0/midas/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-13 14:06:03.263121 midas-weather-1.1.0/midas/modules/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-13 14:06:03.263121 midas-weather-1.1.0/midas/modules/weather/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2023-07-13 13:26:00.000000 midas-weather-1.1.0/midas/modules/weather/__init__.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8050 2023-07-13 13:26:00.000000 midas-weather-1.1.0/midas/modules/weather/download.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1467 2023-07-13 13:37:54.000000 midas-weather-1.1.0/midas/modules/weather/meta.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-13 14:06:03.263121 midas-weather-1.1.0/midas/modules/weather/model/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-13 13:26:00.000000 midas-weather-1.1.0/midas/modules/weather/model/__init__.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4091 2023-07-13 13:37:23.000000 midas-weather-1.1.0/midas/modules/weather/model/current.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7156 2023-07-13 13:26:00.000000 midas-weather-1.1.0/midas/modules/weather/model/forecast.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5894 2023-07-13 14:04:31.000000 midas-weather-1.1.0/midas/modules/weather/model/provider.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6447 2023-07-13 13:26:00.000000 midas-weather-1.1.0/midas/modules/weather/module.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8857 2023-07-13 13:26:00.000000 midas-weather-1.1.0/midas/modules/weather/simulator.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-13 14:06:03.266454 midas-weather-1.1.0/midas_weather.egg-info/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      983 2023-07-13 14:06:03.000000 midas-weather-1.1.0/midas_weather.egg-info/PKG-INFO
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      534 2023-07-13 14:06:03.000000 midas-weather-1.1.0/midas_weather.egg-info/SOURCES.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2023-07-13 14:06:03.000000 midas-weather-1.1.0/midas_weather.egg-info/dependency_links.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      114 2023-07-13 14:06:03.000000 midas-weather-1.1.0/midas_weather.egg-info/requires.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2023-07-13 14:06:03.000000 midas-weather-1.1.0/midas_weather.egg-info/top_level.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2023-07-13 14:06:03.266454 midas-weather-1.1.0/setup.cfg
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1666 2023-07-13 13:26:00.000000 midas-weather-1.1.0/setup.py
```

### Comparing `midas-weather-1.0.1/LICENSE` & `midas-weather-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-weather-1.0.1/PKG-INFO` & `midas-weather-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: midas-weather
-Version: 1.0.1
+Version: 1.1.0
 Summary: A MIDAS module for weather datasets.
 Home-page: https://gitlab.com/midas-mosaik/midas-weather
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,8 +20,7 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MIDAS Weather
-
```

### Comparing `midas-weather-1.0.1/midas/modules/weather/download.py` & `midas-weather-1.1.0/midas/modules/weather/download.py`

 * *Files identical despite different names*

### Comparing `midas-weather-1.0.1/midas/modules/weather/meta.py` & `midas-weather-1.1.0/midas/modules/weather/meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,16 @@
             ],
             "attrs": [
                 "now",
                 "bh_w_per_m2",
                 "dh_w_per_m2",
                 "t_air_deg_celsius",
                 "day_avg_t_air_deg_celsius",
+                "wind_v_m_per_s",
+                "wind_direction_deg",
             ],
         },
         "WeatherForecast": {
             "public": True,
             "params": [
                 "data_path",
                 "start_date",
@@ -39,11 +41,13 @@
             "attrs": [
                 "now",
                 "forecast_horizon_hours",
                 "forecast_bh_w_per_m2",
                 "forecast_dh_w_per_m2",
                 "forecast_t_air_deg_celsius",
                 "forecast_day_avg_t_air_deg_celsius",
+                "forecast_wind_v_m_per_s",
+                "forecast_wind_direction_deg",
             ],
         },
     },
 }
```

### Comparing `midas-weather-1.0.1/midas/modules/weather/model/current.py` & `midas-weather-1.1.0/midas/modules/weather/model/current.py`

 * *Files 19% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         self.randomize = randomize
 
         # State
         self.t_air_deg_celsius = None
         self.day_avg_t_air_deg_celsius = None
         self.bh_w_per_m2 = None
         self.dh_w_per_m2 = None
+        self.wind_v_m_per_s = None
+        self.wind_direction_deg = None
         self.rng = np.random.RandomState(seed)
 
         # Input
         self.step_size = step_size
         self.block_mode = block_mode
         self.frame = frame
 
@@ -113,7 +115,9 @@
         res[3][0] = max(0, res[3][0])
 
         # print(res)
         self.t_air_deg_celsius = res[0][0]
         self.day_avg_t_air_deg_celsius = res[1][0]
         self.bh_w_per_m2 = res[2][0]
         self.dh_w_per_m2 = res[3][0]
+        self.wind_v_m_per_s = res[4][0]
+        self.wind_direction_deg = res[5][0]
```

### Comparing `midas-weather-1.0.1/midas/modules/weather/model/forecast.py` & `midas-weather-1.1.0/midas/modules/weather/model/forecast.py`

 * *Files identical despite different names*

### Comparing `midas-weather-1.0.1/midas/modules/weather/model/provider.py` & `midas-weather-1.1.0/midas/modules/weather/model/provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -81,25 +81,32 @@
                     + data2[AVG_T_AIR].values.tolist()
                 ),
                 (
                     (data1[GHI].values - data1[DI].values).tolist()
                     + (data2[GHI].values - data2[DI].values).tolist()
                 ),
                 (data1[DI].values.tolist() + data2[DI].values.tolist()),
+                (data1[WIND].values.tolist() + data2[WIND].values.tolist()),
+                (
+                    data1[WINDDIR].values.tolist()
+                    + data2[WINDDIR].values.tolist()
+                ),
             ]
 
         else:
 
             data = self.wdata.loc[start:end]
 
             return [
                 data[T_AIR].values.tolist(),
                 data[AVG_T_AIR].values.tolist(),
                 (data[GHI].values - data[DI].values).tolist(),
                 data[DI].values.tolist(),
+                data[WIND].values.tolist(),
+                data[WINDDIR].values.tolist(),
             ]
 
     def select_block(self, now_dt, horizon=1, frame=2):
         """Select weather data from a block related to *now_dt*.
 
         Gather the weather data from *frame* days in the past and in
         the future at exactly the same hour of the day and select
@@ -122,14 +129,16 @@
         if frame < 1:
             return self.select_hour(now_dt, horizon)
 
         t_airs = []
         avg_t_airs = []
         ghis = []
         dis = []
+        winds = []
+        winddirs = []
 
         # Iterate over time horizon
         for hour in range(horizon):
             start = now_dt + timedelta(hours=hour)
 
             # Get days of the current time frame
             days_before = [
@@ -154,13 +163,15 @@
             data = self.wdata[self.wdata.index.isin(days)]
 
             # Select randomly from time frame
             t_airs.append(self.rng.choice(data[T_AIR].values.tolist()))
             avg_t_airs.append(self.rng.choice(data[AVG_T_AIR].values.tolist()))
             ghis.append(self.rng.choice(data[GHI].values.tolist()))
             dis.append(self.rng.choice(data[DI].values.tolist()))
+            winds.append(self.rng.choice(data[WIND].values.tolist()))
+            winddirs.append(self.rng.choice(data[WINDDIR].values.tolist()))
 
-        return [t_airs, avg_t_airs, ghis, dis]
+        return [t_airs, avg_t_airs, ghis, dis, wind, winddirs]
 
 
 # if __name__ == "__main__":
 #     WeatherData("data/weather_bre2009-2020.hdf5")
```

### Comparing `midas-weather-1.0.1/midas/modules/weather/module.py` & `midas-weather-1.1.0/midas/modules/weather/module.py`

 * *Files identical despite different names*

### Comparing `midas-weather-1.0.1/midas/modules/weather/simulator.py` & `midas-weather-1.1.0/midas/modules/weather/simulator.py`

 * *Files identical despite different names*

### Comparing `midas-weather-1.0.1/midas_weather.egg-info/PKG-INFO` & `midas-weather-1.1.0/midas_weather.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: midas-weather
-Version: 1.0.1
+Version: 1.1.0
 Summary: A MIDAS module for weather datasets.
 Home-page: https://gitlab.com/midas-mosaik/midas-weather
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,8 +20,7 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MIDAS Weather
-
```

### Comparing `midas-weather-1.0.1/midas_weather.egg-info/SOURCES.txt` & `midas-weather-1.1.0/midas_weather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midas-weather-1.0.1/setup.py` & `midas-weather-1.1.0/setup.py`

 * *Files identical despite different names*

