# Comparing `tmp/mly_pipeline-0.5.5.tar.gz` & `tmp/mly_pipeline-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.5.5.tar", last modified: Mon Jul 10 15:13:23 2023, max compression
+gzip compressed data, was "mly_pipeline-0.5.7.tar", last modified: Thu Jul 13 11:30:31 2023, max compression
```

## Comparing `mly_pipeline-0.5.5.tar` & `mly_pipeline-0.5.7.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.521055 mly_pipeline-0.5.5/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.5/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.5/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.5/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-10 15:13:23.521055 mly_pipeline-0.5.5/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.5/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.047051 mly_pipeline-0.5.5/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.5/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.021050 mly_pipeline-0.5.5/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.196052 mly_pipeline-0.5.5/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.5/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.5/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.5/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.5/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.5/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.312053 mly_pipeline-0.5.5/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.342053 mly_pipeline-0.5.5/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.5/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.352053 mly_pipeline-0.5.5/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.430054 mly_pipeline-0.5.5/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.5/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.5/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.5/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.5/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.5/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.482055 mly_pipeline-0.5.5/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.5/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.5/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.5/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.5/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.512055 mly_pipeline-0.5.5/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.5/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28059 2023-07-10 09:53:54.000000 mly_pipeline-0.5.5/mly_pipeline/continuous_FAR.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.5/mly_pipeline/continuous_FAR_test.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    30861 2023-07-10 11:35:08.000000 mly_pipeline-0.5.5/mly_pipeline/initialization.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.5/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33484 2023-07-07 10:13:32.000000 mly_pipeline-0.5.5/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5596 2023-07-10 10:12:27.000000 mly_pipeline-0.5.5/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    18914 2023-07-10 10:17:57.000000 mly_pipeline-0.5.5/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17379 2023-07-10 09:45:05.000000 mly_pipeline-0.5.5/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49627 2023-07-10 11:35:33.000000 mly_pipeline-0.5.5/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.519055 mly_pipeline-0.5.5/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.5/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.5/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.517055 mly_pipeline-0.5.5/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2630 2023-07-10 15:13:23.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-10 15:12:37.000000 mly_pipeline-0.5.5/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-10 15:13:23.521055 mly_pipeline-0.5.5/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:31.303146 mly_pipeline-0.5.7/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.7/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.7/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.7/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-13 11:30:31.302147 mly_pipeline-0.5.7/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.7/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:29.338128 mly_pipeline-0.5.7/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.7/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:28.672122 mly_pipeline-0.5.7/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:29.360128 mly_pipeline-0.5.7/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.7/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.7/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2501596 2023-07-13 11:09:22.000000 mly_pipeline-0.5.7/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6427 2023-07-13 11:07:14.000000 mly_pipeline-0.5.7/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9090 2023-07-11 13:01:11.000000 mly_pipeline-0.5.7/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9551 2023-07-13 11:09:22.000000 mly_pipeline-0.5.7/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    69042 2023-07-11 13:01:11.000000 mly_pipeline-0.5.7/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:29.382128 mly_pipeline-0.5.7/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:29.772132 mly_pipeline-0.5.7/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.7/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:29.778132 mly_pipeline-0.5.7/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-13 11:06:23.000000 mly_pipeline-0.5.7/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:31.269146 mly_pipeline-0.5.7/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14813 2023-07-13 11:09:24.000000 mly_pipeline-0.5.7/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-07-13 11:09:24.000000 mly_pipeline-0.5.7/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-07-13 11:09:24.000000 mly_pipeline-0.5.7/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4472 2023-05-12 22:36:26.000000 mly_pipeline-0.5.7/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      420 2023-07-13 11:09:24.000000 mly_pipeline-0.5.7/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.7/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-07-13 11:09:24.000000 mly_pipeline-0.5.7/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-07-13 11:09:24.000000 mly_pipeline-0.5.7/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18215 2023-05-12 22:36:26.000000 mly_pipeline-0.5.7/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.7/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.7/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3011 2023-07-13 11:09:23.000000 mly_pipeline-0.5.7/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.7/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9141 2023-07-13 11:09:22.000000 mly_pipeline-0.5.7/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8507 2023-07-11 13:01:12.000000 mly_pipeline-0.5.7/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1715 2023-07-13 11:09:24.000000 mly_pipeline-0.5.7/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.7/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7976 2023-07-13 11:09:23.000000 mly_pipeline-0.5.7/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3314 2023-07-13 11:09:23.000000 mly_pipeline-0.5.7/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26439 2023-07-13 11:09:24.000000 mly_pipeline-0.5.7/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27114 2023-07-11 13:01:12.000000 mly_pipeline-0.5.7/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:31.278146 mly_pipeline-0.5.7/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-07-13 11:13:26.000000 mly_pipeline-0.5.7/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2023-07-13 11:06:23.000000 mly_pipeline-0.5.7/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.7/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1763 2023-07-13 11:09:19.000000 mly_pipeline-0.5.7/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2017 2023-07-13 10:41:45.000000 mly_pipeline-0.5.7/docs/source/runningasearchoffline.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13127 2023-07-13 10:22:53.000000 mly_pipeline-0.5.7/docs/source/runningasearchonline.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14239 2023-07-11 11:08:34.000000 mly_pipeline-0.5.7/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:31.291146 mly_pipeline-0.5.7/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.7/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    27971 2023-07-11 10:01:40.000000 mly_pipeline-0.5.7/mly_pipeline/continuous_FAR.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.7/mly_pipeline/continuous_FAR_test.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    30927 2023-07-12 09:32:36.000000 mly_pipeline-0.5.7/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.7/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33579 2023-07-11 13:15:40.000000 mly_pipeline-0.5.7/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5596 2023-07-10 10:12:27.000000 mly_pipeline-0.5.7/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    19130 2023-07-12 09:55:13.000000 mly_pipeline-0.5.7/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17439 2023-07-11 10:20:15.000000 mly_pipeline-0.5.7/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49627 2023-07-10 11:35:33.000000 mly_pipeline-0.5.7/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:31.301147 mly_pipeline-0.5.7/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.7/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.7/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-13 11:30:31.298147 mly_pipeline-0.5.7/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-13 11:30:28.000000 mly_pipeline-0.5.7/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2705 2023-07-13 11:30:28.000000 mly_pipeline-0.5.7/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-13 11:30:28.000000 mly_pipeline-0.5.7/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-13 11:30:28.000000 mly_pipeline-0.5.7/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-13 11:30:28.000000 mly_pipeline-0.5.7/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-13 11:30:28.000000 mly_pipeline-0.5.7/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-13 11:13:19.000000 mly_pipeline-0.5.7/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-13 11:30:31.303146 mly_pipeline-0.5.7/setup.cfg
```

### Comparing `mly_pipeline-0.5.5/.gitlab-ci.yml` & `mly_pipeline-0.5.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/LICENSE` & `mly_pipeline-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/PKG-INFO` & `mly_pipeline-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.5.5
+Version: 0.5.7
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.5/README.md` & `mly_pipeline-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/Makefile` & `mly_pipeline-0.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.5.7/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.5.7/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.5.7/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.5.7/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/doctrees/index.doctree` & `mly_pipeline-0.5.7/docs/build/doctrees/index.doctree`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 95a6 1800 0000 0000 008c 0f73 7068  .............sph
+00000000: 8005 9510 1900 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
 00000070: 6805 8cd0 6d6c 7950 6970 656c 696e 6520  h...mlyPipeline 
@@ -28,369 +28,375 @@
 000001b0: 2032 3032 322e 0a59 6f75 2063 616e 2061   2022..You can a
 000001c0: 6461 7074 2074 6869 7320 6669 6c65 2063  dapt this file c
 000001d0: 6f6d 706c 6574 656c 7920 746f 2079 6f75  ompletely to you
 000001e0: 7220 6c69 6b69 6e67 2c20 6275 7420 6974  r liking, but it
 000001f0: 2073 686f 756c 6420 6174 206c 6561 7374   should at least
 00000200: 0a63 6f6e 7461 696e 2074 6865 2072 6f6f  .contain the roo
 00000210: 7420 6074 6f63 7472 6565 6020 6469 7265  t `toctree` dire
-00000220: 6374 6976 652e 9485 9481 947d 9428 6805  ctive......}.(h.
-00000230: 6806 8c06 7061 7265 6e74 9468 0c75 6261  h...parent.h.uba
-00000240: 8c0a 6174 7472 6962 7574 6573 947d 9428  ..attributes.}.(
-00000250: 8c03 6964 7394 5d94 8c07 636c 6173 7365  ..ids.]...classe
-00000260: 7394 5d94 8c05 6e61 6d65 7394 5d94 8c08  s.]...names.]...
-00000270: 6475 706e 616d 6573 945d 948c 0862 6163  dupnames.]...bac
-00000280: 6b72 6566 7394 5d94 8c09 786d 6c3a 7370  krefs.]...xml:sp
-00000290: 6163 6594 8c08 7072 6573 6572 7665 9475  ace...preserve.u
-000002a0: 8c07 7461 676e 616d 6594 680a 6816 6803  ..tagname.h.h.h.
-000002b0: 6801 6803 8c06 736f 7572 6365 948c 3a2f  h.h...source..:/
-000002c0: 686f 6d65 2f76 6173 696c 6569 6f73 2e73  home/vasileios.s
-000002d0: 6b6c 6972 6973 2f6d 6c79 5f70 6970 656c  kliris/mly_pipel
-000002e0: 696e 652f 646f 6373 2f73 6f75 7263 652f  ine/docs/source/
-000002f0: 696e 6465 782e 7273 7494 8c04 6c69 6e65  index.rst...line
-00000300: 944b 0575 6268 098c 0773 6563 7469 6f6e  .K.ubh...section
-00000310: 9493 9429 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-00000320: 9428 6809 8c05 7469 746c 6594 9394 2981  .(h...title...).
-00000330: 947d 9428 6805 8c28 5765 6c63 6f6d 6520  .}.(h..(Welcome 
-00000340: 746f 204d 4c79 2d50 6970 656c 696e 6527  to MLy-Pipeline'
-00000350: 7320 646f 6375 6d65 6e74 6174 696f 6e21  s documentation!
-00000360: 9468 075d 9468 118c 2a57 656c 636f 6d65  .h.].h..*Welcome
-00000370: 2074 6f20 4d4c 792d 5069 7065 6c69 6e65   to MLy-Pipeline
-00000380: e280 9973 2064 6f63 756d 656e 7461 7469  ...s documentati
-00000390: 6f6e 2194 8594 8194 7d94 2868 0568 3268  on!.....}.(h.h2h
-000003a0: 1668 3068 0168 0368 264e 6828 4e75 6261  .h0h.h.h&Nh(Nuba
-000003b0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-000003c0: 9468 1f5d 9468 215d 9475 6825 682e 6816  .h.].h!].uh%h.h.
-000003d0: 682b 6801 6803 6826 6827 6828 4b07 7562  h+h.h.h&h'h(K.ub
-000003e0: 6809 8c09 7061 7261 6772 6170 6894 9394  h...paragraph...
-000003f0: 2981 947d 9428 6805 8cf2 4d4c 792d 5069  )..}.(h...MLy-Pi
-00000400: 7065 6c69 6e65 2069 7320 6120 636f 6c6c  peline is a coll
-00000410: 6563 7469 6f6e 206f 6620 7079 7468 6f6e  ection of python
-00000420: 2073 6372 6970 7473 2074 6861 7420 7573   scripts that us
-00000430: 6520 4d4c 7920 7061 636b 6167 6520 746f  e MLy package to
-00000440: 6f6c 7320 746f 2063 7265 6174 6520 6c6f  ols to create lo
-00000450: 772d 6c61 7465 6e63 792c 2067 7261 7669  w-latency, gravi
-00000460: 7461 7469 6f6e 616c 2077 6176 6520 7365  tational wave se
-00000470: 6172 6368 206f 6620 7375 622d 7365 636f  arch of sub-seco
-00000480: 6e64 2073 6967 6e61 6c73 2077 6974 6820  nd signals with 
-00000490: 6765 6e65 7269 6320 6d6f 7270 686f 6c6f  generic morpholo
-000004a0: 6769 6573 2e20 5468 6973 2064 6f63 756d  gies. This docum
-000004b0: 656e 7461 7469 6f6e 2077 6173 2063 7265  entation was cre
-000004c0: 6174 6564 2066 6f72 2074 6865 206e 6565  ated for the nee
-000004d0: 6420 6f66 2072 6576 6965 7769 6e67 204d  d of reviewing M
-000004e0: 4c79 2d50 6970 656c 696e 652e 9468 075d  Ly-Pipeline..h.]
-000004f0: 9468 118c f24d 4c79 2d50 6970 656c 696e  .h...MLy-Pipelin
-00000500: 6520 6973 2061 2063 6f6c 6c65 6374 696f  e is a collectio
-00000510: 6e20 6f66 2070 7974 686f 6e20 7363 7269  n of python scri
-00000520: 7074 7320 7468 6174 2075 7365 204d 4c79  pts that use MLy
-00000530: 2070 6163 6b61 6765 2074 6f6f 6c73 2074   package tools t
-00000540: 6f20 6372 6561 7465 206c 6f77 2d6c 6174  o create low-lat
-00000550: 656e 6379 2c20 6772 6176 6974 6174 696f  ency, gravitatio
-00000560: 6e61 6c20 7761 7665 2073 6561 7263 6820  nal wave search 
-00000570: 6f66 2073 7562 2d73 6563 6f6e 6420 7369  of sub-second si
-00000580: 676e 616c 7320 7769 7468 2067 656e 6572  gnals with gener
-00000590: 6963 206d 6f72 7068 6f6c 6f67 6965 732e  ic morphologies.
-000005a0: 2054 6869 7320 646f 6375 6d65 6e74 6174   This documentat
-000005b0: 696f 6e20 7761 7320 6372 6561 7465 6420  ion was created 
-000005c0: 666f 7220 7468 6520 6e65 6564 206f 6620  for the need of 
-000005d0: 7265 7669 6577 696e 6720 4d4c 792d 5069  reviewing MLy-Pi
-000005e0: 7065 6c69 6e65 2e94 8594 8194 7d94 2868  peline......}.(h
-000005f0: 0568 4268 1668 4068 0168 0368 264e 6828  .hBh.h@h.h.h&Nh(
-00000600: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
-00000610: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
-00000620: 683e 6826 6827 6828 4b09 6816 682b 6801  h>h&h'h(K.h.h+h.
-00000630: 6803 7562 6809 8c08 636f 6d70 6f75 6e64  h.ubh...compound
-00000640: 9493 9429 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-00000650: 9468 008c 0774 6f63 7472 6565 9493 9429  .h...toctree...)
-00000660: 8194 7d94 2868 0568 0668 075d 9468 177d  ..}.(h.h.h.].h.}
-00000670: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00000680: 5d94 6821 5d94 6816 8c05 696e 6465 7894  ].h!].h...index.
-00000690: 8c07 656e 7472 6965 7394 5d94 8c0c 696e  ..entries.]...in
-000006a0: 636c 7564 6566 696c 6573 945d 948c 086d  cludefiles.]...m
-000006b0: 6178 6465 7074 6894 4aff ffff ff8c 0763  axdepth.J......c
-000006c0: 6170 7469 6f6e 948c 0943 6f6e 7465 6e74  aption...Content
-000006d0: 733a 948c 0467 6c6f 6294 898c 0668 6964  s:...glob....hid
-000006e0: 6465 6e94 898c 0d69 6e63 6c75 6465 6869  den....includehi
-000006f0: 6464 656e 9489 8c08 6e75 6d62 6572 6564  dden....numbered
-00000700: 944b 008c 0a74 6974 6c65 736f 6e6c 7994  .K...titlesonly.
-00000710: 898c 0a72 6177 656e 7472 6965 7394 5d94  ...rawentries.].
-00000720: 8c0a 7261 7763 6170 7469 6f6e 9468 6575  ..rawcaption.heu
-00000730: 6825 6853 6826 6827 6828 4b0b 6816 6850  h%hSh&h'h(K.h.hP
-00000740: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00000750: 8c0f 746f 6374 7265 652d 7772 6170 7065  ..toctree-wrappe
-00000760: 7294 6168 1d5d 9468 1f5d 9468 215d 9475  r.ah.].h.].h!].u
-00000770: 6825 684e 6816 682b 6801 6803 6826 6827  h%hNh.h+h.h.h&h'
-00000780: 6828 4e75 6268 098c 046e 6f74 6594 9394  h(Nubh...note...
-00000790: 2981 947d 9428 6805 8c40 5468 6973 2070  )..}.(h..@This p
-000007a0: 726f 6a65 6374 2061 6e64 2069 7473 2064  roject and its d
-000007b0: 6f63 756d 656e 7461 7469 6f6e 2061 7265  ocumentation are
-000007c0: 2075 6e64 6572 2061 6374 6976 6520 6465   under active de
-000007d0: 7665 6c6f 706d 656e 742e 9468 075d 9468  velopment..h.].h
-000007e0: 3f29 8194 7d94 2868 0568 7968 075d 9468  ?)..}.(h.hyh.].h
-000007f0: 118c 4054 6869 7320 7072 6f6a 6563 7420  ..@This project 
-00000800: 616e 6420 6974 7320 646f 6375 6d65 6e74  and its document
-00000810: 6174 696f 6e20 6172 6520 756e 6465 7220  ation are under 
-00000820: 6163 7469 7665 2064 6576 656c 6f70 6d65  active developme
-00000830: 6e74 2e94 8594 8194 7d94 2868 0568 7968  nt......}.(h.hyh
-00000840: 1668 7b75 6261 6817 7d94 2868 195d 9468  .h{ubah.}.(h.].h
-00000850: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
-00000860: 6825 683e 6826 6827 6828 4b10 6816 6877  h%h>h&h'h(K.h.hw
-00000870: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00000880: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-00000890: 7568 1668 2b68 0168 0368 2668 2768 284e  uh.h+h.h.h&h'h(N
-000008a0: 7562 6568 177d 9428 6819 5d94 8c27 7765  ubeh.}.(h.]..'we
-000008b0: 6c63 6f6d 652d 746f 2d6d 6c79 2d70 6970  lcome-to-mly-pip
-000008c0: 656c 696e 652d 732d 646f 6375 6d65 6e74  eline-s-document
-000008d0: 6174 696f 6e94 6168 1b5d 9468 1d5d 948c  ation.ah.].h.]..
-000008e0: 2877 656c 636f 6d65 2074 6f20 6d6c 792d  (welcome to mly-
-000008f0: 7069 7065 6c69 6e65 2773 2064 6f63 756d  pipeline's docum
-00000900: 656e 7461 7469 6f6e 2194 6168 1f5d 9468  entation!.ah.].h
-00000910: 215d 9475 6825 6829 6816 6803 6801 6803  !].uh%h)h.h.h.h.
-00000920: 6826 6827 6828 4b07 7562 682a 2981 947d  h&h'h(K.ubh*)..}
-00000930: 9428 6805 6806 6807 5d94 2868 2f29 8194  .(h.h.h.].(h/)..
-00000940: 7d94 2868 058c 1249 6e64 6963 6573 2061  }.(h...Indices a
-00000950: 6e64 2074 6162 6c65 7394 6807 5d94 6811  nd tables.h.].h.
-00000960: 8c12 496e 6469 6365 7320 616e 6420 7461  ..Indices and ta
-00000970: 626c 6573 9485 9481 947d 9428 6805 689b  bles.....}.(h.h.
-00000980: 6816 6899 6801 6803 6826 4e68 284e 7562  h.h.h.h.h&Nh(Nub
-00000990: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-000009a0: 5d94 681f 5d94 6821 5d94 7568 2568 2e68  ].h.].h!].uh%h.h
-000009b0: 1668 9668 0168 0368 2668 2768 284b 1475  .h.h.h.h&h'h(K.u
-000009c0: 6268 098c 0b62 756c 6c65 745f 6c69 7374  bh...bullet_list
-000009d0: 9493 9429 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-000009e0: 9428 6809 8c09 6c69 7374 5f69 7465 6d94  .(h...list_item.
-000009f0: 9394 2981 947d 9428 6805 8c0f 3a72 6566  ..)..}.(h...:ref
-00000a00: 3a60 6765 6e69 6e64 6578 6094 6807 5d94  :`genindex`.h.].
-00000a10: 683f 2981 947d 9428 6805 68b0 6807 5d94  h?)..}.(h.h.h.].
-00000a20: 6800 8c0c 7065 6e64 696e 675f 7872 6566  h...pending_xref
-00000a30: 9493 9429 8194 7d94 2868 0568 b068 075d  ...)..}.(h.h.h.]
-00000a40: 9468 098c 0669 6e6c 696e 6594 9394 2981  .h...inline...).
-00000a50: 947d 9428 6805 68b0 6807 5d94 6811 8c08  .}.(h.h.h.].h...
-00000a60: 6765 6e69 6e64 6578 9485 9481 947d 9428  genindex.....}.(
-00000a70: 6805 6806 6816 68bc 7562 6168 177d 9428  h.h.h.h.ubah.}.(
-00000a80: 6819 5d94 681b 5d94 288c 0478 7265 6694  h.].h.].(..xref.
-00000a90: 8c03 7374 6494 8c07 7374 642d 7265 6694  ..std...std-ref.
-00000aa0: 6568 1d5d 9468 1f5d 9468 215d 9475 6825  eh.].h.].h!].uh%
-00000ab0: 68ba 6816 68b7 7562 6168 177d 9428 6819  h.h.h.ubah.}.(h.
-00000ac0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-00000ad0: 5d94 8c06 7265 6664 6f63 9468 5e8c 0972  ]...refdoc.h^..r
-00000ae0: 6566 646f 6d61 696e 9468 c78c 0772 6566  efdomain.h...ref
-00000af0: 7479 7065 948c 0372 6566 948c 0b72 6566  type...ref...ref
-00000b00: 6578 706c 6963 6974 9489 8c07 7265 6677  explicit....refw
-00000b10: 6172 6e94 888c 0972 6566 7461 7267 6574  arn....reftarget
-00000b20: 948c 0867 656e 696e 6465 7894 7568 2568  ...genindex.uh%h
-00000b30: b568 2668 2768 284b 1668 1668 b275 6261  .h&h'h(K.h.h.uba
-00000b40: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00000b50: 9468 1f5d 9468 215d 9475 6825 683e 6826  .h.].h!].uh%h>h&
-00000b60: 6827 6828 4b16 6816 68ae 7562 6168 177d  h'h(K.h.h.ubah.}
-00000b70: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00000b80: 5d94 6821 5d94 7568 2568 ac68 1668 a968  ].h!].uh%h.h.h.h
-00000b90: 0168 0368 2668 2768 284e 7562 68ad 2981  .h.h&h'h(Nubh.).
-00000ba0: 947d 9428 6805 8c0f 3a72 6566 3a60 6d6f  .}.(h...:ref:`mo
-00000bb0: 6469 6e64 6578 6094 6807 5d94 683f 2981  dindex`.h.].h?).
-00000bc0: 947d 9428 6805 68e8 6807 5d94 68b6 2981  .}.(h.h.h.].h.).
-00000bd0: 947d 9428 6805 68e8 6807 5d94 68bb 2981  .}.(h.h.h.].h.).
-00000be0: 947d 9428 6805 68e8 6807 5d94 6811 8c08  .}.(h.h.h.].h...
-00000bf0: 6d6f 6469 6e64 6578 9485 9481 947d 9428  modindex.....}.(
-00000c00: 6805 6806 6816 68f0 7562 6168 177d 9428  h.h.h.h.ubah.}.(
-00000c10: 6819 5d94 681b 5d94 2868 c68c 0373 7464  h.].h.].(h...std
-00000c20: 948c 0773 7464 2d72 6566 9465 681d 5d94  ...std-ref.eh.].
-00000c30: 681f 5d94 6821 5d94 7568 2568 ba68 1668  h.].h!].uh%h.h.h
-00000c40: ed75 6261 6817 7d94 2868 195d 9468 1b5d  .ubah.}.(h.].h.]
-00000c50: 9468 1d5d 9468 1f5d 9468 215d 948c 0672  .h.].h.].h!]...r
-00000c60: 6566 646f 6394 685e 8c09 7265 6664 6f6d  efdoc.h^..refdom
-00000c70: 6169 6e94 68fa 8c07 7265 6674 7970 6594  ain.h...reftype.
-00000c80: 8c03 7265 6694 8c0b 7265 6665 7870 6c69  ..ref...refexpli
-00000c90: 6369 7494 898c 0772 6566 7761 726e 9488  cit....refwarn..
-00000ca0: 68d8 8c08 6d6f 6469 6e64 6578 9475 6825  h...modindex.uh%
-00000cb0: 68b5 6826 6827 6828 4b17 6816 68ea 7562  h.h&h'h(K.h.h.ub
-00000cc0: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-00000cd0: 5d94 681f 5d94 6821 5d94 7568 2568 3e68  ].h.].h!].uh%h>h
-00000ce0: 2668 2768 284b 1768 1668 e675 6261 6817  &h'h(K.h.h.ubah.
-00000cf0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000d00: 1f5d 9468 215d 9475 6825 68ac 6816 68a9  .].h!].uh%h.h.h.
-00000d10: 6801 6803 6826 6827 6828 4e75 6268 ad29  h.h.h&h'h(Nubh.)
-00000d20: 8194 7d94 2868 058c 0f3a 7265 663a 6073  ..}.(h...:ref:`s
-00000d30: 6561 7263 6860 0a0a 9468 075d 9468 3f29  earch`...h.].h?)
-00000d40: 8194 7d94 2868 058c 0d3a 7265 663a 6073  ..}.(h...:ref:`s
-00000d50: 6561 7263 6860 9468 075d 9468 b629 8194  earch`.h.].h.)..
-00000d60: 7d94 2868 056a 1e01 0000 6807 5d94 68bb  }.(h.j....h.].h.
-00000d70: 2981 947d 9428 6805 6a1e 0100 0068 075d  )..}.(h.j....h.]
-00000d80: 9468 118c 0673 6561 7263 6894 8594 8194  .h...search.....
-00000d90: 7d94 2868 0568 0668 166a 2301 0000 7562  }.(h.h.h.j#...ub
-00000da0: 6168 177d 9428 6819 5d94 681b 5d94 2868  ah.}.(h.].h.].(h
-00000db0: c68c 0373 7464 948c 0773 7464 2d72 6566  ...std...std-ref
-00000dc0: 9465 681d 5d94 681f 5d94 6821 5d94 7568  .eh.].h.].h!].uh
-00000dd0: 2568 ba68 166a 2001 0000 7562 6168 177d  %h.h.j ...ubah.}
-00000de0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00000df0: 5d94 6821 5d94 8c06 7265 6664 6f63 9468  ].h!]...refdoc.h
-00000e00: 5e8c 0972 6566 646f 6d61 696e 946a 2d01  ^..refdomain.j-.
-00000e10: 0000 8c07 7265 6674 7970 6594 8c03 7265  ....reftype...re
-00000e20: 6694 8c0b 7265 6665 7870 6c69 6369 7494  f...refexplicit.
-00000e30: 898c 0772 6566 7761 726e 9488 68d8 8c06  ...refwarn..h...
-00000e40: 7365 6172 6368 9475 6825 68b5 6826 6827  search.uh%h.h&h'
-00000e50: 6828 4b18 6816 6a1c 0100 0075 6261 6817  h(K.h.j....ubah.
-00000e60: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000e70: 1f5d 9468 215d 9475 6825 683e 6826 6827  .].h!].uh%h>h&h'
-00000e80: 6828 4b18 6816 6a18 0100 0075 6261 6817  h(K.h.j....ubah.
-00000e90: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000ea0: 1f5d 9468 215d 9475 6825 68ac 6816 68a9  .].h!].uh%h.h.h.
-00000eb0: 6801 6803 6826 6827 6828 4e75 6265 6817  h.h.h&h'h(Nubeh.
-00000ec0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000ed0: 1f5d 9468 215d 948c 0662 756c 6c65 7494  .].h!]...bullet.
-00000ee0: 8c01 2a94 7568 2568 a768 2668 2768 284b  ..*.uh%h.h&h'h(K
-00000ef0: 1668 1668 9668 0168 0375 6268 2a29 8194  .h.h.h.h.ubh*)..
-00000f00: 7d94 2868 0568 0668 075d 9428 682f 2981  }.(h.h.h.].(h/).
-00000f10: 947d 9428 6805 8c08 436f 6e74 656e 7473  .}.(h...Contents
-00000f20: 9468 075d 9468 118c 0843 6f6e 7465 6e74  .h.].h...Content
-00000f30: 7394 8594 8194 7d94 2868 056a 5801 0000  s.....}.(h.jX...
-00000f40: 6816 6a56 0100 0068 0168 0368 264e 6828  h.jV...h.h.h&Nh(
-00000f50: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
-00000f60: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
-00000f70: 682e 6816 6a53 0100 0068 0168 0368 2668  h.h.jS...h.h.h&h
-00000f80: 2768 284b 1c75 6268 4f29 8194 7d94 2868  'h(K.ubhO)..}.(h
-00000f90: 0568 0668 075d 9468 5429 8194 7d94 2868  .h.h.].hT)..}.(h
-00000fa0: 0568 0668 075d 9468 177d 9428 6819 5d94  .h.h.].h.}.(h.].
-00000fb0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00000fc0: 6816 685e 685f 5d94 284e 8c0c 696e 7374  h.h^h_].(N..inst
-00000fd0: 616c 6c61 7469 6f6e 9486 944e 8c10 7365  allation...N..se
-00000fe0: 7474 696e 6775 7061 7365 6172 6368 9486  ttingupasearch..
-00000ff0: 944e 8c0e 7275 6e6e 696e 6761 7365 6172  .N..runningasear
-00001000: 6368 9486 9465 6861 5d94 286a 7101 0000  ch...eha].(jq...
-00001010: 6a73 0100 006a 7501 0000 6568 634b 0268  js...ju...ehcK.h
-00001020: 644e 6866 8968 6789 6868 8968 694b 0068  dNhf.hg.hh.hiK.h
-00001030: 6a89 686b 5d94 7568 2568 5368 2668 2768  j.hk].uh%hSh&h'h
-00001040: 284b 1e68 166a 6401 0000 7562 6168 177d  (K.h.jd...ubah.}
-00001050: 9428 6819 5d94 681b 5d94 6871 6168 1d5d  .(h.].h.].hqah.]
-00001060: 9468 1f5d 9468 215d 9475 6825 684e 6816  .h.].h!].uh%hNh.
-00001070: 6a53 0100 0068 0168 0368 2668 2768 284e  jS...h.h.h&h'h(N
-00001080: 7562 6568 177d 9428 6819 5d94 8c08 636f  ubeh.}.(h.]...co
-00001090: 6e74 656e 7473 9461 681b 5d94 681d 5d94  ntents.ah.].h.].
-000010a0: 8c08 636f 6e74 656e 7473 9461 681f 5d94  ..contents.ah.].
-000010b0: 6821 5d94 7568 2568 2968 1668 9668 0168  h!].uh%h)h.h.h.h
-000010c0: 0368 2668 2768 284b 1c75 6265 6817 7d94  .h&h'h(K.ubeh.}.
-000010d0: 2868 195d 948c 1269 6e64 6963 6573 2d61  (h.]...indices-a
-000010e0: 6e64 2d74 6162 6c65 7394 6168 1b5d 9468  nd-tables.ah.].h
-000010f0: 1d5d 948c 1269 6e64 6963 6573 2061 6e64  .]...indices and
-00001100: 2074 6162 6c65 7394 6168 1f5d 9468 215d   tables.ah.].h!]
-00001110: 9475 6825 6829 6816 6803 6801 6803 6826  .uh%h)h.h.h.h.h&
-00001120: 6827 6828 4b14 7562 6568 177d 9428 6819  h'h(K.ubeh.}.(h.
-00001130: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-00001140: 5d94 8c06 736f 7572 6365 9468 2775 6825  ]...source.h'uh%
-00001150: 6801 8c0e 6375 7272 656e 745f 736f 7572  h...current_sour
-00001160: 6365 944e 8c0c 6375 7272 656e 745f 6c69  ce.N..current_li
-00001170: 6e65 944e 8c08 7365 7474 696e 6773 948c  ne.N..settings..
-00001180: 1164 6f63 7574 696c 732e 6672 6f6e 7465  .docutils.fronte
-00001190: 6e64 948c 0656 616c 7565 7394 9394 2981  nd...Values...).
-000011a0: 947d 9428 682e 4e8c 0967 656e 6572 6174  .}.(h.N..generat
-000011b0: 6f72 944e 8c09 6461 7465 7374 616d 7094  or.N..datestamp.
-000011c0: 4e8c 0b73 6f75 7263 655f 6c69 6e6b 944e  N..source_link.N
-000011d0: 8c0a 736f 7572 6365 5f75 726c 944e 8c0d  ..source_url.N..
-000011e0: 746f 635f 6261 636b 6c69 6e6b 7394 8c05  toc_backlinks...
-000011f0: 656e 7472 7994 8c12 666f 6f74 6e6f 7465  entry...footnote
-00001200: 5f62 6163 6b6c 696e 6b73 944b 018c 0d73  _backlinks.K...s
-00001210: 6563 746e 756d 5f78 666f 726d 944b 018c  ectnum_xform.K..
-00001220: 0e73 7472 6970 5f63 6f6d 6d65 6e74 7394  .strip_comments.
-00001230: 4e8c 1b73 7472 6970 5f65 6c65 6d65 6e74  N..strip_element
-00001240: 735f 7769 7468 5f63 6c61 7373 6573 944e  s_with_classes.N
-00001250: 8c0d 7374 7269 705f 636c 6173 7365 7394  ..strip_classes.
-00001260: 4e8c 0c72 6570 6f72 745f 6c65 7665 6c94  N..report_level.
-00001270: 4b02 8c0a 6861 6c74 5f6c 6576 656c 944b  K...halt_level.K
-00001280: 058c 1165 7869 745f 7374 6174 7573 5f6c  ...exit_status_l
-00001290: 6576 656c 944b 058c 0564 6562 7567 944e  evel.K...debug.N
-000012a0: 8c0e 7761 726e 696e 675f 7374 7265 616d  ..warning_stream
-000012b0: 944e 8c09 7472 6163 6562 6163 6b94 888c  .N..traceback...
-000012c0: 0e69 6e70 7574 5f65 6e63 6f64 696e 6794  .input_encoding.
-000012d0: 8c09 7574 662d 382d 7369 6794 8c1c 696e  ..utf-8-sig...in
-000012e0: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
-000012f0: 6f72 5f68 616e 646c 6572 948c 0673 7472  or_handler...str
-00001300: 6963 7494 8c0f 6f75 7470 7574 5f65 6e63  ict...output_enc
-00001310: 6f64 696e 6794 8c05 7574 662d 3894 8c1d  oding...utf-8...
-00001320: 6f75 7470 7574 5f65 6e63 6f64 696e 675f  output_encoding_
-00001330: 6572 726f 725f 6861 6e64 6c65 7294 6ab2  error_handler.j.
-00001340: 0100 008c 0e65 7272 6f72 5f65 6e63 6f64  .....error_encod
-00001350: 696e 6794 8c05 7574 662d 3894 8c1c 6572  ing...utf-8...er
-00001360: 726f 725f 656e 636f 6469 6e67 5f65 7272  ror_encoding_err
-00001370: 6f72 5f68 616e 646c 6572 948c 1062 6163  or_handler...bac
-00001380: 6b73 6c61 7368 7265 706c 6163 6594 8c0d  kslashreplace...
-00001390: 6c61 6e67 7561 6765 5f63 6f64 6594 8c02  language_code...
-000013a0: 656e 948c 1372 6563 6f72 645f 6465 7065  en...record_depe
-000013b0: 6e64 656e 6369 6573 944e 8c06 636f 6e66  ndencies.N..conf
-000013c0: 6967 944e 8c09 6964 5f70 7265 6669 7894  ig.N..id_prefix.
-000013d0: 6806 8c0e 6175 746f 5f69 645f 7072 6566  h...auto_id_pref
-000013e0: 6978 948c 0269 6494 8c0d 6475 6d70 5f73  ix...id...dump_s
-000013f0: 6574 7469 6e67 7394 4e8c 0e64 756d 705f  ettings.N..dump_
-00001400: 696e 7465 726e 616c 7394 4e8c 0f64 756d  internals.N..dum
-00001410: 705f 7472 616e 7366 6f72 6d73 944e 8c0f  p_transforms.N..
-00001420: 6475 6d70 5f70 7365 7564 6f5f 786d 6c94  dump_pseudo_xml.
-00001430: 4e8c 1065 7870 6f73 655f 696e 7465 726e  N..expose_intern
-00001440: 616c 7394 4e8c 0e73 7472 6963 745f 7669  als.N..strict_vi
-00001450: 7369 746f 7294 4e8c 0f5f 6469 7361 626c  sitor.N.._disabl
-00001460: 655f 636f 6e66 6967 944e 8c07 5f73 6f75  e_config.N.._sou
-00001470: 7263 6594 6827 8c0c 5f64 6573 7469 6e61  rce.h'.._destina
-00001480: 7469 6f6e 944e 8c0d 5f63 6f6e 6669 675f  tion.N.._config_
-00001490: 6669 6c65 7394 5d94 8c0e 7065 705f 7265  files.]...pep_re
-000014a0: 6665 7265 6e63 6573 944e 8c0c 7065 705f  ferences.N..pep_
-000014b0: 6261 7365 5f75 726c 948c 1868 7474 7073  base_url...https
-000014c0: 3a2f 2f70 6570 732e 7079 7468 6f6e 2e6f  ://peps.python.o
-000014d0: 7267 2f94 8c15 7065 705f 6669 6c65 5f75  rg/...pep_file_u
-000014e0: 726c 5f74 656d 706c 6174 6594 8c08 7065  rl_template...pe
-000014f0: 702d 2530 3464 948c 0e72 6663 5f72 6566  p-%04d...rfc_ref
-00001500: 6572 656e 6365 7394 4e8c 0c72 6663 5f62  erences.N..rfc_b
-00001510: 6173 655f 7572 6c94 8c26 6874 7470 733a  ase_url..&https:
-00001520: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
-00001530: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
-00001540: 948c 0974 6162 5f77 6964 7468 944b 088c  ...tab_width.K..
-00001550: 1d74 7269 6d5f 666f 6f74 6e6f 7465 5f72  .trim_footnote_r
-00001560: 6566 6572 656e 6365 5f73 7061 6365 9489  eference_space..
-00001570: 8c16 6669 6c65 5f69 6e73 6572 7469 6f6e  ..file_insertion
-00001580: 5f65 6e61 626c 6564 9488 8c0b 7261 775f  _enabled....raw_
-00001590: 656e 6162 6c65 6494 4b01 8c10 7379 6e74  enabled.K...synt
-000015a0: 6178 5f68 6967 686c 6967 6874 948c 046c  ax_highlight...l
-000015b0: 6f6e 6794 8c0c 736d 6172 745f 7175 6f74  ong...smart_quot
-000015c0: 6573 9488 8c13 736d 6172 7471 756f 7465  es....smartquote
-000015d0: 735f 6c6f 6361 6c65 7394 5d94 8c1d 6368  s_locales.]...ch
-000015e0: 6172 6163 7465 725f 6c65 7665 6c5f 696e  aracter_level_in
-000015f0: 6c69 6e65 5f6d 6172 6b75 7094 898c 0e64  line_markup....d
-00001600: 6f63 7469 746c 655f 7866 6f72 6d94 898c  octitle_xform...
-00001610: 0d64 6f63 696e 666f 5f78 666f 726d 944b  .docinfo_xform.K
-00001620: 018c 1273 6563 7473 7562 7469 746c 655f  ...sectsubtitle_
-00001630: 7866 6f72 6d94 898c 0d69 6d61 6765 5f6c  xform....image_l
-00001640: 6f61 6469 6e67 948c 046c 696e 6b94 8c10  oading...link...
-00001650: 656d 6265 645f 7374 796c 6573 6865 6574  embed_stylesheet
-00001660: 9489 8c15 636c 6f61 6b5f 656d 6169 6c5f  ....cloak_email_
-00001670: 6164 6472 6573 7365 7394 888c 1173 6563  addresses....sec
-00001680: 7469 6f6e 5f73 656c 665f 6c69 6e6b 9489  tion_self_link..
-00001690: 8c0c 656d 6265 645f 696d 6167 6573 9489  ..embed_images..
-000016a0: 8c03 656e 7694 4e75 628c 0872 6570 6f72  ..env.Nub..repor
-000016b0: 7465 7294 4e8c 1069 6e64 6972 6563 745f  ter.N..indirect_
-000016c0: 7461 7267 6574 7394 5d94 8c11 7375 6273  targets.]...subs
-000016d0: 7469 7475 7469 6f6e 5f64 6566 7394 7d94  titution_defs.}.
-000016e0: 8c12 7375 6273 7469 7475 7469 6f6e 5f6e  ..substitution_n
-000016f0: 616d 6573 947d 948c 0872 6566 6e61 6d65  ames.}...refname
-00001700: 7394 7d94 8c06 7265 6669 6473 947d 948c  s.}...refids.}..
-00001710: 076e 616d 6569 6473 947d 9428 6893 6890  .nameids.}.(h.h.
-00001720: 6a8c 0100 006a 8901 0000 6a84 0100 006a  j....j....j....j
-00001730: 8101 0000 758c 096e 616d 6574 7970 6573  ....u..nametypes
-00001740: 947d 9428 6893 4e6a 8c01 0000 4e6a 8401  .}.(h.Nj....Nj..
-00001750: 0000 4e75 6819 7d94 2868 9068 2b6a 8901  ..Nuh.}.(h.h+j..
-00001760: 0000 6896 6a81 0100 006a 5301 0000 758c  ..h.j....jS...u.
-00001770: 0d66 6f6f 746e 6f74 655f 7265 6673 947d  .footnote_refs.}
-00001780: 948c 0d63 6974 6174 696f 6e5f 7265 6673  ...citation_refs
-00001790: 947d 948c 0d61 7574 6f66 6f6f 746e 6f74  .}...autofootnot
-000017a0: 6573 945d 948c 1161 7574 6f66 6f6f 746e  es.]...autofootn
-000017b0: 6f74 655f 7265 6673 945d 948c 1073 796d  ote_refs.]...sym
-000017c0: 626f 6c5f 666f 6f74 6e6f 7465 7394 5d94  bol_footnotes.].
-000017d0: 8c14 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-000017e0: 655f 7265 6673 945d 948c 0966 6f6f 746e  e_refs.]...footn
-000017f0: 6f74 6573 945d 948c 0963 6974 6174 696f  otes.]...citatio
-00001800: 6e73 945d 948c 1261 7574 6f66 6f6f 746e  ns.]...autofootn
-00001810: 6f74 655f 7374 6172 7494 4b01 8c15 7379  ote_start.K...sy
-00001820: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7374  mbol_footnote_st
-00001830: 6172 7494 4b00 8c0a 6964 5f63 6f75 6e74  art.K...id_count
-00001840: 6572 948c 0b63 6f6c 6c65 6374 696f 6e73  er...collections
-00001850: 948c 0743 6f75 6e74 6572 9493 947d 9485  ...Counter...}..
-00001860: 9452 948c 0e70 6172 7365 5f6d 6573 7361  .R...parse_messa
-00001870: 6765 7394 5d94 8c12 7472 616e 7366 6f72  ges.]...transfor
-00001880: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
-00001890: 7261 6e73 666f 726d 6572 944e 8c0a 6465  ransformer.N..de
-000018a0: 636f 7261 7469 6f6e 944e 6801 6803 7562  coration.Nh.h.ub
-000018b0: 2e                                       .
+00000220: 6374 6976 652e 9485 9481 947d 948c 0670  ctive......}...p
+00000230: 6172 656e 7494 680c 7362 618c 0a61 7474  arent.h.sba..att
+00000240: 7269 6275 7465 7394 7d94 288c 0369 6473  ributes.}.(..ids
+00000250: 945d 948c 0763 6c61 7373 6573 945d 948c  .]...classes.]..
+00000260: 056e 616d 6573 945d 948c 0864 7570 6e61  .names.]...dupna
+00000270: 6d65 7394 5d94 8c08 6261 636b 7265 6673  mes.]...backrefs
+00000280: 945d 948c 0978 6d6c 3a73 7061 6365 948c  .]...xml:space..
+00000290: 0870 7265 7365 7276 6594 758c 0774 6167  .preserve.u..tag
+000002a0: 6e61 6d65 9468 0a68 1668 038c 095f 646f  name.h.h.h..._do
+000002b0: 6375 6d65 6e74 9468 038c 0673 6f75 7263  cument.h...sourc
+000002c0: 6594 8c3a 2f68 6f6d 652f 7661 7369 6c65  e..:/home/vasile
+000002d0: 696f 732e 736b 6c69 7269 732f 6d6c 795f  ios.skliris/mly_
+000002e0: 7069 7065 6c69 6e65 2f64 6f63 732f 736f  pipeline/docs/so
+000002f0: 7572 6365 2f69 6e64 6578 2e72 7374 948c  urce/index.rst..
+00000300: 046c 696e 6594 4b05 7562 6809 8c07 7365  .line.K.ubh...se
+00000310: 6374 696f 6e94 9394 2981 947d 9428 6805  ction...)..}.(h.
+00000320: 6806 6807 5d94 2868 098c 0574 6974 6c65  h.h.].(h...title
+00000330: 9493 9429 8194 7d94 2868 058c 2857 656c  ...)..}.(h..(Wel
+00000340: 636f 6d65 2074 6f20 4d4c 792d 5069 7065  come to MLy-Pipe
+00000350: 6c69 6e65 2773 2064 6f63 756d 656e 7461  line's documenta
+00000360: 7469 6f6e 2194 6807 5d94 6811 8c2a 5765  tion!.h.].h..*We
+00000370: 6c63 6f6d 6520 746f 204d 4c79 2d50 6970  lcome to MLy-Pip
+00000380: 656c 696e 65e2 8099 7320 646f 6375 6d65  eline...s docume
+00000390: 6e74 6174 696f 6e21 9485 9481 947d 9428  ntation!.....}.(
+000003a0: 6816 6831 6826 6803 6827 4e68 294e 7562  h.h1h&h.h'Nh)Nub
+000003b0: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
+000003c0: 5d94 681f 5d94 6821 5d94 7568 2568 2f68  ].h.].h!].uh%h/h
+000003d0: 1668 2c68 2668 0368 2768 2868 294b 0775  .h,h&h.h'h(h)K.u
+000003e0: 6268 098c 0970 6172 6167 7261 7068 9493  bh...paragraph..
+000003f0: 9429 8194 7d94 2868 058c f24d 4c79 2d50  .)..}.(h...MLy-P
+00000400: 6970 656c 696e 6520 6973 2061 2063 6f6c  ipeline is a col
+00000410: 6c65 6374 696f 6e20 6f66 2070 7974 686f  lection of pytho
+00000420: 6e20 7363 7269 7074 7320 7468 6174 2075  n scripts that u
+00000430: 7365 204d 4c79 2070 6163 6b61 6765 2074  se MLy package t
+00000440: 6f6f 6c73 2074 6f20 6372 6561 7465 206c  ools to create l
+00000450: 6f77 2d6c 6174 656e 6379 2c20 6772 6176  ow-latency, grav
+00000460: 6974 6174 696f 6e61 6c20 7761 7665 2073  itational wave s
+00000470: 6561 7263 6820 6f66 2073 7562 2d73 6563  earch of sub-sec
+00000480: 6f6e 6420 7369 676e 616c 7320 7769 7468  ond signals with
+00000490: 2067 656e 6572 6963 206d 6f72 7068 6f6c   generic morphol
+000004a0: 6f67 6965 732e 2054 6869 7320 646f 6375  ogies. This docu
+000004b0: 6d65 6e74 6174 696f 6e20 7761 7320 6372  mentation was cr
+000004c0: 6561 7465 6420 666f 7220 7468 6520 6e65  eated for the ne
+000004d0: 6564 206f 6620 7265 7669 6577 696e 6720  ed of reviewing 
+000004e0: 4d4c 792d 5069 7065 6c69 6e65 2e94 6807  MLy-Pipeline..h.
+000004f0: 5d94 6811 8cf2 4d4c 792d 5069 7065 6c69  ].h...MLy-Pipeli
+00000500: 6e65 2069 7320 6120 636f 6c6c 6563 7469  ne is a collecti
+00000510: 6f6e 206f 6620 7079 7468 6f6e 2073 6372  on of python scr
+00000520: 6970 7473 2074 6861 7420 7573 6520 4d4c  ipts that use ML
+00000530: 7920 7061 636b 6167 6520 746f 6f6c 7320  y package tools 
+00000540: 746f 2063 7265 6174 6520 6c6f 772d 6c61  to create low-la
+00000550: 7465 6e63 792c 2067 7261 7669 7461 7469  tency, gravitati
+00000560: 6f6e 616c 2077 6176 6520 7365 6172 6368  onal wave search
+00000570: 206f 6620 7375 622d 7365 636f 6e64 2073   of sub-second s
+00000580: 6967 6e61 6c73 2077 6974 6820 6765 6e65  ignals with gene
+00000590: 7269 6320 6d6f 7270 686f 6c6f 6769 6573  ric morphologies
+000005a0: 2e20 5468 6973 2064 6f63 756d 656e 7461  . This documenta
+000005b0: 7469 6f6e 2077 6173 2063 7265 6174 6564  tion was created
+000005c0: 2066 6f72 2074 6865 206e 6565 6420 6f66   for the need of
+000005d0: 2072 6576 6965 7769 6e67 204d 4c79 2d50   reviewing MLy-P
+000005e0: 6970 656c 696e 652e 9485 9481 947d 9428  ipeline......}.(
+000005f0: 6816 6841 6826 6803 6827 4e68 294e 7562  h.hAh&h.h'Nh)Nub
+00000600: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
+00000610: 5d94 681f 5d94 6821 5d94 7568 2568 3f68  ].h.].h!].uh%h?h
+00000620: 2768 2868 294b 0968 1668 2c68 2668 0375  'h(h)K.h.h,h&h.u
+00000630: 6268 098c 0863 6f6d 706f 756e 6494 9394  bh...compound...
+00000640: 2981 947d 9428 6805 6806 6807 5d94 6800  )..}.(h.h.h.].h.
+00000650: 8c07 746f 6374 7265 6594 9394 2981 947d  ..toctree...)..}
+00000660: 9428 6805 6806 6807 5d94 6817 7d94 2868  .(h.h.h.].h.}.(h
+00000670: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00000680: 215d 9468 168c 0569 6e64 6578 948c 0765  !].h...index...e
+00000690: 6e74 7269 6573 945d 948c 0c69 6e63 6c75  ntries.]...inclu
+000006a0: 6465 6669 6c65 7394 5d94 8c08 6d61 7864  defiles.]...maxd
+000006b0: 6570 7468 944a ffff ffff 8c07 6361 7074  epth.J......capt
+000006c0: 696f 6e94 8c09 436f 6e74 656e 7473 3a94  ion...Contents:.
+000006d0: 8c04 676c 6f62 9489 8c06 6869 6464 656e  ..glob....hidden
+000006e0: 9489 8c0d 696e 636c 7564 6568 6964 6465  ....includehidde
+000006f0: 6e94 898c 086e 756d 6265 7265 6494 4b00  n....numbered.K.
+00000700: 8c0a 7469 746c 6573 6f6e 6c79 9489 8c0a  ..titlesonly....
+00000710: 7261 7765 6e74 7269 6573 945d 948c 0a72  rawentries.]...r
+00000720: 6177 6361 7074 696f 6e94 6866 7568 2568  awcaption.hfuh%h
+00000730: 5468 2768 2868 294b 0b68 1668 5175 6261  Th'h(h)K.h.hQuba
+00000740: 6817 7d94 2868 195d 9468 1b5d 948c 0f74  h.}.(h.].h.]...t
+00000750: 6f63 7472 6565 2d77 7261 7070 6572 9461  octree-wrapper.a
+00000760: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+00000770: 4f68 1668 2c68 2668 0368 2768 2868 294e  Oh.h,h&h.h'h(h)N
+00000780: 7562 6809 8c04 6e6f 7465 9493 9429 8194  ubh...note...)..
+00000790: 7d94 2868 058c 4054 6869 7320 7072 6f6a  }.(h..@This proj
+000007a0: 6563 7420 616e 6420 6974 7320 646f 6375  ect and its docu
+000007b0: 6d65 6e74 6174 696f 6e20 6172 6520 756e  mentation are un
+000007c0: 6465 7220 6163 7469 7665 2064 6576 656c  der active devel
+000007d0: 6f70 6d65 6e74 2e94 6807 5d94 6840 2981  opment..h.].h@).
+000007e0: 947d 9428 6805 687a 6807 5d94 6811 8c40  .}.(h.hzh.].h..@
+000007f0: 5468 6973 2070 726f 6a65 6374 2061 6e64  This project and
+00000800: 2069 7473 2064 6f63 756d 656e 7461 7469   its documentati
+00000810: 6f6e 2061 7265 2075 6e64 6572 2061 6374  on are under act
+00000820: 6976 6520 6465 7665 6c6f 706d 656e 742e  ive development.
+00000830: 9485 9481 947d 9428 6816 687c 6826 6803  .....}.(h.h|h&h.
+00000840: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+00000850: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+00000860: 5d94 7568 2568 3f68 2768 2868 294b 1068  ].uh%h?h'h(h)K.h
+00000870: 1668 7875 6261 6817 7d94 2868 195d 9468  .hxubah.}.(h.].h
+00000880: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+00000890: 6825 6876 6816 682c 6826 6803 6827 6828  h%hvh.h,h&h.h'h(
+000008a0: 6829 4e75 6265 6817 7d94 2868 195d 948c  h)Nubeh.}.(h.]..
+000008b0: 2777 656c 636f 6d65 2d74 6f2d 6d6c 792d  'welcome-to-mly-
+000008c0: 7069 7065 6c69 6e65 2d73 2d64 6f63 756d  pipeline-s-docum
+000008d0: 656e 7461 7469 6f6e 9461 681b 5d94 681d  entation.ah.].h.
+000008e0: 5d94 8c28 7765 6c63 6f6d 6520 746f 206d  ]..(welcome to m
+000008f0: 6c79 2d70 6970 656c 696e 6527 7320 646f  ly-pipeline's do
+00000900: 6375 6d65 6e74 6174 696f 6e21 9461 681f  cumentation!.ah.
+00000910: 5d94 6821 5d94 7568 2568 2a68 1668 0368  ].h!].uh%h*h.h.h
+00000920: 2668 0368 2768 2868 294b 0775 6268 2b29  &h.h'h(h)K.ubh+)
+00000930: 8194 7d94 2868 0568 0668 075d 9428 6830  ..}.(h.h.h.].(h0
+00000940: 2981 947d 9428 6805 8c12 496e 6469 6365  )..}.(h...Indice
+00000950: 7320 616e 6420 7461 626c 6573 9468 075d  s and tables.h.]
+00000960: 9468 118c 1249 6e64 6963 6573 2061 6e64  .h...Indices and
+00000970: 2074 6162 6c65 7394 8594 8194 7d94 2868   tables.....}.(h
+00000980: 1668 9a68 2668 0368 274e 6829 4e75 6261  .h.h&h.h'Nh)Nuba
+00000990: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+000009a0: 9468 1f5d 9468 215d 9475 6825 682f 6816  .h.].h!].uh%h/h.
+000009b0: 6897 6826 6803 6827 6828 6829 4b14 7562  h.h&h.h'h(h)K.ub
+000009c0: 6809 8c0b 6275 6c6c 6574 5f6c 6973 7494  h...bullet_list.
+000009d0: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+000009e0: 2868 098c 096c 6973 745f 6974 656d 9493  (h...list_item..
+000009f0: 9429 8194 7d94 2868 058c 0f3a 7265 663a  .)..}.(h...:ref:
+00000a00: 6067 656e 696e 6465 7860 9468 075d 9468  `genindex`.h.].h
+00000a10: 4029 8194 7d94 2868 0568 b168 075d 9468  @)..}.(h.h.h.].h
+00000a20: 008c 0c70 656e 6469 6e67 5f78 7265 6694  ...pending_xref.
+00000a30: 9394 2981 947d 9428 6805 68b1 6807 5d94  ..)..}.(h.h.h.].
+00000a40: 6809 8c06 696e 6c69 6e65 9493 9429 8194  h...inline...)..
+00000a50: 7d94 2868 0568 b168 075d 9468 118c 0867  }.(h.h.h.].h...g
+00000a60: 656e 696e 6465 7894 8594 8194 7d94 2868  enindex.....}.(h
+00000a70: 1668 bd68 2668 0368 274e 6829 4e75 6261  .h.h&h.h'Nh)Nuba
+00000a80: 6817 7d94 2868 195d 9468 1b5d 9428 8c04  h.}.(h.].h.].(..
+00000a90: 7872 6566 948c 0373 7464 948c 0773 7464  xref...std...std
+00000aa0: 2d72 6566 9465 681d 5d94 681f 5d94 6821  -ref.eh.].h.].h!
+00000ab0: 5d94 7568 2568 bb68 1668 b875 6261 6817  ].uh%h.h.h.ubah.
+00000ac0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00000ad0: 1f5d 9468 215d 948c 0672 6566 646f 6394  .].h!]...refdoc.
+00000ae0: 685f 8c09 7265 6664 6f6d 6169 6e94 68c8  h_..refdomain.h.
+00000af0: 8c07 7265 6674 7970 6594 8c03 7265 6694  ..reftype...ref.
+00000b00: 8c0b 7265 6665 7870 6c69 6369 7494 898c  ..refexplicit...
+00000b10: 0772 6566 7761 726e 9488 8c09 7265 6674  .refwarn....reft
+00000b20: 6172 6765 7494 8c08 6765 6e69 6e64 6578  arget...genindex
+00000b30: 9475 6825 68b6 6827 6828 6829 4b16 6816  .uh%h.h'h(h)K.h.
+00000b40: 68b3 7562 6168 177d 9428 6819 5d94 681b  h.ubah.}.(h.].h.
+00000b50: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00000b60: 2568 3f68 2768 2868 294b 1668 1668 af75  %h?h'h(h)K.h.h.u
+00000b70: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00000b80: 1d5d 9468 1f5d 9468 215d 9475 6825 68ad  .].h.].h!].uh%h.
+00000b90: 6816 68aa 6826 6803 6827 6828 6829 4e75  h.h.h&h.h'h(h)Nu
+00000ba0: 6268 ae29 8194 7d94 2868 058c 0f3a 7265  bh.)..}.(h...:re
+00000bb0: 663a 606d 6f64 696e 6465 7860 9468 075d  f:`modindex`.h.]
+00000bc0: 9468 4029 8194 7d94 2868 0568 e968 075d  .h@)..}.(h.h.h.]
+00000bd0: 9468 b729 8194 7d94 2868 0568 e968 075d  .h.)..}.(h.h.h.]
+00000be0: 9468 bc29 8194 7d94 2868 0568 e968 075d  .h.)..}.(h.h.h.]
+00000bf0: 9468 118c 086d 6f64 696e 6465 7894 8594  .h...modindex...
+00000c00: 8194 7d94 2868 1668 f168 2668 0368 274e  ..}.(h.h.h&h.h'N
+00000c10: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
+00000c20: 1b5d 9428 68c7 8c03 7374 6494 8c07 7374  .].(h...std...st
+00000c30: 642d 7265 6694 6568 1d5d 9468 1f5d 9468  d-ref.eh.].h.].h
+00000c40: 215d 9475 6825 68bb 6816 68ee 7562 6168  !].uh%h.h.h.ubah
+00000c50: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000c60: 681f 5d94 6821 5d94 8c06 7265 6664 6f63  h.].h!]...refdoc
+00000c70: 9468 5f8c 0972 6566 646f 6d61 696e 9468  .h_..refdomain.h
+00000c80: fb8c 0772 6566 7479 7065 948c 0372 6566  ...reftype...ref
+00000c90: 948c 0b72 6566 6578 706c 6963 6974 9489  ...refexplicit..
+00000ca0: 8c07 7265 6677 6172 6e94 8868 d98c 086d  ..refwarn..h...m
+00000cb0: 6f64 696e 6465 7894 7568 2568 b668 2768  odindex.uh%h.h'h
+00000cc0: 2868 294b 1768 1668 eb75 6261 6817 7d94  (h)K.h.h.ubah.}.
+00000cd0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00000ce0: 9468 215d 9475 6825 683f 6827 6828 6829  .h!].uh%h?h'h(h)
+00000cf0: 4b17 6816 68e7 7562 6168 177d 9428 6819  K.h.h.ubah.}.(h.
+00000d00: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+00000d10: 5d94 7568 2568 ad68 1668 aa68 2668 0368  ].uh%h.h.h.h&h.h
+00000d20: 2768 2868 294e 7562 68ae 2981 947d 9428  'h(h)Nubh.)..}.(
+00000d30: 6805 8c0f 3a72 6566 3a60 7365 6172 6368  h...:ref:`search
+00000d40: 600a 0a94 6807 5d94 6840 2981 947d 9428  `...h.].h@)..}.(
+00000d50: 6805 8c0d 3a72 6566 3a60 7365 6172 6368  h...:ref:`search
+00000d60: 6094 6807 5d94 68b7 2981 947d 9428 6805  `.h.].h.)..}.(h.
+00000d70: 6a1f 0100 0068 075d 9468 bc29 8194 7d94  j....h.].h.)..}.
+00000d80: 2868 056a 1f01 0000 6807 5d94 6811 8c06  (h.j....h.].h...
+00000d90: 7365 6172 6368 9485 9481 947d 9428 6816  search.....}.(h.
+00000da0: 6a24 0100 0068 2668 0368 274e 6829 4e75  j$...h&h.h'Nh)Nu
+00000db0: 6261 6817 7d94 2868 195d 9468 1b5d 9428  bah.}.(h.].h.].(
+00000dc0: 68c7 8c03 7374 6494 8c07 7374 642d 7265  h...std...std-re
+00000dd0: 6694 6568 1d5d 9468 1f5d 9468 215d 9475  f.eh.].h.].h!].u
+00000de0: 6825 68bb 6816 6a21 0100 0075 6261 6817  h%h.h.j!...ubah.
+00000df0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00000e00: 1f5d 9468 215d 948c 0672 6566 646f 6394  .].h!]...refdoc.
+00000e10: 685f 8c09 7265 6664 6f6d 6169 6e94 6a2e  h_..refdomain.j.
+00000e20: 0100 008c 0772 6566 7479 7065 948c 0372  .....reftype...r
+00000e30: 6566 948c 0b72 6566 6578 706c 6963 6974  ef...refexplicit
+00000e40: 9489 8c07 7265 6677 6172 6e94 8868 d98c  ....refwarn..h..
+00000e50: 0673 6561 7263 6894 7568 2568 b668 2768  .search.uh%h.h'h
+00000e60: 2868 294b 1868 166a 1d01 0000 7562 6168  (h)K.h.j....ubah
+00000e70: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000e80: 681f 5d94 6821 5d94 7568 2568 3f68 2768  h.].h!].uh%h?h'h
+00000e90: 2868 294b 1868 166a 1901 0000 7562 6168  (h)K.h.j....ubah
+00000ea0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000eb0: 681f 5d94 6821 5d94 7568 2568 ad68 1668  h.].h!].uh%h.h.h
+00000ec0: aa68 2668 0368 2768 2868 294e 7562 6568  .h&h.h'h(h)Nubeh
+00000ed0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000ee0: 681f 5d94 6821 5d94 8c06 6275 6c6c 6574  h.].h!]...bullet
+00000ef0: 948c 012a 9475 6825 68a8 6827 6828 6829  ...*.uh%h.h'h(h)
+00000f00: 4b16 6816 6897 6826 6803 7562 682b 2981  K.h.h.h&h.ubh+).
+00000f10: 947d 9428 6805 6806 6807 5d94 2868 3029  .}.(h.h.h.].(h0)
+00000f20: 8194 7d94 2868 058c 0843 6f6e 7465 6e74  ..}.(h...Content
+00000f30: 7394 6807 5d94 6811 8c08 436f 6e74 656e  s.h.].h...Conten
+00000f40: 7473 9485 9481 947d 9428 6816 6a57 0100  ts.....}.(h.jW..
+00000f50: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
+00000f60: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00000f70: 1f5d 9468 215d 9475 6825 682f 6816 6a54  .].h!].uh%h/h.jT
+00000f80: 0100 0068 2668 0368 2768 2868 294b 1c75  ...h&h.h'h(h)K.u
+00000f90: 6268 5029 8194 7d94 2868 0568 0668 075d  bhP)..}.(h.h.h.]
+00000fa0: 9468 5529 8194 7d94 2868 0568 0668 075d  .hU)..}.(h.h.h.]
+00000fb0: 9468 177d 9428 6819 5d94 681b 5d94 681d  .h.}.(h.].h.].h.
+00000fc0: 5d94 681f 5d94 6821 5d94 6816 685f 6860  ].h.].h!].h.h_h`
+00000fd0: 5d94 284e 8c0c 696e 7374 616c 6c61 7469  ].(N..installati
+00000fe0: 6f6e 9486 944e 8c10 7365 7474 696e 6775  on...N..settingu
+00000ff0: 7061 7365 6172 6368 9486 944e 8c0e 7275  pasearch...N..ru
+00001000: 6e6e 696e 6761 7365 6172 6368 9486 944e  nningasearch...N
+00001010: 8c15 7275 6e6e 696e 6761 7365 6172 6368  ..runningasearch
+00001020: 6f66 666c 696e 6594 8694 4e8c 1472 756e  offline...N..run
+00001030: 6e69 6e67 6173 6561 7263 686f 6e6c 696e  ningasearchonlin
+00001040: 6594 8694 6568 625d 9428 6a72 0100 006a  e...ehb].(jr...j
+00001050: 7401 0000 6a76 0100 006a 7801 0000 6a7a  t...jv...jx...jz
+00001060: 0100 0065 6864 4b02 6865 4e68 6789 6868  ...ehdK.heNhg.hh
+00001070: 8968 6989 686a 4b00 686b 8968 6c5d 9475  .hi.hjK.hk.hl].u
+00001080: 6825 6854 6827 6828 6829 4b1e 6816 6a65  h%hTh'h(h)K.h.je
+00001090: 0100 0075 6261 6817 7d94 2868 195d 9468  ...ubah.}.(h.].h
+000010a0: 1b5d 9468 7261 681d 5d94 681f 5d94 6821  .].hrah.].h.].h!
+000010b0: 5d94 7568 2568 4f68 166a 5401 0000 6826  ].uh%hOh.jT...h&
+000010c0: 6803 6827 6828 6829 4e75 6265 6817 7d94  h.h'h(h)Nubeh.}.
+000010d0: 2868 195d 948c 0863 6f6e 7465 6e74 7394  (h.]...contents.
+000010e0: 6168 1b5d 9468 1d5d 948c 0863 6f6e 7465  ah.].h.]...conte
+000010f0: 6e74 7394 6168 1f5d 9468 215d 9475 6825  nts.ah.].h!].uh%
+00001100: 682a 6816 6897 6826 6803 6827 6828 6829  h*h.h.h&h.h'h(h)
+00001110: 4b1c 7562 6568 177d 9428 6819 5d94 8c12  K.ubeh.}.(h.]...
+00001120: 696e 6469 6365 732d 616e 642d 7461 626c  indices-and-tabl
+00001130: 6573 9461 681b 5d94 681d 5d94 8c12 696e  es.ah.].h.]...in
+00001140: 6469 6365 7320 616e 6420 7461 626c 6573  dices and tables
+00001150: 9461 681f 5d94 6821 5d94 7568 2568 2a68  .ah.].h!].uh%h*h
+00001160: 1668 0368 2668 0368 2768 2868 294b 1475  .h.h&h.h'h(h)K.u
+00001170: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
+00001180: 1d5d 9468 1f5d 9468 215d 948c 0673 6f75  .].h.].h!]...sou
+00001190: 7263 6594 6828 7568 2568 018c 0e63 7572  rce.h(uh%h...cur
+000011a0: 7265 6e74 5f73 6f75 7263 6594 4e8c 0c63  rent_source.N..c
+000011b0: 7572 7265 6e74 5f6c 696e 6594 4e8c 0873  urrent_line.N..s
+000011c0: 6574 7469 6e67 7394 8c11 646f 6375 7469  ettings...docuti
+000011d0: 6c73 2e66 726f 6e74 656e 6494 8c06 5661  ls.frontend...Va
+000011e0: 6c75 6573 9493 9429 8194 7d94 288c 066f  lues...)..}.(..o
+000011f0: 7574 7075 7494 4e68 2f4e 8c09 6765 6e65  utput.Nh/N..gene
+00001200: 7261 746f 7294 4e8c 0964 6174 6573 7461  rator.N..datesta
+00001210: 6d70 944e 8c0b 736f 7572 6365 5f6c 696e  mp.N..source_lin
+00001220: 6b94 4e8c 0a73 6f75 7263 655f 7572 6c94  k.N..source_url.
+00001230: 4e8c 0d74 6f63 5f62 6163 6b6c 696e 6b73  N..toc_backlinks
+00001240: 948c 0565 6e74 7279 948c 1266 6f6f 746e  ...entry...footn
+00001250: 6f74 655f 6261 636b 6c69 6e6b 7394 4b01  ote_backlinks.K.
+00001260: 8c0d 7365 6374 6e75 6d5f 7866 6f72 6d94  ..sectnum_xform.
+00001270: 4b01 8c0e 7374 7269 705f 636f 6d6d 656e  K...strip_commen
+00001280: 7473 944e 8c1b 7374 7269 705f 656c 656d  ts.N..strip_elem
+00001290: 656e 7473 5f77 6974 685f 636c 6173 7365  ents_with_classe
+000012a0: 7394 4e8c 0d73 7472 6970 5f63 6c61 7373  s.N..strip_class
+000012b0: 6573 944e 8c0c 7265 706f 7274 5f6c 6576  es.N..report_lev
+000012c0: 656c 944b 028c 0a68 616c 745f 6c65 7665  el.K...halt_leve
+000012d0: 6c94 4b05 8c11 6578 6974 5f73 7461 7475  l.K...exit_statu
+000012e0: 735f 6c65 7665 6c94 4b05 8c05 6465 6275  s_level.K...debu
+000012f0: 6794 4e8c 0e77 6172 6e69 6e67 5f73 7472  g.N..warning_str
+00001300: 6561 6d94 4e8c 0974 7261 6365 6261 636b  eam.N..traceback
+00001310: 9488 8c0e 696e 7075 745f 656e 636f 6469  ....input_encodi
+00001320: 6e67 948c 0975 7466 2d38 2d73 6967 948c  ng...utf-8-sig..
+00001330: 1c69 6e70 7574 5f65 6e63 6f64 696e 675f  .input_encoding_
+00001340: 6572 726f 725f 6861 6e64 6c65 7294 8c06  error_handler...
+00001350: 7374 7269 6374 948c 0f6f 7574 7075 745f  strict...output_
+00001360: 656e 636f 6469 6e67 948c 0575 7466 2d38  encoding...utf-8
+00001370: 948c 1d6f 7574 7075 745f 656e 636f 6469  ...output_encodi
+00001380: 6e67 5f65 7272 6f72 5f68 616e 646c 6572  ng_error_handler
+00001390: 946a b801 0000 8c0e 6572 726f 725f 656e  .j......error_en
+000013a0: 636f 6469 6e67 948c 0575 7466 2d38 948c  coding...utf-8..
+000013b0: 1c65 7272 6f72 5f65 6e63 6f64 696e 675f  .error_encoding_
+000013c0: 6572 726f 725f 6861 6e64 6c65 7294 8c10  error_handler...
+000013d0: 6261 636b 736c 6173 6872 6570 6c61 6365  backslashreplace
+000013e0: 948c 0d6c 616e 6775 6167 655f 636f 6465  ...language_code
+000013f0: 948c 0265 6e94 8c13 7265 636f 7264 5f64  ...en...record_d
+00001400: 6570 656e 6465 6e63 6965 7394 4e8c 0663  ependencies.N..c
+00001410: 6f6e 6669 6794 4e8c 0969 645f 7072 6566  onfig.N..id_pref
+00001420: 6978 9468 068c 0e61 7574 6f5f 6964 5f70  ix.h...auto_id_p
+00001430: 7265 6669 7894 8c02 6964 948c 0d64 756d  refix...id...dum
+00001440: 705f 7365 7474 696e 6773 944e 8c0e 6475  p_settings.N..du
+00001450: 6d70 5f69 6e74 6572 6e61 6c73 944e 8c0f  mp_internals.N..
+00001460: 6475 6d70 5f74 7261 6e73 666f 726d 7394  dump_transforms.
+00001470: 4e8c 0f64 756d 705f 7073 6575 646f 5f78  N..dump_pseudo_x
+00001480: 6d6c 944e 8c10 6578 706f 7365 5f69 6e74  ml.N..expose_int
+00001490: 6572 6e61 6c73 944e 8c0e 7374 7269 6374  ernals.N..strict
+000014a0: 5f76 6973 6974 6f72 944e 8c0f 5f64 6973  _visitor.N.._dis
+000014b0: 6162 6c65 5f63 6f6e 6669 6794 4e8c 075f  able_config.N.._
+000014c0: 736f 7572 6365 9468 288c 0c5f 6465 7374  source.h(.._dest
+000014d0: 696e 6174 696f 6e94 4e8c 0d5f 636f 6e66  ination.N.._conf
+000014e0: 6967 5f66 696c 6573 945d 948c 1666 696c  ig_files.]...fil
+000014f0: 655f 696e 7365 7274 696f 6e5f 656e 6162  e_insertion_enab
+00001500: 6c65 6494 888c 0b72 6177 5f65 6e61 626c  led....raw_enabl
+00001510: 6564 944b 018c 116c 696e 655f 6c65 6e67  ed.K...line_leng
+00001520: 7468 5f6c 696d 6974 944d 1027 8c0e 7065  th_limit.M.'..pe
+00001530: 705f 7265 6665 7265 6e63 6573 944e 8c0c  p_references.N..
+00001540: 7065 705f 6261 7365 5f75 726c 948c 1868  pep_base_url...h
+00001550: 7474 7073 3a2f 2f70 6570 732e 7079 7468  ttps://peps.pyth
+00001560: 6f6e 2e6f 7267 2f94 8c15 7065 705f 6669  on.org/...pep_fi
+00001570: 6c65 5f75 726c 5f74 656d 706c 6174 6594  le_url_template.
+00001580: 8c08 7065 702d 2530 3464 948c 0e72 6663  ..pep-%04d...rfc
+00001590: 5f72 6566 6572 656e 6365 7394 4e8c 0c72  _references.N..r
+000015a0: 6663 5f62 6173 655f 7572 6c94 8c26 6874  fc_base_url..&ht
+000015b0: 7470 733a 2f2f 6461 7461 7472 6163 6b65  tps://datatracke
+000015c0: 722e 6965 7466 2e6f 7267 2f64 6f63 2f68  r.ietf.org/doc/h
+000015d0: 746d 6c2f 948c 0974 6162 5f77 6964 7468  tml/...tab_width
+000015e0: 944b 088c 1d74 7269 6d5f 666f 6f74 6e6f  .K...trim_footno
+000015f0: 7465 5f72 6566 6572 656e 6365 5f73 7061  te_reference_spa
+00001600: 6365 9489 8c10 7379 6e74 6178 5f68 6967  ce....syntax_hig
+00001610: 686c 6967 6874 948c 046c 6f6e 6794 8c0c  hlight...long...
+00001620: 736d 6172 745f 7175 6f74 6573 9488 8c13  smart_quotes....
+00001630: 736d 6172 7471 756f 7465 735f 6c6f 6361  smartquotes_loca
+00001640: 6c65 7394 5d94 8c1d 6368 6172 6163 7465  les.]...characte
+00001650: 725f 6c65 7665 6c5f 696e 6c69 6e65 5f6d  r_level_inline_m
+00001660: 6172 6b75 7094 898c 0e64 6f63 7469 746c  arkup....doctitl
+00001670: 655f 7866 6f72 6d94 898c 0d64 6f63 696e  e_xform....docin
+00001680: 666f 5f78 666f 726d 944b 018c 1273 6563  fo_xform.K...sec
+00001690: 7473 7562 7469 746c 655f 7866 6f72 6d94  tsubtitle_xform.
+000016a0: 898c 0d69 6d61 6765 5f6c 6f61 6469 6e67  ...image_loading
+000016b0: 948c 046c 696e 6b94 8c10 656d 6265 645f  ...link...embed_
+000016c0: 7374 796c 6573 6865 6574 9489 8c15 636c  stylesheet....cl
+000016d0: 6f61 6b5f 656d 6169 6c5f 6164 6472 6573  oak_email_addres
+000016e0: 7365 7394 888c 1173 6563 7469 6f6e 5f73  ses....section_s
+000016f0: 656c 665f 6c69 6e6b 9489 8c03 656e 7694  elf_link....env.
+00001700: 4e75 628c 0872 6570 6f72 7465 7294 4e8c  Nub..reporter.N.
+00001710: 1069 6e64 6972 6563 745f 7461 7267 6574  .indirect_target
+00001720: 7394 5d94 8c11 7375 6273 7469 7475 7469  s.]...substituti
+00001730: 6f6e 5f64 6566 7394 7d94 8c12 7375 6273  on_defs.}...subs
+00001740: 7469 7475 7469 6f6e 5f6e 616d 6573 947d  titution_names.}
+00001750: 948c 0872 6566 6e61 6d65 7394 7d94 8c06  ...refnames.}...
+00001760: 7265 6669 6473 947d 948c 076e 616d 6569  refids.}...namei
+00001770: 6473 947d 9428 6894 6891 6a91 0100 006a  ds.}.(h.h.j....j
+00001780: 8e01 0000 6a89 0100 006a 8601 0000 758c  ....j....j....u.
+00001790: 096e 616d 6574 7970 6573 947d 9428 6894  .nametypes.}.(h.
+000017a0: 896a 9101 0000 896a 8901 0000 8975 6819  .j.....j.....uh.
+000017b0: 7d94 2868 9168 2c6a 8e01 0000 6897 6a86  }.(h.h,j....h.j.
+000017c0: 0100 006a 5401 0000 758c 0d66 6f6f 746e  ...jT...u..footn
+000017d0: 6f74 655f 7265 6673 947d 948c 0d63 6974  ote_refs.}...cit
+000017e0: 6174 696f 6e5f 7265 6673 947d 948c 0d61  ation_refs.}...a
+000017f0: 7574 6f66 6f6f 746e 6f74 6573 945d 948c  utofootnotes.]..
+00001800: 1161 7574 6f66 6f6f 746e 6f74 655f 7265  .autofootnote_re
+00001810: 6673 945d 948c 1073 796d 626f 6c5f 666f  fs.]...symbol_fo
+00001820: 6f74 6e6f 7465 7394 5d94 8c14 7379 6d62  otnotes.]...symb
+00001830: 6f6c 5f66 6f6f 746e 6f74 655f 7265 6673  ol_footnote_refs
+00001840: 945d 948c 0966 6f6f 746e 6f74 6573 945d  .]...footnotes.]
+00001850: 948c 0963 6974 6174 696f 6e73 945d 948c  ...citations.]..
+00001860: 1261 7574 6f66 6f6f 746e 6f74 655f 7374  .autofootnote_st
+00001870: 6172 7494 4b01 8c15 7379 6d62 6f6c 5f66  art.K...symbol_f
+00001880: 6f6f 746e 6f74 655f 7374 6172 7494 4b00  ootnote_start.K.
+00001890: 8c0a 6964 5f63 6f75 6e74 6572 948c 0b63  ..id_counter...c
+000018a0: 6f6c 6c65 6374 696f 6e73 948c 0743 6f75  ollections...Cou
+000018b0: 6e74 6572 9493 947d 9485 9452 948c 0e70  nter...}...R...p
+000018c0: 6172 7365 5f6d 6573 7361 6765 7394 5d94  arse_messages.].
+000018d0: 8c12 7472 616e 7366 6f72 6d5f 6d65 7373  ..transform_mess
+000018e0: 6167 6573 945d 948c 0b74 7261 6e73 666f  ages.]...transfo
+000018f0: 726d 6572 944e 8c0b 696e 636c 7564 655f  rmer.N..include_
+00001900: 6c6f 6794 5d94 8c0a 6465 636f 7261 7469  log.]...decorati
+00001910: 6f6e 944e 6826 6803 7562 2e              on.Nh&h.ub.
```

### Comparing `mly_pipeline-0.5.5/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.5.7/docs/build/doctrees/installation.doctree`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9587 2300 0000 0000 008c 0f73 7068  ....#........sph
+00000000: 8005 9577 2300 0000 0000 008c 0f73 7068  ...w#........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -527,44 +527,43 @@
 000020e0: 6f5f 7866 6f72 6d94 4b01 8c12 7365 6374  o_xform.K...sect
 000020f0: 7375 6274 6974 6c65 5f78 666f 726d 9489  subtitle_xform..
 00002100: 8c0d 696d 6167 655f 6c6f 6164 696e 6794  ..image_loading.
 00002110: 8c04 6c69 6e6b 948c 1065 6d62 6564 5f73  ..link...embed_s
 00002120: 7479 6c65 7368 6565 7494 898c 1563 6c6f  tylesheet....clo
 00002130: 616b 5f65 6d61 696c 5f61 6464 7265 7373  ak_email_address
 00002140: 6573 9488 8c11 7365 6374 696f 6e5f 7365  es....section_se
-00002150: 6c66 5f6c 696e 6b94 898c 0c65 6d62 6564  lf_link....embed
-00002160: 5f69 6d61 6765 7394 898c 0365 6e76 944e  _images....env.N
-00002170: 7562 8c08 7265 706f 7274 6572 944e 8c10  ub..reporter.N..
-00002180: 696e 6469 7265 6374 5f74 6172 6765 7473  indirect_targets
-00002190: 945d 948c 1173 7562 7374 6974 7574 696f  .]...substitutio
-000021a0: 6e5f 6465 6673 947d 948c 1273 7562 7374  n_defs.}...subst
-000021b0: 6974 7574 696f 6e5f 6e61 6d65 7394 7d94  itution_names.}.
-000021c0: 8c08 7265 666e 616d 6573 947d 948c 0672  ..refnames.}...r
-000021d0: 6566 6964 7394 7d94 8c07 6e61 6d65 6964  efids.}...nameid
-000021e0: 7394 7d94 286a 9101 0000 6a8e 0100 0068  s.}.(j....j....h
-000021f0: 5668 5368 fb68 f86a 8901 0000 6a86 0100  VhSh.h.j....j...
-00002200: 0075 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
-00002210: 286a 9101 0000 8968 5688 68fb 896a 8901  (j.....hV.h..j..
-00002220: 0000 8975 6821 7d94 286a 8e01 0000 680c  ...uh!}.(j....h.
-00002230: 6853 684d 68f8 6865 6a86 0100 0068 fe75  hShMh.hej....h.u
-00002240: 8c0d 666f 6f74 6e6f 7465 5f72 6566 7394  ..footnote_refs.
-00002250: 7d94 8c0d 6369 7461 7469 6f6e 5f72 6566  }...citation_ref
-00002260: 7394 7d94 8c0d 6175 746f 666f 6f74 6e6f  s.}...autofootno
-00002270: 7465 7394 5d94 8c11 6175 746f 666f 6f74  tes.]...autofoot
-00002280: 6e6f 7465 5f72 6566 7394 5d94 8c10 7379  note_refs.]...sy
-00002290: 6d62 6f6c 5f66 6f6f 746e 6f74 6573 945d  mbol_footnotes.]
-000022a0: 948c 1473 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
-000022b0: 7465 5f72 6566 7394 5d94 8c09 666f 6f74  te_refs.]...foot
-000022c0: 6e6f 7465 7394 5d94 8c09 6369 7461 7469  notes.]...citati
-000022d0: 6f6e 7394 5d94 8c12 6175 746f 666f 6f74  ons.]...autofoot
-000022e0: 6e6f 7465 5f73 7461 7274 944b 018c 1573  note_start.K...s
-000022f0: 796d 626f 6c5f 666f 6f74 6e6f 7465 5f73  ymbol_footnote_s
-00002300: 7461 7274 944b 008c 0a69 645f 636f 756e  tart.K...id_coun
-00002310: 7465 7294 8c0b 636f 6c6c 6563 7469 6f6e  ter...collection
-00002320: 7394 8c07 436f 756e 7465 7294 9394 7d94  s...Counter...}.
-00002330: 8594 5294 8c0e 7061 7273 655f 6d65 7373  ..R...parse_mess
-00002340: 6167 6573 945d 948c 1274 7261 6e73 666f  ages.]...transfo
-00002350: 726d 5f6d 6573 7361 6765 7394 5d94 8c0b  rm_messages.]...
-00002360: 7472 616e 7366 6f72 6d65 7294 4e8c 0b69  transformer.N..i
-00002370: 6e63 6c75 6465 5f6c 6f67 945d 948c 0a64  nclude_log.]...d
-00002380: 6563 6f72 6174 696f 6e94 4e68 1c68 0375  ecoration.Nh.h.u
-00002390: 622e                                     b.
+00002150: 6c66 5f6c 696e 6b94 898c 0365 6e76 944e  lf_link....env.N
+00002160: 7562 8c08 7265 706f 7274 6572 944e 8c10  ub..reporter.N..
+00002170: 696e 6469 7265 6374 5f74 6172 6765 7473  indirect_targets
+00002180: 945d 948c 1173 7562 7374 6974 7574 696f  .]...substitutio
+00002190: 6e5f 6465 6673 947d 948c 1273 7562 7374  n_defs.}...subst
+000021a0: 6974 7574 696f 6e5f 6e61 6d65 7394 7d94  itution_names.}.
+000021b0: 8c08 7265 666e 616d 6573 947d 948c 0672  ..refnames.}...r
+000021c0: 6566 6964 7394 7d94 8c07 6e61 6d65 6964  efids.}...nameid
+000021d0: 7394 7d94 286a 9101 0000 6a8e 0100 0068  s.}.(j....j....h
+000021e0: 5668 5368 fb68 f86a 8901 0000 6a86 0100  VhSh.h.j....j...
+000021f0: 0075 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
+00002200: 286a 9101 0000 8968 5688 68fb 896a 8901  (j.....hV.h..j..
+00002210: 0000 8975 6821 7d94 286a 8e01 0000 680c  ...uh!}.(j....h.
+00002220: 6853 684d 68f8 6865 6a86 0100 0068 fe75  hShMh.hej....h.u
+00002230: 8c0d 666f 6f74 6e6f 7465 5f72 6566 7394  ..footnote_refs.
+00002240: 7d94 8c0d 6369 7461 7469 6f6e 5f72 6566  }...citation_ref
+00002250: 7394 7d94 8c0d 6175 746f 666f 6f74 6e6f  s.}...autofootno
+00002260: 7465 7394 5d94 8c11 6175 746f 666f 6f74  tes.]...autofoot
+00002270: 6e6f 7465 5f72 6566 7394 5d94 8c10 7379  note_refs.]...sy
+00002280: 6d62 6f6c 5f66 6f6f 746e 6f74 6573 945d  mbol_footnotes.]
+00002290: 948c 1473 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
+000022a0: 7465 5f72 6566 7394 5d94 8c09 666f 6f74  te_refs.]...foot
+000022b0: 6e6f 7465 7394 5d94 8c09 6369 7461 7469  notes.]...citati
+000022c0: 6f6e 7394 5d94 8c12 6175 746f 666f 6f74  ons.]...autofoot
+000022d0: 6e6f 7465 5f73 7461 7274 944b 018c 1573  note_start.K...s
+000022e0: 796d 626f 6c5f 666f 6f74 6e6f 7465 5f73  ymbol_footnote_s
+000022f0: 7461 7274 944b 008c 0a69 645f 636f 756e  tart.K...id_coun
+00002300: 7465 7294 8c0b 636f 6c6c 6563 7469 6f6e  ter...collection
+00002310: 7394 8c07 436f 756e 7465 7294 9394 7d94  s...Counter...}.
+00002320: 8594 5294 8c0e 7061 7273 655f 6d65 7373  ..R...parse_mess
+00002330: 6167 6573 945d 948c 1274 7261 6e73 666f  ages.]...transfo
+00002340: 726d 5f6d 6573 7361 6765 7394 5d94 8c0b  rm_messages.]...
+00002350: 7472 616e 7366 6f72 6d65 7294 4e8c 0b69  transformer.N..i
+00002360: 6e63 6c75 6465 5f6c 6f67 945d 948c 0a64  nclude_log.]...d
+00002370: 6563 6f72 6174 696f 6e94 4e68 1c68 0375  ecoration.Nh.h.u
+00002380: 622e                                     b.
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/Getting Started.html` & `mly_pipeline-0.5.7/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/GettingStarted.html` & `mly_pipeline-0.5.7/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/How to use.html` & `mly_pipeline-0.5.7/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/HowToUse.html` & `mly_pipeline-0.5.7/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/Installation.html` & `mly_pipeline-0.5.7/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_modules/index.html` & `mly_pipeline-0.5.7/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_modules/io.html` & `mly_pipeline-0.5.7/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.5.7/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.5.7/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.5.7/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.5.7/docs/build/html/_sources/index.rst.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,7 +29,9 @@
 
 .. toctree::
     :maxdepth: 2
     
     installation
     settingupasearch
     runningasearch
+    runningasearchoffline
+    runningasearchonline
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.5.7/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.5.7/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/basic.css` & `mly_pipeline-0.5.7/docs/build/html/_static/basic.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
@@ -320,25 +320,25 @@
     clear: right;
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
+
 nav.contents,
 aside.topic,
-
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
+
 nav.contents,
 aside.topic,
-
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -371,25 +371,23 @@
 
 /* -- content of sidebars/topics/admonitions -------------------------------- */
 
 div.sidebar > :last-child,
 aside.sidebar > :last-child,
 nav.contents > :last-child,
 aside.topic > :last-child,
-
 div.topic > :last-child,
 div.admonition > :last-child {
     margin-bottom: 0;
 }
 
 div.sidebar::after,
 aside.sidebar::after,
 nav.contents::after,
 aside.topic::after,
-
 div.topic::after,
 div.admonition::after,
 blockquote::after {
     display: block;
     content: '';
     clear: both;
 }
@@ -607,33 +605,14 @@
 }
 
 ol.simple p,
 ul.simple p {
     margin-bottom: 0;
 }
 
-/* Docutils 0.17 and older (footnotes & citations) */
-dl.footnote > dt,
-dl.citation > dt {
-    float: left;
-    margin-right: 0.5em;
-}
-
-dl.footnote > dd,
-dl.citation > dd {
-    margin-bottom: 0em;
-}
-
-dl.footnote > dd:after,
-dl.citation > dd:after {
-    content: "";
-    clear: both;
-}
-
-/* Docutils 0.18+ (footnotes & citations) */
 aside.footnote > span,
 div.citation > span {
     float: left;
 }
 aside.footnote > span:last-of-type,
 div.citation > span:last-of-type {
   padding-right: 0.5em;
@@ -650,32 +629,26 @@
 }
 aside.footnote > p:last-of-type:after,
 div.citation > p:last-of-type:after {
     content: "";
     clear: both;
 }
 
-/* Footnotes & citations ends */
-
 dl.field-list {
     display: grid;
     grid-template-columns: fit-content(30%) auto;
 }
 
 dl.field-list > dt {
     font-weight: bold;
     word-break: break-word;
     padding-left: 0.5em;
     padding-right: 5px;
 }
 
-dl.field-list > dt:after {
-    content: ":";
-}
-
 dl.field-list > dd {
     padding-left: 0.5em;
     margin-top: 0em;
     margin-left: 0em;
     margin-bottom: 0em;
 }
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.5.7/docs/build/html/_static/bizstyle.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * bizstyle.css_t
  * ~~~~~~~~~~~~~~
  *
  * Sphinx stylesheet -- business style theme.
  *
- * :copyright: Copyright 2011-2014 by Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 @import url("basic.css");
 
 /* -- page layout ----------------------------------------------------------- */
@@ -290,17 +290,17 @@
 div.quotebar {
     background-color: #f8f8f8;
     max-width: 250px;
     float: right;
     padding: 2px 7px;
     border: 1px solid #ccc;
 }
+
 nav.contents,
 aside.topic,
-
 div.topic {
     background-color: #f8f8f8;
 }
 
 table {
     border-collapse: collapse;
     margin: 0 -0.5em 0 -0.5em;
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.5.7/docs/build/html/_static/bizstyle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 // bizstyle.js
 // ~~~~~~~~~~~
 //
 // Sphinx javascript -- for bizstyle theme.
 //
 // This theme was created by referring to 'sphinxdoc'
 //
-// :copyright: Copyright 2012-2014 by Sphinx team, see AUTHORS.
+// :copyright: Copyright 2007-2023 by Sphinx team, see AUTHORS.
 // :license: BSD, see LICENSE for details.
 //
 const initialiseBizStyle = () => {
     if (navigator.userAgent.indexOf("iPhone") > 0 || navigator.userAgent.indexOf("Android") > 0) {
         document.querySelector("li.nav-item-0 a").innerText = "Top"
     }
     const truncator = item => {
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.5.7/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.5.7/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.5.7/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/jquery.js` & `mly_pipeline-0.5.7/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/language_data.js` & `mly_pipeline-0.5.7/docs/build/html/_static/language_data.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 /*
  * language_data.js
  * ~~~~~~~~~~~~~~~~
  *
  * This script contains the language-specific data used by searchtools.js,
  * namely the list of stopwords, stemmer, scorer and splitter.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/pygments.css` & `mly_pipeline-0.5.7/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.5.7/docs/build/html/_static/searchtools.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 /**
  * Simple result scoring code.
@@ -53,22 +53,22 @@
 
 /**
  * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping
  */
 const _escapeRegExp = (string) =>
     string.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&"); // $& means the whole matched string
 
-const _displayItem = (item, highlightTerms, searchTerms) => {
+const _displayItem = (item, searchTerms) => {
     const docBuilder = DOCUMENTATION_OPTIONS.BUILDER;
     const docUrlRoot = DOCUMENTATION_OPTIONS.URL_ROOT;
     const docFileSuffix = DOCUMENTATION_OPTIONS.FILE_SUFFIX;
     const docLinkSuffix = DOCUMENTATION_OPTIONS.LINK_SUFFIX;
     const showSearchSummary = DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY;
 
-    const [docName, title, anchor, descr] = item;
+    const [docName, title, anchor, descr, score, _filename] = item;
 
     let listItem = document.createElement("li");
     let requestUrl;
     let linkUrl;
     if (docBuilder === "dirhtml") {
         // dirhtml builder
         let dirname = docName + "/";
@@ -78,29 +78,28 @@
         requestUrl = docUrlRoot + dirname;
         linkUrl = requestUrl;
     } else {
         // normal html builders
         requestUrl = docUrlRoot + docName + docFileSuffix;
         linkUrl = docName + docLinkSuffix;
     }
-    const params = new URLSearchParams();
-    params.set("highlight", [...highlightTerms].join(" "));
     let linkEl = listItem.appendChild(document.createElement("a"));
-    linkEl.href = linkUrl + "?" + params.toString() + anchor;
+    linkEl.href = linkUrl + anchor;
+    linkEl.dataset.score = score;
     linkEl.innerHTML = title;
     if (descr)
-        listItem.appendChild(document.createElement("span")).innerText =
+        listItem.appendChild(document.createElement("span")).innerHTML =
         " (" + descr + ")";
     else if (showSearchSummary)
         fetch(requestUrl)
         .then((responseData) => responseData.text())
         .then((data) => {
             if (data)
                 listItem.appendChild(
-                    Search.makeSearchSummary(data, searchTerms, highlightTerms)
+                    Search.makeSearchSummary(data, searchTerms)
                 );
         });
     Search.output.appendChild(listItem);
 };
 const _finishSearch = (resultCount) => {
     Search.stopPulse();
     Search.title.innerText = _("Search Results");
@@ -112,23 +111,22 @@
         Search.status.innerText = _(
             `Search finished, found ${resultCount} page(s) matching the search query.`
         );
 };
 const _displayNextItem = (
     results,
     resultCount,
-    highlightTerms,
     searchTerms
 ) => {
     // results left, load the summary and display it
     // this is intended to be dynamic (don't sub resultsCount)
     if (results.length) {
-        _displayItem(results.pop(), highlightTerms, searchTerms);
+        _displayItem(results.pop(), searchTerms);
         setTimeout(
-            () => _displayNextItem(results, resultCount, highlightTerms, searchTerms),
+            () => _displayNextItem(results, resultCount, searchTerms),
             5
         );
     }
     // search finished, update title and status message
     else _finishSearch(resultCount);
 };
 
@@ -151,18 +149,18 @@
  */
 const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
     htmlToText: (htmlString) => {
-        const htmlElement = document
-            .createRange()
-            .createContextualFragment(htmlString);
-        _removeChildren(htmlElement.querySelectorAll(".headerlink"));
+        const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
+        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
+            el.remove()
+        });
         const docContent = htmlElement.querySelector('[role="main"]');
         if (docContent !== undefined) return docContent.textContent;
         console.warn(
             "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
         );
         return "";
     },
@@ -235,14 +233,20 @@
         else Search.deferQuery(query);
     },
 
     /**
      * execute search (requires search index to be loaded)
      */
     query: (query) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
         // stem the search terms and add them to the correct list
         const stemmer = new Stemmer();
         const searchTerms = new Set();
         const excludedTerms = new Set();
         const highlightTerms = new Set();
         const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
         splitQuery(query.trim()).forEach((queryTerm) => {
@@ -262,22 +266,60 @@
             if (word[0] === "-") excludedTerms.add(word.substr(1));
             else {
                 searchTerms.add(word);
                 highlightTerms.add(queryTermLower);
             }
         });
 
+        if (SPHINX_HIGHLIGHT_ENABLED) { // set in sphinx_highlight.js
+            localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
+        }
+
         // console.debug("SEARCH: searching for:");
         // console.info("required: ", [...searchTerms]);
         // console.info("excluded: ", [...excludedTerms]);
 
         // array of [docname, title, anchor, descr, score, filename]
         let results = [];
         _removeChildren(document.getElementById("search-progress"));
 
+        const queryLower = query.toLowerCase();
+        for (const [title, foundTitles] of Object.entries(allTitles)) {
+            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+                for (const [file, id] of foundTitles) {
+                    let score = Math.round(100 * queryLower.length / title.length)
+                    results.push([
+                        docNames[file],
+                        titles[file] !== title ? `${titles[file]} > ${title}` : title,
+                        id !== null ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
+
+        // search for explicit entries in index directives
+        for (const [entry, foundEntries] of Object.entries(indexEntries)) {
+            if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
+                for (const [file, id] of foundEntries) {
+                    let score = Math.round(100 * queryLower.length / entry.length)
+                    results.push([
+                        docNames[file],
+                        titles[file],
+                        id ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
+
         // lookup as object
         objectTerms.forEach((term) =>
             results.push(...Search.performObjectSearch(term, objectTerms))
         );
 
         // lookup as search terms in fulltext
         results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
@@ -316,15 +358,15 @@
         results = results.reverse();
 
         // for debugging
         //Search.lastresults = results.slice();  // a copy
         // console.info("search results:", Search.lastresults);
 
         // print the results
-        _displayNextItem(results, results.length, highlightTerms, searchTerms);
+        _displayNextItem(results, results.length, searchTerms);
     },
 
     /**
      * search for object names
      */
     performObjectSearch: (object, objectTerms) => {
         const filenames = Search._index.filenames;
@@ -397,16 +439,16 @@
     /**
      * search for full-text terms in the index
      */
     performTermsSearch: (searchTerms, excludedTerms) => {
         // prepare search
         const terms = Search._index.terms;
         const titleTerms = Search._index.titleterms;
-        const docNames = Search._index.docnames;
         const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
         const titles = Search._index.titles;
 
         const scoreMap = new Map();
         const fileMap = new Map();
 
         // perform the search on the required terms
         searchTerms.forEach((word) => {
@@ -504,37 +546,32 @@
         }
         return results;
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
-     * of stemmed words, highlightWords is the list of normal, unstemmed
-     * words. the first one is used to find the occurrence, the
-     * latter for highlighting it.
+     * of stemmed words.
      */
-    makeSearchSummary: (htmlText, keywords, highlightWords) => {
-        const text = Search.htmlToText(htmlText).toLowerCase();
+    makeSearchSummary: (htmlText, keywords) => {
+        const text = Search.htmlToText(htmlText);
         if (text === "") return null;
 
+        const textLower = text.toLowerCase();
         const actualStartPosition = [...keywords]
-            .map((k) => text.indexOf(k.toLowerCase()))
+            .map((k) => textLower.indexOf(k.toLowerCase()))
             .filter((i) => i > -1)
             .slice(-1)[0];
         const startWithContext = Math.max(actualStartPosition - 120, 0);
 
         const top = startWithContext === 0 ? "" : "...";
         const tail = startWithContext + 240 < text.length ? "..." : "";
 
-        let summary = document.createElement("div");
+        let summary = document.createElement("p");
         summary.classList.add("context");
-        summary.innerText = top + text.substr(startWithContext, 240).trim() + tail;
-
-        highlightWords.forEach((highlightWord) =>
-            _highlightText(summary, highlightWord, "highlighted")
-        );
+        summary.textContent = top + text.substr(startWithContext, 240).trim() + tail;
 
         return summary;
     },
 };
 
 _ready(Search.init);
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.5.7/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/underscore.js` & `mly_pipeline-0.5.7/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/_static/websupport.js` & `mly_pipeline-0.5.7/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/genindex.html` & `mly_pipeline-0.5.7/docs/build/html/genindex.html`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,16 @@
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Index &#8212; mlyPipeline 0.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/bizstyle.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/bizstyle.js"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
     <meta name="viewport" content="width=device-width,initial-scale=1.0" />
     <!--[if lt IE 9]>
     <script src="_static/css3-mediaqueries.js"></script>
     <![endif]-->
