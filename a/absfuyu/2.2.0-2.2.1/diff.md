# Comparing `tmp/absfuyu-2.2.0.tar.gz` & `tmp/absfuyu-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-_vasoj_t\absfuyu-2.2.0.tar", last modified: Tue Jun 27 11:09:14 2023, max compression
+gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-bakrli7g\absfuyu-2.2.1.tar", last modified: Thu Jul 13 18:11:23 2023, max compression
```

## Comparing `absfuyu-2.2.0.tar` & `absfuyu-2.2.1.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/
--rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.2.0/LICENSE
--rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3836 2023-06-27 11:09:14.000000 absfuyu-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.2.0/README.md
--rw-rw-rw-   0        0        0     1161 2023-06-05 17:50:56.000000 absfuyu-2.2.0/extra_requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/images/
--rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.2.0/images/repository-image-crop.png
--rw-rw-rw-   0        0        0      193 2023-06-05 17:50:56.000000 absfuyu-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.2.0/requirements.txt
--rw-rw-rw-   0        0        0     1360 2023-06-27 11:09:14.000000 absfuyu-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/
--rw-rw-rw-   0        0        0      941 2023-06-27 11:01:33.000000 absfuyu-2.2.0/src/absfuyu/__init__.py
--rw-rw-rw-   0        0        0     6530 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/__main__.py
--rw-rw-rw-   0        0        0     2566 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/calculation.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/collections/
--rw-rw-rw-   0        0        0     1938 2023-06-09 13:43:36.000000 absfuyu-2.2.0/src/absfuyu/collections/__init__.py
--rw-rw-rw-   0        0        0    14620 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/collections/content.py
--rw-rw-rw-   0        0        0    22151 2023-06-16 11:44:52.000000 absfuyu-2.2.0/src/absfuyu/collections/data_extension.py
--rw-rw-rw-   0        0        0     6742 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/collections/generator.py
--rw-rw-rw-   0        0        0     5822 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/collections/human.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/config/
--rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.2.0/src/absfuyu/config/__init__.py
--rw-rw-rw-   0        0        0      791 2023-06-27 11:08:57.000000 absfuyu-2.2.0/src/absfuyu/config/config.json
--rw-rw-rw-   0        0        0     1555 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/config/config2.py
--rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.2.0/src/absfuyu/config/template.json
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/contrib/
--rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.2.0/src/absfuyu/contrib/__init__.py
--rw-rw-rw-   0        0        0     8190 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/contrib/basic_lunar_calendar.py
--rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.2.0/src/absfuyu/contrib/color_extract.py
--rw-rw-rw-   0        0        0     3313 2023-06-15 07:52:56.000000 absfuyu-2.2.0/src/absfuyu/core.py
--rw-rw-rw-   0        0        0      832 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/everything.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/extensions/
--rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.2.0/src/absfuyu/extensions/__init__.py
--rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.2.0/src/absfuyu/extensions/beautiful.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/
--rw-rw-rw-   0        0        0    11971 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/WGS.py
--rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/__init__.py
--rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/horoscope.py
--rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/password_hash.py
--rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/pkglib.py
--rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/primo_cal.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/short_link/
--rw-rw-rw-   0        0        0      150 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/short_link/__init__.py
--rw-rw-rw-   0        0        0     5069 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/short_link/rebrandly.py
--rw-rw-rw-   0        0        0     2775 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/extensions/dev/tarot.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/extensions/extra/
--rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.2.0/src/absfuyu/extensions/extra/__init__.py
--rw-rw-rw-   0        0        0     7416 2023-06-27 10:59:07.000000 absfuyu-2.2.0/src/absfuyu/extensions/extra/data_analysis.py
--rw-rw-rw-   0        0        0     6001 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/fun.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/game/
--rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.2.0/src/absfuyu/game/__init__.py
--rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.2.0/src/absfuyu/game/sudoku.py
--rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.2.0/src/absfuyu/game/tictactoe.py
--rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.2.0/src/absfuyu/game/wordle.py
--rw-rw-rw-   0        0        0     3752 2023-06-09 09:17:28.000000 absfuyu-2.2.0/src/absfuyu/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/pkg_data/
--rw-rw-rw-   0        0        0     3016 2023-06-27 11:00:53.000000 absfuyu-2.2.0/src/absfuyu/pkg_data/__init__.py
--rw-rw-rw-   0        0        0   247094 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/pkg_data/chemistry.json
--rw-rw-rw-   0        0        0    86614 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/pkg_data/tarot.json
--rw-rw-rw-   0        0        0     5848 2023-06-25 13:09:10.000000 absfuyu-2.2.0/src/absfuyu/sort.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/tools/
--rw-rw-rw-   0        0        0      136 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/__init__.py
--rw-rw-rw-   0        0        0     5853 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/converter.py
--rw-rw-rw-   0        0        0     7292 2023-06-09 14:49:10.000000 absfuyu-2.2.0/src/absfuyu/tools/keygen.py
--rw-rw-rw-   0        0        0     8482 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/obfuscator.py
--rw-rw-rw-   0        0        0     3008 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/stats.py
--rw-rw-rw-   0        0        0     1180 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/tools/web.py
--rw-rw-rw-   0        0        0    12499 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/unused.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu/util/
--rw-rw-rw-   0        0        0     2396 2023-06-09 13:47:13.000000 absfuyu-2.2.0/src/absfuyu/util/__init__.py
--rw-rw-rw-   0        0        0     2769 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/util/api.py
--rw-rw-rw-   0        0        0     2366 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/util/json_method.py
--rw-rw-rw-   0        0        0     5512 2023-06-15 08:10:16.000000 absfuyu-2.2.0/src/absfuyu/util/path.py
--rw-rw-rw-   0        0        0     3829 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/util/performance.py
--rw-rw-rw-   0        0        0     1230 2023-06-09 13:48:37.000000 absfuyu-2.2.0/src/absfuyu/util/pkl.py
--rw-rw-rw-   0        0        0     2499 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/util/zipped.py
--rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-2.2.0/src/absfuyu/version.py
--rw-rw-rw-   0        0        0     9951 2023-06-05 17:50:56.000000 absfuyu-2.2.0/src/absfuyu/version2.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/
--rw-rw-rw-   0        0        0     3836 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2531 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1266 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 11:09:14.000000 absfuyu-2.2.0/src/absfuyu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 11:09:14.000000 absfuyu-2.2.0/tests/
--rw-rw-rw-   0        0        0      805 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_DictKai.py
--rw-rw-rw-   0        0        0     3049 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_Generator.py
--rw-rw-rw-   0        0        0     3206 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_IntNumber.py
--rw-rw-rw-   0        0        0     2068 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_ListKai.py
--rw-rw-rw-   0        0        0     3246 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_Text.py
--rw-rw-rw-   0        0        0      632 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_api.py
--rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.2.0/tests/test_beautiful.py
--rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.2.0/tests/test_config.py
--rw-rw-rw-   0        0        0      769 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_converter.py
--rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.2.0/tests/test_everything.py
--rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.2.0/tests/test_extensions.py
--rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.2.0/tests/test_fun.py
--rw-rw-rw-   0        0        0      425 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_json_method.py
--rw-rw-rw-   0        0        0      706 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_obfuscator.py
--rw-rw-rw-   0        0        0      649 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_path.py
--rw-rw-rw-   0        0        0      119 2023-05-25 10:14:50.000000 absfuyu-2.2.0/tests/test_pkg_data.py
--rw-rw-rw-   0        0        0     1133 2023-06-05 17:50:56.000000 absfuyu-2.2.0/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/
+-rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3836 2023-07-13 18:11:23.000000 absfuyu-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.2.1/README.md
+-rw-rw-rw-   0        0        0     1161 2023-06-05 17:50:56.000000 absfuyu-2.2.1/extra_requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:22.000000 absfuyu-2.2.1/images/
+-rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.2.1/images/repository-image-crop.png
+-rw-rw-rw-   0        0        0      193 2023-06-05 17:50:56.000000 absfuyu-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.2.1/requirements.txt
+-rw-rw-rw-   0        0        0     1360 2023-07-13 18:11:23.000000 absfuyu-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:22.000000 absfuyu-2.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:22.000000 absfuyu-2.2.1/src/absfuyu/
+-rw-rw-rw-   0        0        0      941 2023-06-27 11:01:33.000000 absfuyu-2.2.1/src/absfuyu/__init__.py
+-rw-rw-rw-   0        0        0     6530 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/__main__.py
+-rw-rw-rw-   0        0        0     2566 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/calculation.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/collections/
+-rw-rw-rw-   0        0        0     1938 2023-06-09 13:43:36.000000 absfuyu-2.2.1/src/absfuyu/collections/__init__.py
+-rw-rw-rw-   0        0        0    14620 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/collections/content.py
+-rw-rw-rw-   0        0        0    22151 2023-06-16 11:44:52.000000 absfuyu-2.2.1/src/absfuyu/collections/data_extension.py
+-rw-rw-rw-   0        0        0     6742 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/collections/generator.py
+-rw-rw-rw-   0        0        0     7436 2023-07-13 18:06:22.000000 absfuyu-2.2.1/src/absfuyu/collections/human.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/config/
+-rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.2.1/src/absfuyu/config/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-07-13 18:11:05.000000 absfuyu-2.2.1/src/absfuyu/config/config.json
+-rw-rw-rw-   0        0        0     1555 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/config/config2.py
+-rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.2.1/src/absfuyu/config/template.json
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/contrib/
+-rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.2.1/src/absfuyu/contrib/__init__.py
+-rw-rw-rw-   0        0        0     8190 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/contrib/basic_lunar_calendar.py
+-rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.2.1/src/absfuyu/contrib/color_extract.py
+-rw-rw-rw-   0        0        0     3313 2023-06-15 07:52:56.000000 absfuyu-2.2.1/src/absfuyu/core.py
+-rw-rw-rw-   0        0        0      832 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/everything.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/extensions/
+-rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.2.1/src/absfuyu/extensions/__init__.py
+-rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.2.1/src/absfuyu/extensions/beautiful.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/
+-rw-rw-rw-   0        0        0    11971 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/WGS.py
+-rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-06-29 19:18:21.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/country.py
+-rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/horoscope.py
+-rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/password_hash.py
+-rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/pkglib.py
+-rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/primo_cal.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/short_link/
+-rw-rw-rw-   0        0        0      150 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/short_link/__init__.py
+-rw-rw-rw-   0        0        0     5069 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/short_link/rebrandly.py
+-rw-rw-rw-   0        0        0     2775 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/extensions/dev/tarot.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/extensions/extra/
+-rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.2.1/src/absfuyu/extensions/extra/__init__.py
+-rw-rw-rw-   0        0        0     7890 2023-06-28 07:52:19.000000 absfuyu-2.2.1/src/absfuyu/extensions/extra/data_analysis.py
+-rw-rw-rw-   0        0        0     6001 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/fun.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/game/
+-rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.2.1/src/absfuyu/game/__init__.py
+-rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.2.1/src/absfuyu/game/sudoku.py
+-rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.2.1/src/absfuyu/game/tictactoe.py
+-rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.2.1/src/absfuyu/game/wordle.py
+-rw-rw-rw-   0        0        0     3752 2023-06-09 09:17:28.000000 absfuyu-2.2.1/src/absfuyu/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/pkg_data/
+-rw-rw-rw-   0        0        0     3016 2023-06-27 11:00:53.000000 absfuyu-2.2.1/src/absfuyu/pkg_data/__init__.py
+-rw-rw-rw-   0        0        0   247094 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/pkg_data/chemistry.json
+-rw-rw-rw-   0        0        0    86614 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/pkg_data/tarot.json
+-rw-rw-rw-   0        0        0     5848 2023-06-25 13:09:10.000000 absfuyu-2.2.1/src/absfuyu/sort.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/tools/
+-rw-rw-rw-   0        0        0      136 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/tools/__init__.py
+-rw-rw-rw-   0        0        0     5853 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/tools/converter.py
+-rw-rw-rw-   0        0        0     7292 2023-06-09 14:49:10.000000 absfuyu-2.2.1/src/absfuyu/tools/keygen.py
+-rw-rw-rw-   0        0        0     8482 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/tools/obfuscator.py
+-rw-rw-rw-   0        0        0     3008 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/tools/stats.py
+-rw-rw-rw-   0        0        0     1180 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/tools/web.py
+-rw-rw-rw-   0        0        0    12499 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/unused.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu/util/
+-rw-rw-rw-   0        0        0     2484 2023-07-13 17:26:49.000000 absfuyu-2.2.1/src/absfuyu/util/__init__.py
+-rw-rw-rw-   0        0        0     2769 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/util/api.py
+-rw-rw-rw-   0        0        0     2374 2023-06-29 17:58:12.000000 absfuyu-2.2.1/src/absfuyu/util/json_method.py
+-rw-rw-rw-   0        0        0    12561 2023-06-30 03:50:11.000000 absfuyu-2.2.1/src/absfuyu/util/lunar.py
+-rw-rw-rw-   0        0        0     5512 2023-06-29 19:18:59.000000 absfuyu-2.2.1/src/absfuyu/util/path.py
+-rw-rw-rw-   0        0        0     3829 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/util/performance.py
+-rw-rw-rw-   0        0        0     1230 2023-06-09 13:48:37.000000 absfuyu-2.2.1/src/absfuyu/util/pkl.py
+-rw-rw-rw-   0        0        0     2499 2023-06-05 17:50:56.000000 absfuyu-2.2.1/src/absfuyu/util/zipped.py
+-rw-rw-rw-   0        0        0     8608 2023-06-29 18:07:07.000000 absfuyu-2.2.1/src/absfuyu/version.py
+-rw-rw-rw-   0        0        0    11177 2023-06-29 18:47:40.000000 absfuyu-2.2.1/src/absfuyu/version2.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/src/absfuyu.egg-info/
+-rw-rw-rw-   0        0        0     3836 2023-07-13 18:11:22.000000 absfuyu-2.2.1/src/absfuyu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2595 2023-07-13 18:11:22.000000 absfuyu-2.2.1/src/absfuyu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 18:11:22.000000 absfuyu-2.2.1/src/absfuyu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-13 18:11:22.000000 absfuyu-2.2.1/src/absfuyu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1266 2023-07-13 18:11:22.000000 absfuyu-2.2.1/src/absfuyu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 18:11:22.000000 absfuyu-2.2.1/src/absfuyu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 18:11:23.000000 absfuyu-2.2.1/tests/
+-rw-rw-rw-   0        0        0      805 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_DictKai.py
+-rw-rw-rw-   0        0        0     3049 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_Generator.py
+-rw-rw-rw-   0        0        0     3206 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_IntNumber.py
+-rw-rw-rw-   0        0        0     2068 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_ListKai.py
+-rw-rw-rw-   0        0        0     3246 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_Text.py
+-rw-rw-rw-   0        0        0      632 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_api.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.2.1/tests/test_beautiful.py
+-rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.2.1/tests/test_config.py
+-rw-rw-rw-   0        0        0      769 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_converter.py
+-rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.2.1/tests/test_everything.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.2.1/tests/test_extensions.py
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.2.1/tests/test_fun.py
+-rw-rw-rw-   0        0        0      425 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_json_method.py
+-rw-rw-rw-   0        0        0      706 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_obfuscator.py
+-rw-rw-rw-   0        0        0      649 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_path.py
+-rw-rw-rw-   0        0        0      152 2023-06-28 01:45:31.000000 absfuyu-2.2.1/tests/test_pkg_data.py
+-rw-rw-rw-   0        0        0     1133 2023-06-05 17:50:56.000000 absfuyu-2.2.1/tests/test_util.py
```

### Comparing `absfuyu-2.2.0/LICENSE` & `absfuyu-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/PKG-INFO` & `absfuyu-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 2.2.0
+Version: 2.2.1
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -18,29 +18,29 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: beautiful
 Provides-Extra: rich
 Provides-Extra: dev
