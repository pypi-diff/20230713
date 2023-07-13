# Comparing `tmp/sport-activities-features-0.3.8.tar.gz` & `tmp/sport-activities-features-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sport-activities-features-0.3.8.tar", max compression
+gzip compressed data, was "sport-activities-features-0.3.9.tar", max compression
```

## Comparing `sport-activities-features-0.3.8.tar` & `sport-activities-features-0.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1085 2022-12-21 16:09:24.950077 sport-activities-features-0.3.8/LICENSE
--rw-r--r--   0        0        0    25300 2022-12-21 16:09:24.950077 sport-activities-features-0.3.8/README.md
--rw-r--r--   0        0        0     1539 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1813 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/__init__.py
--rw-r--r--   0        0        0     1642 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/activity_generator.py
--rw-r--r--   0        0        0    17167 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/area_identification.py
--rw-r--r--   0        0        0      659 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/classes.py
--rw-r--r--   0        0        0     3556 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/data_analysis.py
--rw-r--r--   0        0        0     2500 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/data_extraction.py
--rw-r--r--   0        0        0     2598 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/data_extraction_from_csv.py
--rw-r--r--   0        0        0    15137 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/dead_end_identification.py
--rw-r--r--   0        0        0     3520 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/file_manipulation.py
--rw-r--r--   0        0        0    12040 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/gpx_manipulation.py
--rw-r--r--   0        0        0     6268 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/hill_identification.py
--rw-r--r--   0        0        0     4148 2022-12-21 16:09:24.979077 sport-activities-features-0.3.8/sport_activities_features/interruptions/exercise.py
--rw-r--r--   0        0        0     4578 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/interruptions/exercise_event.py
--rw-r--r--   0        0        0     9639 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/interruptions/interruption_processor.py
--rw-r--r--   0        0        0     4457 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/interruptions/overpass.py
--rw-r--r--   0        0        0    18643 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/interval_identification.py
--rw-r--r--   0        0        0     3312 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/missing_elevation_identification.py
--rw-r--r--   0        0        0     4056 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/overpy_node_manipulation.py
--rw-r--r--   0        0        0     6969 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/plot_data.py
--rw-r--r--   0        0        0     7027 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/tcx_manipulation.py
--rw-r--r--   0        0        0     6895 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/topographic_features.py
--rw-r--r--   0        0        0     5877 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/training_loads.py
--rw-r--r--   0        0        0    10962 2022-12-21 16:09:24.980077 sport-activities-features-0.3.8/sport_activities_features/weather_identification.py
--rw-r--r--   0        0        0     5276 2022-12-21 16:09:24.981077 sport-activities-features-0.3.8/sport_activities_features/weather_objects/AverageWeather.py
--rw-r--r--   0        0        0     5201 2022-12-21 16:09:24.981077 sport-activities-features-0.3.8/sport_activities_features/weather_objects/Weather.py
--rw-r--r--   0        0        0    26907 2022-12-21 16:09:32.151272 sport-activities-features-0.3.8/setup.py
--rw-r--r--   0        0        0    26470 2022-12-21 16:09:32.152944 sport-activities-features-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-01-16 19:03:12.135611 sport-activities-features-0.3.9/LICENSE
+-rw-r--r--   0        0        0    25300 2023-01-16 19:03:12.135611 sport-activities-features-0.3.9/README.md
+-rw-r--r--   0        0        0     1539 2023-01-16 19:03:12.185612 sport-activities-features-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1813 2023-01-16 19:03:12.185612 sport-activities-features-0.3.9/sport_activities_features/__init__.py
+-rw-r--r--   0        0        0     1642 2023-01-16 19:03:12.186612 sport-activities-features-0.3.9/sport_activities_features/activity_generator.py
+-rw-r--r--   0        0        0    17167 2023-01-16 19:03:12.186612 sport-activities-features-0.3.9/sport_activities_features/area_identification.py
+-rw-r--r--   0        0        0      659 2023-01-16 19:03:12.186612 sport-activities-features-0.3.9/sport_activities_features/classes.py
+-rw-r--r--   0        0        0     3556 2023-01-16 19:03:12.186612 sport-activities-features-0.3.9/sport_activities_features/data_analysis.py
+-rw-r--r--   0        0        0     2500 2023-01-16 19:03:12.186612 sport-activities-features-0.3.9/sport_activities_features/data_extraction.py
+-rw-r--r--   0        0        0     2598 2023-01-16 19:03:12.187612 sport-activities-features-0.3.9/sport_activities_features/data_extraction_from_csv.py
+-rw-r--r--   0        0        0    15137 2023-01-16 19:03:12.187612 sport-activities-features-0.3.9/sport_activities_features/dead_end_identification.py
+-rw-r--r--   0        0        0     3520 2023-01-16 19:03:12.187612 sport-activities-features-0.3.9/sport_activities_features/file_manipulation.py
+-rw-r--r--   0        0        0    12202 2023-01-16 19:03:12.187612 sport-activities-features-0.3.9/sport_activities_features/gpx_manipulation.py
+-rw-r--r--   0        0        0     6268 2023-01-16 19:03:12.187612 sport-activities-features-0.3.9/sport_activities_features/hill_identification.py
+-rw-r--r--   0        0        0     4148 2023-01-16 19:03:12.188612 sport-activities-features-0.3.9/sport_activities_features/interruptions/exercise.py
+-rw-r--r--   0        0        0     4578 2023-01-16 19:03:12.188612 sport-activities-features-0.3.9/sport_activities_features/interruptions/exercise_event.py
+-rw-r--r--   0        0        0     9639 2023-01-16 19:03:12.188612 sport-activities-features-0.3.9/sport_activities_features/interruptions/interruption_processor.py
+-rw-r--r--   0        0        0     4457 2023-01-16 19:03:12.189612 sport-activities-features-0.3.9/sport_activities_features/interruptions/overpass.py
+-rw-r--r--   0        0        0    18643 2023-01-16 19:03:12.189612 sport-activities-features-0.3.9/sport_activities_features/interval_identification.py
+-rw-r--r--   0        0        0     3312 2023-01-16 19:03:12.189612 sport-activities-features-0.3.9/sport_activities_features/missing_elevation_identification.py
+-rw-r--r--   0        0        0     4056 2023-01-16 19:03:12.189612 sport-activities-features-0.3.9/sport_activities_features/overpy_node_manipulation.py
+-rw-r--r--   0        0        0     6969 2023-01-16 19:03:12.189612 sport-activities-features-0.3.9/sport_activities_features/plot_data.py
+-rw-r--r--   0        0        0     7027 2023-01-16 19:03:12.189612 sport-activities-features-0.3.9/sport_activities_features/tcx_manipulation.py
+-rw-r--r--   0        0        0     6895 2023-01-16 19:03:12.190612 sport-activities-features-0.3.9/sport_activities_features/topographic_features.py
+-rw-r--r--   0        0        0     5877 2023-01-16 19:03:12.190612 sport-activities-features-0.3.9/sport_activities_features/training_loads.py
+-rw-r--r--   0        0        0    10962 2023-01-16 19:03:12.190612 sport-activities-features-0.3.9/sport_activities_features/weather_identification.py
+-rw-r--r--   0        0        0     5276 2023-01-16 19:03:12.190612 sport-activities-features-0.3.9/sport_activities_features/weather_objects/AverageWeather.py
+-rw-r--r--   0        0        0     5201 2023-01-16 19:03:12.191612 sport-activities-features-0.3.9/sport_activities_features/weather_objects/Weather.py
+-rw-r--r--   0        0        0    26907 2023-01-16 19:03:23.168101 sport-activities-features-0.3.9/setup.py
+-rw-r--r--   0        0        0    26470 2023-01-16 19:03:23.170717 sport-activities-features-0.3.9/PKG-INFO
```

### Comparing `sport-activities-features-0.3.8/LICENSE` & `sport-activities-features-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/README.md` & `sport-activities-features-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/pyproject.toml` & `sport-activities-features-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sport-activities-features"
-version = "0.3.8"
+version = "0.3.9"
 description = "A minimalistic toolbox for extracting features from sport activity files"
 license = "MIT"
 authors = ["Iztok Fister Jr. <iztok@iztok-jr-fister.eu>", "Luka Lukač <luka.lukac@student.um.si>", "Alen Rajšp <alen.rajsp@.um.si>", "Luka Pečnik <luka.pecnik@student.um.si>", "Dušan Fister <dusan.fister@um.si>"]
 keywords = ['computational intelligence', 'data mining', 'datasets', 'gpx', 'optimization', 'sport activities', 'tcx']
 homepage = "https://github.com/firefly-cpp/sport-activities-features"
 repository = "https://github.com/firefly-cpp/sport-activities-features"
 readme = "README.md"