@@ -75,11 +73,11 @@
              >index</a></li>
         <li class="nav-item nav-item-0"><a href="index.html">mlyPipeline 0.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2022, Vasileios Skliris.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -12,8 +12,8 @@
 ****** Index ******
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * mlyPipeline_0.4.2_documentation »
     * Index
-© Copyright 2022, Vasileios Skliris. Created using Sphinx 5.0.2.
+© Copyright 2022, Vasileios Skliris. Created using Sphinx 7.0.1.
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/gettingstarted.html` & `mly_pipeline-0.5.7/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/howtouse.html` & `mly_pipeline-0.5.7/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/index.html` & `mly_pipeline-0.5.7/docs/build/html/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,16 @@
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
     <title>Welcome to MLy-Pipeline’s documentation! &#8212; mlyPipeline 0.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/bizstyle.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/bizstyle.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Installation" href="installation.html" />
     <meta name="viewport" content="width=device-width,initial-scale=1.0" />
     <!--[if lt IE 9]>
     <script src="_static/css3-mediaqueries.js"></script>
@@ -73,24 +71,36 @@
 <li class="toctree-l1"><a class="reference internal" href="settingupasearch.html">Setting up a search</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="settingupasearch.html#setting-up-directories">Setting up directories</a></li>
 <li class="toctree-l2"><a class="reference internal" href="settingupasearch.html#the-runall-sh-script">The runall.sh script</a></li>
 <li class="toctree-l2"><a class="reference internal" href="settingupasearch.html#configuration-file">Configuration File</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="runningasearch.html">Running a search</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#ending-an-online-search">Ending an online search</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#with-every-inference">With every inference</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#how-manager-py-manages-the-search-part-1">How manager.py manages the search part 1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#continuous-false-alarm-rate-estimation">Continuous False Alarm Rate estimation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#efficiency-tests">Efficiency Tests</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#trigger-handling">Trigger handling</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#how-manager-py-manages-the-search-part-2">How manager.py manages the search part 2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#monitoring-the-search">Monitoring the search</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#after-the-first-ten-minutes">After the first ten minutes</a></li>
