# Comparing `tmp/OnlySnarf-4.5.0.tar.gz` & `tmp/OnlySnarf-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnlySnarf-4.5.0.tar", last modified: Tue Jul 11 19:45:09 2023, max compression
+gzip compressed data, was "OnlySnarf-4.5.1.tar", last modified: Wed Jul 12 22:44:07 2023, max compression
```

## Comparing `OnlySnarf-4.5.0.tar` & `OnlySnarf-4.5.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    31118 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/CHANGELOG.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/LICENSE.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/MANIFEST.in
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/__main__.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/classes/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/discount.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/element.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/classes/file.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12176 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/message.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1974 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/poll.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.0/OnlySnarf/classes/profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/promotion.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4922 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/schedule.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    18096 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/classes/user.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/conf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/conf/config.conf
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2263 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/conf/test-config.conf
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/elements/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/elements/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/elements/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/elements/login.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/elements/profile.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/lib/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/lib/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   163518 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/lib/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/lib/ffmpeg.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5130 2023-07-06 00:06:23.000000 OnlySnarf-4.5.0/OnlySnarf/menu.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5069 2023-05-29 23:03:04.000000 OnlySnarf-4.5.0/OnlySnarf/snarf.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/OnlySnarf/util/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/util/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1372 2023-07-06 00:40:42.000000 OnlySnarf-4.5.0/OnlySnarf/util/args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/util/colorize.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1482 2023-05-29 23:59:50.000000 OnlySnarf-4.5.0/OnlySnarf/util/config.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3183 2023-05-29 23:06:57.000000 OnlySnarf-4.5.0/OnlySnarf/util/defaults.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/util/logger.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12269 2023-05-29 23:06:57.000000 OnlySnarf-4.5.0/OnlySnarf/util/optional_args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    19436 2023-07-06 00:06:23.000000 OnlySnarf-4.5.0/OnlySnarf/util/settings.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/util/validators.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf.egg-info/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1171 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/SOURCES.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/dependency_links.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/entry_points.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       62 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/requires.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/top_level.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.0/README.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/setup.cfg
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1351 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/setup.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/tests/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/tests/test_profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/tests/test_promotion.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    31578 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/CHANGELOG.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/LICENSE.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/MANIFEST.in
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       47 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/__main__.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf/classes/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/discount.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/element.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.1/OnlySnarf/classes/file.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12549 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/classes/message.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1974 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/poll.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.1/OnlySnarf/classes/profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/promotion.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/classes/schedule.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    18262 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/classes/user.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf/conf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/conf/config.conf
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2263 2023-07-11 19:44:50.000000 OnlySnarf-4.5.1/OnlySnarf/conf/test-config.conf
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf/elements/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/elements/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/elements/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/elements/login.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/elements/profile.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/OnlySnarf/lib/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/lib/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   163926 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/lib/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/lib/ffmpeg.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5130 2023-07-06 00:06:23.000000 OnlySnarf-4.5.1/OnlySnarf/menu.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5069 2023-07-11 22:15:14.000000 OnlySnarf-4.5.1/OnlySnarf/snarf.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/OnlySnarf/util/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/util/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/util/args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/util/colorize.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1483 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/util/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3183 2023-05-29 23:06:57.000000 OnlySnarf-4.5.1/OnlySnarf/util/defaults.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/util/logger.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12269 2023-05-29 23:06:57.000000 OnlySnarf-4.5.1/OnlySnarf/util/optional_args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20018 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/util/settings.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.1/OnlySnarf/util/validators.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf.egg-info/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1171 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/entry_points.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       73 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/requires.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/top_level.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.1/README.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/setup.cfg
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1373 2023-07-12 22:43:39.000000 OnlySnarf-4.5.1/setup.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/tests/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/tests/test_profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/tests/test_promotion.py
```

### Comparing `OnlySnarf-4.5.0/CHANGELOG.md` & `OnlySnarf-4.5.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -675,34 +675,45 @@
   **4.4.12: 3/24/2023**
   - RPi4 debugging
   - fixed element bug when posting
   - fixed users
   - fixed error message on close
   **4/15/2023**
   - cleaned up git repo size / long clone time
