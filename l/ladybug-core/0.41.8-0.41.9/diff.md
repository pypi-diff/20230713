# Comparing `tmp/ladybug-core-0.41.8.tar.gz` & `tmp/ladybug-core-0.41.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-core-0.41.8.tar", last modified: Tue Jan 17 01:59:59 2023, max compression
+gzip compressed data, was "dist/ladybug-core-0.41.9.tar", last modified: Sat Jan 21 20:32:55 2023, max compression
```

## Comparing `ladybug-core-0.41.8.tar` & `ladybug-core-0.41.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51971 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/_datacollectionbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/analysisperiod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/cli/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/cli/setconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/climatezone.py
--rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    67221 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datacollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datacollectionimmutable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug/datatype/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/area.py
--rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/energyflux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/energyintensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/fraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/illuminance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/luminance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/massflowrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/power.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/rvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/specificenergy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/temperaturedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/temperaturetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/thermalcondition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/uvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/volumeflowrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datatype/volumeflowrateintensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/datautil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/ddy.py
--rw-r--r--   0 runner    (1001) docker     (123)    58123 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/designday.py
--rw-r--r--   0 runner    (1001) docker     (123)    18177 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)    85289 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/epw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/futil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/graphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/header.py
--rw-r--r--   0 runner    (1001) docker     (123)    25056 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/hourlyplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    84125 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/logutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    50531 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/monthlychart.py
--rw-r--r--   0 runner    (1001) docker     (123)    42331 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/psychchart.py
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/psychrometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/rootfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    55789 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/skymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/solarenvelope.py
--rw-r--r--   0 runner    (1001) docker     (123)    48107 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    36110 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    57112 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/sunpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    30461 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/viewsphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    53418 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/wea.py
--rw-r--r--   0 runner    (1001) docker     (123)    39127 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/windprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)    37860 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/ladybug/windrose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/ladybug_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-17 01:59:59.000000 ladybug-core-0.41.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-01-17 01:58:37.000000 ladybug-core-0.41.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51971 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/_datacollectionbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/analysisperiod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/cli/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/cli/setconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/climatezone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67221 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datacollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datacollectionimmutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug/datatype/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/energyflux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/energyintensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/luminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/massflowrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/rvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/specificenergy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/temperaturedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/temperaturetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/thermalcondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/uvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/volumeflowrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datatype/volumeflowrateintensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/datautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/ddy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58123 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/designday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18177 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85289 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/epw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/futil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/graphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25056 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/hourlyplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84125 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/logutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50531 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/monthlychart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42331 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/psychchart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/psychrometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/rootfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55789 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/solarenvelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48107 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36110 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57112 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/sunpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30461 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/viewsphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53418 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/wea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39127 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/windprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37860 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/ladybug/windrose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/ladybug_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-21 20:32:55.000000 ladybug-core-0.41.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-01-21 20:31:48.000000 ladybug-core-0.41.9/setup.py
```

### Comparing `ladybug-core-0.41.8/LICENSE` & `ladybug-core-0.41.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/PKG-INFO` & `ladybug-core-0.41.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-core
-Version: 0.41.8
+Version: 0.41.9
 Summary: Python library to load, analyze and modify EnergyPlus Weather files (epw).
 Home-page: https://github.com/ladybug-tools/ladybug
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ladybug-core-0.41.8/README.md` & `ladybug-core-0.41.9/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/dev-requirements.txt` & `ladybug-core-0.41.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/__init__.py` & `ladybug-core-0.41.9/ladybug/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/_datacollectionbase.py` & `ladybug-core-0.41.9/ladybug/_datacollectionbase.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/analysisperiod.py` & `ladybug-core-0.41.9/ladybug/analysisperiod.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/cli/__init__.py` & `ladybug-core-0.41.9/ladybug/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/cli/_helper.py` & `ladybug-core-0.41.9/ladybug/cli/_helper.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/cli/setconfig.py` & `ladybug-core-0.41.9/ladybug/cli/setconfig.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/cli/translate.py` & `ladybug-core-0.41.9/ladybug/cli/translate.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/climatezone.py` & `ladybug-core-0.41.9/ladybug/climatezone.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/color.py` & `ladybug-core-0.41.9/ladybug/color.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/compass.py` & `ladybug-core-0.41.9/ladybug/compass.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/config.py` & `ladybug-core-0.41.9/ladybug/config.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datacollection.py` & `ladybug-core-0.41.9/ladybug/datacollection.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datacollectionimmutable.py` & `ladybug-core-0.41.9/ladybug/datacollectionimmutable.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/__init__.py` & `ladybug-core-0.41.9/ladybug/datatype/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/angle.py` & `ladybug-core-0.41.9/ladybug/datatype/angle.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/area.py` & `ladybug-core-0.41.9/ladybug/datatype/area.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/base.py` & `ladybug-core-0.41.9/ladybug/datatype/base.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/current.py` & `ladybug-core-0.41.9/ladybug/datatype/current.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/distance.py` & `ladybug-core-0.41.9/ladybug/datatype/distance.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/energy.py` & `ladybug-core-0.41.9/ladybug/datatype/energy.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/energyflux.py` & `ladybug-core-0.41.9/ladybug/datatype/energyflux.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/energyintensity.py` & `ladybug-core-0.41.9/ladybug/datatype/energyintensity.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/fraction.py` & `ladybug-core-0.41.9/ladybug/datatype/fraction.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/generic.py` & `ladybug-core-0.41.9/ladybug/datatype/generic.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/illuminance.py` & `ladybug-core-0.41.9/ladybug/datatype/illuminance.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/luminance.py` & `ladybug-core-0.41.9/ladybug/datatype/luminance.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/mass.py` & `ladybug-core-0.41.9/ladybug/datatype/mass.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/massflowrate.py` & `ladybug-core-0.41.9/ladybug/datatype/massflowrate.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/power.py` & `ladybug-core-0.41.9/ladybug/datatype/power.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/pressure.py` & `ladybug-core-0.41.9/ladybug/datatype/pressure.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/rvalue.py` & `ladybug-core-0.41.9/ladybug/datatype/rvalue.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/specificenergy.py` & `ladybug-core-0.41.9/ladybug/datatype/specificenergy.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/speed.py` & `ladybug-core-0.41.9/ladybug/datatype/speed.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/temperature.py` & `ladybug-core-0.41.9/ladybug/datatype/temperature.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/temperaturedelta.py` & `ladybug-core-0.41.9/ladybug/datatype/temperaturedelta.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/temperaturetime.py` & `ladybug-core-0.41.9/ladybug/datatype/temperaturetime.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/thermalcondition.py` & `ladybug-core-0.41.9/ladybug/datatype/thermalcondition.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/time.py` & `ladybug-core-0.41.9/ladybug/datatype/time.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/uvalue.py` & `ladybug-core-0.41.9/ladybug/datatype/uvalue.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/voltage.py` & `ladybug-core-0.41.9/ladybug/datatype/voltage.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/volume.py` & `ladybug-core-0.41.9/ladybug/datatype/volume.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/volumeflowrate.py` & `ladybug-core-0.41.9/ladybug/datatype/volumeflowrate.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datatype/volumeflowrateintensity.py` & `ladybug-core-0.41.9/ladybug/datatype/volumeflowrateintensity.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/datautil.py` & `ladybug-core-0.41.9/ladybug/datautil.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/ddy.py` & `ladybug-core-0.41.9/ladybug/ddy.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/designday.py` & `ladybug-core-0.41.9/ladybug/designday.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/dt.py` & `ladybug-core-0.41.9/ladybug/dt.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/epw.py` & `ladybug-core-0.41.9/ladybug/epw.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/futil.py` & `ladybug-core-0.41.9/ladybug/futil.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/graphic.py` & `ladybug-core-0.41.9/ladybug/graphic.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/header.py` & `ladybug-core-0.41.9/ladybug/header.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/hourlyplot.py` & `ladybug-core-0.41.9/ladybug/hourlyplot.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/legend.py` & `ladybug-core-0.41.9/ladybug/legend.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/location.py` & `ladybug-core-0.41.9/ladybug/location.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/logutil.py` & `ladybug-core-0.41.9/ladybug/logutil.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/monthlychart.py` & `ladybug-core-0.41.9/ladybug/monthlychart.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/psychchart.py` & `ladybug-core-0.41.9/ladybug/psychchart.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/psychrometrics.py` & `ladybug-core-0.41.9/ladybug/psychrometrics.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/rootfinding.py` & `ladybug-core-0.41.9/ladybug/rootfinding.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/skymodel.py` & `ladybug-core-0.41.9/ladybug/skymodel.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/solarenvelope.py` & `ladybug-core-0.41.9/ladybug/solarenvelope.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/sql.py` & `ladybug-core-0.41.9/ladybug/sql.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/stat.py` & `ladybug-core-0.41.9/ladybug/stat.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/sunpath.py` & `ladybug-core-0.41.9/ladybug/sunpath.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/viewsphere.py` & `ladybug-core-0.41.9/ladybug/viewsphere.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/wea.py` & `ladybug-core-0.41.9/ladybug/wea.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/windprofile.py` & `ladybug-core-0.41.9/ladybug/windprofile.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug/windrose.py` & `ladybug-core-0.41.9/ladybug/windrose.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/ladybug_core.egg-info/PKG-INFO` & `ladybug-core-0.41.9/ladybug_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-core
-Version: 0.41.8
+Version: 0.41.9
 Summary: Python library to load, analyze and modify EnergyPlus Weather files (epw).
 Home-page: https://github.com/ladybug-tools/ladybug
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ladybug-core-0.41.8/ladybug_core.egg-info/SOURCES.txt` & `ladybug-core-0.41.9/ladybug_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.41.8/setup.py` & `ladybug-core-0.41.9/setup.py`

 * *Files identical despite different names*