-<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#after-roughly-an-hour">After roughly an hour</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#ending-a-search">Ending a search</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#pickle-format">Pickle format</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearch.html#timelines">Timelines</a></li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="runningasearchoffline.html">Offline search timeline</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchoffline.html#data-processing">Data Processing</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchoffline.html#background-estimation">Background estimation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchoffline.html#zero-lag-search">Zero-lag search</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchoffline.html#efficiency-test-not-working-yet">Efficiency test (not working yet)</a></li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="runningasearchonline.html">Online Search Timeline</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#with-every-inference">With every inference</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#how-manager-py-manages-the-search-part-1">How manager.py manages the search part 1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#continuous-false-alarm-rate-estimation">Continuous False Alarm Rate estimation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#efficiency-tests">Efficiency Tests</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#trigger-handling">Trigger handling</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#how-manager-py-manages-the-search-part-2">How manager.py manages the search part 2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#monitoring-the-search">Monitoring the search</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#after-the-first-ten-minutes">After the first ten minutes</a></li>
+<li class="toctree-l2"><a class="reference internal" href="runningasearchonline.html#after-roughly-an-hour">After roughly an hour</a></li>
 </ul>
 </li>
 </ul>
 </div>
 </section>
 </section>
 
@@ -149,11 +159,11 @@
              >next</a> |</li>
         <li class="nav-item nav-item-0"><a href="#">mlyPipeline 0.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to MLy-Pipeline’s documentation!</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2022, Vasileios Skliris.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -28,15 +28,23 @@
           o Environment_and_installation_of_MLy-Pipeline
           o Updating_MLy-Pipeline
     * Setting_up_a_search
           o Setting_up_directories
           o The_runall.sh_script
           o Configuration_File
     * Running_a_search