-Provides-Extra: click
-Provides-Extra: extra
+Provides-Extra: beautiful
 Provides-Extra: cli
+Provides-Extra: extra
+Provides-Extra: click
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
 Provides-Extra: setuptools
 Provides-Extra: wheel
 Provides-Extra: pipx
-Provides-Extra: tools
 Provides-Extra: requests
+Provides-Extra: tools
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
 Provides-Extra: fixers
 Provides-Extra: autoimport
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: absfuyu Version: 2.2.0 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.2.1 Summary: A small collection
 of code Home-page: https://github.com/AbsoluteWinter/absfuyu Author:
 somewhatcold (AbsoluteWinter) Author-email:
 this.is.a.fake.mail@fakemail.absfuyu.com License: MIT Project-URL:
 Documentation, https://absolutewinter.github.io/absfuyu Project-URL: Source
 Code, https://github.com/AbsoluteWinter/absfuyu Project-URL: Bug Tracker,
 https://github.com/AbsoluteWinter/absfuyu/issues Keywords: utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Development Status :: 5 - Production/
 Stable Classifier: Natural Language :: English Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown Provides-Extra: beautiful Provides-
-Extra: rich Provides-Extra: dev Provides-Extra: click Provides-Extra: extra
-Provides-Extra: cli Provides-Extra: colorama Provides-Extra: build Provides-
+Description-Content-Type: text/markdown Provides-Extra: rich Provides-Extra:
+dev Provides-Extra: beautiful Provides-Extra: cli Provides-Extra: extra
+Provides-Extra: click Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
-Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
-requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
-matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
+Extra: wheel Provides-Extra: pipx Provides-Extra: requests Provides-Extra:
+tools Provides-Extra: numpy Provides-Extra: pandas Provides-Extra: matplotlib
+Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra: fixers
+Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
 Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
 sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
 Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
