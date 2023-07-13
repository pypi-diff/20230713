# Comparing `tmp/metar-1.8.0.tar.gz` & `tmp/metar-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metar-1.8.0.tar", last modified: Tue Dec 29 02:33:46 2020, max compression
+gzip compressed data, was "metar-1.9.0.tar", last modified: Mon Jan  3 02:11:49 2022, max compression
```

## Comparing `metar-1.8.0.tar` & `metar-1.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 akrherz  (43306) domain users   (101)        0 2020-12-29 02:33:46.385093 metar-1.8.0/
--rw-r--r--   0 akrherz  (43306) domain users   (101)     8817 2020-12-29 02:33:33.000000 metar-1.8.0/CHANGELOG.md
--rw-rw-r--   0 akrherz  (43306) domain users   (101)     1088 2018-09-20 14:56:51.000000 metar-1.8.0/LICENSE
--rw-rw-r--   0 akrherz  (43306) domain users   (101)       83 2018-08-21 01:18:42.000000 metar-1.8.0/MANIFEST.in
--rw-r--r--   0 akrherz  (43306) domain users   (101)     1744 2020-12-29 02:33:46.385093 metar-1.8.0/PKG-INFO
--rw-r--r--   0 akrherz  (43306) domain users   (101)     6505 2020-12-07 19:28:03.000000 metar-1.8.0/README.md
-drwxr-xr-x   0 akrherz  (43306) domain users   (101)        0 2020-12-29 02:33:46.382093 metar-1.8.0/metar/
--rw-r--r--   0 akrherz  (43306) domain users   (101)    16595 2020-12-07 19:28:03.000000 metar-1.8.0/metar/Datatypes.py
--rw-r--r--   0 akrherz  (43306) domain users   (101)    45273 2020-12-15 18:09:15.000000 metar-1.8.0/metar/Metar.py
--rw-r--r--   0 akrherz  (43306) domain users   (101)     1210 2020-12-07 14:34:47.000000 metar-1.8.0/metar/Station.py
--rw-r--r--   0 akrherz  (43306) domain users   (101)     2618 2020-12-29 02:33:33.000000 metar-1.8.0/metar/__init__.py
--rw-rw-r--   0 akrherz  (43306) domain users   (101)   525591 2017-07-18 15:22:06.000000 metar-1.8.0/metar/nsd_cccc.txt
-drwxr-xr-x   0 akrherz  (43306) domain users   (101)        0 2020-12-29 02:33:46.383093 metar-1.8.0/metar.egg-info/
--rw-rw-r--   0 akrherz  (43306) domain users   (101)     1744 2020-12-29 02:33:46.000000 metar-1.8.0/metar.egg-info/PKG-INFO
--rw-rw-r--   0 akrherz  (43306) domain users   (101)      471 2020-12-29 02:33:46.000000 metar-1.8.0/metar.egg-info/SOURCES.txt
--rw-rw-r--   0 akrherz  (43306) domain users   (101)        1 2020-12-29 02:33:46.000000 metar-1.8.0/metar.egg-info/dependency_links.txt
--rw-rw-r--   0 akrherz  (43306) domain users   (101)       15 2020-12-29 02:33:46.000000 metar-1.8.0/metar.egg-info/requires.txt
--rw-rw-r--   0 akrherz  (43306) domain users   (101)        6 2020-12-29 02:33:46.000000 metar-1.8.0/metar.egg-info/top_level.txt
--rw-r--r--   0 akrherz  (43306) domain users   (101)      141 2020-12-29 02:33:46.385093 metar-1.8.0/setup.cfg
--rwxr-xr-x   0 akrherz  (43306) domain users   (101)     1973 2020-12-07 14:34:47.000000 metar-1.8.0/setup.py
-drwxr-xr-x   0 akrherz  (43306) domain users   (101)        0 2020-12-29 02:33:46.384093 metar-1.8.0/test/
--rw-rw-r--   0 akrherz  (43306) domain users   (101)     1663 2018-10-02 15:22:23.000000 metar-1.8.0/test/test_direction.py
--rw-r--r--   0 akrherz  (43306) domain users   (101)     3284 2020-12-07 14:34:47.000000 metar-1.8.0/test/test_distance.py
--rw-r--r--   0 akrherz  (43306) domain users   (101)    23273 2020-12-15 18:09:15.000000 metar-1.8.0/test/test_metar.py
--rw-rw-r--   0 akrherz  (43306) domain users   (101)      290 2018-10-02 15:22:23.000000 metar-1.8.0/test/test_precipitation.py
--rw-rw-r--   0 akrherz  (43306) domain users   (101)     2106 2018-10-02 15:22:23.000000 metar-1.8.0/test/test_pressure.py
--rw-rw-r--   0 akrherz  (43306) domain users   (101)     2220 2018-10-02 15:22:23.000000 metar-1.8.0/test/test_speed.py
--rw-r--r--   0 akrherz  (43306) domain users   (101)      178 2020-12-07 14:34:47.000000 metar-1.8.0/test/test_station.py
--rw-rw-r--   0 akrherz  (43306) domain users   (101)     2158 2018-10-02 15:22:23.000000 metar-1.8.0/test/test_temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 02:11:49.631011 metar-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     9849 2022-01-03 02:11:37.000000 metar-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-01-03 02:11:37.000000 metar-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-01-03 02:11:37.000000 metar-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-01-03 02:11:49.631011 metar-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6434 2022-01-03 02:11:37.000000 metar-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 02:11:49.631011 metar-1.9.0/metar/
+-rw-r--r--   0 runner    (1001) docker     (121)    15900 2022-01-03 02:11:37.000000 metar-1.9.0/metar/Datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45852 2022-01-03 02:11:37.000000 metar-1.9.0/metar/Metar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-01-03 02:11:37.000000 metar-1.9.0/metar/Station.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2618 2022-01-03 02:11:37.000000 metar-1.9.0/metar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   525591 2022-01-03 02:11:37.000000 metar-1.9.0/metar/nsd_cccc.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 02:11:49.631011 metar-1.9.0/metar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-01-03 02:11:49.000000 metar-1.9.0/metar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-01-03 02:11:49.000000 metar-1.9.0/metar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 02:11:49.000000 metar-1.9.0/metar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-03 02:11:49.000000 metar-1.9.0/metar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-03 02:11:49.000000 metar-1.9.0/metar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-01-03 02:11:49.635011 metar-1.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1973 2022-01-03 02:11:37.000000 metar-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 02:11:49.631011 metar-1.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-01-03 02:11:37.000000 metar-1.9.0/test/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-01-03 02:11:37.000000 metar-1.9.0/test/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24847 2022-01-03 02:11:37.000000 metar-1.9.0/test/test_metar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-01-03 02:11:37.000000 metar-1.9.0/test/test_precipitation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-01-03 02:11:37.000000 metar-1.9.0/test/test_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2220 2022-01-03 02:11:37.000000 metar-1.9.0/test/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-01-03 02:11:37.000000 metar-1.9.0/test/test_station.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-01-03 02:11:37.000000 metar-1.9.0/test/test_temperature.py
```

### Comparing `metar-1.8.0/CHANGELOG.md` & `metar-1.9.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 Change Log
 ==========
 