-          o Ending_an_online_search
+          o Ending_a_search
+          o Pickle_format
+          o Timelines
+    * Offline_search_timeline
+          o Data_Processing
+          o Background_estimation
+          o Zero-lag_search
+          o Efficiency_test_(not_working_yet)
+    * Online_Search_Timeline
           o With_every_inference
           o How_manager.py_manages_the_search_part_1
           o Continuous_False_Alarm_Rate_estimation
           o Efficiency_Tests
           o Trigger_handling
           o How_manager.py_manages_the_search_part_2
           o Monitoring_the_search
@@ -54,8 +62,8 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * mlyPipeline_0.4.2_documentation »
     * Welcome to MLy-Pipelineâs documentation!
-© Copyright 2022, Vasileios Skliris. Created using Sphinx 5.0.2.
+© Copyright 2022, Vasileios Skliris. Created using Sphinx 7.0.1.
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/installation.html` & `mly_pipeline-0.5.7/docs/build/html/installation.html`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,16 @@
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
     <title>Installation &#8212; mlyPipeline 0.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/bizstyle.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/bizstyle.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Setting up a search" href="settingupasearch.html" />
     <link rel="prev" title="Welcome to MLy-Pipeline’s documentation!" href="index.html" />
     <meta name="viewport" content="width=device-width,initial-scale=1.0" />
     <!--[if lt IE 9]>
@@ -146,11 +144,11 @@
              >previous</a> |</li>
         <li class="nav-item nav-item-0"><a href="index.html">mlyPipeline 0.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Installation</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2022, Vasileios Skliris.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -63,8 +63,8 @@
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * previous |
     * mlyPipeline_0.4.2_documentation »
     * Installation
-© Copyright 2022, Vasileios Skliris. Created using Sphinx 5.0.2.
+© Copyright 2022, Vasileios Skliris. Created using Sphinx 7.0.1.
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/py-modindex.html` & `mly_pipeline-0.5.7/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/build/html/search.html` & `mly_pipeline-0.5.7/docs/build/html/search.html`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,16 @@
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Search &#8212; mlyPipeline 0.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/bizstyle.css" />
     
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/bizstyle.js"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
   <script src="searchindex.js" defer></script>
   