```

### Comparing `absfuyu-2.2.0/README.md` & `absfuyu-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/extra_requirements.txt` & `absfuyu-2.2.1/extra_requirements.txt`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/images/repository-image-crop.png` & `absfuyu-2.2.1/images/repository-image-crop.png`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/setup.cfg` & `absfuyu-2.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/setup.py` & `absfuyu-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/__init__.py` & `absfuyu-2.2.1/src/absfuyu/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/__main__.py` & `absfuyu-2.2.1/src/absfuyu/__main__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/calculation.py` & `absfuyu-2.2.1/src/absfuyu/calculation.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/collections/__init__.py` & `absfuyu-2.2.1/src/absfuyu/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/collections/content.py` & `absfuyu-2.2.1/src/absfuyu/collections/content.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/collections/data_extension.py` & `absfuyu-2.2.1/src/absfuyu/collections/data_extension.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/collections/generator.py` & `absfuyu-2.2.1/src/absfuyu/collections/generator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/collections/human.py` & `absfuyu-2.2.1/src/absfuyu/collections/human.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,137 @@
 """
 Absfuyu: Human
 ---
 Human related stuff
 
-Version: 1.0.0
-Date updated: 19/04/2023 (dd/mm/yyyy)
+Version: 1.2.0
+Date updated: 14/07/2023 (dd/mm/yyyy)
 """
 
 
 # Module level
 ###########################################################################
 __all__ = [
     "Human", "Person"
 ]
 
 
 # Library
 ###########################################################################