@@ -15,15 +15,15 @@
 geopy = "^2.0.0"
 requests = "^2.25.1"
 overpy = "^0.6"
 gpxpy = "^1.4.2"
 geotiler = "^0.14.5"
 dotmap = "^1.3.25"
 numpy = "^1.23.1"
-tcxreader = "^0.4.1"
+tcxreader = "^0.4.4"
 pandas = "*"
 niaaml = "^1.1.10"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^3.5.1"
 sphinx-rtd-theme = "^0.5.1"
 coveralls = "^2.2.0"
```

### Comparing `sport-activities-features-0.3.8/sport_activities_features/__init__.py` & `sport-activities-features-0.3.9/sport_activities_features/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,8 +53,8 @@
     'Weather',
     'WeatherIdentification',
     'AverageWeather',
     'ElevationIdentification',
     'InterruptionProcessor'
 ]
 
-__version__ = '0.3.8'
+__version__ = '0.3.9'
```

### Comparing `sport-activities-features-0.3.8/sport_activities_features/activity_generator.py` & `sport-activities-features-0.3.9/sport_activities_features/activity_generator.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/area_identification.py` & `sport-activities-features-0.3.9/sport_activities_features/area_identification.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/classes.py` & `sport-activities-features-0.3.9/sport_activities_features/classes.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/data_analysis.py` & `sport-activities-features-0.3.9/sport_activities_features/data_analysis.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/data_extraction.py` & `sport-activities-features-0.3.9/sport_activities_features/data_extraction.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/data_extraction_from_csv.py` & `sport-activities-features-0.3.9/sport_activities_features/data_extraction_from_csv.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/dead_end_identification.py` & `sport-activities-features-0.3.9/sport_activities_features/dead_end_identification.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/file_manipulation.py` & `sport-activities-features-0.3.9/sport_activities_features/file_manipulation.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/gpx_manipulation.py` & `sport-activities-features-0.3.9/sport_activities_features/gpx_manipulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,21 @@
                     'speeds': speeds
                  }
         Note:
             In the case of missing value in raw data, we assign None.
         """
         NAMESPACE = "{http://www.garmin.com/xmlschemas/TrackPointExtension/v1}"
         points = []
-        gpx_file = open(filename)
-        gpx = gpxpy.parse(gpx_file)
+        gpx = None
+        try:
+            gpx_file = open(filename, encoding='utf-8')
+            gpx = gpxpy.parse(gpx_file)
+        except Exception:
+            gpx_file = open(filename)
+            gpx = gpxpy.parse(gpx_file)
         previous_point = None
         for track in gpx.tracks:
             for segment in track.segments:
                 for point_gpx in segment.points:
                     trackpoint = GPXTrackPoint()
                     trackpoint.from_GPX(point_gpx)
                     if len(point_gpx.extensions) > 0:
```

### Comparing `sport-activities-features-0.3.8/sport_activities_features/hill_identification.py` & `sport-activities-features-0.3.9/sport_activities_features/hill_identification.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/interruptions/exercise.py` & `sport-activities-features-0.3.9/sport_activities_features/interruptions/exercise.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/interruptions/exercise_event.py` & `sport-activities-features-0.3.9/sport_activities_features/interruptions/exercise_event.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/interruptions/interruption_processor.py` & `sport-activities-features-0.3.9/sport_activities_features/interruptions/interruption_processor.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/interruptions/overpass.py` & `sport-activities-features-0.3.9/sport_activities_features/interruptions/overpass.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/interval_identification.py` & `sport-activities-features-0.3.9/sport_activities_features/interval_identification.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/missing_elevation_identification.py` & `sport-activities-features-0.3.9/sport_activities_features/missing_elevation_identification.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/overpy_node_manipulation.py` & `sport-activities-features-0.3.9/sport_activities_features/overpy_node_manipulation.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/plot_data.py` & `sport-activities-features-0.3.9/sport_activities_features/plot_data.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/tcx_manipulation.py` & `sport-activities-features-0.3.9/sport_activities_features/tcx_manipulation.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/topographic_features.py` & `sport-activities-features-0.3.9/sport_activities_features/topographic_features.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/training_loads.py` & `sport-activities-features-0.3.9/sport_activities_features/training_loads.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/weather_identification.py` & `sport-activities-features-0.3.9/sport_activities_features/weather_identification.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/weather_objects/AverageWeather.py` & `sport-activities-features-0.3.9/sport_activities_features/weather_objects/AverageWeather.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/sport_activities_features/weather_objects/Weather.py` & `sport-activities-features-0.3.9/sport_activities_features/weather_objects/Weather.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-0.3.8/setup.py` & `sport-activities-features-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,19 @@
  'gpxpy>=1.4.2,<2.0.0',
  'matplotlib>=3.3.3,<4.0.0',
  'niaaml>=1.1.10,<2.0.0',
  'numpy>=1.23.1,<2.0.0',
  'overpy>=0.6,<0.7',
  'pandas',
  'requests>=2.25.1,<3.0.0',
- 'tcxreader>=0.4.1,<0.5.0']
+ 'tcxreader>=0.4.4,<0.5.0']
 
 setup_kwargs = {
     'name': 'sport-activities-features',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'A minimalistic toolbox for extracting features from sport activity files',
     'long_description': '<p align="center">\n  <img width="200" src="https://raw.githubusercontent.com/firefly-cpp/sport-activities-features/main/.github/logo/sport_activities.png">\n</p>\n\n---\n\n# sport-activities-features --- A minimalistic toolbox for extracting features from sports activity files written in Python\n\n---\n\n[![PyPI Version](https://img.shields.io/pypi/v/sport-activities-features.svg)](https://pypi.python.org/pypi/sport-activities-features)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sport-activities-features.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/sport-activities-features.svg)\n[![Downloads](https://pepy.tech/badge/sport-activities-features)](https://pepy.tech/project/sport-activities-features)\n![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/sport-activities-features?style=flat-square)\n[![GitHub license](https://img.shields.io/github/license/firefly-cpp/sport-activities-features.svg)](https://github.com/firefly-cpp/sport-activities-features/blob/master/LICENSE)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/sport-activities-features.svg)\n[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/sport-activities-features.svg)](http://isitmaintained.com/project/firefly-cpp/sport-activities-features "Average time to resolve an issue")\n[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/sport-activities-features.svg)](http://isitmaintained.com/project/firefly-cpp/sport-activities-features "Percentage of issues still open")\n[![All Contributors](https://img.shields.io/badge/all_contributors-6-orange.svg?style=flat-square)](#contributors-)\n[![Fedora package](https://img.shields.io/fedora/v/python3-sport-activities-features?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-sport-activities-features)\n[![AUR package](https://img.shields.io/aur/version/python-sport-activities-features?color=blue&label=Arch%20Linux&logo=arch-linux)](https://aur.archlinux.org/packages/python-sport-activities-features)\n[![DOI](https://img.shields.io/badge/DOI-10.1109/INES52918.2021.9512927-blue)](https://doi.org/10.1109/INES52918.2021.9512927)\n\n## General outline of the framework\nMonitoring sports activities produce many geographic, topologic, and personalized data, with a vast majority of details hidden. Thus, a rigorous ex-post data analysis and statistic evaluation are required to extract them. Namely, most mainstream solutions for analyzing sports activities files rely on integral metrics, such as total duration, total distance, and average heart rate, which may suffer from the "overall (integral) metrics problem." Among others, such problems are expressed in capturing sports activities in general only (omitting crucial components), calculating potentially fallacious and misleading metrics, not recognizing different stages/phases of the sports activity (warm-up, endurance, intervals), and others.\n\nThe sport-activities-framework, on the other side, offers a detailed insight into the sports activity files. The framework supports both identification and extraction methods, such as identifying the number of hills, extracting the average altitudes of identified hills, measuring the total distance of identified hills, deriving climbing ratios (total distance of identified hills vs. total distance), average/total ascents of hills and so much more. The framework also integrates many other extensions, among others, historical weather parsing, statistical evaluations, and ex-post visualizations. Previous work on these topical questions was addressed in [relevant scientific papers on data mining](http://iztok-jr-fister.eu/static/publications/42.pdf), also in combination with the [generating/predicting automated sport training sessions](http://iztok-jr-fister.eu/static/publications/189.pdf).\n\n\n## Detailed insights\nThe sport-activities-features framework is compatible with TCX & GPX activity files and [Overpass API](https://wiki.openstreetmap.org/wiki/Overpass_API) nodes. The current version withholds (but is not limited to) the following functions:\n- extracting integral metrics, such as total distance, total duration, calories ([see example](examples/integral_metrics_extraction.py)),\n- extracting topographic features, such as the number of hills, the average altitude of identified hills, the total distance of identified hills, climbing ratio, average ascent of hills, total ascent, and total descent ([see example](examples/hill_data_extraction.py)),\n- plotting identified hills ([see example](examples/draw_map_with_identified_hills.py)),\n- extracting the intervals, such as number of intervals, maximum/minimum/average duration of intervals, maximum/minimum/average distance of intervals, maximum/minimum/average heart rate during intervals,\n- plotting the identified intervals ([see example](examples/draw_map_with_identified_intervals.py)),\n- calculating the training loads, such as Banister TRIMP, Lucia TRIMP([see example](examples/calculate_training_load.py)),\n- parsing the historical weather data from an external service,\n- extracting the integral metrics of the activity inside the area given with coordinates (distance, heart rate, speed) ([see example](examples/extract_data_inside_area.py)),\n- extracting the activities from CSV file(s) and randomly selecting the specific number of activities ([see example](examples/extract_random_activities_from_csv.py)),\n- extracting the dead ends,\n- and much more.\n\nThe framework comes with two (testing) benchmark datasets, which are freely available to download from: [DATASET1](http://iztok-jr-fister.eu/static/publications/Sport5.zip), [DATASET2](http://iztok-jr-fister.eu/static/css/datasets/Sport.zip).\n\n\n## Installation\n\n### pip3\n\nInstall sport-activities-features with pip3:\n\n```sh\npip3 install sport-activities-features\n```\n\n### Alpine Linux\n\nTo install sport-activities-features on Alpine, use:\n\n```sh\n$ apk add py3-sport-activities-features\n```\n\n### Fedora Linux\n\nTo install sport-activities-features on Fedora, use:\n\n```sh\n$ dnf install python3-sport-activities-features\n```\n\n### Arch Linux\n\nTo install sport-activities-features on Arch Linux, please use an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers):\n\n```sh\n$ yay -Syyu python-sport-activities-features\n```\n\n## API\n\nThere is a simple API for remote work with the sport-activities-features package available [here](https://github.com/alenrajsp/sport-activities-features-api).\n\n\n## Historical weather data\nWeather data parsed is collected from the [Visual Crossing Weather API](https://www.visualcrossing.com/).\nPlease note that this is an external unaffiliated service, and users must register to use the API.\nThe service has a free tier (1000 Weather reports/day) but is otherwise operating on a pay-as-you-go model.\nFor pricing and terms of use, please read the [official documentation](https://www.visualcrossing.com/weather-data-editions) of the API provider.\n\n## Overpass API & Open Elevation API integration\nWithout performing activities, we can use the [OpenStreetMap](https://www.openstreetmap.org/) for the identification of hills,\ntotal ascent, and descent. This is done using the [Overpass API](https://wiki.openstreetmap.org/wiki/Overpass_API)\nwhich is a read-only API that allows querying of OSM map data. In addition to that altitude, data is retrieved by using the\n[Open-Elevation API](https://open-elevation.com/) which is an open-source and free alternative to the Google Elevation API.\nBoth of the solutions can be used by using free publicly acessible APIs ([Overpass](https://wiki.openstreetmap.org/wiki/Overpass_API), [Open-Elevation](https://open-elevation.com/#public-api)) or can be self hosted on a server or as a Docker container ([Overpass](https://wiki.openstreetmap.org/wiki/Overpass_API/Installation), [Open-Elevation](https://github.com/Jorl17/open-elevation/blob/master/docs/host-your-own.md)).\n\n## CODE EXAMPLES:\n\n### Reading files\n\n#### (*.TCX)\n```python\nfrom sport_activities_features.tcx_manipulation import TCXFile\n\n# Class for reading TCX files\ntcx_file=TCXFile()\ndata = tcx_file.read_one_file("path_to_the_file") # Represents data as dictionary of lists\n\n# Alternative choice\ndata = tcx_file.read_one_file("path_to_the_file", numpy_array= True) # Represents data as dictionary of numpy.arrays\n\n```\n\n#### (*.GPX)\n```python\nfrom sport_activities_features.gpx_manipulation import GPXFile\n\n# Class for reading GPX files\ngpx_file=GPXFile()\n\n# Read the file and generate a dictionary with \ndata = gpx_file.read_one_file("path_to_the_file") # Represents data as dictionary of lists\n\n# Alternative choice\ndata = gpx_file.read_one_file("path_to_the_file", numpy_array= True) # Represents data as dictionary of numpy.arrays\n\n```\n\n\n\n### Extraction of topographic features\n```python\nfrom sport_activities_features.hill_identification import HillIdentification\nfrom sport_activities_features.tcx_manipulation import TCXFile\nfrom sport_activities_features.topographic_features import TopographicFeatures\nfrom sport_activities_features.plot_data import PlotData\n\n# Read TCX file\ntcx_file = TCXFile()\nactivity = tcx_file.read_one_file("path_to_the_file")\n\n# Detect hills in data\nHill = HillIdentification(activity[\'altitudes\'], 30)\nHill.identify_hills()\nall_hills = Hill.return_hills()\n\n# Extract features from data\nTop = TopographicFeatures(all_hills)\nnum_hills = Top.num_of_hills()\navg_altitude = Top.avg_altitude_of_hills(activity[\'altitudes\'])\navg_ascent = Top.avg_ascent_of_hills(activity[\'altitudes\'])\ndistance_hills = Top.distance_of_hills(activity[\'positions\'])\nhills_share = Top.share_of_hills(distance_hills, activity[\'total_distance\'])\n```\n\n### Extraction of intervals\n```python\nimport sys\nsys.path.append(\'../\')\n\nfrom sport_activities_features.interval_identification import IntervalIdentificationByPower, IntervalIdentificationByHeartrate\nfrom sport_activities_features.tcx_manipulation import TCXFile\n\n# Reading the TCX file\ntcx_file = TCXFile()\nactivity = tcx_file.read_one_file("path_to_the_data")\n\n# Identifying the intervals in the activity by power\nIntervals = IntervalIdentificationByPower(activity["distances"], activity["timestamps"], activity["altitudes"], 70)\nIntervals.identify_intervals()\nall_intervals = Intervals.return_intervals()\n\n# Identifying the intervals in the activity by heart rate\nIntervals = IntervalIdentificationByHeartrate(activity["timestamps"], activity["altitudes"], activity["heartrates"])\nIntervals.identify_intervals()\nall_intervals = Intervals.return_intervals()\n```\n\n### Parsing of Historical weather data from an external service\n```python\nfrom sport_activities_features import WeatherIdentification\nfrom sport_activities_features import TCXFile\n\n# Read TCX file\ntcx_file = TCXFile()\ntcx_data = tcx_file.read_one_file("path_to_file")\n\n# Configure visual crossing api key\nvisual_crossing_api_key = "weather_api_key" # https://www.visualcrossing.com/weather-api\n\n# Explanation of elements - https://www.visualcrossing.com/resources/documentation/weather-data/weather-data-documentation/\nweather = WeatherIdentification(tcx_data[\'positions\'], tcx_data[\'timestamps\'], visual_crossing_api_key)\nweatherlist = weather.get_weather(time_delta=30)\ntcx_weather = weather.get_average_weather_data(timestamps=tcx_data[\'timestamps\'],weather=weatherlist)\n# Add weather to TCX data\ntcx_data.update({\'weather\':tcx_weather})\n```\n\nThe weather list is of the following type:\n```json\n     [\n        {\n            "temperature": 14.3,\n            "maximum_temperature": 14.3,\n            "minimum_temperature": 14.3,\n            "wind_chill": null,\n            "heat_index": null,\n            "solar_radiation": null,\n            "precipitation": 0.0,\n            "sea_level_pressure": 1021.6,\n            "snow_depth": null,\n            "wind_speed": 6.9,\n            "wind_direction": 129.0,\n            "wind_gust": null,\n            "visibility": 40.0,\n            "cloud_cover": 54.3,\n            "relative_humidity": 47.6,\n            "dew_point": 3.3,\n            "weather_type": "",\n            "conditions": "Partially cloudy",\n            "date": "2016-04-02T17:26:09+00:00",\n            "location": [\n                46.079871179535985,\n                14.738618675619364\n            ],\n            "index": 0\n        }, ...\n    ]\n```\n\n### Extraction of integral metrics\n```python\nimport sys\nsys.path.append(\'../\')\n\nfrom sport_activities_features.tcx_manipulation import TCXFile\n\n# Read TCX file\ntcx_file = TCXFile()\n\nintegral_metrics = tcx_file.extract_integral_metrics("path_to_the_file")\n\nprint(integral_metrics)\n\n```\n\n### Weather data extraction\n```python\nfrom sport_activities_features.weather_identification import WeatherIdentification\nfrom sport_activities_features.tcx_manipulation import TCXFile\n\n#read TCX file\ntcx_file = TCXFile()\ntcx_data = tcx_file.read_one_file("path_to_the_file")\n\n#configure visual crossing api key\nvisual_crossing_api_key = "API_KEY" # https://www.visualcrossing.com/weather-api\n\n#return weather objects\nweather = WeatherIdentification(tcx_data[\'positions\'], tcx_data[\'timestamps\'], visual_crossing_api_key)\nweatherlist = weather.get_weather()\n```\n\n### Using Overpass queried Open Street Map nodes\n```python\nimport overpy\nfrom sport_activities_features.overpy_node_manipulation import OverpyNodesReader\n\n# External service Overpass API (https://wiki.openstreetmap.org/wiki/Overpass_API) (can be self-hosted)\noverpass_api = "https://lz4.overpass-api.de/api/interpreter"\n\n# External service Open Elevation API (https://api.open-elevation.com/api/v1/lookup) (can be self-hosted)\nopen_elevation_api = "https://api.open-elevation.com/api/v1/lookup"\n\n# OSM Way (https://wiki.openstreetmap.org/wiki/Way)\nopen_street_map_way = 164477980\n\noverpass_api = overpy.Overpass(url=overpass_api)\n\n# Get an example Overpass way\nq = f"""(way({open_street_map_way});<;);out geom;"""\nquery = overpass_api.query(q)\n\n# Get nodes of an Overpass way\nnodes = query.ways[0].get_nodes(resolve_missing=True)\n\n# Extract basic data from nodes (you can, later on, use Hill Identification and Hill Data Extraction on them)\noverpy_reader = OverpyNodesReader(open_elevation_api=open_elevation_api)\n# Returns {\n#         \'positions\': positions, \'altitudes\': altitudes, \'distances\': distances, \'total_distance\': total_distance\n#         }\ndata = overpy_reader.read_nodes(nodes)\n```\n\n### Extraction of data inside the area\n```python\nimport numpy as np\nimport sys\nsys.path.append(\'../\')\n\nfrom sport_activities_features.area_identification import AreaIdentification\nfrom sport_activities_features.tcx_manipulation import TCXFile\n\n# Reading the TCX file.\ntcx_file = TCXFile()\nactivity = tcx_file.read_one_file(\'path_to_the_data\')\n\n# Converting the read data to arrays.\npositions = np.array([*activity[\'positions\']])\ndistances = np.array([*activity[\'distances\']])\ntimestamps = np.array([*activity[\'timestamps\']])\nheartrates = np.array([*activity[\'heartrates\']])\n\n# Area coordinates should be given in clockwise orientation in the form of 3D array (number_of_hulls, hull_coordinates, 2).\n# Holes in area are permitted.\narea_coordinates = np.array([[[10, 10], [10, 50], [50, 50], [50, 10]],\n                             [[19, 19], [19, 21], [21, 21], [21, 19]]])\n\n# Extracting the data inside the given area.\narea = AreaIdentification(positions, distances, timestamps, heartrates, area_coordinates)\narea.identify_points_in_area()\narea_data = area.extract_data_in_area()\n```\n\n### Identify interruptions\n```python\nfrom sport_activities_features.interruptions.interruption_processor import InterruptionProcessor\nfrom sport_activities_features.tcx_manipulation import TCXFile\n\n"""\nIdentify interruption events from a TCX or GPX file.\n"""\n\n# read TCX file (also works with GPX files)\ntcx_file = TCXFile()\ntcx_data = tcx_file.read_one_file("path_to_the_data")\n\n"""\nTime interval = time before and after the start of an event\nMin speed = Threshold speed to trigger an event/interruption (trigger when under min_speed)\noverpass_api_url = Set to something self-hosted, or use a public instance from https://wiki.openstreetmap.org/wiki/Overpass_API\n"""\ninterruptionProcessor = InterruptionProcessor(time_interval=60, min_speed=2,\n                                              overpass_api_url="url_to_overpass_api")\n\n"""\nIf classify is set to true, also discover if interruptions are close to intersections. Returns a list of [ExerciseEvent]\n"""\nevents = interruptionProcessor.events(tcx_data, True)\n```\n\n### Overpy (Overpass API) node manipulation\nGenerate TCXFile parsed like data object from overpy.Node objects\n```python\nimport overpy\nfrom sport_activities_features.overpy_node_manipulation import OverpyNodesReader\n\n\n# External service Overpass API (https://wiki.openstreetmap.org/wiki/Overpass_API) (can be self-hosted)\noverpass_api = "https://lz4.overpass-api.de/api/interpreter"\n\n# External service Open Elevation API (https://api.open-elevation.com/api/v1/lookup) (can be self-hosted)\nopen_elevation_api = "https://api.open-elevation.com/api/v1/lookup"\n\n# OSM Way (https://wiki.openstreetmap.org/wiki/Way)\nopen_street_map_way = 164477980\n\noverpass_api = overpy.Overpass(url=overpass_api)\n\n# Get an example Overpass way\nq = f"""(way({open_street_map_way});<;);out geom;"""\nquery = overpass_api.query(q)\n\n# Get nodes of an Overpass way\nnodes = query.ways[0].get_nodes(resolve_missing=True)\n\n# Extract basic data from nodes (you can, later on, use Hill Identification and Hill Data Extraction on them)\noverpy_reader = OverpyNodesReader(open_elevation_api=open_elevation_api)\n# Returns {\n#         \'positions\': positions, \'altitudes\': altitudes, \'distances\': distances, \'total_distance\': total_distance\n#         }\ndata = overpy_reader.read_nodes(nodes)\n```\n### Missing elevation data extraction\n```python\nfrom sport_activities_features import ElevationIdentification\nfrom sport_activities_features import TCXFile\n\ntcx_file = TCXFile()\ntcx_data = tcx_file.read_one_file(\'path_to_file\')\n\nelevations = ElevationIdentification(tcx_data[\'positions\'])\n"""Adds tcx_data[\'elevation\'] = eg. [124, 21, 412] for each position"""\ntcx_data.update({\'elevations\':elevations})\n```\n\n### Example of a visualization of the area detection\n\n![Area Figure](https://i.imgur.com/Iz8Ga3B.png)\n\n### Example of visualization of dead-end identification\n![Dead End Figure](https://imgur.com/LgZzCFS.png)\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n\n## Cite us\n\nI. Jr. Fister, L. Lukač, A. Rajšp, I. Fister, L. Pečnik and D. Fister, "[A minimalistic toolbox for extracting features from sport activity files](http://iztok-jr-fister.eu/static/publications/294.pdf)", 2021 IEEE 25th International Conference on Intelligent Engineering Systems (INES), 2021, pp. 121-126, doi: [10.1109/INES52918.2021.9512927](http://dx.doi.org/10.1109/INES52918.2021.9512927).\n\n## Contributors ✨\n\nThanks go to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center"><a href="https://github.com/alenrajsp"><img src="https://avatars.githubusercontent.com/u/27721714?v=4?s=100" width="100px;" alt="alenrajsp"/><br /><sub><b>alenrajsp</b></sub></a><br /><a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=alenrajsp" title="Code">💻</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=alenrajsp" title="Tests">⚠️</a> <a href="#example-alenrajsp" title="Examples">💡</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=alenrajsp" title="Documentation">📖</a> <a href="#ideas-alenrajsp" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/firefly-cpp/sport-activities-features/issues?q=author%3Aalenrajsp" title="Bug reports">🐛</a> <a href="#maintenance-alenrajsp" title="Maintenance">🚧</a></td>\n      <td align="center"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=firefly-cpp" title="Code">💻</a> <a href="https://github.com/firefly-cpp/sport-activities-features/issues?q=author%3Afirefly-cpp" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=firefly-cpp" title="Tests">⚠️</a> <a href="#example-firefly-cpp" title="Examples">💡</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=firefly-cpp" title="Documentation">📖</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑\u200d🏫</a> <a href="#platform-firefly-cpp" title="Packaging/porting to new platform">📦</a> <a href="#maintenance-firefly-cpp" title="Maintenance">🚧</a> <a href="#data-firefly-cpp" title="Data">🔣</a></td>\n      <td align="center"><a href="https://github.com/luckyLukac"><img src="https://avatars.githubusercontent.com/u/73126820?v=4?s=100" width="100px;" alt="luckyLukac"/><br /><sub><b>luckyLukac</b></sub></a><br /><a href="#ideas-luckyLukac" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=luckyLukac" title="Code">💻</a> <a href="https://github.com/firefly-cpp/sport-activities-features/issues?q=author%3AluckyLukac" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=luckyLukac" title="Tests">⚠️</a> <a href="#example-luckyLukac" title="Examples">💡</a></td>\n      <td align="center"><a href="https://github.com/rhododendrom"><img src="https://avatars.githubusercontent.com/u/3198785?v=4?s=100" width="100px;" alt="rhododendrom"/><br /><sub><b>rhododendrom</b></sub></a><br /><a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=rhododendrom" title="Code">💻</a> <a href="#design-rhododendrom" title="Design">🎨</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=rhododendrom" title="Documentation">📖</a> <a href="#ideas-rhododendrom" title="Ideas, Planning, & Feedback">🤔</a></td>\n      <td align="center"><a href="https://github.com/lukapecnik"><img src="https://avatars.githubusercontent.com/u/23029992?v=4?s=100" width="100px;" alt="Luka Pečnik"/><br /><sub><b>Luka Pečnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=lukapecnik" title="Code">💻</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=lukapecnik" title="Documentation">📖</a> <a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=lukapecnik" title="Tests">⚠️</a> <a href="https://github.com/firefly-cpp/sport-activities-features/issues?q=author%3Alukapecnik" title="Bug reports">🐛</a></td>\n      <td align="center"><a href="https://github.com/spelap"><img src="https://avatars.githubusercontent.com/u/19300429?v=4?s=100" width="100px;" alt="spelap"/><br /><sub><b>spelap</b></sub></a><br /><a href="https://github.com/firefly-cpp/sport-activities-features/commits?author=spelap" title="Code">💻</a></td>\n      <td align="center"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="#maintenance-carlosal1015" title="Maintenance">🚧</a></td>\n    </tr>\n    <tr>\n      <td align="center"><a href="https://github.com/KoprivcLuka"><img src="https://avatars.githubusercontent.com/u/45632449?v=4?s=100" width="100px;" alt="Luka Koprivc"/><br /><sub><b>Luka Koprivc</b></sub></a><br /><a href="https://github.com/firefly-cpp/sport-activities-features/issues?q=author%3AKoprivcLuka" title="Bug reports">🐛</a></td>\n      <td align="center"><a href="https://github.com/garyjellyarms"><img src="https://avatars.githubusercontent.com/u/79595804?v=4?s=100" width="100px;" alt="Nejc Graj"/><br /><sub><b>Nejc Graj</b></sub></a><br /><a href="https://github.com/firefly-cpp/sport-activities-features/issues?q=author%3Agaryjellyarms" title="Bug reports">🐛</a></td>\n      <td align="center"><a href="https://github.com/Mtvrt123"><img src="https://avatars.githubusercontent.com/u/50879568?v=4?s=100" width="100px;" alt="MlinaricNejc"/><br /><sub><b>MlinaricNejc</b></sub></a><br /><a href="https://github.com/firefly-cpp/sport-activities-features/issues?q=author%3AMtvrt123" title="Bug reports">🐛</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind are welcome!\n',
     'author': 'Iztok Fister Jr.',
     'author_email': 'iztok@iztok-jr-fister.eu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/firefly-cpp/sport-activities-features',