@@ -94,11 +92,11 @@
              >index</a></li>
         <li class="nav-item nav-item-0"><a href="index.html">mlyPipeline 0.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2022, Vasileios Skliris.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -13,8 +13,8 @@
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * mlyPipeline_0.4.2_documentation »
     * Search
-© Copyright 2022, Vasileios Skliris. Created using Sphinx 5.0.2.
+© Copyright 2022, Vasileios Skliris. Created using Sphinx 7.0.1.
```

### Comparing `mly_pipeline-0.5.5/docs/build/html/settingupasearch.html` & `mly_pipeline-0.5.7/docs/build/html/settingupasearch.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 
 
 <!doctype html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
+
     <title>Setting up a search &#8212; mlyPipeline 0.4.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/bizstyle.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/bizstyle.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Running a search" href="runningasearch.html" />
     <link rel="prev" title="Installation" href="installation.html" />
     <meta name="viewport" content="width=device-width,initial-scale=1.0" />
     <!--[if lt IE 9]>
@@ -43,31 +42,30 @@
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
-  <div class="section" id="setting-up-a-search">
+  <section id="setting-up-a-search">
 <span id="id1"></span><h1>Setting up a search<a class="headerlink" href="#setting-up-a-search" title="Permalink to this heading">¶</a></h1>