-from datetime import datetime
+from datetime import datetime, time
+from typing import Optional, Union
 
 try:
     from dateutil.relativedelta import relativedelta
 except:
     import subprocess
     subprocess.run("pip install -U python-dateutil".split())
 
 from absfuyu.calculation import add_to_one_digit
 from absfuyu.fun import zodiac_sign
+# from absfuyu.util import set_min_max
+from absfuyu.version import Version_
 
 
 # Class
 ###########################################################################
+class BloodType:
+    A_PLUS = "A+"
+    A_MINUS = "A-"
+    AB_PLUS = "AB+"
+    AB_MINUS = "AB-"
+    B_PLUS = "B+"
+    B_MINUS = "B-"
+    O_PLUS = "O+"
+    O_MINUS = "O-"
+    A = "A"
+    AB = "AB"
+    B = "B"
+    O = "O"
+    OTHER = None
+
+
 class Human:
     """
     Basic human data
-
-    Birthday in yyyy/mm/dd format
     """
 
     __MEASUREMENT = "m|kg" # Metric system
-    __VERSION = {"major": 1, "minor": 0, "patch": 4} # Internal version class check
+    __VERSION = Version_(1, 1, 0) # Internal version class check
 
-    def __init__(self,
-                 first_name: str,
-                 last_name: str = None,
-                 birthday: str = None
+    def __init__(
+            self,
+            first_name: str,
+            last_name: Optional[str] = None,
+            birthday: Union[str, datetime, None] = None,
+            birth_time: Optional[str] = None,
+            gender: Union[bool, None] = None
         ) -> None:
+        """
+        :param first_name: First name
+        :param last_name: Last name
+        :param birthday: Birthday in format: `yyyy/mm/dd`
+        :param birth_time: Birth time in format: `hh:mm`
+        :param gender: `True`: Male; `False`: Female (biologicaly)
+        """
         # Name
         self.first_name = first_name
         self.last_name = last_name
         self.name = f"{self.last_name}, {self.first_name}" if self.last_name is not None else self.first_name
 
         # Birthday
-        self.birthday = birthday
-        date_str = self.birthday
-        if date_str is None:
-            # date_str = "1970/01/01"
-            self.birthday = datetime.now().date()
+        now = datetime.now()
+        if birthday is None:
+            modified_birthday = now.date()
         else:
             for x in ["/", "-"]:
-                date_str = date_str.replace(x, "/")
-        # split = date_str.split("/")
-            date = datetime.strptime(date_str, "%Y/%m/%d")
-            self.birthday = date
+                birthday = birthday.replace(x, "/")
+            modified_birthday = datetime.strptime(birthday, "%Y/%m/%d")
+            # birthday = list(map(int, birthday.split("/")))
+            # modified_birthday = date(*birthday)
+            # modified_birthday = date(birthday[0], birthday[1], birthday[2])
+
+        if birth_time is None:
+            modified_birthtime = now.time()
+        else:
+            birth_time = list(map(int, birth_time.split(":")))
+            modified_birthtime = time(*birth_time)
+            # modified_birthtime = time(birth_time[0], birth_time[1])
+        
+        self.birthday = modified_birthday.date()
+        self.birth_time = modified_birthtime
+
+        self.birth = datetime(
+            modified_birthday.year,
+            modified_birthday.month,
+            modified_birthday.day,
+            modified_birthtime.hour,
+            modified_birthtime.minute
+        )
 
         # Others
-        self.gender: bool = None # True: Male; False: Female
+        self.gender: bool = gender # True: Male; False: Female
         self.height: float = None # centimeter
         self.weight: float = None # kilogram
-        self.blood_type: str = None # ["A+", "A-", "B+", "B-", "O+", "O-", "AB+", "AB-"]
+        self.blood_type: Union[str, BloodType] = BloodType.OTHER
     
     def __str__(self) -> str:
         class_name = self.__class__.__name__
         return f"{class_name}({str(self.name)})"
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
         name = str(self.name)
         gender = "M" if self.is_male else "F"
         return f"{class_name}({name} ({self.age}|{gender}))"
     
     @classmethod
     def JohnDoe(cls):
         """Dummy Human for test"""
-        temp = cls("John", "Doe", "1980/01/01")
+        temp = cls("John", "Doe", "1980/01/01", "00:00")
         temp.update({"gender": True, "height": 180, "weight": 80, "blood_type": "O+"})
         return temp
     
     @property
     def is_male(self) -> bool:
         """
         True: Male; False: Female
@@ -116,15 +160,16 @@
                 rdelta = relativedelta(now, self.birthday)
             return round(rdelta.years + rdelta.months/12, 2)
         else:
             return None
     
     @property
     def is_adult(self):
-        return self.age > 18
+        """Check if age >= 18"""
+        return self.age >= 18
     
     @property
     def bmi(self):
         r"""
         Body Mass Index (kg/m^2)
 
         Formula: $\frac{weight (kg)}{height (m)^2}$
@@ -157,18 +202,25 @@
 
 
 class Person(Human):
     """
     More detail Human data
     """
 
-    __VERSION = {"major": 1, "minor": 0, "patch": 1} # Internal version class check
+    __VERSION = Version_(1, 1, 0) # Internal version class check
 
-    def __init__(self, first_name: str, last_name: str = None, birthday: str = None) -> None:
-        super().__init__(first_name, last_name, birthday)
+    def __init__(
+            self,
+            first_name: str,
+            last_name: Optional[str] = None,
+            birthday: Union[str, datetime, None] = None,
+            birth_time: Optional[str] = None,
+            gender: Union[bool, None] = None
+        ) -> None:
+        super().__init__(first_name, last_name, birthday, birth_time, gender)
         self.address: str = None
         self.hometown: str = None
         self.email: str = None
         self.phone_number: str = None
         self.nationality = None
         self.likes: list = None
         self.hates: list = None
@@ -196,8 +248,8 @@
         temp = f"{self.birthday.year}{self.birthday.month}{self.birthday.day}"
         return add_to_one_digit(temp, master_number=True)
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
-    print(Person.JohnDoe().dir_())
+    print(Person.JohnDoe().__dict__)
```

### Comparing `absfuyu-2.2.0/src/absfuyu/config/__init__.py` & `absfuyu-2.2.1/src/absfuyu/config/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/config/config.json` & `absfuyu-2.2.1/src/absfuyu/config/template.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925%*

 * *Differences: {"'version'": "{'major': 1, 'minor': 1, 'patch': 4}"}*

```diff
@@ -18,14 +18,14 @@
         "test": {
             "default": false,
             "help": "Test",
             "value": false
         }
     },
     "version": {
-        "major": 2,
-        "minor": 2,
-        "patch": 0,
+        "major": 1,
+        "minor": 1,
+        "patch": 4,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-2.2.0/src/absfuyu/config/config2.py` & `absfuyu-2.2.1/src/absfuyu/config/config2.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/config/template.json` & `absfuyu-2.2.1/src/absfuyu/config/config.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925%*

 * *Differences: {"'version'": "{'major': 2, 'minor': 2, 'patch': 1}"}*

```diff
@@ -18,14 +18,14 @@
         "test": {
             "default": false,
             "help": "Test",
             "value": false
         }
     },
     "version": {
-        "major": 1,
-        "minor": 1,
-        "patch": 4,
+        "major": 2,
+        "minor": 2,
+        "patch": 1,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-2.2.0/src/absfuyu/contrib/basic_lunar_calendar.py` & `absfuyu-2.2.1/src/absfuyu/contrib/basic_lunar_calendar.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/contrib/color_extract.py` & `absfuyu-2.2.1/src/absfuyu/contrib/color_extract.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/core.py` & `absfuyu-2.2.1/src/absfuyu/core.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/everything.py` & `absfuyu-2.2.1/src/absfuyu/everything.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/beautiful.py` & `absfuyu-2.2.1/src/absfuyu/extensions/beautiful.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/dev/WGS.py` & `absfuyu-2.2.1/src/absfuyu/extensions/dev/WGS.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/dev/__init__.py` & `absfuyu-2.2.1/src/absfuyu/extensions/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/dev/horoscope.py` & `absfuyu-2.2.1/src/absfuyu/extensions/dev/horoscope.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/dev/password_hash.py` & `absfuyu-2.2.1/src/absfuyu/extensions/dev/password_hash.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/dev/pkglib.py` & `absfuyu-2.2.1/src/absfuyu/extensions/dev/pkglib.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/dev/primo_cal.py` & `absfuyu-2.2.1/src/absfuyu/extensions/dev/primo_cal.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/dev/short_link/rebrandly.py` & `absfuyu-2.2.1/src/absfuyu/extensions/dev/short_link/rebrandly.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/dev/tarot.py` & `absfuyu-2.2.1/src/absfuyu/extensions/dev/tarot.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/extensions/extra/__init__.py` & `absfuyu-2.2.1/src/absfuyu/extensions/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/fun.py` & `absfuyu-2.2.1/src/absfuyu/fun.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/game/__init__.py` & `absfuyu-2.2.1/src/absfuyu/game/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/game/sudoku.py` & `absfuyu-2.2.1/src/absfuyu/game/sudoku.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/game/tictactoe.py` & `absfuyu-2.2.1/src/absfuyu/game/tictactoe.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/game/wordle.py` & `absfuyu-2.2.1/src/absfuyu/game/wordle.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/logger.py` & `absfuyu-2.2.1/src/absfuyu/logger.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/pkg_data/__init__.py` & `absfuyu-2.2.1/src/absfuyu/pkg_data/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/pkg_data/chemistry.json` & `absfuyu-2.2.1/src/absfuyu/pkg_data/chemistry.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/pkg_data/tarot.json` & `absfuyu-2.2.1/src/absfuyu/pkg_data/tarot.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/sort.py` & `absfuyu-2.2.1/src/absfuyu/sort.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/tools/converter.py` & `absfuyu-2.2.1/src/absfuyu/tools/converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/tools/keygen.py` & `absfuyu-2.2.1/src/absfuyu/tools/keygen.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/tools/obfuscator.py` & `absfuyu-2.2.1/src/absfuyu/tools/obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/tools/stats.py` & `absfuyu-2.2.1/src/absfuyu/tools/stats.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/tools/web.py` & `absfuyu-2.2.1/src/absfuyu/tools/web.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/unused.py` & `absfuyu-2.2.1/src/absfuyu/unused.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/util/__init__.py` & `absfuyu-2.2.1/src/absfuyu/util/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Absufyu: Utilities
 ---
 Some random utilities
 
-Version: 1.2.0
-Date updated: 09/06/2023 (dd/mm/yyyy)
+Version: 1.3.0
+Date updated: 14/07/2023 (dd/mm/yyyy)
 """
 
 
 # Library
 ###########################################################################
 import pkg_resources
 from typing import Union
 
 from absfuyu.logger import logger, log_debug
 from absfuyu.util.api import APIRequest
 from absfuyu.util.json_method import JsonFile, load_json
+from absfuyu.util.lunar import LunarCalendar
 from absfuyu.util.path import DirStructure
-from absfuyu.util.performance import *
+from absfuyu.util.performance import measure_performance, source_this, var_check
 from absfuyu.util.pkl import Pickler
 from absfuyu.util.zipped import Zipper
 
 
 # Function
 ###########################################################################
 def get_installed_package(version_included: bool = False):
```

### Comparing `absfuyu-2.2.0/src/absfuyu/util/api.py` & `absfuyu-2.2.1/src/absfuyu/util/api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/util/json_method.py` & `absfuyu-2.2.1/src/absfuyu/util/json_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.sort_keys = sort_keys
         self.data = {}
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.json_file_location.name})"
     def __repr__(self) -> str:
         return self.__str__()
     
-    def load_json(self):
+    def load_json(self) -> dict:
         """Load json file"""
         with open(self.json_file_location, "r", encoding=self.encoding) as file:
             self.data = json.load(file)
         return self.data
 
     def save_json(self):
         """Save json file"""
```

### Comparing `absfuyu-2.2.0/src/absfuyu/util/path.py` & `absfuyu-2.2.1/src/absfuyu/util/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Absfuyu: Path
 ---
 Path related
 
-Version: 1.1.1
-Date updated: 15/06/2023 (dd/mm/yyyy)
+Version: 1.1.2
+Date updated: 30/06/2023 (dd/mm/yyyy)
 
 Feature:
 - DirStructure
 """
 
 
 # Module level
@@ -158,17 +158,17 @@
         ---
         For typical python library
         ```
         >>> test = DirStructure(<source path>)
         >>> test.list_structure(
                 "__pycache__",
                 ".pyc",
-                "tempCodeRunnerFile.py",
                 "__init__", 
-                "__main__"
+                "__main__",
+                "tempCodeRunnerFile.py"
             )
         ...
         ```
         """
         temp = self._list_dir(*ignore)
         out = self._separate_dir_and_files(temp)
         return "\n".join(out)
```

### Comparing `absfuyu-2.2.0/src/absfuyu/util/performance.py` & `absfuyu-2.2.1/src/absfuyu/util/performance.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/util/pkl.py` & `absfuyu-2.2.1/src/absfuyu/util/pkl.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/util/zipped.py` & `absfuyu-2.2.1/src/absfuyu/util/zipped.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/src/absfuyu/version.py` & `absfuyu-2.2.1/src/absfuyu/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,30 @@
     "check_for_update",
 ]
 
 
 
 # Library
 ##############################################################
+from collections import namedtuple
 import json as __json
 import subprocess as __subprocess
 # from typing import Dict as __Dict
 from typing import Optional as __Optional
 # from typing import Union as __Union
 from urllib.error import URLError as __URLError
 from urllib.request import Request as __Request
 from urllib.request import urlopen as __urlopen
 
 from . import config as __config
 
 
+Version_ = namedtuple("Version_", ["major", "minor", "patch"])
+
+
 # Function
 ##############################################################
 #__ABSFUYU_RSS = "https://pypi.org/rss/project/absfuyu/releases.xml"
 
 def __get_latest_version_legacy(package_name: str = "absfuyu"):
     """
     Load data from PyPI's RSS -- OLD
```

### Comparing `absfuyu-2.2.0/src/absfuyu/version2.py` & `absfuyu-2.2.1/src/absfuyu/version2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,162 +1,179 @@
 """
 Absfuyu: Version [W.I.P]
 ---
 Package versioning module
 
-Version: 2.0.0
-Date updated: 22/05/2023 (dd/mm/yyyy)
+Version: 2.0.0dev1
+Date updated: 30/06/2023 (dd/mm/yyyy)
 
 Features:
 - Version
 
 Todo:
 - Fix config loader
 - finish version bump
 """
 
 
 # Module level
 ###########################################################################
 __all__ = [
-    "__version__",
+    "__version__"
 ]
 
 # Library
 ###########################################################################
 from collections import namedtuple
 import json
+from pathlib import Path
 import subprocess
+from typing import List, Optional, Union
 from urllib.error import URLError
-from urllib.request import Request
-from urllib.request import urlopen
+from urllib.request import Request, urlopen
 
-from absfuyu import config
+# from absfuyu import __title__
+from absfuyu.core import CONFIG_PATH
 from absfuyu.logger import logger
-from absfuyu.util.json_method import load_json
+from absfuyu.util.json_method import JsonFile
+
+
+# Setup - Type hint
+###########################################################################
+Version_ = namedtuple("Version_", ["major", "minor", "patch"])
+VersionSerial = namedtuple("VersionSerial", ["major", "minor", "patch", "serial"])
 
 
 # Class
 ###########################################################################
 class ReleaseOption:
     """
     `MAJOR`, `MINOR`, `PATCH`
     """
     MAJOR: str = "major"
     MINOR: str = "minor"
     PATCH: str = "patch"
 
-    def all_option():
+    # @staticmethod
+    def all_option() -> List[str]:
         return [__class__.MAJOR, __class__.MINOR, __class__.PATCH]
 
 class ReleaseLevel:
     """
     `FINAL`, `DEV`, `RC`
     """
     FINAL: str = "final"
     DEV: str = "dev"
     RC: str = "rc" # Release candidate
 
-    def all_level():
+    # @staticmethod
+    def all_level() -> List[str]:
         return [__class__.FINAL, __class__.DEV, __class__.RC]
 
 class Version:
     """
     Versioning module
     """
-    def __init__(self, package_name: str = "absfuyu") -> None:
+    def __init__(
+            self,
+            package_name: Optional[str] = None,
+            *,
+            config_file_location: Union[str, Path, None] = None
+        ) -> None:
+        """
+        package_name: Name of the package
+        config_file_location: Location of the config file (.json file) if any
+        """
         # Get config
         try:
-            cfg = load_json(config.CONFIG_LOC)
-            version = cfg["version"]
+            self.config_file = JsonFile(Path(config_file_location))
+            cfg: dict = self.config_file.load_json()
+            # version: dict = cfg.get("version", {"major": 1, "minor": 0, "patch": 0, "release_level": ReleaseLevel.FINAL, "serial": 0})
+            version: dict = cfg.get("version")
         except:
-            logger.warning("Can't load config file")
+            logger.error("Can't load config file")
 
-        self.major: int = version["major"]
-        self.minor: int = version["minor"]
-        self.patch: int = version["patch"]
-        self.release_level: str = version["release_level"]
-        self.serial: int = version["serial"]
+        self.major: int = version.get("major")
+        self.minor: int = version.get("minor")
+        self.patch: int = version.get("patch")
+        self.release_level: str = version.get("release_level")
+        self.serial: int = version.get("serial")
 
+        # Set package name
         self.package_name = package_name
     
     def __str__(self) -> str:
         temp = ".".join(map(str, self.version))
         return temp
     def __repr__(self) -> str:
         return self.__str__()
     
     @property
-    def version(self):
+    def version(self) -> Union[Version_, VersionSerial]:
         """Convert into `tuple`"""
-        Ver = namedtuple("Ver", ["major", "minor", "patch"])
-        VerSerial = namedtuple("VersionSerial", ["major", "minor", "patch", "serial"])
         if self.release_level.startswith(ReleaseLevel.FINAL):
-            return Ver(self.major, self.minor, self.patch)
+            return Version_(self.major, self.minor, self.patch)
         else:
             temp = self.release_level + str(self.serial)
-            return VerSerial(self.major, self.minor, self.patch, temp)
+            return VersionSerial(self.major, self.minor, self.patch, temp)
     
-    def to_dict(self):
+    def to_dict(self) -> dict:
         """Convert into `dict`"""
         return {
             "major": self.major,
             "minor": self.minor,
             "patch": self.patch,
             "release_level": self.release_level,
             "serial": self.serial
         }
     
 
     # Check for update
-    def _get_latest_version_legacy(self):
-        """
-        Load data from PyPI's RSS -- OLD
-        """
-        rss = f"https://pypi.org/rss/project/{self.package_name}/releases.xml"
-        req = Request(rss)
+    @staticmethod
+    def _fetch_data_from_server(link: str):
+        """Fetch version data of package from pypi.org"""
+        req = Request(link)
         try:
             response = urlopen(req)
+            # return response
         except URLError as e:
             if hasattr(e, "reason"):
-                print("Failed to reach server.")
-                print("Reason: ", e.reason)
+                logger.error("Failed to reach server.")
+                logger.error("Reason: ", e.reason)
             elif hasattr(e, "code"):
-                print("The server couldn\'t fulfill the request.")
-                print("Error code: ", e.code)
+                logger.error("The server couldn\'t fulfill the request.")
+                logger.error("Error code: ", e.code)
+        except:
+            logger.error("Fetch failed!")
         else:
-            xml_file = response.read().decode()
-            ver = xml_file[xml_file.find("<item>"):xml_file.find("</item>")]
-            version = ver[ver.find("<title>")+len("<title>"):ver.find("</title>")]
-            return version
+            return response.read().decode()
 
-    def _load_data_from_json(self, json_link: str):
+    def _get_latest_version_legacy(self) -> str:
+        """
+        Load data from PyPI's RSS -- OLD
+        """
+        rss = f"https://pypi.org/rss/project/{self.package_name}/releases.xml"
+        xml_file: str = self._fetch_data_from_server(rss)
+        ver = xml_file[xml_file.find("<item>"):xml_file.find("</item>")] # First item
+        version = ver[ver.find("<title>")+len("<title>"):ver.find("</title>")]
+        return version
+
+    def _load_data_from_json(self, json_link: str) -> dict:
         """
         Load data from api then convert to json
         """
-        req = Request(json_link)
-        try:
-            response = urlopen(req)
-        except URLError as e:
-            if hasattr(e, "reason"):
-                print("Failed to reach server.")
-                print("Reason: ", e.reason)
-            elif hasattr(e, "code"):
-                print("The server couldn't fulfill the request.")
-                print("Error code: ", e.code)
-        else:
-            json_file = response.read().decode()
-            return json.loads(json_file)
+        json_file: str = self._fetch_data_from_server(json_link)
+        return json.loads(json_file)
 
-    def _get_latest_version(self):
+    def _get_latest_version(self) -> str:
         """
         Get latest version from PyPI's API
         """
         link = f"https://pypi.org/pypi/{self.package_name}/json"
-        ver = self._load_data_from_json(link)["info"]["version"]
+        ver: str = self._load_data_from_json(link)["info"]["version"]
         logger.debug(f"Latest: {ver}")
         return ver
 
     def _get_update(self):
         """
         Run pip upgrade command
         """
@@ -166,15 +183,21 @@
     def check_for_update(
             self,
             *,
             force_update: bool = False,
         ) -> None:
         """
         Check for latest update
+
+        force_update: Auto update the package when run
         """
+        if self.package_name is None:
+            logger.warning("No package name provided")
+            return None
+        
         try:
             latest = self._get_latest_version()
         except:
             latest = self._get_latest_version_legacy()
         current = __version__
         logger.debug(f"Current: {current} | Lastest: {latest}")
         
@@ -272,19 +295,21 @@
 
 
     def __release_to_pypi(
             self,
             option: str = ReleaseOption.PATCH,
             channel: str = ReleaseLevel.FINAL,
             safety_lock_off: bool = False,
-        ):
+        ) -> None:
         """
-        Not intended for end-user
+        Developer only! Not intended for end-user
         
-        Developer only!
+        option: ReleaseOption
+        channel: ReleaseLevel
+        safety_lock_off: Set to `True` to execute this function
         """
         if not safety_lock_off:
             return None
         
         logger.debug("Bumping version...")
         
         self.bump(option=option, channel=channel)
