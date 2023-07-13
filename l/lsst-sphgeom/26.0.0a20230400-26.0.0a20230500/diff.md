# Comparing `tmp/lsst-sphgeom-26.0.0a20230400.tar.gz` & `tmp/lsst-sphgeom-26.0.0a20230500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-sphgeom-26.0.0a20230400.tar", last modified: Thu Jan 26 09:56:20 2023, max compression
+gzip compressed data, was "lsst-sphgeom-26.0.0a20230500.tar", last modified: Thu Feb  2 14:05:04 2023, max compression
```

## Comparing `lsst-sphgeom-26.0.0a20230400.tar` & `lsst-sphgeom-26.0.0a20230500.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.742854 lsst-sphgeom-26.0.0a20230400/
--rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-01-26 09:56:20.742854 lsst-sphgeom-26.0.0a20230400/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.722854 lsst-sphgeom-26.0.0a20230400/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.722854 lsst-sphgeom-26.0.0a20230400/include/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.730854 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Angle.h
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/AngleInterval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/BigInteger.h
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Box.h
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Box3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Chunker.h
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Circle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/CompoundRegion.h
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/ConvexPolygon.h
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Ellipse.h
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/HtmPixelization.h
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Interval.h
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Interval1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/LonLat.h
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Matrix3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Mq3cPixelization.h
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/NormalizedAngle.h
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/NormalizedAngleInterval.h
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Pixelization.h
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Q3cPixelization.h
--rw-r--r--   0 runner    (1001) docker     (123)    21900 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/RangeSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Region.h
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Relationship.h
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/UnitVector3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Vector3d.h
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/codec.h
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/curve.h
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/orientation.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.730854 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python/
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python/interval.h
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python/relationship.h
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python.h
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.722854 lsst-sphgeom-26.0.0a20230400/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.730854 lsst-sphgeom-26.0.0a20230400/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.738854 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_angle.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_angleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_box.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_box3d.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_chunker.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_circle.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_compoundRegion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_convexPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_curve.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_ellipse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_healpixPixelization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_htmPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_interval1d.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_lonLat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_matrix3d.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_mq3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_normalizedAngle.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_normalizedAngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_orientation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_pixelization.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_q3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_rangeSet.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_region.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_relationship.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_sphgeom.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_unitVector3d.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_vector3d.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/pixelization_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-26 09:56:20.000000 lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.738854 lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-01-26 09:56:20.000000 lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-01-26 09:56:20.000000 lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 09:56:20.000000 lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 09:56:19.000000 lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-26 09:56:20.000000 lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-26 09:56:20.000000 lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-26 09:56:20.746854 lsst-sphgeom-26.0.0a20230400/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:56:20.742854 lsst-sphgeom-26.0.0a20230400/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Angle.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/AngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/BigInteger.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19470 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Box.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Box3d.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Chunker.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Circle.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/CompoundRegion.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/ConvexPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/ConvexPolygonImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Ellipse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/HtmPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Interval1d.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/LonLat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Matrix3d.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Mq3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/NormalizedAngle.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/NormalizedAngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/PixelFinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Q3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Q3cPixelizationImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/RangeSet.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Region.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/UnitVector3d.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/Vector3d.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/orientation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-01-26 09:56:01.000000 lsst-sphgeom-26.0.0a20230400/src/utils.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.774105 lsst-sphgeom-26.0.0a20230500/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-02-02 14:05:04.774105 lsst-sphgeom-26.0.0a20230500/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.766106 lsst-sphgeom-26.0.0a20230500/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.766106 lsst-sphgeom-26.0.0a20230500/include/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.770105 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Angle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/AngleInterval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/BigInteger.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Box.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Box3d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Chunker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Circle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/CompoundRegion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/ConvexPolygon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Ellipse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/HtmPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Interval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Interval1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/LonLat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Matrix3d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Mq3cPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/NormalizedAngle.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/NormalizedAngleInterval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Pixelization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Q3cPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21900 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/RangeSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Region.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Relationship.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/UnitVector3d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Vector3d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/codec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/curve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/orientation.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.770105 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python/interval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python/relationship.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.766106 lsst-sphgeom-26.0.0a20230500/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.770105 lsst-sphgeom-26.0.0a20230500/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.774105 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_angle.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_angleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_box.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_box3d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_chunker.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_circle.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_compoundRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_convexPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_curve.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_ellipse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_healpixPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_htmPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_interval1d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_lonLat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_matrix3d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_mq3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_normalizedAngle.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_normalizedAngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_orientation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_pixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_q3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_rangeSet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_region.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_relationship.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_sphgeom.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_unitVector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_vector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/pixelization_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-02 14:05:04.000000 lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.774105 lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-02-02 14:05:04.000000 lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-02-02 14:05:04.000000 lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 14:05:04.000000 lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 14:05:03.000000 lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-02 14:05:04.000000 lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-02 14:05:04.000000 lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-02 14:05:04.774105 lsst-sphgeom-26.0.0a20230500/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:05:04.774105 lsst-sphgeom-26.0.0a20230500/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Angle.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/AngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/BigInteger.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19470 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Box.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Box3d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Chunker.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Circle.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/CompoundRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/ConvexPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/ConvexPolygonImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Ellipse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/HtmPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Interval1d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/LonLat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Matrix3d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Mq3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/NormalizedAngle.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/NormalizedAngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/PixelFinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Q3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Q3cPixelizationImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/RangeSet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Region.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/UnitVector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/Vector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/orientation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-02-02 14:04:49.000000 lsst-sphgeom-26.0.0a20230500/src/utils.cc
```

### Comparing `lsst-sphgeom-26.0.0a20230400/LICENSE` & `lsst-sphgeom-26.0.0a20230500/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -668,8 +668,7 @@
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
 <http://www.gnu.org/philosophy/why-not-lgpl.html>.