-<div class="section" id="setting-up-directories">
+<section id="setting-up-directories">
 <h2>Setting up directories<a class="headerlink" href="#setting-up-directories" title="Permalink to this heading">¶</a></h2>
 <p>To run an MLy-Pipeline search we need a directory structure that will be used
 by the features of the pipeline. To make the creation of such directory
 structure easy we have a command automate the creation for us. With the installation of MLy-Pipeline there are soem commands that you can run from the terminal
 to initialize a search. To create a search directory you should use <code class="docutils literal notranslate"><span class="pre">mly-pipeline-init</span></code> comand as shown below:</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>mly-pipeline-init<span class="w"> </span>-p<span class="w"> </span>./mysearch
 </pre></div>
 </div>
 <p>Where instead of <code class="docutils literal notranslate"><span class="pre">mysearch</span></code> you can use a more apropriate name that fits your
 need. The command above will create the directory <code class="docutils literal notranslate"><span class="pre">./mysearch</span></code> and also the subdirectories
 below (these are their default names):</p>
 <blockquote>
 <div><ul class="simple">
-<li><p>triggerplot_directory</p></li>
 <li><p>trigger_directory</p></li>
 <li><p>output_directory</p></li>
 <li><p>masterDirectory</p></li>
 <li><p>bufferDirectory</p></li>
 <li><p>falseAlarmRates</p></li>
 <li><p>efficiencies</p></li>
 <li><p>log</p></li>
@@ -79,15 +77,15 @@
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>mly-pipeline-init<span class="w"> </span>-p<span class="w"> </span>./mysearch<span class="w"> </span>--masterDirectory<span class="w"> </span>customName
 </pre></div>
 </div>
 <p>This applies for all the other directories.</p>
 <p>In addition to that, inside the search directory, it will also create a script to run the search called runall.sh
 and the config.json file that has the parameters that are used by the search.
 <strong>It is up to the user to change those parameters to conduct the search the way they want.</strong></p>
-<div class="section" id="running-the-search-under-different-circumstances">
+<section id="running-the-search-under-different-circumstances">
 <h3>Running the search under different circumstances<a class="headerlink" href="#running-the-search-under-different-circumstances" title="Permalink to this heading">¶</a></h3>
 <p>You might want to just run the search as it would be run in low latency (in real time).
 In case you want to run the search on MDC data for example, which means you need a fixed background, then
 there is a light version of the same command. When we run on MDC we do not need some of the
 directories, and also some configuration parameters will need to change to ignore specific
 functionalities. The comand below will create a version of the search that does not do the
 continuous FAR estimation and neither does efficiency tests. It also points the search to the
@@ -109,19 +107,19 @@
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>mly-pipeline-init<span class="w"> </span>-p<span class="w"> </span>./mysearch<span class="w"> </span>--search_mode<span class="w"> </span>BENCHMARK_MDC_OFFLINE
 </pre></div>
 </div>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>At version 0.4 the new command way of doing things has not been tested for offline search much.</p>
 </div>
-</div>
-</div>
-<div class="section" id="the-runall-sh-script">
+</section>
+</section>
+<section id="the-runall-sh-script">
 <h2>The runall.sh script<a class="headerlink" href="#the-runall-sh-script" title="Permalink to this heading">¶</a></h2>
-<div class="section" id="online-search">
+<section id="online-search">
 <h3>Online search<a class="headerlink" href="#online-search" title="Permalink to this heading">¶</a></h3>
 <p>The <code class="docutils literal notranslate"><span class="pre">runall.sh</span></code> is the only thing that you need to run from inside <code class="docutils literal notranslate"><span class="pre">./mysearch</span></code>
 (or however you named it) directory for the search to comence. Processing a second
 during a search, doing inference and issiuing a possible alert takes more than a second. For that reason we split our
 search into many scripts to avoid queing delays. Hence is only one parameter that
 can be adjusted in the inside the runall script and that is the <code class="docutils literal notranslate"><span class="pre">STEP</span></code> parameter.
 This paramater breaks the search into <code class="docutils literal notranslate"><span class="pre">STEP</span></code> in number, non overlaping scripts.
@@ -137,158 +135,157 @@
 <li><p><code class="docutils literal notranslate"><span class="pre">continuous_FAR.py</span></code> is called with two different parameters does two things in parallel.</p>
 <ul>
 <li><p><code class="docutils literal notranslate"><span class="pre">continuous_FAR.py</span> <span class="pre">--mode</span> <span class="pre">generation</span></code> takes the data of the last hour saved in the masterDirectory and generates condor jobs. Each jobs greates a specific amount of timeshifted versions of these data and saves them in a temporary file in the scrach directory (falseAlarmRates/temp), ready to be used for background testing.</p></li>
 <li><p><code class="docutils literal notranslate"><span class="pre">continuous_FAR.py</span> <span class="pre">--mode</span> <span class="pre">inference</span></code> does inference on the data generated using available GPUs or the GPUs specified in <code class="docutils literal notranslate"><span class="pre">selectedGPUs</span></code> parameter. This script will load any time-lag data available and return a pandas data frame with the results. The asemble of those files is done by the managers script.</p></li>
 </ul>
 </li>
 </ul>
-</div>
-<div class="section" id="offline-search">
+</section>
+<section id="offline-search">
 <h3>Offline search<a class="headerlink" href="#offline-search" title="Permalink to this heading">¶</a></h3>
 <p>For searches that run offline there is only one script that will be run through the runall.sh and that is:</p>
 <ul class="simple">
 <li><p><code class="docutils literal notranslate"><span class="pre">offline_search.py</span></code> It runs the offline search by breaking the searh in jobs equivalent to the segments provided. It also does all the management of events.</p></li>
 </ul>
-</div>
-</div>
-<div class="section" id="configuration-file">
+</section>
+</section>
+<section id="configuration-file">
 <h2>Configuration File<a class="headerlink" href="#configuration-file" title="Permalink to this heading">¶</a></h2>
 <p>All the above functions get their parameters from the <code class="docutils literal notranslate"><span class="pre">config.json</span></code> file. Below we are going to give descriptions about each config parameter. By changing the
 config you change the way the search will run, so make sure that you check that
 config is the way you want it after you create the search directory.</p>
-<div class="section" id="file-names-and-paths">
+<section id="file-names-and-paths">
 <h3>File Names and Paths<a class="headerlink" href="#file-names-and-paths" title="Permalink to this heading">¶</a></h3>
 <p>The following are just the directory names of the directories created by with
 the <code class="docutils literal notranslate"><span class="pre">initialization.py</span></code>. If the default names were used, this will look like:</p>
 <ul class="simple">
 <li><p><strong>output_directory</strong>:”output_directory”</p></li>
 <li><p><strong>trigger_directory</strong>:”trigger_directory”</p></li>
-<li><p><strong>triggerplot_directory</strong>:”triggerplot_directory”</p></li>
 <li><p><strong>masterDirectory</strong>:”masterDirectory”</p></li>
 <li><p><strong>bufferDirectory</strong>:”bufferDirectory”</p></li>
 <li><p><strong>falseAlarmRates</strong>:”falseAlarmRates”</p></li>
 <li><p><strong>efficiencies</strong>:”efficiencies”</p></li>
+<li><p><strong>log</strong>:”log”</p></li>
 </ul>
-<p>After this we have the path to your local mlyPipeline installation. This is
-identified automatically when you run the <code class="docutils literal notranslate"><span class="pre">initialization.py</span></code>, and it will look
-like below, do not edit that unles you moved your mlyPipeline directory.</p>
-<ul class="simple">
-<li><p><strong>mlyPipelineSource</strong>:”/home/&lt;albert.einstein&gt;/extraPath/mlyPipeline”</p></li>
-</ul>
+<p>The log level that will be used for the log files.
+* <strong>log_level</strong>:”INFO”</p>
 <p>User and accounting group for condor jobs.</p>
 <ul class="simple">
 <li><p><strong>user_name</strong>: This is automatically filled by the enviroment</p></li>
 <li><p><strong>accounting_group_user</strong>: It defaults to be the same as user_name.</p></li>
-<li><p><strong>accounting_group</strong>: “allsky.mlyonline”</p></li>
+<li><p><strong>accounting_group</strong>: “ligo.dev.o4.burst.allsky.mlyonline”</p></li>
 </ul>
 <p>This is the name of the search directory, in our case it will look like:</p>
 <ul class="simple">
 <li><p><strong>path</strong> :”./mysearch”</p></li>
 </ul>
-</div>
-<div class="section" id="generator-function-parameters">
+</section>
+<section id="generator-function-parameters">
 <h3>Generator Function Parameters<a class="headerlink" href="#generator-function-parameters" title="Permalink to this heading">¶</a></h3>
 <p>The following parameters are passed to the generator function that processes
 the data before inference. The values assigned are the default values.</p>
 <ul class="simple">
 <li><p><strong>fs</strong>:1024 Sample frequency</p></li>
 <li><p><strong>duration</strong>:1 Duration of processing window</p></li>
 <li><p><strong>detectors</strong>:”HLV” Detectors used for the search</p></li>
 </ul>
 <p>The prefix dictionary of the paths of directories where O3-replay and MDC data are. If the
 source of the data you use is different, you need to edit this parameter, after
 creating the search directory.</p>
 <ul class="simple">
-<li><p><strong>frames_directory</strong>: A dictionary with entries for H, L and V for the detectors. For each detector it has a path to the directory of the frame files that are going to be used. The default is empty but if you specified a mode of initialization then this will be filled with the respective paths.</p></li>
+<li><p><strong>frames_directory</strong>: A dictionary with entries for H, L and V for the detectors. For each detector it has a path to the directory of the frame files that are going to be used or a frame name recognised by gwdatafind. The default is empty but if you specified a mode of initialization then this will be filled with the respective paths.</p></li>
 <li><p><strong>channels</strong>: Also a dictionary with entries for H, L and V for the detectors. For each detector it has the channel that is going to be used. The default is empty but if you specified a mode of initialization then this will be filled with the respective channels.</p></li>