-**4.4.13: 4/17/2023**
+  **4.4.13: 4/17/2023**
   - Windows compatability testing
   - updated pathings for Windows
   - retested google login (remains disabled)
-**4.4.14 : 5/29/2023**
+  **4.4.14 : 5/29/2023**
   - beginning readd of cli menu
   - switch from pyinquirer to inquirer
-**4.4.15 : 6/2/2023**
+  **4.4.15 : 6/2/2023**
   - fixed cookies bug
-**4.4.16 : 7/5/2023**
+  **4.4.16 : 7/5/2023**
   - update readme and help&menu docs / added personal touchups
   - fixed get random user for discount test 
 **4.5.0 : 7/11/2023**
   - added wget functionality to input for when a url is provided
   - cleaned up bin/test scripts
-  
+  - added basic api setup
+  - added test scripts for flask & api
+  - beginning modifications for receiving api calls
+**4.5.1 : 7/12/2023**
+  - fixed package req: validators
+  - added modifications for running via api
+
+
 ------------------------------------------------------------------------------------
 
 ## TODO
 
+
+- look into Marshmellow package for class / object cleanup
+- reconfigure how args & config values are passed through into Settings --> to fix when setting a variable like post.schedule = "text" is referenced after the args check step
+
 - fix how tabs open and scroll and then the process opens another tab to find the same elements and scroll again ala: find users then discount user
 
 - add smart idea for getting statement information
 - add better version notes to readme's list of "works on"
 - re-add stuff for testing on multiple platforms ala mac ;) 
 
 - double check how tags & performers are implemented in config and text config and then re-add to docs
```

### Comparing `OnlySnarf-4.5.0/LICENSE.txt` & `OnlySnarf-4.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/discount.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/discount.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/element.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/element.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/file.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/file.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/message.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,15 +140,25 @@
         Returns
         -------
         list
             Files in a list
 
         """
 
-        if len(self.files) > 0: return self.files[:int(Settings.get_upload_max())]
+        if len(self.files) > 0:
+            files_ = []
+            for file in self.files[:int(Settings.get_upload_max())]:
+                if not isinstance(file, File):
+                    file_ = File()
+                    setattr(file_, "path", file)
+                    files_.append(file_)
+                else:
+                    files_.append(file)
+            return files_
+            # return self.files[:int(Settings.get_upload_max())]
         files = Settings.get_input_as_files()
         if len(files) > 0:
             Settings.dev_print("fetched input files for upload")
             self.files = files[:int(Settings.get_upload_max())] # reduce by max
             # self.files = files
             # return files
         return self.files
@@ -322,15 +332,15 @@
         OnlyFans post object
 
         A post is just a message on a profile with different options made available. So all posts are messages, as all messages are messages.
             Squares and rectangles.
 
         """
 
-        super().__init__()
+        super().__init__(self)
         self.expiration = 0
         self.poll = None
         self.schedule = None
 
     # def __str__(self):
     #     return "fooPost"
 
@@ -423,15 +433,15 @@
         -------
         Schedule
             Schedule object with proper values.
 
         """
 
         if self.schedule: return self.schedule
-        self.schedule = Schedule()
+        # self.schedule = Schedule()
         return self.schedule
 
     def send(self):
         """
         Sends a post.
```

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/poll.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/poll.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/profile.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/promotion.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/promotion.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/schedule.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/schedule.py`

 * *Files 7% similar despite different names*