+metar-1.9.0 (2 January 2022)
+
+This release is mostly a maintanence release with one small API break that
+was unused within this library.
+
+- [#110](https://github.com/python-metar/python-metar/issues/110) *API Break*,
+Remove unused/broken position.getdistance API.
+- [#139](https://github.com/python-metar/python-metar/issues/139) Defaults wind
+speed units to knots for sites with US identifiers and meters per second for
+all others.
+- [#147](https://github.com/python-metar/python-metar/issues/147) Allow parsing
+of METARs with wind and visibility after the sky condition group.
+- [#148](https://github.com/python-metar/python-metar/issues/148) Parse sea
+level pressure (SLP) when found after the altimeter value.
+- [#24](https://github.com/python-metar/python-metar/issues/24) Fix parsing
+of runway identifier in windshear group.
+- [#136](https://github.com/python-metar/python-metar/issues/136) Allow for
+one digit temperatures.
+- [#156](https://github.com/python-metar/python-metar/issues/156) Rename
+`master` branch to `main`.
+
 metar-1.8.0 (28 December 2020)
 ------------------------------
 
 This release is a bug fix and enhancement release with no known API breakages. The highlights include:
 
 - [#84](https://github.com/python-metar/python-metar/issues/84) handle METAR strings that end with `=`.
 - [#121](https://github.com/python-metar/python-metar/issues/121) allow METAR with `COR AUTO` to be parsed.
```

### Comparing `metar-1.8.0/LICENSE` & `metar-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metar-1.8.0/PKG-INFO` & `metar-1.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: metar
-Version: 1.8.0
+Version: 1.9.0
 Summary: Metar - a package to parse METAR-coded weather reports
 Home-page: https://github.com/python-metar/python-metar
 Author: Tom Pollard
 Author-email: pollard@alum.mit.edu
 License: BSD
-Description: 
-        Metar is a python package for interpreting METAR and SPECI weather reports.
-        
-        METAR is an international format for reporting weather observations.
-        The standard specification for the METAR and SPECI codes is given
-        in the WMO Manual on Codes, vol I.1, Part A (WMO-306 I.i.A).  US
-        conventions for METAR/SPECI reports are described in chapter 12 of
-        the Federal Meteorological Handbook No.1. (FMC-H1-2017), issued by
-        NOAA.  See http://www.ofcm.gov/publications/fmh/FMH1/FMH1.pdf
-        
-        This module extracts the data recorded in the main-body groups of
-        reports that follow the WMO spec or the US conventions, except for
-        the runway state and trend groups, which are parsed but ignored.
-        The most useful remark groups defined in the US spec are parsed,
-        as well, such as the cumulative precipitation, min/max temperature,
-        peak wind and sea-level pressure groups.  No other regional conventions
-        are formally supported, but a large number of variant formats found
-        in international reports are accepted.
 Platform: Python 2.5 and later.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
+License-File: LICENSE
+
+
+Metar is a python package for interpreting METAR and SPECI weather reports.
+
+METAR is an international format for reporting weather observations.
+The standard specification for the METAR and SPECI codes is given
+in the WMO Manual on Codes, vol I.1, Part A (WMO-306 I.i.A).  US
+conventions for METAR/SPECI reports are described in chapter 12 of
+the Federal Meteorological Handbook No.1. (FMC-H1-2017), issued by
+NOAA.  See http://www.ofcm.gov/publications/fmh/FMH1/FMH1.pdf
+
+This module extracts the data recorded in the main-body groups of
+reports that follow the WMO spec or the US conventions, except for
+the runway state and trend groups, which are parsed but ignored.
+The most useful remark groups defined in the US spec are parsed,
+as well, such as the cumulative precipitation, min/max temperature,
+peak wind and sea-level pressure groups.  No other regional conventions
+are formally supported, but a large number of variant formats found
+in international reports are accepted.
+
```

### Comparing `metar-1.8.0/README.md` & `metar-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 --------------------
 
 The [Federal Meteorological Handbook No.1. (FMC-H1-2017)](http://www.ofcm.gov/publications/fmh/FMH1/FMH1.pdf) describes the U.S. standards for METAR. The [World Meteorological Organization (WMO) Manual on Codes](http://www.wmo.int/pages/prog/www/WMOCodes.html), vol I.1, Part A (WMO-306 I.i.A) is another good reference.
 
 Author
 ------
 
-The `python-metar` library was orignally authored by [Tom Pollard](https://github.com/tomp) in January 2005, and is now maintained by contributers on Github.
+The `python-metar` library was orignally authored by [Tom Pollard](https://github.com/tomp) in January 2005, and is now maintained by contributors on Github.
 
 Installation
 ------------------------------------------------------------------------
 
 Install this package in the usual way,
 
     python setup.py install
@@ -130,16 +130,15 @@
 METAR: METAR KEWR 111851Z VRB03G19KT 2SM R04R/3000VP6000FT TSRA BR FEW015 BKN040CB BKN065 OVC200 22/22 A2987 RMK AO2 PK WND 29028/1817 WSHFT 1812 TSB05RAB22 SLP114 FRQ LTGICCCCG TS OHD AND NW -N-E MOV NE P0013 T02270215
 >>>>
 ```
 
 Tests
 ------------------------------------------------------------------------
 
-The library is tested against Python 2.6, Python 2.7, Python 3.2, Python 3.3,
-Python 3.4, Python 3.5, and Python 3.6. A [tox](https://tox.readthedocs.io/en/latest/)
+The library is tested against Python 3.7-3.10. A [tox](https://tox.readthedocs.io/en/latest/)
 configuration file is included to easily run tests against each of these
 environments. To run tests against all environments, install tox and run:
 
     >>> tox
 
 To run against a specific environment, use the `-e` flag:
```

### Comparing `metar-1.8.0/metar/Datatypes.py` & `metar-1.9.0/metar/Datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,32 +465,14 @@
     def __init__(self, latitude=None, longitude=None):
         self.latitude = latitude
         self.longitude = longitude
 
     def __str__(self):
         return self.string()
 
-    def getdistance(self, position2):
-        """
-        Calculate the great-circle distance to another location using the Haversine
-        formula.  See <http://www.movable-type.co.uk/scripts/LatLong.html>
-        and <http://mathforum.org/library/drmath/sets/select/dm_lat_long.html>
-        """
-        earth_radius = 637100.0
-        lat1 = self.latitude
-        long1 = self.longitude
-        lat2 = position2.latitude
-        long2 = position2.longitude
-        a = (sin(0.5(lat2 - lat1))) ** 2 + cos(lat1) * cos(lat2) * (sin(
-            0.5 * (long2 - long1)) ** 2
-        )
-        c = 2.0 * atan(sqrt(a) * sqrt(1.0 - a))
-        d = distance(earth_radius * c, "M")
-        return d
-
     def getdirection(self, position2):
         """
         Calculate the initial direction to another location.  (The direction
         typically changes as you trace the great circle path to that location.)
         See <http://www.movable-type.co.uk/scripts/LatLong.html>.
         """
         lat1 = self.latitude
```

### Comparing `metar-1.8.0/metar/Metar.py` & `metar-1.9.0/metar/Metar.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 SKY_RE = re.compile(
     r"""^(?P<cover>VV|CLR|SKC|SCK|NSC|NCD|BKN|SCT|FEW|[O0]VC|///)
         (?P<height>[\dO]{2,4}|///)?
         (?P<cloud>([A-Z][A-Z]+|///))?\s+""",
     re.VERBOSE,
 )
 TEMP_RE = re.compile(
-    r"""^(?P<temp>(M|-)?\d+|//|XX|MM)/
-        (?P<dewpt>(M|-)?\d+|//|XX|MM)?\s+""",
+    r"""^(?P<temp>(M|-)?\d{1,2}|//|XX|MM)/
+        (?P<dewpt>(M|-)?\d{1,2}|//|XX|MM)?\s+""",
     re.VERBOSE,
 )
 PRESS_RE = re.compile(
     r"""^(?P<unit>A|Q|QNH)?
         (?P<press>[\dO]{3,4}|////)
         (?P<unit2>INS)?\s+""",
     re.VERBOSE,
@@ -98,27 +98,28 @@
 RECENT_RE = re.compile(
     r"""^RE(?P<desc>MI|PR|BC|DR|BL|SH|TS|FZ)?
         (?P<prec>(DZ|RA|SN|SG|IC|PL|GR|GS|UP)*)?
         (?P<obsc>BR|FG|FU|VA|DU|SA|HZ|PY)?
         (?P<other>PO|SQ|FC|SS|DS)?\s+""",
     re.VERBOSE,
 )
-WINDSHEAR_RE = re.compile(r"^(WS\s+)?(ALL\s+RWY|RWY(?P<name>\d\d(RR?|L?|C)?))\s+")
+WINDSHEAR_RE = re.compile(r"^(WS\s+)?(ALL\s+RWY|R(WY)?(?P<name>\d\d(RR?|L?|C)?))\s+")
 COLOR_RE = re.compile(
     r"""^(BLACK)?(BLU|GRN|WHT|RED)\+?
                         (/?(BLACK)?(BLU|GRN|WHT|RED)\+?)*\s*""",
     re.VERBOSE,
 )
 RUNWAYSTATE_RE = re.compile(
-    r"""((?P<name>\d\d) | R(?P<namenew>\d\d)(RR?|LL?|C)?/?)
+    r"""((?P<snoclo>R/SNOCLO) |
+        ((?P<name>\d\d) | R(?P<namenew>\d\d)(RR?|LL?|C)?/?)
         ((?P<special> SNOCLO|CLRD(\d\d|//)) |
         (?P<deposit>(\d|/))
         (?P<extent>(\d|/))
         (?P<depth>(\d\d|//))
-        (?P<friction>(\d\d|//)))\s+""",
+        (?P<friction>(\d\d|//))))\s+""",
     re.VERBOSE,
 )
 TREND_RE = re.compile(r"^(?P<trend>TEMPO|BECMG|FCST|NOSIG)\s+")
 
 TRENDTIME_RE = re.compile(r"(?P<when>(FM|TL|AT))(?P<hour>\d\d)(?P<min>\d\d)\s+")
 
 REMARK_RE = re.compile(r"^(RMKS?|NOSPECI|NOSIG)\s+")
@@ -614,14 +615,22 @@
             wind_dir_to        [int]
         """
         wind_dir = d["dir"].replace("O", "0")
         if wind_dir != "VRB" and wind_dir != "///" and wind_dir != "MMM":
             self.wind_dir = direction(wind_dir)
         wind_speed = d["speed"].replace("O", "0")
         units = d["units"]
+        # Ambiguous METAR when no wind speed units are provided
+        if units is None and self.station_id is not None:
+            # Assume US METAR sites are reporting in KT
+            if len(self.station_id) == 3 or self.station_id.startswith("K"):
+                units = "KT"
+        # If units are still None, default to MPS
+        if units is None:
+            units = "MPS"
         if units == "KTS" or units == "K" or units == "T" or units == "LT":
             units = "KT"
         if wind_speed.startswith("P"):
             self.wind_speed = speed(wind_speed[1:], units, ">")
         elif not MISSING_RE.match(wind_speed):
             self.wind_speed = speed(wind_speed, units)
         if d["gust"]:
@@ -1038,16 +1047,19 @@
         (TIME_RE, _handleTime, False),
         (MODIFIER_RE, _handleModifier, False),
         (WIND_RE, _handleWind, False),
         (VISIBILITY_RE, _handleVisibility, True),
         (RUNWAY_RE, _handleRunway, True),
         (WEATHER_RE, _handleWeather, True),
         (SKY_RE, _handleSky, True),
+        (WIND_RE, _handleWind, False),
+        (VISIBILITY_RE, _handleVisibility, True),
         (TEMP_RE, _handleTemp, False),
         (PRESS_RE, _handlePressure, True),
+        (SEALVL_PRESS_RE, _handleSealvlPressRemark, False),
         (RECENT_RE, _handleRecent, True),
         (WINDSHEAR_RE, _handleWindShear, True),
         (COLOR_RE, _handleColor, True),
         (RUNWAYSTATE_RE, _handleRunwayState, True),
         (TREND_RE, _handleTrend, True),
         (REMARK_RE, _startRemarks, False),
     ]
```

### Comparing `metar-1.8.0/metar/Station.py` & `metar-1.9.0/metar/Station.py`

 * *Files identical despite different names*

### Comparing `metar-1.8.0/metar/__init__.py` & `metar-1.9.0/metar/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 where <cycle> is a 2-digit cycle number (e.g., "00", "05" or "23").
 """
 
 __author__ = "Tom Pollard"
 
 __email__ = "pollard@alum.mit.edu"
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 __doc__ = """metar v%s (c) 2009, %s
 
 Metar is a python package that interprets coded METAR and SPECI weather reports.
 
 Please e-mail bug reports to: %s""" % (
     __version__,
```

### Comparing `metar-1.8.0/metar/nsd_cccc.txt` & `metar-1.9.0/metar/nsd_cccc.txt`

 * *Files identical despite different names*

### Comparing `metar-1.8.0/metar.egg-info/PKG-INFO` & `metar-1.9.0/metar.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: metar
-Version: 1.8.0
+Version: 1.9.0
 Summary: Metar - a package to parse METAR-coded weather reports
 Home-page: https://github.com/python-metar/python-metar
 Author: Tom Pollard
 Author-email: pollard@alum.mit.edu
 License: BSD
-Description: 
-        Metar is a python package for interpreting METAR and SPECI weather reports.
-        
-        METAR is an international format for reporting weather observations.
-        The standard specification for the METAR and SPECI codes is given
-        in the WMO Manual on Codes, vol I.1, Part A (WMO-306 I.i.A).  US
-        conventions for METAR/SPECI reports are described in chapter 12 of
-        the Federal Meteorological Handbook No.1. (FMC-H1-2017), issued by
-        NOAA.  See http://www.ofcm.gov/publications/fmh/FMH1/FMH1.pdf
-        
-        This module extracts the data recorded in the main-body groups of
-        reports that follow the WMO spec or the US conventions, except for
-        the runway state and trend groups, which are parsed but ignored.
-        The most useful remark groups defined in the US spec are parsed,
-        as well, such as the cumulative precipitation, min/max temperature,
-        peak wind and sea-level pressure groups.  No other regional conventions
-        are formally supported, but a large number of variant formats found
-        in international reports are accepted.
 Platform: Python 2.5 and later.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
+License-File: LICENSE
+
+
+Metar is a python package for interpreting METAR and SPECI weather reports.
+
+METAR is an international format for reporting weather observations.
+The standard specification for the METAR and SPECI codes is given
+in the WMO Manual on Codes, vol I.1, Part A (WMO-306 I.i.A).  US
+conventions for METAR/SPECI reports are described in chapter 12 of
+the Federal Meteorological Handbook No.1. (FMC-H1-2017), issued by
+NOAA.  See http://www.ofcm.gov/publications/fmh/FMH1/FMH1.pdf
+
+This module extracts the data recorded in the main-body groups of
+reports that follow the WMO spec or the US conventions, except for
+the runway state and trend groups, which are parsed but ignored.
+The most useful remark groups defined in the US spec are parsed,
+as well, such as the cumulative precipitation, min/max temperature,
+peak wind and sea-level pressure groups.  No other regional conventions
+are formally supported, but a large number of variant formats found
+in international reports are accepted.
+
```

### Comparing `metar-1.8.0/setup.py` & `metar-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `metar-1.8.0/test/test_direction.py` & `metar-1.9.0/test/test_direction.py`

 * *Files identical despite different names*

### Comparing `metar-1.8.0/test/test_distance.py` & `metar-1.9.0/test/test_distance.py`

 * *Files identical despite different names*

### Comparing `metar-1.8.0/test/test_metar.py` & `metar-1.9.0/test/test_metar.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,15 +363,16 @@
     assert report("OOOOOKT").wind_speed.value() == 0
     assert report("OOOOOKT").wind() == "calm"
 
     assert report("09010K").wind_speed.string() == "10 knots"
     assert report("09010T").wind_speed.string() == "10 knots"
     assert report("09010LT").wind_speed.string() == "10 knots"
     assert report("09010KTS").wind_speed.string() == "10 knots"
-    assert report("09010").wind_speed.string() == "10 mps"
+    # Default wind speed units are knots since US station_id is used
+    assert report("09010").wind_speed.string() == "10 knots"
 
     assert report("VRBOOK").wind_speed.value() == 0
     assert report("VRBOOK").wind() == "calm"
 
     assert report("///00KT").wind() == "calm"
     assert report("/////KT").wind() == "missing"
     assert report("000//KT").wind() == "missing"
@@ -386,14 +387,20 @@
     assert report("MMMMMKT").wind() == "missing"
     assert report("000MMKT").wind() == "missing"
     assert report("MMMMM").wind() == "missing"
     assert report("MMMMMGMMKT").wind() == "missing"
     assert report("MMMMMG01KT").wind() == "missing"
 
 
+def test_issue139_no_wind_unit():
+    """Check the default wind speed units for international sites."""
+    report = Metar.Metar("CXXX 101651Z 09010G20")
+    assert report.wind_speed.string() == "10 mps"
+
+
 def test_issue51_strict():
     """Check that setting strict=False prevents a ParserError"""
     with warnings.catch_warnings(record=True) as w:
         report = Metar.Metar(sta_time + "90010KT", strict=False)
     assert len(w) == 1
     assert report.wind_speed is None
 
@@ -545,14 +552,19 @@
 
     assert report("09690692 27550591").temp.value() == -1.0
     assert report("09690692 27550591").remarks() == ""
 
     assert report("09SNOCLO").remarks() == ""
     assert report("09CLRD//").remarks() == ""
 
+    assert report("R/SNOCLO").remarks() == ""
+    assert report("R09/CLRD//").remarks() == ""
+
+    assert report("R01R/SNOCLO ").remarks() == ""
+
 
 def test_300_parseTrend():
     """Check parsing of trend forecasts."""
 
     def report(trend_group, remarks=""):
         """(Macro)
         Return Metar object for a report containing the given trend
@@ -642,7 +654,51 @@
     code = (
         "METAR KADW 252356Z COR AUTO 10008KT 10SM CLR 19/11 A2986 "
         "RMK AO2 SLP117 T01880111 10230 20188 50004 $ COR 0007="
     )
     m = Metar.Metar(code, year=2019)
 
     assert m.mod == 'COR AUTO'
+
+
+def test_slp_outside_remarks():
+    """
+    Test parsing of a METAR that lists sea level pressure after the altimeter
+    setting instead of in the remarks.
+    """
+
+    code = (
+        "METAR KCOF 191855Z 18015G22KT 7SM FEW049 SCT300 28/18 A3001 SLP162 "
+        "RMK WND DATA ESTMD"
+    )
+    m = Metar.Metar(code, year=2007)
+    m.press_sea_level.value() == 1016.2
+
+def test_wind_after_sky():
+    """
+    Test parsing of a METAR that lists wind after the sky groups
+    """
+
+    code = (
+        "METAR KCOF 281855Z FEW029TCU FEW040 SCT250 09008KT 7SM 32/25 A3008 "
+        "RMK VIRGA E TCU NE AND DSNT ALQDS SLP186"
+    )
+    m = Metar.Metar(code, year=2007)
+
+    assert m.wind_dir.value() == 90
+    assert m.wind_speed.value() == 8
+
+def test_issue136_temperature():
+    raisesParserError("METAR EDDM 022150Z 26006KT CAVOK 201/16")
+
+
+def test_windshear_runway_identifier():
+    code = "METAR EDDH 300720Z WS R23"
+    m = Metar.Metar(code)
+    assert len(m.windshear) == 1
+    assert m.windshear[0] == "23"
+
+    code = "METAR EFHK 151350Z WS RWY22L"
+    m = Metar.Metar(code)
+    assert len(m.windshear) == 1
+    assert m.windshear[0] == "22L"
+
```

### Comparing `metar-1.8.0/test/test_pressure.py` & `metar-1.9.0/test/test_pressure.py`

 * *Files identical despite different names*

### Comparing `metar-1.8.0/test/test_speed.py` & `metar-1.9.0/test/test_speed.py`

 * *Files identical despite different names*

### Comparing `metar-1.8.0/test/test_temperature.py` & `metar-1.9.0/test/test_temperature.py`

 * *Files identical despite different names*