+<li><p><strong>state_vector</strong>: Dictionary with the statevectors used only for the online search. For anything else, it is empty.</p></li>
 <li><p><strong>segment_list</strong>: This can be a path to a file that has segment intervals or it can be a list of two intervals corresponding to a start GPS time and an end GPS time. It is used only in offline searches. It defaults to an empty list.</p></li>
 <li><p><strong>max_continuous_segment</strong>: If the segments provided are too big we might want to break them in smaller runs. This parameter is the minimum segment size that will be used for one job. Also used only during offline searches. Defaults to 10000.</p></li>
 </ul>
-</div>
-<div class="section" id="requesting-data-parameters">
+</section>
+<section id="requesting-data-parameters">
 <h3>Requesting Data Parameters<a class="headerlink" href="#requesting-data-parameters" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p><strong>parallel_scripts</strong>: 4 This is the STEP parameter inside the runall.sh script (see above).</p></li>
 <li><p><strong>wait</strong>:0.5 Time to wait before requesting a segment of data again</p></li>
 <li><p><strong>timeout</strong>:20 How many times to try requesting a data segment before going to the next.</p></li>
 <li><p><strong>required_buffer</strong>:16 How many seconds of data to request.</p></li>
 <li><p><strong>start_lag</strong>:92 How many seconds before the current gps time to start the search from. We expect that given the reset time below this will be reseted in the first attempt.</p></li>
 <li><p><strong>gps_reset_time</strong>:32 The amount of time difference in seconds where we reset the gps that we request to the current one. This is for cases where latency is running behind momenterily.</p></li>
 <li><p><strong>farfile</strong>: “/home/vasileios.skliris/mly-hermes/outputs/FARfile” The path to an initial FAR directory. When the search starts there will be no background estimation yet. This will take sometime to be produced and until then we use another background. <strong>The initial FAR estimation will be used until one year of background has been estimated. Then the manager will overight this path to the path of the search</strong>: <code class="docutils literal notranslate"><span class="pre">mysearch/falseAlarmRates/FARfile</span></code></p></li>
 </ul>
-</div>
-<div class="section" id="models">
+</section>
+<section id="models">
 <h3>Models<a class="headerlink" href="#models" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p><strong>model1_path</strong>:”/home/mly/models/model1_32V_No5.h5” Coincidence model (model 1).</p></li>
 <li><p><strong>model2_path</strong>:”/home/mly/models/model2_32V_No6.h5” Coherency model (model 2).</p></li>
 <li><p><strong>td_pe_model_path</strong>:”/home/mly/models/td_model” Time domain parameter estimation model.</p></li>
 <li><p><strong>fd_pe_model_path</strong>:”/home/mly/models/fd_model” Frequency domain parameter estimation model.</p></li>
 </ul>
-</div>
-<div class="section" id="skymap">
+</section>
+<section id="skymap">
 <h3>Skymap<a class="headerlink" href="#skymap" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
-<li><p><strong>skymap</strong>:true Option for generation of skymaps with each issued event.</p></li>
+<li><p><strong>skymap</strong>:0 Option for generation of skymaps with each issued event. Currently 0 until skymap is ready.</p></li>
 <li><p><strong>nside</strong>:64 Parameter related to the resolution of the skymap.</p></li>
 </ul>
-</div>
-<div class="section" id="efficiecy-calculation-parameters">
+</section>
+<section id="efficiecy-calculation-parameters">
 <h3>Efficiecy Calculation Parameters<a class="headerlink" href="#efficiecy-calculation-parameters" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p><strong>eff_config</strong> A dictionary of parameters that are related to the efficiency tests.</p>
 <ul>
 <li><p><strong>injectionDirectoryPath</strong>:”/home/mly/injections/” The path were all injection type directories are.</p></li>
 <li><p><strong>injectionsWithHRSS</strong>: [“SGE70Q3”, “SGE153Q8d9”, “SGL153Q8d9”, “WNB250”] The list of the injection directories that use HRSS.</p></li>
 <li><p><strong>injectionsWithSNR</strong>: [“cbc_20_20”, “wnb_03_train_pod”, “cusp_00”] The list of the injection directories that use SNR.</p></li>
 <li><p><strong>injectionHRSS</strong>:”1e-22,1e-21,1e-22” Intervals for tests that use HRSS (first, last, step).</p></li>
 <li><p><strong>injectionSNR</strong>:”0,50,5” Intervals for tests that use SNR (first, last step).</p></li>
 <li><p><strong>testSize</strong>:”100” Number of tests on each value of HRSS or SNR respectively.</p></li>
 <li><p><strong>howOften</strong>: 3600 After how many successful inferences to run an efficiency test.</p></li>
 </ul>
 </li>
 </ul>
-</div>
-<div class="section" id="continuous-far-estimation-parameters">
+</section>
+<section id="continuous-far-estimation-parameters">
 <h3>continuous FAR estimation Parameters<a class="headerlink" href="#continuous-far-estimation-parameters" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p><strong>far_config</strong> A dictionary of parameters that are related to the continuous FAR tests.</p>
 <ul>
+<li><p><strong>far_enabled</strong>: true Option to opt out from false alarm rate calculation. Used by offline and online search at the initialisation of the search. If false make sure you provide a valid FARfile in the config entry <strong>farfile</strong>.</p></li>
 <li><p><strong>batch_size</strong>: 1024 Batch size of inference. Used by hermes client inference.</p></li>
 <li><p><strong>threshold</strong>: 2.3148e-05 Default for once per 2 days (Hz). <strong>Used to define what is an event and what not.</strong></p></li>
 <li><p><strong>restriction</strong>: 0.0001 The minimum score of an inference to keep it in the history.</p></li>
 <li><p><strong>max_lag</strong>: 3600 The maximum time distance allowed, between two lagged segments.</p></li>
 <li><p><strong>lags</strong>: 1024 The number of timeshifts applied on the zero-lagged data to produced background tests.</p></li>
 <li><p><strong>batches</strong>: The amount of condor jobs to break the generation of background tests. <strong>This can be adjusted if they do not finish within the hour.</strong></p></li>
 <li><p><strong>visible_gpu_devices</strong>: “local” GPU devices to use. Local will make all the local GPUs visible.</p></li>
 <li><p><strong>selectedGPUs</strong>: [0] An index list to choose which GPUs are to be used. Default is to use the first visible.</p></li>
 <li><p><strong>parallelGenerations</strong>: 3 How many dags ( each corresponding to an hour of data) are allowed to run at the same time. This is actually a condor_job number restriction. As the default values are, it will restrict the jobs to dags + jobs &lt; parallelGenerations*batches.</p></li>
 </ul>
 </li>
 </ul>
-</div>
-<div class="section" id="misc">
+</section>
+<section id="misc">
 <h3>Misc<a class="headerlink" href="#misc" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p><strong>maxDataFrameSize</strong>:3600 The number of outputs grouped together in one data frame from the manager.</p></li>
 <li><dl class="simple">
 <dt><strong>trigger_destination</strong>:null Which domain of GraceDB to send the event (test,dev,playground). When left empty it it does not send an event but it creates follow-up and seves it in a file with made up ID. If not, it takes one of the following options, shown below with the corresponding destination.</dt><dd><ul>
 <li><p><cite>test</cite> which sends the alerts to: “<a class="reference external" href="https://gracedb-test.ligo.org/api">https://gracedb-test.ligo.org/api</a>” (needs certificate to work)</p></li>
 <li><p><cite>playground</cite> which sends the alerts to: “<a class="reference external" href="https://gracedb-playground.ligo.org/api">https://gracedb-playground.ligo.org/api</a>” (needs certificate to work)</p></li>
 <li><p><cite>dev1</cite> which sends the alerts to: “<a class="reference external" href="https://gracedb-dev1.ligo.org/api">https://gracedb-dev1.ligo.org/api</a>” (needs certificate to work)</p></li>
 <li><p><cite>online</cite> which sends the alerts to: “<a class="reference external" href="https://gracedb.ligo.org/api">https://gracedb.ligo.org/api</a>” (used only for realtime online search after pipeline is approved)</p></li>
+<li><p>There are also some other entries that might appear here when the config will be updated at somepoint within the search. They are to be ignored.</p></li>
 </ul>
 </dd>
 </dl>
 </li>
 </ul>
 <p>Now that the we went through the setting up of the search and the configuration parameters of it, we can see how to run such a search</p>
-</div>
-</div>
-</div>
+</section>
+</section>
+</section>
 
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
@@ -367,11 +364,11 @@
              >previous</a> |</li>
         <li class="nav-item nav-item-0"><a href="index.html">mlyPipeline 0.4.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Setting up a search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2022, Vasileios Skliris.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -21,15 +21,14 @@
 installation of MLy-Pipeline there are soem commands that you can run from the
 terminal to initialize a search. To create a search directory you should use
 mly-pipeline-init comand as shown below:
 mly-pipeline-init -p ./mysearch
 Where instead of mysearch you can use a more apropriate name that fits your
 need. The command above will create the directory ./mysearch and also the
 subdirectories below (these are their default names):
-         * triggerplot_directory
          * trigger_directory
          * output_directory
          * masterDirectory
          * bufferDirectory
          * falseAlarmRates
          * efficiencies
          * log
@@ -63,14 +62,15 @@
 the configuration file. There are templates of offline searches, for example to
 run an offline search on the O3 burst all-sky benchmark project you can
 initialize the search using the following command.
 mly-pipeline-init -p ./mysearch --search_mode BENCHMARK_MDC_OFFLINE
 Note
 At version 0.4 the new command way of doing things has not been tested for
 offline search much.
+
 ***** The runall.sh scriptÂ¶ *****
 **** Online searchÂ¶ ****
 The runall.sh is the only thing that you need to run from inside ./mysearch (or
 however you named it) directory for the search to comence. Processing a second
 during a search, doing inference and issiuing a possible alert takes more than
 a second. For that reason we split our search into many scripts to avoid queing
 delays. Hence is only one parameter that can be adjusted in the inside the
@@ -100,71 +100,74 @@
             saves them in a temporary file in the scrach directory
             (falseAlarmRates/temp), ready to be used for background testing.
           o continuous_FAR.py --mode inference does inference on the data
             generated using available GPUs or the GPUs specified in
             selectedGPUs parameter. This script will load any time-lag data
             available and return a pandas data frame with the results. The
             asemble of those files is done by the managers script.
+
 **** Offline searchÂ¶ ****
 For searches that run offline there is only one script that will be run through
 the runall.sh and that is:
     * offline_search.py It runs the offline search by breaking the searh in
       jobs equivalent to the segments provided. It also does all the management
       of events.
+
 ***** Configuration FileÂ¶ *****
 All the above functions get their parameters from the config.json file. Below
 we are going to give descriptions about each config parameter. By changing the
 config you change the way the search will run, so make sure that you check that
 config is the way you want it after you create the search directory.
 **** File Names and PathsÂ¶ ****
 The following are just the directory names of the directories created by with
 the initialization.py. If the default names were used, this will look like:
     * output_directory:âoutput_directoryâ
     * trigger_directory:âtrigger_directoryâ
-    * triggerplot_directory:âtriggerplot_directoryâ
     * masterDirectory:âmasterDirectoryâ
     * bufferDirectory:âbufferDirectoryâ
     * falseAlarmRates:âfalseAlarmRatesâ
     * efficiencies:âefficienciesâ
-After this we have the path to your local mlyPipeline installation. This is
-identified automatically when you run the initialization.py, and it will look
-like below, do not edit that unles you moved your mlyPipeline directory.
-    * mlyPipelineSource:â/home/<albert.einstein>/extraPath/mlyPipelineâ
+    * log:âlogâ
+The log level that will be used for the log files. * log_level:âINFOâ
 User and accounting group for condor jobs.
     * user_name: This is automatically filled by the enviroment
     * accounting_group_user: It defaults to be the same as user_name.
-    * accounting_group: âallsky.mlyonlineâ
+    * accounting_group: âligo.dev.o4.burst.allsky.mlyonlineâ
 This is the name of the search directory, in our case it will look like:
     * path :â./mysearchâ
+
 **** Generator Function ParametersÂ¶ ****
 The following parameters are passed to the generator function that processes
 the data before inference. The values assigned are the default values.
     * fs:1024 Sample frequency
     * duration:1 Duration of processing window
     * detectors:âHLVâ Detectors used for the search
 The prefix dictionary of the paths of directories where O3-replay and MDC data
 are. If the source of the data you use is different, you need to edit this
 parameter, after creating the search directory.
     * frames_directory: A dictionary with entries for H, L and V for the
       detectors. For each detector it has a path to the directory of the frame
-      files that are going to be used. The default is empty but if you
-      specified a mode of initialization then this will be filled with the
-      respective paths.
+      files that are going to be used or a frame name recognised by gwdatafind.
+      The default is empty but if you specified a mode of initialization then
+      this will be filled with the respective paths.
     * channels: Also a dictionary with entries for H, L and V for the
       detectors. For each detector it has the channel that is going to be used.
       The default is empty but if you specified a mode of initialization then
       this will be filled with the respective channels.
+    * state_vector: Dictionary with the statevectors used only for the online
+      search. For anything else, it is empty.
     * segment_list: This can be a path to a file that has segment intervals or
       it can be a list of two intervals corresponding to a start GPS time and
       an end GPS time. It is used only in offline searches. It defaults to an
       empty list.
     * max_continuous_segment: If the segments provided are too big we might
       want to break them in smaller runs. This parameter is the minimum segment
       size that will be used for one job. Also used only during offline
       searches. Defaults to 10000.
+
 **** Requesting Data ParametersÂ¶ ****
     * parallel_scripts: 4 This is the STEP parameter inside the runall.sh
       script (see above).
     * wait:0.5 Time to wait before requesting a segment of data again
     * timeout:20 How many times to try requesting a data segment before going
       to the next.
     * required_buffer:16 How many seconds of data to request.
@@ -177,26 +180,30 @@
     * farfile: â/home/vasileios.skliris/mly-hermes/outputs/FARfileâ The
       path to an initial FAR directory. When the search starts there will be no
       background estimation yet. This will take sometime to be produced and
       until then we use another background. The initial FAR estimation will be
       used until one year of background has been estimated. Then the manager
       will overight this path to the path of the search: mysearch/
       falseAlarmRates/FARfile
+
 **** ModelsÂ¶ ****
     * model1_path:â/home/mly/models/model1_32V_No5.h5â Coincidence model
       (model 1).
     * model2_path:â/home/mly/models/model2_32V_No6.h5â Coherency model
       (model 2).
     * td_pe_model_path:â/home/mly/models/td_modelâ Time domain parameter
       estimation model.
     * fd_pe_model_path:â/home/mly/models/fd_modelâ Frequency domain
       parameter estimation model.
+
 **** SkymapÂ¶ ****
-    * skymap:true Option for generation of skymaps with each issued event.
+    * skymap:0 Option for generation of skymaps with each issued event.
+      Currently 0 until skymap is ready.
     * nside:64 Parameter related to the resolution of the skymap.
+
 **** Efficiecy Calculation ParametersÂ¶ ****
     * eff_config A dictionary of parameters that are related to the efficiency
       tests.
           o injectionDirectoryPath:â/home/mly/injections/â The path were
             all injection type directories are.
           o injectionsWithHRSS: [âSGE70Q3â, âSGE153Q8d9â,
             âSGL153Q8d9â, âWNB250â] The list of the injection
@@ -207,17 +214,22 @@
             HRSS (first, last, step).
           o injectionSNR:â0,50,5â Intervals for tests that use SNR (first,
             last step).
           o testSize:â100â Number of tests on each value of HRSS or SNR
             respectively.
           o howOften: 3600 After how many successful inferences to run an
             efficiency test.
+
 **** continuous FAR estimation ParametersÂ¶ ****
     * far_config A dictionary of parameters that are related to the continuous
       FAR tests.
+          o far_enabled: true Option to opt out from false alarm rate
+            calculation. Used by offline and online search at the
+            initialisation of the search. If false make sure you provide a
+            valid FARfile in the config entry farfile.
           o batch_size: 1024 Batch size of inference. Used by hermes client
             inference.
           o threshold: 2.3148e-05 Default for once per 2 days (Hz). Used to
             define what is an event and what not.
           o restriction: 0.0001 The minimum score of an inference to keep it in
             the history.
           o max_lag: 3600 The maximum time distance allowed, between two lagged
@@ -231,14 +243,15 @@
             make all the local GPUs visible.
           o selectedGPUs: [0] An index list to choose which GPUs are to be
             used. Default is to use the first visible.
           o parallelGenerations: 3 How many dags ( each corresponding to an
             hour of data) are allowed to run at the same time. This is actually
             a condor_job number restriction. As the default values are, it will
             restrict the jobs to dags + jobs < parallelGenerations*batches.
+
 **** MiscÂ¶ ****
     * maxDataFrameSize:3600 The number of outputs grouped together in one data
       frame from the manager.
     *   trigger_destination:null Which domain of GraceDB to send the event
         (test,dev,playground). When left empty it it does not send an event but
         it creates follow-up and seves it in a file with made up ID. If not, it
         takes one of the following options, shown below with the corresponding
@@ -248,16 +261,20 @@
                 o playgroundwhich sends the alerts to: âhttps://gracedb-
                   playground.ligo.org/apiâ (needs certificate to work)
                 o dev1which sends the alerts to: âhttps://gracedb-
                   dev1.ligo.org/apiâ (needs certificate to work)
                 o onlinewhich sends the alerts to: âhttps://gracedb.ligo.org/
                   apiâ (used only for realtime online search after pipeline
                   is approved)
+                o There are also some other entries that might appear here when
+                  the config will be updated at somepoint within the search.
+                  They are to be ignored.
 Now that the we went through the setting up of the search and the configuration
 parameters of it, we can see how to run such a search
+
 **** Table_of_Contents ****
     * Setting_up_a_search
           o Setting_up_directories
                 # Running_the_search_under_different_circumstances
           o The_runall.sh_script
                 # Online_search
                 # Offline_search
@@ -280,8 +297,8 @@
 [q                   ] [Go]
 **** Navigation ****
     * index
     * next |
     * previous |
     * mlyPipeline_0.4.2_documentation »
     * Setting up a search
-© Copyright 2022, Vasileios Skliris. Created using Sphinx 5.0.2.
+© Copyright 2022, Vasileios Skliris. Created using Sphinx 7.0.1.
```

### Comparing `mly_pipeline-0.5.5/docs/source/conf.py` & `mly_pipeline-0.5.7/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 project = 'mlyPipeline'
 copyright = '2022, Vasileios Skliris'
 author = 'Vasileios Skliris'
 
 # The short X.Y version
 version = ''
 # The full version, including alpha/beta/rc tags
-release = '0.4.2'
+release = '0.5.7'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `mly_pipeline-0.5.5/docs/source/index.rst` & `mly_pipeline-0.5.7/docs/source/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -29,7 +29,9 @@
 
 .. toctree::
     :maxdepth: 2
     
     installation
     settingupasearch
     runningasearch
+    runningasearchoffline
+    runningasearchonline
```

### Comparing `mly_pipeline-0.5.5/docs/source/installation.rst` & `mly_pipeline-0.5.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/docs/source/runningasearch.rst` & `mly_pipeline-0.5.7/docs/source/runningasearchonline.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,21 @@
-.. _Running_a_search
+.. _Online_search_timeline:
 
-Running a search
-################
-
-
-To run the search you only have to get inside the search directory (we assume here that this is ``./mysearch``) and run ``mly-pipeline-start``
-
-
-.. code-block:: bash
-    
-    cd ./mysearch
-    mly-pipeline-start    
-
-This will run the ``runall.sh`` script on the background and it will not terminate when you close your terminal. The output and error messages will all go into ``runall.out``.
-
-.. note:: Before you start any type of search, check the config file to make sure the parameters that are there are the ones you want.  
-
-
-Ending an online search
------------------------
-
-Online search runs a series of scripts that would be usefull to be able to stop easily. For that reason when you want to end or pause a search, you can run the following command inside the search directory.
-
-.. code-block:: bash
-    
-    mly-pipeline-stop
-
-If you want to resume the online search you run again the ``mly-pipeline-start`` command. The stop command is only for the online search. For offline searches is not yet implement given that they do not run indefinetly.
-
-
-Pickle format
-=============
-
-Many files that are saved during a search will be of pickle format. This format preserves the python object to be saved. The types of objects saved are python dictionary, mly.DataPod, mly.DataSet and pandas.DataFrame. We save them in such format to be able to change them for different purposes.
 
 Online Search Timeline