```diff
@@ -139,24 +139,21 @@
 
         """
 
         Settings.dev_print("validating schedule...")
         today = datetime.strptime(str(datetime.now().strftime(DEFAULT.SCHEDULE_FORMAT)), DEFAULT.SCHEDULE_FORMAT)
         # schedule = datetime.strptime(str(Settings.get_schedule().now().strftime(DEFAULT.SCHEDULE_FORMAT)), DEFAULT.SCHEDULE_FORMAT)
         schedule = Settings.get_schedule()
+        if not schedule: return False
         if isinstance(schedule, str):
             schedule = datetime.strptime(schedule, DEFAULT.SCHEDULE_FORMAT)
         # should invalidate if all default settings
         if str(self.get_date()) == DEFAULT.DATE and (str(self.get_time()) == DEFAULT.TIME or str(self.get_time()) == DEFAULT.TIME_NONE):
             Settings.dev_print("invalid schedule! (default date and time)")
             return False
         # cannot post in the past
         # TODO: possibly add margin of error if necessary
         elif schedule <= today:
             Settings.dev_print("invalid schedule! (must be in future)")
             return False
         Settings.dev_print("valid schedule!")
         return True
-
-# round to 5
-def myround(x, base=5):
-    return base * round(x/base)
```

### Comparing `OnlySnarf-4.5.0/OnlySnarf/classes/user.py` & `OnlySnarf-4.5.1/OnlySnarf/classes/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,22 +150,23 @@
             # enter the text of the message
             def enter_text(text): return driver.message_text(text)
             # enter the price to send the message to the user
             def enter_price(price):
                 if not price: return True
                 return driver.message_price(price)
             def enter_files(files):
-                for file in files:
+                # TODO: requires proper debugging
+                # for file in files:
                     # enter files by filepath while checking for already sent files
-                    file_name = file.get_title()
-                    if str(file_name) in self.sent_files:
-                        Settings.warn_print("file already sent to user: {} <-- {}".format(self.username, file_name))
-                        Settings.maybe_print("skipping...")
-                        continue
-                    self.sent_files.append(file_name)
+                    # file_name = file.get_title()
+                    # if str(file_name) in self.sent_files:
+                    #     Settings.warn_print("file already sent to user: {} <-- {}".format(self.username, file_name))
+                    #     Settings.maybe_print("skipping...")
+                    #     continue
+                    # self.sent_files.append(file_name)
                 return driver.upload_files(files)
             if all([enter_text(message["text"]), enter_price(message["price"]), enter_files(message["files"])]): return confirm_message()
         except Exception as e:
             Settings.err_print("message failed!")
             Settings.dev_print(e)
         return False
 
@@ -212,15 +213,15 @@
 
         """
 
         Settings.dev_print("getting all users...")
         users = []
         if Settings.is_prefer_local():
             users = User.read_users_local()
-        else:
+        if len(users) == 0:
             for user in Driver.users_get():
                 if user is None: continue
                 users.append(User(user))
         Settings.maybe_print("users: {}".format(len(users)))
         User.write_users_local(users=users)
         Settings.set_prefer_local(True)
         return users
@@ -441,16 +442,18 @@
 
         Parameters
         ----------
         message : Object
             The message to send as a serialized Message object from get_message.
         """
 