@@ -301,18 +326,18 @@
         except:
             logger.warning("Release failed!")
             return None
 
 
 # Init
 ###########################################################################
-__version__ = str(Version())
+__version__ = str(Version(package_name="absfuyu", config_file_location=CONFIG_PATH))
 # __version__ = Version()
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     logger.setLevel(10)
-    test = Version()
-    print(test.version)
-    print(test.bump())
+    test = Version(package_name="absfuyu", config_file_location=CONFIG_PATH)
+    print(test.version, __version__, test.__dict__)
+    # print(test.bump())
```

### Comparing `absfuyu-2.2.0/src/absfuyu.egg-info/PKG-INFO` & `absfuyu-2.2.1/src/absfuyu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 2.2.0
+Version: 2.2.1
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -18,29 +18,29 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: beautiful
 Provides-Extra: rich
 Provides-Extra: dev
-Provides-Extra: click
-Provides-Extra: extra
+Provides-Extra: beautiful
 Provides-Extra: cli
+Provides-Extra: extra
+Provides-Extra: click
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
 Provides-Extra: setuptools
 Provides-Extra: wheel
 Provides-Extra: pipx
-Provides-Extra: tools
 Provides-Extra: requests
+Provides-Extra: tools
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
 Provides-Extra: fixers
 Provides-Extra: autoimport
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: absfuyu Version: 2.2.0 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.2.1 Summary: A small collection
 of code Home-page: https://github.com/AbsoluteWinter/absfuyu Author:
 somewhatcold (AbsoluteWinter) Author-email:
 this.is.a.fake.mail@fakemail.absfuyu.com License: MIT Project-URL:
 Documentation, https://absolutewinter.github.io/absfuyu Project-URL: Source
 Code, https://github.com/AbsoluteWinter/absfuyu Project-URL: Bug Tracker,
 https://github.com/AbsoluteWinter/absfuyu/issues Keywords: utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Development Status :: 5 - Production/
 Stable Classifier: Natural Language :: English Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown Provides-Extra: beautiful Provides-
