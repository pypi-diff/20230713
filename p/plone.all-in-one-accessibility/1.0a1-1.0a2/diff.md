# Comparing `tmp/plone.all_in_one_accessibility-1.0a1.tar.gz` & `tmp/plone.all_in_one_accessibility-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.all_in_one_accessibility-1.0a1.tar", last modified: Thu Jul 13 09:03:11 2023, max compression
+gzip compressed data, was "plone.all_in_one_accessibility-1.0a2.tar", last modified: Thu Jul 13 09:52:50 2023, max compression
```

## Comparing `plone.all_in_one_accessibility-1.0a1.tar` & `plone.all_in_one_accessibility-1.0a2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.666593 plone.all_in_one_accessibility-1.0a1/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      118 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/CHANGES.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)       92 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/CONTRIBUTORS.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1338 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/DEVELOP.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)    18092 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/LICENSE.GPL
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      688 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/LICENSE.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      115 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/MANIFEST.in
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     4303 2023-07-13 09:03:11.666593 plone.all_in_one_accessibility-1.0a1/PKG-INFO
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2928 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/README.rst
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.606594 plone.all_in_one_accessibility-1.0a1/docs/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     8023 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/docs/conf.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      113 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/docs/index.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      340 2023-07-13 09:03:11.666593 plone.all_in_one_accessibility-1.0a1/setup.cfg
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2565 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/setup.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.602594 plone.all_in_one_accessibility-1.0a1/src/
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.606594 plone.all_in_one_accessibility-1.0a1/src/plone/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)       80 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/__init__.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.618594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      147 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/__init__.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.618594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      304 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/configure.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.626594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/services/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/services/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      299 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/services/configure.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.630594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/services/widget/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/services/widget/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      330 2023-07-13 08:53:23.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/services/widget/configure.zcml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2502 2023-07-13 08:53:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/services/widget/get.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.630594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/browser/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/browser/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      635 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/browser/configure.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.630594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/browser/overrides/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/browser/overrides/.gitkeep
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.630594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/browser/static/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/browser/static/.gitkeep
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1499 2023-07-13 08:52:27.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/configure.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.630594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/content/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/content/__init__.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2377 2023-07-13 08:51:11.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      330 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      276 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/interfaces.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.638594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      611 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/README.rst
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/__init__.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.602594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/en/
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.650593 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)       28 2023-07-13 08:58:49.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/plone.all_in_one_accessibility.mo
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/plone.all_in_one_accessibility.po
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/plone.all_in_one_accessibility.pot
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1776 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/update.py
--rwxrwxr-x   0 skynet    (1000) skynet    (1000)      527 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/update.sh
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      442 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/permissions.zcml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.602594 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.650593 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      213 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/browserlayer.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      105 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/catalog.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      319 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/metadata.xml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.662593 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/registry/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      188 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/registry/main.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      371 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/rolemap.xml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.662593 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/types/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     3406 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/types/All_in_One_Accessibility_Setting.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      335 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/types.xml
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.662593 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/uninstall/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      140 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      811 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/setuphandlers.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     1768 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/testing.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.662593 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/__init__.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.662593 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/robot/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     3268 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/robot/test_ct_all_in_one_accessibility_setting.robot
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2051 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/robot/test_example.robot
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2855 2023-07-13 08:49:35.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/test_ct_all_in_one_accessibility_setting.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      935 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/test_robot.py
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     2691 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/test_setup.py
-drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:03:11.614594 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     4303 2023-07-13 09:03:11.000000 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-r--   0 skynet    (1000) skynet    (1000)     3246 2023-07-13 09:03:11.000000 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        1 2023-07-13 09:03:11.000000 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      135 2023-07-13 09:03:11.000000 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/entry_points.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        6 2023-07-13 09:03:11.000000 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/namespace_packages.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        1 2023-07-13 08:53:47.000000 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/not-zip-safe
--rw-rw-r--   0 skynet    (1000) skynet    (1000)      159 2023-07-13 09:03:11.000000 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/requires.txt
--rw-rw-r--   0 skynet    (1000) skynet    (1000)        6 2023-07-13 09:03:11.000000 plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/top_level.txt
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      118 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/CHANGES.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)       92 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/CONTRIBUTORS.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1338 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/DEVELOP.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)    18092 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/LICENSE.GPL
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      688 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/LICENSE.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      115 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/MANIFEST.in
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2209 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/PKG-INFO
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1220 2023-07-13 09:51:37.000000 plone.all_in_one_accessibility-1.0a2/README.rst
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.577025 plone.all_in_one_accessibility-1.0a2/docs/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     8023 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/docs/conf.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      113 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/docs/index.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      340 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/setup.cfg
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2573 2023-07-13 09:52:45.000000 plone.all_in_one_accessibility-1.0a2/setup.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.573025 plone.all_in_one_accessibility-1.0a2/src/
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.577025 plone.all_in_one_accessibility-1.0a2/src/plone/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)       80 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/__init__.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      147 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/__init__.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      304 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/configure.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/services/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/services/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      299 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/services/configure.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/services/widget/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/services/widget/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      330 2023-07-13 08:53:23.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/services/widget/configure.zcml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2657 2023-07-13 09:49:46.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/services/widget/get.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/browser/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/browser/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      635 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/browser/configure.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/browser/overrides/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/browser/overrides/.gitkeep
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/browser/static/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/browser/static/.gitkeep
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1499 2023-07-13 08:52:27.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/configure.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/content/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/content/__init__.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2667 2023-07-13 09:49:04.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      330 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      276 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/interfaces.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      611 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/README.rst
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/__init__.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.573025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/en/
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.581025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)       28 2023-07-13 08:58:49.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/plone.all_in_one_accessibility.mo
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/en/LC_MESSAGES/plone.all_in_one_accessibility.po
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/plone.all_in_one_accessibility.pot
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1776 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/update.py
+-rwxrwxr-x   0 skynet    (1000) skynet    (1000)      527 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/update.sh
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      442 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/permissions.zcml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.577025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      213 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/browserlayer.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      105 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/catalog.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      319 2023-07-13 08:51:10.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/metadata.xml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/registry/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      188 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/registry/main.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      371 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/rolemap.xml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/types/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     3406 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/types/All_in_One_Accessibility_Setting.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      335 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/types.xml
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/uninstall/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      140 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      811 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/setuphandlers.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     1768 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/testing.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        0 2023-07-12 05:51:28.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/__init__.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.585025 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/robot/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     3268 2023-07-13 08:49:34.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/robot/test_ct_all_in_one_accessibility_setting.robot
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2051 2023-07-13 08:48:18.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/robot/test_example.robot
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2855 2023-07-13 08:49:35.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/test_ct_all_in_one_accessibility_setting.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      935 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/test_robot.py
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2691 2023-07-13 08:48:21.000000 plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/test_setup.py
+drwxrwxr-x   0 skynet    (1000) skynet    (1000)        0 2023-07-13 09:52:50.577025 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     2209 2023-07-13 09:52:50.000000 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)     3246 2023-07-13 09:52:50.000000 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        1 2023-07-13 09:52:50.000000 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      135 2023-07-13 09:52:50.000000 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/entry_points.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        6 2023-07-13 09:52:50.000000 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/namespace_packages.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        1 2023-07-13 08:53:47.000000 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/not-zip-safe
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)      159 2023-07-13 09:52:50.000000 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-r--   0 skynet    (1000) skynet    (1000)        6 2023-07-13 09:52:50.000000 plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/top_level.txt
```

### Comparing `plone.all_in_one_accessibility-1.0a1/DEVELOP.rst` & `plone.all_in_one_accessibility-1.0a2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/LICENSE.GPL` & `plone.all_in_one_accessibility-1.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/LICENSE.rst` & `plone.all_in_one_accessibility-1.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/docs/conf.py` & `plone.all_in_one_accessibility-1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/setup.py` & `plone.all_in_one_accessibility-1.0a2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 long_description = '\n\n'.join([
     open('README.rst').read(),
-    open('CONTRIBUTORS.rst').read(),
-    open('CHANGES.rst').read(),
+    # open('CONTRIBUTORS.rst').read(),
+    # open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='plone.all_in_one_accessibility',
-    version='1.0a1',
+    version='1.0a2',
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -33,16 +33,16 @@
     ],
     keywords='Python Plone CMS',
     author='Skynet Technologies USA LLC',
     author_email='developer3@skynettechnologies.com',
     url='https://github.com/collective/plone.all_in_one_accessibility',
     project_urls={
         'PyPI': 'https://pypi.org/project/plone.all_in_one_accessibility/',
-        'Source': 'https://github.com/collective/plone.all_in_one_accessibility',
-        'Tracker': 'https://github.com/collective/plone.all_in_one_accessibility/issues',
+        # 'Source': 'https://github.com/collective/plone.all_in_one_accessibility',
+        # 'Tracker': 'https://github.com/collective/plone.all_in_one_accessibility/issues',
         # 'Documentation': 'https://plone.all_in_one_accessibility.readthedocs.io/en/latest/',
     },
     license='GPL version 2',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['plone'],
     package_dir={'': 'src'},
     include_package_data=True,
```

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/api/services/widget/get.py` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/api/services/widget/get.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,14 +55,19 @@
         # result['widget']['items'] = items
         # return result
 
 
 class WidgetGet(Service):
 
     def reply(self):
+        print(self.context.portal_type)
+        print(self.context.aioa_key)
+        # value = ""
+        # if self.context.aioa_key == None:
+            
         # value = {"url": "https://www.skynettechnologies.com/accessibility/js/all-in-one-accessibility-js-widget-minify.js?colorcode={}&token={}&t={}&position={}".format(self.context.aioa_color,self.context.aioa_key,str(random.randint(0,999999)),self.context.aioa_place)}
         
         
         #base_URL = str(value)
         # value = '{"url":"https://www.skynettechnologies.com/accessibility/js/all-in-one-accessibility-js-widget-minify.js?colorcode=420083&token=DRUPAL6CQ9-00H7-QXQS-30ZN-KA45-KTNL&t=0.5294880354467668&position=bottom_right"}'
         
         value = '{"test":"demo"}'
```

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/browser/configure.zcml` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/configure.zcml` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.py` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/content/all_in_one_accessibility_setting.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,23 +8,32 @@
 # from plone.namedfile import field as namedfile
 from plone.supermodel import model
 
 # from plone.supermodel.directives import fieldset
 # from z3c.form.browser.radio import RadioFieldWidget
 from zope import schema
 from zope.interface import implementer
+from zope.schema.interfaces import IContextAwareDefaultFactory
+from zope.i18n import translate
+
 
 
 aioa_NOTE = "<span class='validate_pro'><p>You are currently using Free version which have limited features. </br>Please <a href='https://www.skynettechnologies.com/add-ons/product/all-in-one-accessibility/'>purchase</a> License Key for additional features on the ADA Widget</p></span><script>if(document.querySelector('#form-widgets-aioa_key').value != ''){document.querySelector('.validate_pro').style.display='none';} else {document.querySelector('.validate_pro').style.display='block';}</script>"
+
+# @provider(IContextAwareDefaultFactory)
+# def translate_header(context):
+#     # use zope.i18n translate and pass in the request as the translation context
+#     return translate(_(u"Recently Updated Indicators"), context=context.REQUEST) 
 class IAllInOneAccessibilitySetting(model.Schema):
     aioa_key = schema.TextLine(
         title='License Key',
         required=False,
         readonly=False,
-        description = aioa_NOTE
+        description = aioa_NOTE,
+        default = u""
     )
     
     aioa_color = schema.TextLine(
         title='Hex color code',
         description='You can cutomize the ADA Widget color. For example: #FF5733',
         
        
@@ -43,21 +52,17 @@
       'bottom_center',
       'bottom_right']
     )
 
 
 @implementer(IAllInOneAccessibilitySetting)
 class AllInOneAccessibilitySetting(Item):