-        user = User({"username":username,"id":user_id})
-        return user.message(message) 
+        if str(username).lower() == "random":
+            User.get_random_user().message(message)
+        else:
+            User({"username":username,"id":user_id}).message(message)
 
     @staticmethod
     def read_following_local():
         """
         Read the locally saved following file.
 
         Returns
```

### Comparing `OnlySnarf-4.5.0/OnlySnarf/conf/config.conf` & `OnlySnarf-4.5.1/OnlySnarf/conf/config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/conf/test-config.conf` & `OnlySnarf-4.5.1/OnlySnarf/conf/test-config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/elements/driver.py` & `OnlySnarf-4.5.1/OnlySnarf/elements/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/elements/login.py` & `OnlySnarf-4.5.1/OnlySnarf/elements/login.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/elements/profile.py` & `OnlySnarf-4.5.1/OnlySnarf/elements/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/lib/driver.py` & `OnlySnarf-4.5.1/OnlySnarf/lib/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 # from webdriver_manager.microsoft import EdgeChromiumDriverManager
 # from msedge.selenium_tools import Edge, EdgeOptions
 # opera
 from webdriver_manager.opera import OperaDriverManager
 ##
 from ..classes.element import Element
 from ..util.settings import Settings
+#
+from ..classes.file import File
 
 ###################
 ##### Globals #####
 ###################
 
 # Urls
 ONLYFANS_HOME_URL = "https://onlyfans.com"
@@ -1457,14 +1459,17 @@
             Settings.dev_print("attempting to start message for {}...".format(username))
             type__ = None # default
             # if the username is a key string it will behave differently
             if str(username).lower() == "all": type__ = "messageAll"
             elif str(username).lower() == "recent": type__ = "messageRecent"
             elif str(username).lower() == "favorite": type__ = "messageFavorite"
             elif str(username).lower() == "renew on": type__ = "messageRenewers"
+            elif str(username).lower() == "random":
+                from ..classes.user import User
+                username = User.get_random_user().username
             successful = False
             if type__ != None:
                 driver.go_to_page(ONLYFANS_NEW_MESSAGE_URL)
                 Settings.dev_print("clicking message type: {}".format(username))
                 driver.find_element_to_click(type__).click()
                 successful = True
             else:
@@ -1937,15 +1942,15 @@
         Settings.print("- Files: {}".format(len(message["files"])))
         Settings.print("- Performers: {}".format(message["performers"]))
         Settings.print("- Tags: {}".format(message["tags"]))
         Settings.print("- Text: {}".format(message["text"]))
         Settings.print("- Tweeting: {}".format(Settings.is_tweeting()))
         ## Expires, Schedule, Poll ##
         if not driver.expires(message["expiration"]): return False
-        if message["schedule"].validate() and not driver.schedule(message["schedule"].get()): return False
+        if message["schedule"] and message["schedule"].validate() and not driver.schedule(message["schedule"].get()): return False
         if message["poll"].validate() and not driver.poll(message["poll"].get()): return False
         Settings.print("====================")
         ############################################################
 
         ## Tweeting ##
         ## TODO
         ## test this
@@ -1958,15 +1963,15 @@
 
         ## Upload Files ##
         try:
 
             if not driver.enter_text(message["text"]):
                 Settings.err_print("unable to post!")
                 return False
-            
+
             successful, skipped = driver.upload_files(message["files"])
             if successful and not skipped:
                 # twitter tweet button is 1st, post is 2nd
                 postButton = [ele for ele in driver.browser.find_elements(By.TAG_NAME, "button") if "Post" in ele.get_attribute("innerHTML")][0]
                 WebDriverWait(driver.browser, Settings.get_upload_max_duration(), poll_frequency=3).until(EC.element_to_be_clickable(postButton))
                 Settings.dev_print("upload complete")
 
@@ -3219,15 +3224,20 @@
 
         import threading
         import concurrent.futures
 
         files_ = []
 
         def prepare(file):
-            uploadable = file.prepare() # downloads if Google_File
+            # add a better check for this w/ the new API
+            if not isinstance(file, File):
+                _file = File()
+                setattr(_file, "path", file)
+                file = _file
+            uploadable = file.prepare() # downloads if necessary
             if not uploadable: Settings.err_print("unable to upload - {}".format(file.get_title()))
             else: files_.append(file)    
 
         with concurrent.futures.ThreadPoolExecutor(max_workers=3) as executor:
             executor.map(prepare, files)
 
         Settings.dev_print("files prepared: {}".format(len(files_)))
```

### Comparing `OnlySnarf-4.5.0/OnlySnarf/lib/ffmpeg.py` & `OnlySnarf-4.5.1/OnlySnarf/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/menu.py` & `OnlySnarf-4.5.1/OnlySnarf/menu.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/snarf.py` & `OnlySnarf-4.5.1/OnlySnarf/snarf.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/util/args.py` & `OnlySnarf-4.5.1/OnlySnarf/util/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,25 +26,23 @@
 apply_args(parser)
 
 ##
 import pkg_resources
 parser.version = str(pkg_resources.get_distribution("onlysnarf").version)
 parser.add_argument('-version', action='version')
 
-parser.add_argument('-version', action='version')
-
 ############################################################################################
 
 try:
   parsedargs, unknownargs = parser.parse_known_args()
   # print("unknown args: {}".format(unknownargs))
   args.update(vars(parsedargs))
 except Exception as e:
-  print(e)
-  print("Error: Incorrect arg format")
-  parser.exit(1)
+    print(e)
+    print("Error: Incorrect arg format")
+    parser.exit(1)
 
 #############
 # Debugging #
 # import sys
 # print(args)
 # sys.exit(0)
```

### Comparing `OnlySnarf-4.5.0/OnlySnarf/util/colorize.py` & `OnlySnarf-4.5.1/OnlySnarf/util/colorize.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/util/config.py` & `OnlySnarf-4.5.1/OnlySnarf/util/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
       configs[key] = config_file[section][key]
       # print(key, config[key])
     else:
       configs[section.lower()+"_"+key.lower()] = config_file[section][key].strip("\"")
       # print(key, config[section.lower()+"_"+key.lower()])
 
 config = {}
+
 # continue to overwrite values from config file with args
 from .args import args
 # print(args.items())
 for key, value in args.items():
   config[key] = value
 for key, value in configs.items():
   config[key] = value
```

### Comparing `OnlySnarf-4.5.0/OnlySnarf/util/defaults.py` & `OnlySnarf-4.5.1/OnlySnarf/util/defaults.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/util/logger.py` & `OnlySnarf-4.5.1/OnlySnarf/util/logger.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/util/optional_args.py` & `OnlySnarf-4.5.1/OnlySnarf/util/optional_args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf/util/settings.py` & `OnlySnarf-4.5.1/OnlySnarf/util/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,20 @@
         return cats
 
     def get_cookies_path():
         # return os.path.join(Settings.get_base_directory(), Settings.get_username(), "cookies.pkl")
         return os.path.join(Settings.get_base_directory(), "cookies.pkl")
 
     def get_price():
-        return config["price"]
+        price = 0
+        try:
+            price = config["price"]
+        except Exception as e:
+            pass
+        return price
 
     def get_price_minimum():
         return DEFAULT.PRICE_MINIMUM
 
     def get_price_maximum():
         return DEFAULT.PRICE_MAXIMUM
 
@@ -200,23 +205,27 @@
                 files.append[file_path]
         return set(files)
 
     def get_input_as_files():
         if Settings.FILES: return Settings.FILES
         from ..classes.file import File
         files = []
-        if isinstance(config["input"], list):
-            for file_path in config["input"]:
+        try:
+            _input = config["input"]
+            if isinstance(_input, list):
+                for file_path in _input:
+                    file = File()
+                    setattr(file, "path", file_path)
+                    files.append(file)
+            else:
                 file = File()
-                setattr(file, "path", file_path)
+                setattr(file, "path", _input)
                 files.append(file)
-        else:
-            file = File()
-            setattr(file, "path", config["input"])
-            files.append(file)
+        except Exception as e:
+            pass
         Settings.FILES = files
         return files
 
     def get_keywords():
         keywords = config["keywords"] or []
         keywords = [n.strip() for n in keywords]
         return keywords
@@ -324,24 +333,35 @@
     def get_remote_password():
         return config["remote_password"] or ""
 
     def get_profile_method():
         return config["profile_method"] or None
 
     def get_schedule():
-        if str(config["schedule"]) == DEFAULT.SCHEDULE:
-            config["schedule"] = datetime.strptime("{} {}".format(Settings.get_date(), Settings.get_time()), DEFAULT.SCHEDULE_FORMAT).strftime(DEFAULT.SCHEDULE_FORMAT)
-        elif not isinstance(config["schedule"], str):
-            config["schedule"] = config["schedule"].strftime(DEFAULT.SCHEDULE_FORMAT)
-        Settings.maybe_print("schedule (settings): {}".format(config["schedule"]))
-        return config["schedule"]
+        schedule = ""
+        try:
+            schedule = config["schedule"]
+            if str(schedule) == DEFAULT.SCHEDULE:
+                schedule = datetime.strptime("{} {}".format(Settings.get_date(), Settings.get_time()), DEFAULT.SCHEDULE_FORMAT).strftime(DEFAULT.SCHEDULE_FORMAT)
+            elif not isinstance(schedule, str):
+                schedule = schedule.strftime(DEFAULT.SCHEDULE_FORMAT)
+            Settings.maybe_print("schedule (settings): {}".format(schedule))
+            return schedule
+        except Exception as e:
+            pass
+        return None
 
     def get_tags():
-        tags = config["tags"] or []
-        tags = [n.strip() for n in tags]
+        tags = []
+        try:
+            tags = config["tags"]
+            tags = [n.strip() for n in tags]
+        except Exception as e:
+            pass
+            # Settings.err_print(e)
         return tags
 
     def get_text():
         return config["text"] or ""
 
     def get_time():
         config["time"] = Settings.format_time(config["time"])        
@@ -359,18 +379,26 @@
     def get_title():
         return config["title"] or ""
         
     def get_skipped_users():
         return config["skipped_users"] or []
         
     def get_questions():
-        return config["questions"] or []
+        try:
+            return config["questions"]
+        except Exception as e:
+            pass
+        return []
         
     def get_upload_max():
-        return config["upload_max"] or DEFAULT.IMAGE_LIMIT
+        try:
+            return config["upload_max"]
+        except Exception as e:
+            pass
+        return DEFAULT.IMAGE_LIMIT
         
     # def get_upload_max_messages():
         # return config["upload_max_messages"] or UPLOAD_MAX_MESSAGES
 
     def get_login_method():
         return config["login"]
```

### Comparing `OnlySnarf-4.5.0/OnlySnarf/util/validators.py` & `OnlySnarf-4.5.1/OnlySnarf/util/validators.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/OnlySnarf.egg-info/PKG-INFO` & `OnlySnarf-4.5.1/OnlySnarf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.0
+Version: 4.5.1
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.0 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.1 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.0/OnlySnarf.egg-info/SOURCES.txt` & `OnlySnarf-4.5.1/OnlySnarf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/PKG-INFO` & `OnlySnarf-4.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.0
+Version: 4.5.1
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.0 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.1 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.0/README.md` & `OnlySnarf-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/setup.py` & `OnlySnarf-4.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OnlySnarf",
-    version="4.5.0",
+    version="4.5.1",
     author="Skeetzo",
     author_email="WebmasterSkeetzo@gmail.com",
     url = 'https://github.com/skeetzo/onlysnarf',
     keywords = ['OnlyFans', 'OnlySnarf', 'selenium', 'snarf'],
     description="OnlyFans Content Distribution Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -17,15 +17,16 @@
     packages=["OnlySnarf", "OnlySnarf/classes","OnlySnarf/conf","OnlySnarf/elements","OnlySnarf/lib","OnlySnarf/util"],
     include_package_data=True,
     install_requires=[
         'ffmpeg',
         'inquirer',
         'wget',
         'selenium',
-        'webdriver_manager'
+        'webdriver_manager',
+        'validators'
         ],
     extras_require={
         'dev': [
             'pytest'
         ]
     },
     entry_points={
```

### Comparing `OnlySnarf-4.5.0/tests/test_profile.py` & `OnlySnarf-4.5.1/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.0/tests/test_promotion.py` & `OnlySnarf-4.5.1/tests/test_promotion.py`

 * *Files identical despite different names*