-Extra: rich Provides-Extra: dev Provides-Extra: click Provides-Extra: extra
-Provides-Extra: cli Provides-Extra: colorama Provides-Extra: build Provides-
+Description-Content-Type: text/markdown Provides-Extra: rich Provides-Extra:
+dev Provides-Extra: beautiful Provides-Extra: cli Provides-Extra: extra
+Provides-Extra: click Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
-Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
-requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
-matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
+Extra: wheel Provides-Extra: pipx Provides-Extra: requests Provides-Extra:
+tools Provides-Extra: numpy Provides-Extra: pandas Provides-Extra: matplotlib
+Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra: fixers
+Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
 Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
 sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
 Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
```

### Comparing `absfuyu-2.2.0/src/absfuyu.egg-info/SOURCES.txt` & `absfuyu-2.2.1/src/absfuyu.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/absfuyu/contrib/__init__.py
 src/absfuyu/contrib/basic_lunar_calendar.py
 src/absfuyu/contrib/color_extract.py
 src/absfuyu/extensions/__init__.py
 src/absfuyu/extensions/beautiful.py
 src/absfuyu/extensions/dev/WGS.py
 src/absfuyu/extensions/dev/__init__.py
+src/absfuyu/extensions/dev/country.py
 src/absfuyu/extensions/dev/horoscope.py
 src/absfuyu/extensions/dev/password_hash.py
 src/absfuyu/extensions/dev/pkglib.py
 src/absfuyu/extensions/dev/primo_cal.py
 src/absfuyu/extensions/dev/tarot.py
 src/absfuyu/extensions/dev/short_link/__init__.py
 src/absfuyu/extensions/dev/short_link/rebrandly.py