-
```

### Comparing `lsst-sphgeom-26.0.0a20230400/PKG-INFO` & `lsst-sphgeom-26.0.0a20230500/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-sphgeom
-Version: 26.0.0a20230400
+Version: 26.0.0a20230500
 Summary: A spherical geometry library.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GPLv3+ License
 Project-URL: Homepage, https://github.com/lsst/sphgeom
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `lsst-sphgeom-26.0.0a20230400/README.md` & `lsst-sphgeom-26.0.0a20230500/README.md`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Angle.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Angle.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/AngleInterval.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/AngleInterval.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/BigInteger.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/BigInteger.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Box.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Box.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Box3d.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Box3d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Chunker.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Chunker.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Circle.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Circle.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/CompoundRegion.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/CompoundRegion.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/ConvexPolygon.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/ConvexPolygon.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Ellipse.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Ellipse.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/HtmPixelization.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/HtmPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Interval.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Interval.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Interval1d.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Interval1d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/LonLat.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/LonLat.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Matrix3d.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Matrix3d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Mq3cPixelization.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Mq3cPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/NormalizedAngle.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/NormalizedAngle.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/NormalizedAngleInterval.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/NormalizedAngleInterval.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Pixelization.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Pixelization.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Q3cPixelization.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Q3cPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/RangeSet.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/RangeSet.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Region.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Region.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Relationship.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Relationship.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/UnitVector3d.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/UnitVector3d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/Vector3d.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/Vector3d.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/codec.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/codec.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/constants.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/constants.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/curve.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/curve.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/orientation.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/orientation.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python/interval.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python/interval.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python/relationship.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python/relationship.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python/utils.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python/utils.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/python.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/python.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/include/lsst/sphgeom/utils.h` & `lsst-sphgeom-26.0.0a20230500/include/lsst/sphgeom/utils.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/pyproject.toml` & `lsst-sphgeom-26.0.0a20230500/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 license-files = ["LICENSE"]
 
 [tool.setuptools.dynamic]
 version = { attr = "lsst_versions.get_lsst_version" }
 
 [tool.black]
 line-length = 110
-target-version = ["py38"]
+target-version = ["py310"]
 
 [tool.isort]
 profile = "black"
 line_length = 110
 
 [tool.lsst_versions]
 write_to = "python/lsst/sphgeom/version.py"