-======================
+######################
 
 By the moment the pipeline starts running and from now on there is a constant production of processed data instances and inference results. Both of which are saved and organised for post processing.
 
 * The script requests at least 16 seconds of data for each inference. These 16 seconds are usually the most recent 16 seconds. We call these data the buffer or **buffer instance**.
 * The buffer is whitened, bandpassed (20,512 Hz) and then the central second (7.5,8.5) is cropped. This is a **timeseries data instance**.
 * The **timeseries data instance** is used to create the pearson **correlation data instance**, which is used in coherency model (model2).
 * The timseries and correlation data instances are fed to the models to produce an **inference result**.
 
-With every inference
+With every inference  
 --------------------
 
 If the **inference result** is above the detection threshold:
 
 * The **inference** result is saved in json format inside ``output_directory`` and in labeled as a **trigger**.
 * A series of actions related to :ref:`trigger handling<Trigger handling>` take place.
 
@@ -180,13 +147,7 @@
 Now that at least one hourly dataset has been saved in the masterDirectory we can generate our first time-lagged data to do a background estimation. Inside ``continuesFAR_generation.out`` you will see the first condor dagmans to be submitted.
 When the first jobs have finished they will save the time-lagged data in ``falseAlarmRates/temp`` directory. Each job will save an individual file. 
 
 The inference script is constantly checking to see if there are any files created for inference. When it sees them you will star seeing the inference information inside ``continuous_FAR_inference_#######``.
 **The continuous FAR inference mode output has a number attached to it. That number is the unix time it was created and it can help us troubleshooting the script. So do not worry if you see many of them appearing over time.**
 
 After two hours you will also be able to see the first efficiency results and plots inside ``efficiencies``.
-
-Offline search timeline
-=======================
-
-For offline search, after the the offline_search script is run, it will create a number of condor jobs whose number is related to the number of segments the search is run on. While the jobs are run, any potential triggers will be saved in trigger_directory and also their corresponding trigger directory will be created inside triggerplot_directory.
-
```

### Comparing `mly_pipeline-0.5.5/docs/source/settingupasearch.rst` & `mly_pipeline-0.5.7/docs/source/settingupasearch.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     
     mly-pipeline-init -p ./mysearch
     
 Where instead of ``mysearch`` you can use a more apropriate name that fits your
 need. The command above will create the directory ``./mysearch`` and also the subdirectories
 below (these are their default names):
 
-    - triggerplot_directory
     - trigger_directory
     - output_directory
     - masterDirectory
     - bufferDirectory
     - falseAlarmRates
     - efficiencies
     - log
@@ -124,33 +123,31 @@
 --------------------
 
 The following are just the directory names of the directories created by with 
 the ``initialization.py``. If the default names were used, this will look like:
 
 * **output_directory**:"output_directory"
 * **trigger_directory**:"trigger_directory"
-* **triggerplot_directory**:"triggerplot_directory"
 * **masterDirectory**:"masterDirectory"
 * **bufferDirectory**:"bufferDirectory"
 * **falseAlarmRates**:"falseAlarmRates"
 * **efficiencies**:"efficiencies"
+* **log**:"log"
 
-After this we have the path to your local mlyPipeline installation. This is 
-identified automatically when you run the ``initialization.py``, and it will look
-like below, do not edit that unles you moved your mlyPipeline directory.
+The log level that will be used for the log files.
+* **log_level**:"INFO"
 
-* **mlyPipelineSource**:"/home/<albert.einstein>/extraPath/mlyPipeline"
 
 User and accounting group for condor jobs.
 
 * **user_name**: This is automatically filled by the enviroment
 
 * **accounting_group_user**: It defaults to be the same as user_name.
 
-* **accounting_group**: "allsky.mlyonline"
+* **accounting_group**: "ligo.dev.o4.burst.allsky.mlyonline"
 
 This is the name of the search directory, in our case it will look like:
 
 * **path** :"./mysearch"
     
 Generator Function Parameters
 -----------------------------
@@ -162,18 +159,20 @@
 * **duration**:1 Duration of processing window
 * **detectors**:"HLV" Detectors used for the search
 
 The prefix dictionary of the paths of directories where O3-replay and MDC data are. If the
 source of the data you use is different, you need to edit this parameter, after
 creating the search directory.
 
-* **frames_directory**: A dictionary with entries for H, L and V for the detectors. For each detector it has a path to the directory of the frame files that are going to be used. The default is empty but if you specified a mode of initialization then this will be filled with the respective paths.
+* **frames_directory**: A dictionary with entries for H, L and V for the detectors. For each detector it has a path to the directory of the frame files that are going to be used or a frame name recognised by gwdatafind. The default is empty but if you specified a mode of initialization then this will be filled with the respective paths.
 
 * **channels**: Also a dictionary with entries for H, L and V for the detectors. For each detector it has the channel that is going to be used. The default is empty but if you specified a mode of initialization then this will be filled with the respective channels.
 
+* **state_vector**: Dictionary with the statevectors used only for the online search. For anything else, it is empty. 
+
 * **segment_list**: This can be a path to a file that has segment intervals or it can be a list of two intervals corresponding to a start GPS time and an end GPS time. It is used only in offline searches. It defaults to an empty list.
 
 * **max_continuous_segment**: If the segments provided are too big we might want to break them in smaller runs. This parameter is the minimum segment size that will be used for one job. Also used only during offline searches. Defaults to 10000.
 
 
 Requesting Data Parameters
 --------------------------
@@ -190,15 +189,15 @@
 * **model1_path**:"/home/mly/models/model1_32V_No5.h5" Coincidence model (model 1).
 * **model2_path**:"/home/mly/models/model2_32V_No6.h5" Coherency model (model 2).
 * **td_pe_model_path**:"/home/mly/models/td_model" Time domain parameter estimation model.
 * **fd_pe_model_path**:"/home/mly/models/fd_model" Frequency domain parameter estimation model.
 
 Skymap
 ------
-* **skymap**:true Option for generation of skymaps with each issued event.
+* **skymap**:0 Option for generation of skymaps with each issued event. Currently 0 until skymap is ready.
 * **nside**:64 Parameter related to the resolution of the skymap.
 
 Efficiecy Calculation Parameters
 --------------------------------
     
 * **eff_config** A dictionary of parameters that are related to the efficiency tests.
 
@@ -212,14 +211,15 @@
 
 
 continuous FAR estimation Parameters
 ------------------------------------
 
 * **far_config** A dictionary of parameters that are related to the continuous FAR tests.
 
+  * **far_enabled**: true Option to opt out from false alarm rate calculation. Used by offline and online search at the initialisation of the search. If false make sure you provide a valid FARfile in the config entry **farfile**.
   * **batch_size**: 1024 Batch size of inference. Used by hermes client inference.
   * **threshold**: 2.3148e-05 Default for once per 2 days (Hz). **Used to define what is an event and what not.**
   * **restriction**: 0.0001 The minimum score of an inference to keep it in the history.
   * **max_lag**: 3600 The maximum time distance allowed, between two lagged segments.
   * **lags**: 1024 The number of timeshifts applied on the zero-lagged data to produced background tests.
   * **batches**: The amount of condor jobs to break the generation of background tests. **This can be adjusted if they do not finish within the hour.**
   * **visible_gpu_devices**: "local" GPU devices to use. Local will make all the local GPUs visible.
@@ -233,8 +233,10 @@
 * **maxDataFrameSize**:3600 The number of outputs grouped together in one data frame from the manager.
 * **trigger_destination**:null Which domain of GraceDB to send the event (test,dev,playground). When left empty it it does not send an event but it creates follow-up and seves it in a file with made up ID. If not, it takes one of the following options, shown below with the corresponding destination.
     * `test` which sends the alerts to: "https://gracedb-test.ligo.org/api" (needs certificate to work)
     * `playground` which sends the alerts to: "https://gracedb-playground.ligo.org/api" (needs certificate to work)
     * `dev1` which sends the alerts to: "https://gracedb-dev1.ligo.org/api" (needs certificate to work)
     * `online` which sends the alerts to: "https://gracedb.ligo.org/api" (used only for realtime online search after pipeline is approved)
 
+    * There are also some other entries that might appear here when the config will be updated at somepoint within the search. They are to be ignored.
+
 Now that the we went through the setting up of the search and the configuration parameters of it, we can see how to run such a search
```

### Comparing `mly_pipeline-0.5.5/mly_pipeline/__init__.py` & `mly_pipeline-0.5.7/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/mly_pipeline/continuous_FAR.py` & `mly_pipeline-0.5.7/mly_pipeline/continuous_FAR.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 batches =  config['far_config']['batches']
 batchNumber = kwdict['batchNumber']
 
 lags = config['far_config']['lags']
 selectedGPUs = config['far_config']['selectedGPUs']
 batch_size = config['far_config']['batch_size']
 parallelGenerations = config["far_config"]["parallelGenerations"]
+log_level = logging.getLevelName(config["log_level"])
 
 
 
 if config['far_config']['visible_gpu_devices']=="local":
     try:
         cuda_visible_devices = os.environ["CUDA_VISIBLE_DEVICES"] 
     except KeyError:
@@ -83,16 +84,16 @@
 
 
 
 
 # # # Initialising logging
 
 # create logger
-logger = logging.getLogger("logger_for_manager")
-logger.setLevel(logging.DEBUG)
+logger = logging.getLogger("logger_for_continious_FAR")
+logger.setLevel(log_level)
 
 
 # create console handler and set level to debug
 ch = logging.handlers.TimedRotatingFileHandler('log/continuousFAR-'+mode+'.log', when='M',interval=1, backupCount=1,)
 ch.setLevel(logging.DEBUG)
 
 # create formatter
@@ -655,15 +656,14 @@
                             results = np.append(results,response[:,1])
 
                     for i in range(int(num_inferences)-5):
                         trials = 1
                         response_ = client.get()
                         while response_ is None:
                             time.sleep(1e-2)
-                            logger.debug(f"PROCESSES client.get {i}: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
                             trials+=1
                             response_ = client.get()
                             if trials>=5000: raise(Exception("Trials exceeded 5000."))
 
                         response, _, __ = response_
                         #print(i,'response type ', type(response) , response.shape ,trials)
```

### Comparing `mly_pipeline-0.5.5/mly_pipeline/continuous_FAR_test.py` & `mly_pipeline-0.5.7/mly_pipeline/continuous_FAR_test.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/mly_pipeline/initialization.py` & `mly_pipeline-0.5.7/mly_pipeline/initialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
 
             if kwargs['far_config']['far_enabled']:
 
                 f.write("nohup python -m mly_pipeline.offline_search --mode set_file_system &> set_file_system.out & echo $!>>.jobids.txt" + "\n\n")
                 
                 f.write("sleep 300" + "\n\n")
 
-                f.write("nohup python -m mly_pipeline.continuous_FAR --mode generation &> continuous_FAR_generation.out & processID+=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
+                f.write("nohup python -m mly_pipeline.continuous_FAR --mode generation &> continuous_FAR_generation.out & generationID=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
                 f.write("nohup python -m mly_pipeline.continuous_FAR --mode inference &> continuous_FAR_inference.out & inferenceID=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
 
                 # Checking if the number of inference files stays 0 for a long time.
                 # If lag files increase without any new inference files, that means
                 # staling, and we add a staling point. If not we reset it to 0.
                 
                 f.write("staling_points=0" + "\n")
@@ -439,15 +439,16 @@
     output_directory = kwargs["output_directory"],
     trigger_directory = kwargs["trigger_directory"],
     masterDirectory = kwargs["masterDirectory"],
     bufferDirectory = kwargs["bufferDirectory"],
     falseAlarmRates = kwargs["falseAlarmRates"],
     efficiencies = kwargs["efficiencies"],
     log = "log",
-    
+    # Logging level
+    log_level = "INFO",
         
     # User name
     
     user_name = os.environ['HOME'].split("/")[-1],
 
 
     accounting_group_user = os.environ['HOME'].split("/")[-1],
@@ -502,16 +503,15 @@
         
     # If search time is left behind by that amount of seconds it skips ahead.
     gps_reset_time=32,
         
     # FAR file that is used to calculate FAR. It is used only at
     # the beggining of the search, until there is enough background estimation.
     
-    farfile= ("/home/vasileios.skliris/mly-hermes/outputs/FARfile" if kwargs['far'] 
-              else kwargs["falseAlarmRates"]+"/FARfile" ),
+    farfile= ("/home/vasileios.skliris/mly-hermes/outputs/FARfile" if (kwargs['far'] and 'ONLINE' in kwargs['search_mode']) else kwargs["falseAlarmRates"]+"/FARfile" ),
     
     # # # Models 
         
     # Model1 path, conincidence model.
     model1_path=("/home/mly/models/model1_32V_No5.h5"), 
         
     # Model2 path, coherence model.
@@ -521,15 +521,15 @@
 
     td_pe_model_path="/home/mly/models/td_model",
     fd_pe_model_path="/home/mly/models/fd_model",    
 
     # # # Skymap parameters
     
     # Skymap run option
-    skymap = 1,
+    skymap = 0,
 
     # Heilpix nside number for generated skymap.
     nside=64,  
         
 
     # # # Efficiency calculation parametersp
```

### Comparing `mly_pipeline-0.5.5/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.5.7/mly_pipeline/make_eff_estimation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/mly_pipeline/manager.py` & `mly_pipeline-0.5.7/mly_pipeline/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,36 +17,14 @@
 
 from mly.tools import dirlist
 from mly.datatools import *
 from .search_functions import *
 
 
 
-# # # Initialising logging
-
-# create logger
-logger = logging.getLogger("logger_for_manager")
-logger.setLevel(logging.DEBUG)
-
-
-
-# create console handler and set level to debug
-ch = logging.handlers.TimedRotatingFileHandler('log/manager.log', when='H',interval=12, backupCount=1,)
-ch.setLevel(logging.DEBUG)
-
-# create formatter
-formatter = logging.Formatter("%(asctime)s %(levelname)s: %(message)s")
-
-# add formatter to ch
-ch.setFormatter(formatter)
-
-# add ch to logger
-logger.addHandler(ch)
-
-
 # # # Managing arguments
 # 
 # List of arguments to pass:
 arguments = [
 
     "restriction",
     "timeUnit"
@@ -69,14 +47,40 @@
     
 with open('config.json') as json_file:
     config = json.load(json_file)
     
 config={ **kwdict , **config}
 
 
+# # # Initialising logging
+log_level = logging.getLevelName(config["log_level"])
+
+# create logger
+logger = logging.getLogger("logger_for_manager")
+logger.setLevel(log_level)
+
+
+
+# create console handler and set level to debug
+ch = logging.handlers.TimedRotatingFileHandler('log/manager.log', when='H',interval=12, backupCount=1,)
+ch.setLevel(logging.DEBUG)
+
+# create formatter
+formatter = logging.Formatter("%(asctime)s %(levelname)s: %(message)s")
+
+# add formatter to ch
+ch.setFormatter(formatter)
+
+# add ch to logger
+logger.addHandler(ch)
+
+
+
+
+
 def main(config):
 
     config = checkOutputDirectoryArguments(config)
 
     # The size in which we group the outputs
     if config['maxDataFrameSize']==None: 
         config['maxDataFrameSize']=3600
@@ -596,18 +600,18 @@
         with open('config.json') as json_file:
             config = json.load(json_file)
     # # # FAR test management 
     #
 
     # The list of all temporary inference files
     if os.path.isdir(config['falseAlarmRates']):
-        if config['restriction']==None: 
-            config['restriction']=0.0
+        if config['far_config']['restriction']==None: 
+            config['far_config']['restriction']=0.0
         
-        restriction=float(config['restriction'])
+        restriction=float(config['far_config']['restriction'])
         
         inference_temp_files = dirlist(config['falseAlarmRates'])
 
         for directory in ['hourly', 'condor', 'FARfile','temp']:
             if directory in inference_temp_files: inference_temp_files.remove(directory)
```

### Comparing `mly_pipeline-0.5.5/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.5.7/mly_pipeline/mly_to_grace.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/mly_pipeline/offline_search.py` & `mly_pipeline-0.5.7/mly_pipeline/offline_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,15 +365,18 @@
                 plt.savefig(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_strain.png")
                 plt.clf()
                 # Creating the correlation plot
                 thepod.plot(type_="correlation")
                 plt.savefig(
                     f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_correlation.png")
                 plt.clf()
-
+                # Creating the tf_map plot
+                thepod.plot('tf_map')
+                plt.savefig(
+                    f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_tfmap.png")
 
                 if config['skymap']:
 
                     # Create skymap plugin:
                     sky_map_plugin = createSkymapPlugin(
                         config["nside"], config["fs"], config["duration"])
```

### Comparing `mly_pipeline-0.5.5/mly_pipeline/search.py` & `mly_pipeline-0.5.7/mly_pipeline/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,33 +7,14 @@
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
 os.environ["OMP_NUM_THREADS"] = "1"
 
 import logging
 from logging import handlers
 import subprocess
 
-
-logger = logging.getLogger("logger_for_search")
-logger.setLevel(logging.DEBUG)
-
-
-# create console handler and set level to debug
-ch = handlers.TimedRotatingFileHandler('log/search.log', when='H',interval=12, backupCount=1,)
-ch.setLevel(logging.DEBUG)
-
-# create formatter
-formatter = logging.Formatter("%(asctime)s %(levelname)s: %(message)s")
-
-# add formatter to ch
-ch.setFormatter(formatter)
-
-# add ch to logger
-logger.addHandler(ch)
-
-
 import numpy as np
 import argparse
 import sys
 import pickle
 
 from lal import gpstime
 
@@ -137,16 +118,33 @@
         config = json.load(json_file)
     
     config = { **config , **kwargs }
     # # # Command line arguments processing
     
     # Check arguments and set values in config dict:
     config = checkArguments(config)
-    config['logger'] = 'search.log'
 
+    log_level = logging.getLevelName(config["log_level"])
+
+    logger = logging.getLogger("logger_for_search")
+    logger.setLevel(logging.DEBUG)
+
+
+    # create console handler and set level to debug
+    ch = handlers.TimedRotatingFileHandler('log/search.log', when='H',interval=12, backupCount=1,)
+    ch.setLevel(log_level)
+
+    # create formatter
+    formatter = logging.Formatter("%(asctime)s %(levelname)s: %(message)s")
+
+    # add formatter to ch
+    ch.setFormatter(formatter)
+
+    # add ch to logger
+    logger.addHandler(ch)
     logger.debug(f"PROCESSES after  loading config: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
 
 
     # # # Setup parameters for the models
     
     # Loading models
```

### Comparing `mly_pipeline-0.5.5/mly_pipeline/search_functions.py` & `mly_pipeline-0.5.7/mly_pipeline/search_functions.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.5.7/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.5.7/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.5/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.5.7/mly_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.5.5
+Version: 0.5.7
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.5/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.5.7/mly_pipeline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 docs/build/html/_static/underscore-1.3.1.js
 docs/build/html/_static/underscore.js
 docs/build/html/_static/websupport.js
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/runningasearch.rst
+docs/source/runningasearchoffline.rst
+docs/source/runningasearchonline.rst
 docs/source/settingupasearch.rst
 mly_pipeline/__init__.py
 mly_pipeline/continuous_FAR.py
 mly_pipeline/continuous_FAR_test.py
 mly_pipeline/initialization.py
 mly_pipeline/make_eff_estimation.py
 mly_pipeline/manager.py
```

### Comparing `mly_pipeline-0.5.5/pyproject.toml` & `mly_pipeline-0.5.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.5.5"
+version = "0.5.7"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
```