@@ -61,14 +62,15 @@
 src/absfuyu/tools/keygen.py
 src/absfuyu/tools/obfuscator.py
 src/absfuyu/tools/stats.py
 src/absfuyu/tools/web.py
 src/absfuyu/util/__init__.py
 src/absfuyu/util/api.py
 src/absfuyu/util/json_method.py
+src/absfuyu/util/lunar.py
 src/absfuyu/util/path.py
 src/absfuyu/util/performance.py
 src/absfuyu/util/pkl.py
 src/absfuyu/util/zipped.py
 tests/test_DictKai.py
 tests/test_Generator.py
 tests/test_IntNumber.py
```

### Comparing `absfuyu-2.2.0/src/absfuyu.egg-info/requires.txt` & `absfuyu-2.2.1/src/absfuyu.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -2,86 +2,86 @@
 [:python_version == "3.7"]
 typing_extensions>=3.7.4
 
 [LunarCalendar]
 LunarCalendar>=0.0.9
 
 [all]
-tox>=3.24.5
-scipy
-pandas
-LunarCalendar>=0.0.9
-unidecode
-autoimport
-virtualenv>=20.13.0
-pytest>=6.2.5
-black>=22.1.0
-build
-sphinx
-sphinx_rtd_theme
-wheel
-rich
-python-dateutil
-click>=8.0.0
+pipx
 twine>=3.7.1