```

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/__init__.py` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_angle.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_angle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_angleInterval.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_angleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_box.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_box.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_box3d.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_box3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_chunker.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_chunker.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_circle.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_circle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_compoundRegion.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_compoundRegion.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_convexPolygon.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_convexPolygon.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_curve.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_curve.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_ellipse.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_ellipse.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_healpixPixelization.py` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_healpixPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_htmPixelization.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_htmPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_interval1d.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_interval1d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_lonLat.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_lonLat.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_matrix3d.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_matrix3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_mq3cPixelization.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_mq3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_normalizedAngle.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_normalizedAngle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_normalizedAngleInterval.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_normalizedAngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_orientation.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_orientation.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_pixelization.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_pixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_q3cPixelization.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_q3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_rangeSet.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_rangeSet.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_region.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_region.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_relationship.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_relationship.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_sphgeom.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_sphgeom.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_unitVector3d.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_unitVector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_utils.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_utils.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_vector3d.cc` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_vector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/_yaml.py` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/_yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,16 +110,15 @@
         "lsst.sphgeom.Mq3cPixelization": Mq3cPixelization,
         "lsst.sphgeom.HtmPixelization": HtmPixelization,
         "lsst.sphgeom.HealpixPixelization": HealpixPixelization,
     }
 
     if className not in pixelMap:
         raise RuntimeError(
-            f"Encountered unexpected class {className} associated with"
-            " sphgeom pixelization YAML constructor"
+            f"Encountered unexpected class {className} associated with sphgeom pixelization YAML constructor"
         )
 
     return pixelMap[className](mapping["level"])
 
 
 # All the pixelization schemes use the same approach with getLevel
 if yaml:
```

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst/sphgeom/pixelization_abc.py` & `lsst-sphgeom-26.0.0a20230500/python/lsst/sphgeom/pixelization_abc.py`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/PKG-INFO` & `lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-sphgeom
-Version: 26.0.0a20230400
+Version: 26.0.0a20230500
 Summary: A spherical geometry library.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GPLv3+ License
 Project-URL: Homepage, https://github.com/lsst/sphgeom
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `lsst-sphgeom-26.0.0a20230400/python/lsst_sphgeom.egg-info/SOURCES.txt` & `lsst-sphgeom-26.0.0a20230500/python/lsst_sphgeom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/setup.py` & `lsst-sphgeom-26.0.0a20230500/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,24 @@
   interface.
 """
 
 import glob
 
 # Importing this automatically enables parallelized builds
 import numpy.distutils.ccompiler  # noqa: F401
-from setuptools import setup
 from pybind11.setup_helpers import Pybind11Extension, build_ext
+from setuptools import setup
 
 # Find the source code -- we can combine it into a single module
 pybind_src = sorted(glob.glob("python/lsst/sphgeom/*.cc"))
 cpp_src = sorted(glob.glob("src/*.cc"))
 
 # Very inefficient approach since this compiles the maing sphgeom
 # library code for every extension rather than building everything once
-ext_modules = [Pybind11Extension("lsst.sphgeom._sphgeom",
-                                 sorted(cpp_src + pybind_src),
-                                 include_dirs=["include"])]
+ext_modules = [
+    Pybind11Extension("lsst.sphgeom._sphgeom", sorted(cpp_src + pybind_src), include_dirs=["include"])
+]
 
 setup(
     ext_modules=ext_modules,
-    cmdclass={'build_ext': build_ext},
+    cmdclass={"build_ext": build_ext},
 )
```

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Angle.cc` & `lsst-sphgeom-26.0.0a20230500/src/Angle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/AngleInterval.cc` & `lsst-sphgeom-26.0.0a20230500/src/AngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/BigInteger.cc` & `lsst-sphgeom-26.0.0a20230500/src/BigInteger.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Box.cc` & `lsst-sphgeom-26.0.0a20230500/src/Box.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Box3d.cc` & `lsst-sphgeom-26.0.0a20230500/src/Box3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Chunker.cc` & `lsst-sphgeom-26.0.0a20230500/src/Chunker.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Circle.cc` & `lsst-sphgeom-26.0.0a20230500/src/Circle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/CompoundRegion.cc` & `lsst-sphgeom-26.0.0a20230500/src/CompoundRegion.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/ConvexPolygon.cc` & `lsst-sphgeom-26.0.0a20230500/src/ConvexPolygon.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/ConvexPolygonImpl.h` & `lsst-sphgeom-26.0.0a20230500/src/ConvexPolygonImpl.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Ellipse.cc` & `lsst-sphgeom-26.0.0a20230500/src/Ellipse.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/HtmPixelization.cc` & `lsst-sphgeom-26.0.0a20230500/src/HtmPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Interval1d.cc` & `lsst-sphgeom-26.0.0a20230500/src/Interval1d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/LonLat.cc` & `lsst-sphgeom-26.0.0a20230500/src/LonLat.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Matrix3d.cc` & `lsst-sphgeom-26.0.0a20230500/src/Matrix3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Mq3cPixelization.cc` & `lsst-sphgeom-26.0.0a20230500/src/Mq3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/NormalizedAngle.cc` & `lsst-sphgeom-26.0.0a20230500/src/NormalizedAngle.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/NormalizedAngleInterval.cc` & `lsst-sphgeom-26.0.0a20230500/src/NormalizedAngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/PixelFinder.h` & `lsst-sphgeom-26.0.0a20230500/src/PixelFinder.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Q3cPixelization.cc` & `lsst-sphgeom-26.0.0a20230500/src/Q3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Q3cPixelizationImpl.h` & `lsst-sphgeom-26.0.0a20230500/src/Q3cPixelizationImpl.h`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/RangeSet.cc` & `lsst-sphgeom-26.0.0a20230500/src/RangeSet.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Region.cc` & `lsst-sphgeom-26.0.0a20230500/src/Region.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/UnitVector3d.cc` & `lsst-sphgeom-26.0.0a20230500/src/UnitVector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/Vector3d.cc` & `lsst-sphgeom-26.0.0a20230500/src/Vector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/orientation.cc` & `lsst-sphgeom-26.0.0a20230500/src/orientation.cc`

 * *Files identical despite different names*

### Comparing `lsst-sphgeom-26.0.0a20230400/src/utils.cc` & `lsst-sphgeom-26.0.0a20230500/src/utils.cc`

 * *Files identical despite different names*