-    """ Content-type class for IAllInOneAccessibilitySetting
-    """
     def __init__(self, id=None, **kwargs):
         catalog = api.portal.get_tool('portal_catalog')
-        brains = catalog(portal_type='All in One Accessibility setting')
+        brains = catalog(portal_type='All in One Accessibility Setting')
         if brains:
             raise Exception('Only one "All in One Accessibility setting" object is allowed per Plone instance')
 
         super(AllInOneAccessibilitySetting, self).__init__(id, **kwargs)
         
 from z3c.form.object import registerFactoryAdapter
-
-
 registerFactoryAdapter(IAllInOneAccessibilitySetting, AllInOneAccessibilitySetting)
```

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/README.rst` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/README.rst`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/update.py` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/update.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/locales/update.sh` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/locales/update.sh`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/profiles/default/types/All_in_One_Accessibility_Setting.xml` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/profiles/default/types/All_in_One_Accessibility_Setting.xml`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/setuphandlers.py` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/testing.py` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/testing.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/robot/test_ct_all_in_one_accessibility_setting.robot` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/robot/test_ct_all_in_one_accessibility_setting.robot`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/robot/test_example.robot` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/test_ct_all_in_one_accessibility_setting.py` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/test_ct_all_in_one_accessibility_setting.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/test_robot.py` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone/all_in_one_accessibility/tests/test_setup.py` & `plone.all_in_one_accessibility-1.0a2/src/plone/all_in_one_accessibility/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.all_in_one_accessibility-1.0a1/src/plone.all_in_one_accessibility.egg-info/SOURCES.txt` & `plone.all_in_one_accessibility-1.0a2/src/plone.all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