+autoimport
 requests
-colorama>=0.4
+rich
+wheel
+scipy
+build
 setuptools>=51.0.0
+pytest>=6.2.5
+unidecode
+pandas
+python-dateutil
 numpy
-pipx
+black>=22.1.0
+colorama>=0.4
+virtualenv>=20.13.0
+sphinx_rtd_theme
+sphinx
 matplotlib
+click>=8.0.0
+tox>=3.24.5
+LunarCalendar>=0.0.9
 
 [autoimport]
 autoimport
 
 [beautiful]
 rich
 
 [black]
 black>=22.1.0
 
 [build]
 build
 
 [cli]
-click>=8.0.0
 colorama>=0.4
+click>=8.0.0
 
 [click]
 click>=8.0.0
 
 [colorama]
 colorama>=0.4
 
 [dev]
-colorama>=0.4
-pytest>=6.2.5
 build
-setuptools>=51.0.0
+colorama>=0.4
+virtualenv>=20.13.0
+sphinx_rtd_theme
 sphinx
+setuptools>=51.0.0
 click>=8.0.0
-twine>=3.7.1
-sphinx_rtd_theme
-wheel
-rich
+pytest>=6.2.5
 pipx
 unidecode
-virtualenv>=20.13.0
+twine>=3.7.1
+rich
+wheel
 
 [extra]
-colorama>=0.4
-python-dateutil
 numpy
+colorama>=0.4
 click>=8.0.0
-pandas
-scipy
-LunarCalendar>=0.0.9
 unidecode
 requests
+pandas
+python-dateutil
 matplotlib
+LunarCalendar>=0.0.9
+scipy
 
 [fixers]
 autoimport
 black>=22.1.0
 
 [matplotlib]
 matplotlib
@@ -116,16 +116,16 @@
 [sphinx]
 sphinx
 
 [sphinx_rtd_theme]
 sphinx_rtd_theme
 
 [test]
-pytest>=6.2.5
 tox>=3.24.5
+pytest>=6.2.5
 
 [tools]
 requests
 
 [tox]
 tox>=3.24.5
```

### Comparing `absfuyu-2.2.0/tests/test_DictKai.py` & `absfuyu-2.2.1/tests/test_DictKai.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_Generator.py` & `absfuyu-2.2.1/tests/test_Generator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_IntNumber.py` & `absfuyu-2.2.1/tests/test_IntNumber.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_ListKai.py` & `absfuyu-2.2.1/tests/test_ListKai.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_Text.py` & `absfuyu-2.2.1/tests/test_Text.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_api.py` & `absfuyu-2.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_config.py` & `absfuyu-2.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_converter.py` & `absfuyu-2.2.1/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_obfuscator.py` & `absfuyu-2.2.1/tests/test_obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_path.py` & `absfuyu-2.2.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.2.0/tests/test_util.py` & `absfuyu-2.2.1/tests/test_util.py`

 * *Files identical despite different names*