```

### Comparing `sport-activities-features-0.3.8/PKG-INFO` & `sport-activities-features-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sport-activities-features
-Version: 0.3.8
+Version: 0.3.9
 Summary: A minimalistic toolbox for extracting features from sport activity files
 Home-page: https://github.com/firefly-cpp/sport-activities-features
 License: MIT
 Keywords: computational intelligence,data mining,datasets,gpx,optimization,sport activities,tcx
 Author: Iztok Fister Jr.
 Author-email: iztok@iztok-jr-fister.eu
 Requires-Python: >=3.9.0,<4.0.0
@@ -18,15 +18,15 @@
 Requires-Dist: gpxpy (>=1.4.2,<2.0.0)
 Requires-Dist: matplotlib (>=3.3.3,<4.0.0)
 Requires-Dist: niaaml (>=1.1.10,<2.0.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Requires-Dist: overpy (>=0.6,<0.7)
 Requires-Dist: pandas
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: tcxreader (>=0.4.1,<0.5.0)
+Requires-Dist: tcxreader (>=0.4.4,<0.5.0)
 Project-URL: Repository, https://github.com/firefly-cpp/sport-activities-features
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img width="200" src="https://raw.githubusercontent.com/firefly-cpp/sport-activities-features/main/.github/logo/sport_activities.png">
 </p>
```

