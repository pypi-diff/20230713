# Comparing `tmp/calcbench_api_client-9.0.1.tar.gz` & `tmp/calcbench_api_client-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\calcbench_api_client-9.0.1.tar", last modified: Tue Jul 11 21:10:22 2023, max compression
+gzip compressed data, was "dist\calcbench_api_client-9.1.0.tar", last modified: Thu Jul 13 20:23:00 2023, max compression
```

## Comparing `calcbench_api_client-9.0.1.tar` & `calcbench_api_client-9.1.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:22.614845 calcbench_api_client-9.0.1/
--rw-rw-rw-   0        0        0      288 2021-05-18 15:59:00.000000 calcbench_api_client-9.0.1/.gitignore
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:21.575475 calcbench_api_client-9.0.1/.vscode/
--rw-rw-rw-   0        0        0      478 2021-05-18 15:57:34.000000 calcbench_api_client-9.0.1/.vscode/launch.json
--rw-rw-rw-   0        0        0     1988 2023-07-11 21:10:22.613844 calcbench_api_client-9.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      984 2023-06-06 17:23:29.000000 calcbench_api_client-9.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:21.610483 calcbench_api_client-9.0.1/calcbench/
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:21.624515 calcbench_api_client-9.0.1/calcbench/.vscode/
--rw-rw-rw-   0        0        0      477 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/calcbench/.vscode/launch.json
--rw-rw-rw-   0        0        0     1812 2023-07-11 21:08:40.000000 calcbench_api_client-9.0.1/calcbench/__init__.py
--rw-rw-rw-   0        0        0    11918 2023-03-16 20:14:00.000000 calcbench_api_client-9.0.1/calcbench/api_client.py
--rw-rw-rw-   0        0        0     2279 2023-01-24 18:56:25.000000 calcbench_api_client-9.0.1/calcbench/api_query_params.py
--rw-rw-rw-   0        0        0    15686 2023-05-08 15:32:07.000000 calcbench_api_client-9.0.1/calcbench/business_combinations.py
--rw-rw-rw-   0        0        0     3920 2021-11-18 16:53:40.000000 calcbench_api_client-9.0.1/calcbench/companies.py
--rw-rw-rw-   0        0        0    17369 2022-02-15 16:51:25.000000 calcbench_api_client-9.0.1/calcbench/dimensional.py
--rw-rw-rw-   0        0        0    18077 2022-11-02 16:00:32.000000 calcbench_api_client-9.0.1/calcbench/disclosures.py
--rw-rw-rw-   0        0        0     5726 2023-05-31 16:10:02.000000 calcbench_api_client-9.0.1/calcbench/downloaders.py
--rw-rw-rw-   0        0        0     3700 2022-05-31 19:56:12.000000 calcbench_api_client-9.0.1/calcbench/face_statements.py
--rw-rw-rw-   0        0        0    11386 2023-01-19 15:50:21.000000 calcbench_api_client-9.0.1/calcbench/filing.py
--rw-rw-rw-   0        0        0     8910 2022-07-15 14:07:23.000000 calcbench_api_client-9.0.1/calcbench/listener.py
--rw-rw-rw-   0        0        0      650 2020-12-11 14:41:26.000000 calcbench_api_client-9.0.1/calcbench/metrics.py
--rw-rw-rw-   0        0        0     3269 2022-11-07 16:43:08.000000 calcbench_api_client-9.0.1/calcbench/press_release.py
--rw-rw-rw-   0        0        0     4456 2021-11-18 17:07:01.000000 calcbench_api_client-9.0.1/calcbench/raw_numeric_XBRL.py
--rw-rw-rw-   0        0        0     5968 2022-03-18 15:19:02.000000 calcbench_api_client-9.0.1/calcbench/raw_numeric_non_XBRL.py
--rw-rw-rw-   0        0        0    19558 2023-07-11 20:43:04.000000 calcbench_api_client-9.0.1/calcbench/standardized_numeric.py
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:21.672476 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/
--rw-rw-rw-   0        0        0     1988 2023-07-11 21:10:21.000000 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2584 2023-07-11 21:10:21.000000 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 21:10:21.000000 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/dependency_links.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:21.698496 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/dist/
--rw-rw-rw-   0        0        0    68879 2022-01-27 15:55:06.000000 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
--rw-rw-rw-   0        0        0   418889 2022-01-27 15:55:05.000000 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz
--rw-rw-rw-   0        0        0      270 2023-07-11 21:10:21.000000 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-11 21:10:21.000000 calcbench_api_client-9.0.1/calcbench_api_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:21.709515 calcbench_api_client-9.0.1/conda-recipe/
--rw-rw-rw-   0        0        0      909 2022-06-30 14:34:48.000000 calcbench_api_client-9.0.1/conda-recipe/meta.yaml
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:21.747474 calcbench_api_client-9.0.1/docs/
--rw-rw-rw-   0        0        0        0 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/docs/.nojekyll
--rw-rw-rw-   0        0        0      654 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:22.007082 calcbench_api_client-9.0.1/docs/html/
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:22.016617 calcbench_api_client-9.0.1/docs/html/_sources/
--rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.0.1/docs/html/_sources/getting-started.rst.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:22.474842 calcbench_api_client-9.0.1/docs/html/_static/
--rw-rw-rw-   0        0        0    11885 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/_static/alabaster.css
--rw-rw-rw-   0        0        0    15541 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/_static/basic.css
--rw-rw-rw-   0        0        0       42 2020-03-19 21:59:59.000000 calcbench_api_client-9.0.1/docs/html/_static/custom.css
--rw-rw-rw-   0        0        0     9630 2021-07-29 16:06:08.000000 calcbench_api_client-9.0.1/docs/html/_static/doctools.js
--rw-rw-rw-   0        0        0      361 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/docs/html/_static/file.png
--rw-rw-rw-   0        0        0   278292 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/docs/html/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0   280364 2020-03-19 22:00:02.000000 calcbench_api_client-9.0.1/docs/html/_static/jquery-3.4.1.js
--rw-rw-rw-   0        0        0   287630 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.1/docs/html/_static/jquery-3.5.1.js
--rw-rw-rw-   0        0        0    89476 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.1/docs/html/_static/jquery.js
--rw-rw-rw-   0        0        0    11151 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/docs/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/docs/html/_static/plus.png
--rw-rw-rw-   0        0        0     4874 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/_static/pygments.css
--rw-rw-rw-   0        0        0    16578 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.1/docs/html/_static/searchtools.js
--rw-rw-rw-   0        0        0    68420 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.1/docs/html/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    35168 2020-03-19 22:00:02.000000 calcbench_api_client-9.0.1/docs/html/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    19530 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.1/docs/html/_static/underscore.js
--rw-rw-rw-   0        0        0    20866 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/business-combinations.html
--rw-rw-rw-   0        0        0    12664 2022-01-27 15:45:17.000000 calcbench_api_client-9.0.1/docs/html/companies.html
--rw-rw-rw-   0        0        0   116341 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/dimensional.html
--rw-rw-rw-   0        0        0    65621 2023-04-12 21:26:04.000000 calcbench_api_client-9.0.1/docs/html/disclosures.html
--rw-rw-rw-   0        0        0    19795 2023-07-10 22:58:11.000000 calcbench_api_client-9.0.1/docs/html/downloaders.html
--rw-rw-rw-   0        0        0    35986 2023-01-26 15:02:06.000000 calcbench_api_client-9.0.1/docs/html/face-statements.html
--rw-rw-rw-   0        0        0    46164 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/filings.html
--rw-rw-rw-   0        0        0   107809 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/genindex.html
--rw-rw-rw-   0        0        0    14252 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.1/docs/html/getting-started.html
--rw-rw-rw-   0        0        0     7429 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/index.html
--rw-rw-rw-   0        0        0     6017 2022-01-27 15:45:17.000000 calcbench_api_client-9.0.1/docs/html/metrics.html
--rw-rw-rw-   0        0        0    37974 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/numeric-data.html
--rw-rw-rw-   0        0        0    20870 2023-04-12 21:26:05.000000 calcbench_api_client-9.0.1/docs/html/press-release.html
--rw-rw-rw-   0        0        0    11099 2023-01-19 19:18:13.000000 calcbench_api_client-9.0.1/docs/html/push-notification.html
--rw-rw-rw-   0        0        0     7083 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/py-modindex.html
--rw-rw-rw-   0        0        0    18689 2022-01-27 15:45:18.000000 calcbench_api_client-9.0.1/docs/html/raw-numeric-XBRL.html
--rw-rw-rw-   0        0        0    36953 2023-01-26 15:02:06.000000 calcbench_api_client-9.0.1/docs/html/raw-numeric-non-XBRL.html
--rw-rw-rw-   0        0        0     4370 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/search.html
--rw-rw-rw-   0        0        0    47607 2023-07-11 13:29:23.000000 calcbench_api_client-9.0.1/docs/html/searchindex.js
--rw-rw-rw-   0        0        0       64 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/docs/index.html
--rwxrwxrwx   0        0        0      796 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-07-11 21:10:22.612848 calcbench_api_client-9.0.1/docs/source/
--rw-rw-rw-   0        0        0      274 2021-06-24 19:28:47.000000 calcbench_api_client-9.0.1/docs/source/business-combinations.rst
--rw-rw-rw-   0        0        0      132 2021-02-22 22:31:03.000000 calcbench_api_client-9.0.1/docs/source/companies.rst
--rw-rw-rw-   0        0        0     1907 2022-01-27 15:45:13.000000 calcbench_api_client-9.0.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      275 2021-10-13 15:58:17.000000 calcbench_api_client-9.0.1/docs/source/dimensional.rst
--rw-rw-rw-   0        0        0      369 2021-07-23 16:57:12.000000 calcbench_api_client-9.0.1/docs/source/disclosures.rst
--rw-rw-rw-   0        0        0      113 2022-01-13 16:45:20.000000 calcbench_api_client-9.0.1/docs/source/downloaders.rst
--rw-rw-rw-   0        0        0      176 2022-05-31 19:08:45.000000 calcbench_api_client-9.0.1/docs/source/face-statements.rst
--rw-rw-rw-   0        0        0       90 2022-01-27 17:08:05.000000 calcbench_api_client-9.0.1/docs/source/filings.rst
--rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.0.1/docs/source/getting-started.rst
--rw-rw-rw-   0        0        0      669 2022-01-13 16:44:16.000000 calcbench_api_client-9.0.1/docs/source/index.rst
--rw-rw-rw-   0        0        0       70 2020-11-12 16:28:47.000000 calcbench_api_client-9.0.1/docs/source/metrics.rst
--rw-rw-rw-   0        0        0      906 2022-11-07 16:43:08.000000 calcbench_api_client-9.0.1/docs/source/numeric-data.rst
--rw-rw-rw-   0        0        0      181 2021-11-18 18:30:32.000000 calcbench_api_client-9.0.1/docs/source/press-release.rst
--rw-rw-rw-   0        0        0     1002 2020-12-11 15:03:48.000000 calcbench_api_client-9.0.1/docs/source/push-notification.rst
--rw-rw-rw-   0        0        0      208 2021-05-04 16:55:43.000000 calcbench_api_client-9.0.1/docs/source/raw-numeric-XBRL.rst
--rw-rw-rw-   0        0        0      215 2021-04-05 15:28:06.000000 calcbench_api_client-9.0.1/docs/source/raw-numeric-non-XBRL.rst
--rw-rw-rw-   0        0        0       93 2020-10-22 17:34:48.000000 calcbench_api_client-9.0.1/publish.PS1
--rw-rw-rw-   0        0        0       42 2023-07-11 21:10:22.614845 calcbench_api_client-9.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-01-26 15:29:46.000000 calcbench_api_client-9.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.927363 calcbench_api_client-9.1.0/
+-rw-rw-rw-   0        0        0      288 2021-05-18 15:59:00.000000 calcbench_api_client-9.1.0/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-13 20:22:59.906591 calcbench_api_client-9.1.0/.vscode/
+-rw-rw-rw-   0        0        0      478 2021-05-18 15:57:34.000000 calcbench_api_client-9.1.0/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1988 2023-07-13 20:23:00.925364 calcbench_api_client-9.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2023-06-06 17:23:29.000000 calcbench_api_client-9.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 20:22:59.948593 calcbench_api_client-9.1.0/calcbench/
+drwxrwxrwx   0        0        0        0 2023-07-13 20:22:59.965736 calcbench_api_client-9.1.0/calcbench/.vscode/
+-rw-rw-rw-   0        0        0      477 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/calcbench/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1812 2023-07-13 20:18:18.000000 calcbench_api_client-9.1.0/calcbench/__init__.py
+-rw-rw-rw-   0        0        0    11918 2023-03-16 20:14:00.000000 calcbench_api_client-9.1.0/calcbench/api_client.py
+-rw-rw-rw-   0        0        0     2325 2023-07-13 19:10:00.000000 calcbench_api_client-9.1.0/calcbench/api_query_params.py
+-rw-rw-rw-   0        0        0    15686 2023-05-08 15:32:07.000000 calcbench_api_client-9.1.0/calcbench/business_combinations.py
+-rw-rw-rw-   0        0        0     3920 2021-11-18 16:53:40.000000 calcbench_api_client-9.1.0/calcbench/companies.py
+-rw-rw-rw-   0        0        0    17369 2022-02-15 16:51:25.000000 calcbench_api_client-9.1.0/calcbench/dimensional.py
+-rw-rw-rw-   0        0        0    18077 2022-11-02 16:00:32.000000 calcbench_api_client-9.1.0/calcbench/disclosures.py
+-rw-rw-rw-   0        0        0     5726 2023-05-31 16:10:02.000000 calcbench_api_client-9.1.0/calcbench/downloaders.py
+-rw-rw-rw-   0        0        0     3700 2022-05-31 19:56:12.000000 calcbench_api_client-9.1.0/calcbench/face_statements.py
+-rw-rw-rw-   0        0        0    11386 2023-01-19 15:50:21.000000 calcbench_api_client-9.1.0/calcbench/filing.py
+-rw-rw-rw-   0        0        0     8910 2022-07-15 14:07:23.000000 calcbench_api_client-9.1.0/calcbench/listener.py
+-rw-rw-rw-   0        0        0      650 2020-12-11 14:41:26.000000 calcbench_api_client-9.1.0/calcbench/metrics.py
+-rw-rw-rw-   0        0        0     3269 2022-11-07 16:43:08.000000 calcbench_api_client-9.1.0/calcbench/press_release.py
+-rw-rw-rw-   0        0        0     4456 2021-11-18 17:07:01.000000 calcbench_api_client-9.1.0/calcbench/raw_numeric_XBRL.py
+-rw-rw-rw-   0        0        0     5968 2022-03-18 15:19:02.000000 calcbench_api_client-9.1.0/calcbench/raw_numeric_non_XBRL.py
+-rw-rw-rw-   0        0        0    20183 2023-07-13 19:27:22.000000 calcbench_api_client-9.1.0/calcbench/standardized_numeric.py
+-rw-rw-rw-   0        0        0      664 2023-07-13 18:24:08.000000 calcbench_api_client-9.1.0/calcbench/standardized_parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.010593 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/
+-rw-rw-rw-   0        0        0     1988 2023-07-13 20:22:59.000000 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-07-13 20:22:59.000000 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 20:22:59.000000 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.039597 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/dist/
+-rw-rw-rw-   0        0        0    68879 2022-01-27 15:55:06.000000 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0   418889 2022-01-27 15:55:05.000000 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz
+-rw-rw-rw-   0        0        0      270 2023-07-13 20:22:59.000000 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 20:22:59.000000 calcbench_api_client-9.1.0/calcbench_api_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.052593 calcbench_api_client-9.1.0/conda-recipe/
+-rw-rw-rw-   0        0        0      909 2022-06-30 14:34:48.000000 calcbench_api_client-9.1.0/conda-recipe/meta.yaml
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.083592 calcbench_api_client-9.1.0/docs/
+-rw-rw-rw-   0        0        0        0 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/docs/.nojekyll
+-rw-rw-rw-   0        0        0      654 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.330365 calcbench_api_client-9.1.0/docs/html/
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.341366 calcbench_api_client-9.1.0/docs/html/_sources/
+-rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.1.0/docs/html/_sources/getting-started.rst.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.808364 calcbench_api_client-9.1.0/docs/html/_static/
+-rw-rw-rw-   0        0        0    11885 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/_static/alabaster.css
+-rw-rw-rw-   0        0        0    15541 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/_static/basic.css
+-rw-rw-rw-   0        0        0       42 2020-03-19 21:59:59.000000 calcbench_api_client-9.1.0/docs/html/_static/custom.css
+-rw-rw-rw-   0        0        0     9630 2021-07-29 16:06:08.000000 calcbench_api_client-9.1.0/docs/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      361 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/docs/html/_static/file.png
+-rw-rw-rw-   0        0        0   278292 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/docs/html/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0   280364 2020-03-19 22:00:02.000000 calcbench_api_client-9.1.0/docs/html/_static/jquery-3.4.1.js
+-rw-rw-rw-   0        0        0   287630 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.0/docs/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0        0        0    89476 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.0/docs/html/_static/jquery.js
+-rw-rw-rw-   0        0        0    11151 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/docs/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/docs/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4874 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    16578 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.0/docs/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0    68420 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.0/docs/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    35168 2020-03-19 22:00:02.000000 calcbench_api_client-9.1.0/docs/html/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    19530 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.0/docs/html/_static/underscore.js
+-rw-rw-rw-   0        0        0    20866 2023-07-13 19:27:28.000000 calcbench_api_client-9.1.0/docs/html/business-combinations.html
+-rw-rw-rw-   0        0        0    12664 2022-01-27 15:45:17.000000 calcbench_api_client-9.1.0/docs/html/companies.html
+-rw-rw-rw-   0        0        0   116341 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/dimensional.html
+-rw-rw-rw-   0        0        0    65621 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.0/docs/html/disclosures.html
+-rw-rw-rw-   0        0        0    19795 2023-07-10 22:58:11.000000 calcbench_api_client-9.1.0/docs/html/downloaders.html
+-rw-rw-rw-   0        0        0    35986 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.0/docs/html/face-statements.html
+-rw-rw-rw-   0        0        0    46164 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/filings.html
+-rw-rw-rw-   0        0        0   107809 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/genindex.html
+-rw-rw-rw-   0        0        0    14252 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.0/docs/html/getting-started.html
+-rw-rw-rw-   0        0        0     7429 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/index.html
+-rw-rw-rw-   0        0        0     6017 2022-01-27 15:45:17.000000 calcbench_api_client-9.1.0/docs/html/metrics.html
+-rw-rw-rw-   0        0        0    39118 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/numeric-data.html
+-rw-rw-rw-   0        0        0    20870 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.0/docs/html/press-release.html
+-rw-rw-rw-   0        0        0    11099 2023-01-19 19:18:13.000000 calcbench_api_client-9.1.0/docs/html/push-notification.html
+-rw-rw-rw-   0        0        0     7083 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/py-modindex.html
+-rw-rw-rw-   0        0        0    18689 2022-01-27 15:45:18.000000 calcbench_api_client-9.1.0/docs/html/raw-numeric-XBRL.html
+-rw-rw-rw-   0        0        0    36953 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.0/docs/html/raw-numeric-non-XBRL.html
+-rw-rw-rw-   0        0        0     4370 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/search.html
+-rw-rw-rw-   0        0        0    47634 2023-07-13 19:27:29.000000 calcbench_api_client-9.1.0/docs/html/searchindex.js
+-rw-rw-rw-   0        0        0       64 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/docs/index.html
+-rwxrwxrwx   0        0        0      796 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-07-13 20:23:00.921366 calcbench_api_client-9.1.0/docs/source/
+-rw-rw-rw-   0        0        0      274 2021-06-24 19:28:47.000000 calcbench_api_client-9.1.0/docs/source/business-combinations.rst
+-rw-rw-rw-   0        0        0      132 2021-02-22 22:31:03.000000 calcbench_api_client-9.1.0/docs/source/companies.rst
+-rw-rw-rw-   0        0        0     1907 2022-01-27 15:45:13.000000 calcbench_api_client-9.1.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      275 2021-10-13 15:58:17.000000 calcbench_api_client-9.1.0/docs/source/dimensional.rst
+-rw-rw-rw-   0        0        0      369 2021-07-23 16:57:12.000000 calcbench_api_client-9.1.0/docs/source/disclosures.rst
+-rw-rw-rw-   0        0        0      113 2022-01-13 16:45:20.000000 calcbench_api_client-9.1.0/docs/source/downloaders.rst
+-rw-rw-rw-   0        0        0      176 2022-05-31 19:08:45.000000 calcbench_api_client-9.1.0/docs/source/face-statements.rst
+-rw-rw-rw-   0        0        0       90 2022-01-27 17:08:05.000000 calcbench_api_client-9.1.0/docs/source/filings.rst
+-rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.1.0/docs/source/getting-started.rst
+-rw-rw-rw-   0        0        0      669 2022-01-13 16:44:16.000000 calcbench_api_client-9.1.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0       70 2020-11-12 16:28:47.000000 calcbench_api_client-9.1.0/docs/source/metrics.rst
+-rw-rw-rw-   0        0        0      906 2022-11-07 16:43:08.000000 calcbench_api_client-9.1.0/docs/source/numeric-data.rst
+-rw-rw-rw-   0        0        0      181 2021-11-18 18:30:32.000000 calcbench_api_client-9.1.0/docs/source/press-release.rst
+-rw-rw-rw-   0        0        0     1002 2020-12-11 15:03:48.000000 calcbench_api_client-9.1.0/docs/source/push-notification.rst
+-rw-rw-rw-   0        0        0      208 2021-05-04 16:55:43.000000 calcbench_api_client-9.1.0/docs/source/raw-numeric-XBRL.rst
+-rw-rw-rw-   0        0        0      215 2021-04-05 15:28:06.000000 calcbench_api_client-9.1.0/docs/source/raw-numeric-non-XBRL.rst
+-rw-rw-rw-   0        0        0       93 2020-10-22 17:34:48.000000 calcbench_api_client-9.1.0/publish.PS1
+-rw-rw-rw-   0        0        0       42 2023-07-13 20:23:00.927363 calcbench_api_client-9.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1418 2023-01-26 15:29:46.000000 calcbench_api_client-9.1.0/setup.py
```

### Comparing `calcbench_api_client-9.0.1/PKG-INFO` & `calcbench_api_client-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcbench_api_client
-Version: 9.0.1
+Version: 9.1.0
 Summary: Client for Calcbench data.
 Home-page: https://github.com/calcbench/python_api_client
 Author: Andrew Kittredge
 Author-email: andrew@calcbench.com
 License: Apache2
 Project-URL: Documentation, http://calcbench.github.io/python_api_client/html/index.html
 Project-URL: Examples, https://github.com/calcbench/notebooks
@@ -45,14 +45,14 @@
         
         @someben https://github.com/calcbench/python_api_client/commit/6c2312525fa365acc91bd8e979037fc2492845f3
         
 Keywords: finance accounting SEC 10-(K|Q)
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: Keyring
-Provides-Extra: pyarrow
 Provides-Extra: Listener
-Provides-Extra: BeautifulSoup
 Provides-Extra: tqdm
+Provides-Extra: BeautifulSoup
 Provides-Extra: Backoff
 Provides-Extra: Pandas
+Provides-Extra: pyarrow
+Provides-Extra: Keyring
```

### Comparing `calcbench_api_client-9.0.1/README.md` & `calcbench_api_client-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/__init__.py` & `calcbench_api_client-9.1.0/calcbench/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The "public" properties on the cb module
 
 """
-__version__ = "9.0.1"
+__version__ = "9.1.0"
 from datetime import datetime
 import logging
 from .api_client import (
     enable_backoff,
     html_diff,
     set_credentials,
     set_proxies,
```

### Comparing `calcbench_api_client-9.0.1/calcbench/api_client.py` & `calcbench_api_client-9.1.0/calcbench/api_client.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/api_query_params.py` & `calcbench_api_client-9.1.0/calcbench/api_query_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,13 +82,14 @@
     endYear: Optional[int] = None
     endPeriod: Optional[PeriodArgument] = None
     allHistory: Optional[bool] = None
     updateDate: Optional[date] = None
     useFiscalPeriod: Optional[bool] = None
     accessionID: Optional[int] = None
     filingID: Optional[int] = None
+    allModifications: Optional[bool] = False
 
 
 class APIQueryParams(BaseModel):
     companiesParameters: Optional[CompaniesParameters]
     periodParameters: Optional[PeriodParameters]
     pageParameters: Optional[object]
```

### Comparing `calcbench_api_client-9.0.1/calcbench/business_combinations.py` & `calcbench_api_client-9.1.0/calcbench/business_combinations.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/companies.py` & `calcbench_api_client-9.1.0/calcbench/companies.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/dimensional.py` & `calcbench_api_client-9.1.0/calcbench/dimensional.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/disclosures.py` & `calcbench_api_client-9.1.0/calcbench/disclosures.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/downloaders.py` & `calcbench_api_client-9.1.0/calcbench/downloaders.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/face_statements.py` & `calcbench_api_client-9.1.0/calcbench/face_statements.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/filing.py` & `calcbench_api_client-9.1.0/calcbench/filing.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/listener.py` & `calcbench_api_client-9.1.0/calcbench/listener.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/metrics.py` & `calcbench_api_client-9.1.0/calcbench/metrics.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/press_release.py` & `calcbench_api_client-9.1.0/calcbench/press_release.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/raw_numeric_XBRL.py` & `calcbench_api_client-9.1.0/calcbench/raw_numeric_XBRL.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/raw_numeric_non_XBRL.py` & `calcbench_api_client-9.1.0/calcbench/raw_numeric_non_XBRL.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench/standardized_numeric.py` & `calcbench_api_client-9.1.0/calcbench/standardized_numeric.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     CompanyIdentifiers,
     DateRange,
     Period,
     PeriodArgument,
     PeriodParameters,
     PeriodType,
 )
+from calcbench.standardized_parameters import StandardizedParameters
 
 if TYPE_CHECKING:
     # https://github.com/microsoft/pyright/issues/1358
     from typing import TypedDict
 else:
     try:
         from typing import TypedDict
@@ -86,14 +87,15 @@
     filing_id: Optional[int] = None,
     all_non_GAAP: bool = False,
     all_metrics: bool = False,
     pit_V2: Optional[bool] = False,
     start_date: Optional[Union[datetime, date]] = None,
     end_date: Optional[Union[datetime, date]] = None,
     XBRL_only: Optional[bool] = False,
+    all_modifications: Optional[bool] = False,
 ) -> Sequence[StandardizedPoint]:
     """Standardized data.
 
     Get normalized data from Calcbench.  Each point is normalized by economic concept and time period.
 
     :param company_identifiers: a sequence of tickers (or CIK codes), eg ['msft', 'goog', 'appl']
     :param metrics: a sequence of metrics, see the full list @ https://www.calcbench.com/home/standardizedmetrics eg. ['revenue', 'accountsreceivable']
@@ -107,14 +109,17 @@
     :param period_type: Either "annual" or "quarterly"
     :param filing_id: Filing id for which to get data.  corresponds to the filing_id in the objects returned by the filings API.
     :param all_non_GAAP: include all non-GAAP metrics from earnings press releases such as EBITDA_NonGAAP.  This is implied when querying by `filing_id`.
     :param all_metrics: All metrics.
     :param start_date: points modified from this date (inclusive).  If no time is specified all points from that date are returned.
     :param end_date: points modified until this date (exclusive).  If not time is specified point modified prior to this date are returned.
     :param XBRL_only: Only get data that appeared in an XBRL document.  If supplied with start_date and end_date it will filter by date_XBRL_confirmed, if a filing_id supplied it will filter by confirming_XBRL_filing_ID.
+
+    :param all_modifications: Include data for which the metadata (XBRL confirmed) was modified in the specified date-range or filing_id.
+
     """
     if [
         bool(company_identifiers),
         bool(entire_universe),
         bool(filing_id),
     ].count(True) != 1:
         raise ValueError(
@@ -221,52 +226,58 @@
         end_period = int(end_period)  # type: ignore
     except (ValueError, TypeError):
         pass
 
     if pit_V2 and not point_in_time:
         raise ValueError("setting pit_V2 without point_in_time does not make sense")
 
+    if all_modifications and not ((start_date or end_date) or filing_id):
+        raise ValueError(
+            "specifying all_modifications without date range or filing_id does not make sense"
+        )
+
     date_range = None
     if start_date or end_date:
         date_range = DateRange(startDate=start_date, endDate=end_date)
 
     period_parameters = PeriodParameters(
         year=start_year,
         period=start_period,
         endYear=end_year,
         endPeriod=end_period,
         allHistory=all_history,
         periodType=period_type,
         useFiscalPeriod=use_fiscal_period,
         filingID=filing_id,
         dateRange=date_range,
+        allModifications=all_modifications,
     )
 
     companies_parameters = CompaniesParameters(
         entireUniverse=entire_universe,
         companyIdentifiers=list(company_identifiers),
     )
 
+    page_parameters = StandardizedParameters(
+        metrics=metrics,
+        includeTrace=include_trace,
+        pointInTime=point_in_time,
+        allFootnotes=all_footnotes,
+        allFace=all_face,
+        allNonGAAP=all_non_GAAP,
+        allMetrics=all_metrics,
+        pointInTimeV2=pit_V2,
+        includePreliminary=True,
+        XBRLOnly=XBRL_only,
+    )
+
     payload = APIQueryParams(
-        **{
-            "pageParameters": {
-                "metrics": metrics,
-                "includeTrace": include_trace,
-                "pointInTime": point_in_time,
-                "allFootnotes": all_footnotes,
-                "allface": all_face,
-                "allNonGAAP": all_non_GAAP,
-                "allMetrics": all_metrics,
-                "pointInTimeV2": pit_V2,
-                "includePreliminary": True,  # only applies to PIT V1,
-                "XBRLOnly": XBRL_only,
-            },
-            "periodParameters": period_parameters,
-            "companiesParameters": companies_parameters,
-        }
+        pageParameters=page_parameters,
+        periodParameters=period_parameters,
+        companiesParameters=companies_parameters,
     )
 
     return _json_POST("mappedData", payload)
 
 
 ORDERED_REGULAR_COLUMNS = [
     "ticker",
@@ -338,14 +349,15 @@
     fiscal_period: PeriodArgument = None,
     start_date: Optional[Union[datetime, date]] = None,
     end_date: Optional[Union[datetime, date]] = None,
     point_in_time: bool = False,
     filing_id: Optional[int] = None,
     pit_V2: Optional[bool] = None,
     XBRL_only: Optional[bool] = False,
+    all_modifications: Optional[bool] = False,
 ):
     """Standardized Numeric Data.
 
 
 
     The data behind the multi-company page, https://www.calcbench.com/multi.
 
@@ -357,14 +369,16 @@
     :param fiscal_period: Fiscal period for which to get data.  If not specified get all history.
     :param start_date:  Restrict to records modified on or after (inclusive) this date/datetime
     :param end_date:  Restric to records modified prior (exclusive) thie date/datetime
     :param point_in_time: Include timestamps when data was published and revision chains.
     :param filing_id: Filing ID for which to get data.  Get all of the data reported in this filing.
     :param pit_V2: Defaults to True, use point in time V2, this only makes sense when point_in_time = True.  This will go away at some point.
     :param XBRL_only: Only get data that appeared in an XBRL document.  If supplied with start_date and end_date it will filter by date_XBRL_confirmed, if a filing_id supplied it will filter by confirming_XBRL_filing_ID.
+    :param all_modifications: Include data for which the metadata (XBRL confirmed) was modified in the specified date-range or filing_id.
+
     :return: Dataframe
 
 
 
     Standardized data with a timestamp when it was published by Calcbench.
 
 
@@ -465,14 +479,15 @@
         all_metrics=not metrics,
         use_fiscal_period=True,
         include_trace=True,
         pit_V2=pit_V2,
         start_date=start_date,
         end_date=end_date,
         XBRL_only=XBRL_only,
+        all_modifications=all_modifications,
     )
 
     data = _build_data_frame(data, point_in_time=point_in_time)
     if data.empty:
         return data
     data["fiscal_period"] = (
         data["fiscal_year"].astype(str) + "-" + data["fiscal_period"].astype(str)
```

### Comparing `calcbench_api_client-9.0.1/calcbench_api_client.egg-info/PKG-INFO` & `calcbench_api_client-9.1.0/calcbench_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcbench-api-client
-Version: 9.0.1
+Version: 9.1.0
 Summary: Client for Calcbench data.
 Home-page: https://github.com/calcbench/python_api_client
 Author: Andrew Kittredge
 Author-email: andrew@calcbench.com
 License: Apache2
 Project-URL: Documentation, http://calcbench.github.io/python_api_client/html/index.html
 Project-URL: Examples, https://github.com/calcbench/notebooks
@@ -45,14 +45,14 @@
         
         @someben https://github.com/calcbench/python_api_client/commit/6c2312525fa365acc91bd8e979037fc2492845f3
         
 Keywords: finance accounting SEC 10-(K|Q)
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: Keyring
-Provides-Extra: pyarrow
 Provides-Extra: Listener
-Provides-Extra: BeautifulSoup
 Provides-Extra: tqdm
+Provides-Extra: BeautifulSoup
 Provides-Extra: Backoff
 Provides-Extra: Pandas
+Provides-Extra: pyarrow
+Provides-Extra: Keyring
```

### Comparing `calcbench_api_client-9.0.1/calcbench_api_client.egg-info/SOURCES.txt` & `calcbench_api_client-9.1.0/calcbench_api_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 calcbench/filing.py
 calcbench/listener.py
 calcbench/metrics.py
 calcbench/press_release.py
 calcbench/raw_numeric_XBRL.py
 calcbench/raw_numeric_non_XBRL.py
 calcbench/standardized_numeric.py
+calcbench/standardized_parameters.py
 calcbench/.vscode/launch.json
 calcbench_api_client.egg-info/PKG-INFO
 calcbench_api_client.egg-info/SOURCES.txt
 calcbench_api_client.egg-info/dependency_links.txt
 calcbench_api_client.egg-info/requires.txt
 calcbench_api_client.egg-info/top_level.txt
 calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
```

### Comparing `calcbench_api_client-9.0.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl` & `calcbench_api_client-9.1.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz` & `calcbench_api_client-9.1.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/conda-recipe/meta.yaml` & `calcbench_api_client-9.1.0/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/Makefile` & `calcbench_api_client-9.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_sources/getting-started.rst.txt` & `calcbench_api_client-9.1.0/docs/html/_sources/getting-started.rst.txt`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/alabaster.css` & `calcbench_api_client-9.1.0/docs/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/basic.css` & `calcbench_api_client-9.1.0/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/doctools.js` & `calcbench_api_client-9.1.0/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/jquery-3.2.1.js` & `calcbench_api_client-9.1.0/docs/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/jquery-3.4.1.js` & `calcbench_api_client-9.1.0/docs/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/jquery-3.5.1.js` & `calcbench_api_client-9.1.0/docs/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/jquery.js` & `calcbench_api_client-9.1.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/language_data.js` & `calcbench_api_client-9.1.0/docs/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/pygments.css` & `calcbench_api_client-9.1.0/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/searchtools.js` & `calcbench_api_client-9.1.0/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/underscore-1.13.1.js` & `calcbench_api_client-9.1.0/docs/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/underscore-1.3.1.js` & `calcbench_api_client-9.1.0/docs/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/_static/underscore.js` & `calcbench_api_client-9.1.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/business-combinations.html` & `calcbench_api_client-9.1.0/docs/html/business-combinations.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/companies.html` & `calcbench_api_client-9.1.0/docs/html/companies.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/dimensional.html` & `calcbench_api_client-9.1.0/docs/html/dimensional.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/disclosures.html` & `calcbench_api_client-9.1.0/docs/html/disclosures.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/downloaders.html` & `calcbench_api_client-9.1.0/docs/html/downloaders.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/face-statements.html` & `calcbench_api_client-9.1.0/docs/html/face-statements.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/filings.html` & `calcbench_api_client-9.1.0/docs/html/filings.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/genindex.html` & `calcbench_api_client-9.1.0/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/getting-started.html` & `calcbench_api_client-9.1.0/docs/html/getting-started.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/index.html` & `calcbench_api_client-9.1.0/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/metrics.html` & `calcbench_api_client-9.1.0/docs/html/metrics.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/numeric-data.html` & `calcbench_api_client-9.1.0/docs/html/numeric-data.html`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 <h1>Standardized Numeric Financials<a class="headerlink" href="#standardized-numeric-financials" title="Permalink to this headline">¶</a></h1>
 <p>Calcbench extracts all of the GAAP numbers in section 8, face statments and footnotes, of the 10-K/Qs.  Face financials from earnings press-releases and 8-Ks are also included.</p>
 <div class="section" id="standardized">
 <h2>Standardized<a class="headerlink" href="#standardized" title="Permalink to this headline">¶</a></h2>
 <p>Calcbench standardizes +1000 metrics to handle differences in filers’s tagging.  The list of stardized points is &#64; <a class="reference external" href="https://www.calcbench.com/home/standardizedmetrics">https://www.calcbench.com/home/standardizedmetrics</a></p>
 <dl class="py function">
 <dt class="sig sig-object py" id="calcbench.standardized">
-<span class="sig-prename descclassname"><span class="pre">calcbench.</span></span><span class="sig-name descname"><span class="pre">standardized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fiscal_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fiscal_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">point_in_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filing_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pit_V2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">XBRL_only</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.standardized" title="Permalink to this definition">¶</a></dt>
+<span class="sig-prename descclassname"><span class="pre">calcbench.</span></span><span class="sig-name descname"><span class="pre">standardized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fiscal_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fiscal_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">point_in_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filing_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pit_V2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">XBRL_only</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_modifications</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.standardized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Standardized Numeric Data.</p>
 <p>The data behind the multi-company page, <a class="reference external" href="https://www.calcbench.com/multi">https://www.calcbench.com/multi</a>.</p>
 <p>Example <a class="reference external" href="https://github.com/calcbench/notebooks/blob/master/python_client_api_demo.ipynb">https://github.com/calcbench/notebooks/blob/master/python_client_api_demo.ipynb</a></p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>company_identifiers</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]) – Tickers/CIK codes. eg. [‘msft’, ‘goog’, ‘appl’, ‘0000066740’].  If not specified get data for all companies.</p></li>
@@ -53,14 +53,15 @@
 <li><p><strong>fiscal_period</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">Period</span></code>, <code class="xref py py-data docutils literal notranslate"><span class="pre">Literal</span></code>[0, 1, 2, 3, 4], <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Fiscal period for which to get data.  If not specified get all history.</p></li>
 <li><p><strong>start_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Restrict to records modified on or after (inclusive) this date/datetime</p></li>
 <li><p><strong>end_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Restric to records modified prior (exclusive) thie date/datetime</p></li>
 <li><p><strong>point_in_time</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>) – Include timestamps when data was published and revision chains.</p></li>
 <li><p><strong>filing_id</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Filing ID for which to get data.  Get all of the data reported in this filing.</p></li>
 <li><p><strong>pit_V2</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Defaults to True, use point in time V2, this only makes sense when point_in_time = True.  This will go away at some point.</p></li>
 <li><p><strong>XBRL_only</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Only get data that appeared in an XBRL document.  If supplied with start_date and end_date it will filter by date_XBRL_confirmed, if a filing_id supplied it will filter by confirming_XBRL_filing_ID.</p></li>
+<li><p><strong>all_modifications</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Include data for which the metadata (XBRL confirmed) was modified in the specified date-range or filing_id.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p>Dataframe</p>
 </dd>
 </dl>
 <p>Standardized data with a timestamp when it was published by Calcbench.</p>
@@ -135,15 +136,15 @@
 <span class="gp">&gt;&gt;&gt; </span><span class="n">return_on_equity</span> <span class="o">=</span> <span class="n">d</span><span class="p">[</span><span class="s1">&#39;NetIncome&#39;</span><span class="p">]</span> <span class="o">/</span> <span class="n">d</span><span class="p">[</span><span class="s1">&#39;StockholdersEquity&#39;</span><span class="p">]</span>
 </pre></div>
 </div>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="calcbench.standardized_raw">
-<span class="sig-prename descclassname"><span class="pre">calcbench.</span></span><span class="sig-name descname"><span class="pre">standardized_raw</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">entire_universe</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">point_in_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">include_trace</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_history</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_fiscal_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_face</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_footnotes</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filing_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_non_GAAP</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pit_V2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">XBRL_only</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.standardized_raw" title="Permalink to this definition">¶</a></dt>
+<span class="sig-prename descclassname"><span class="pre">calcbench.</span></span><span class="sig-name descname"><span class="pre">standardized_raw</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">entire_universe</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">point_in_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">include_trace</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_history</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_fiscal_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_face</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_footnotes</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filing_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_non_GAAP</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pit_V2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">XBRL_only</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_modifications</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.standardized_raw" title="Permalink to this definition">¶</a></dt>
 <dd><p>Standardized data.</p>
 <p>Get normalized data from Calcbench.  Each point is normalized by economic concept and time period.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>company_identifiers</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]) – a sequence of tickers (or CIK codes), eg [‘msft’, ‘goog’, ‘appl’]</p></li>
 <li><p><strong>metrics</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>]) – a sequence of metrics, see the full list &#64; <a class="reference external" href="https://www.calcbench.com/home/standardizedmetrics">https://www.calcbench.com/home/standardizedmetrics</a> eg. [‘revenue’, ‘accountsreceivable’]</p></li>
@@ -157,14 +158,15 @@
 <li><p><strong>period_type</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<a class="reference internal" href="#calcbench.api_query_params.PeriodType" title="calcbench.api_query_params.PeriodType"><code class="xref py py-class docutils literal notranslate"><span class="pre">PeriodType</span></code></a>]) – Either “annual” or “quarterly”</p></li>
 <li><p><strong>filing_id</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Filing id for which to get data.  corresponds to the filing_id in the objects returned by the filings API.</p></li>
 <li><p><strong>all_non_GAAP</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>) – include all non-GAAP metrics from earnings press releases such as EBITDA_NonGAAP.  This is implied when querying by <cite>filing_id</cite>.</p></li>
 <li><p><strong>all_metrics</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>) – All metrics.</p></li>
 <li><p><strong>start_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – points modified from this date (inclusive).  If no time is specified all points from that date are returned.</p></li>
 <li><p><strong>end_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – points modified until this date (exclusive).  If not time is specified point modified prior to this date are returned.</p></li>
 <li><p><strong>XBRL_only</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Only get data that appeared in an XBRL document.  If supplied with start_date and end_date it will filter by date_XBRL_confirmed, if a filing_id supplied it will filter by confirming_XBRL_filing_ID.</p></li>
+<li><p><strong>all_modifications</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Include data for which the metadata (XBRL confirmed) was modified in the specified date-range or filing_id.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Return type</dt>
 <dd class="field-even"><p><code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">StandardizedPoint</span></code>]</p>
 </dd>
 </dl>
 </dd></dl>
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 Ks are also included.
 ***** StandardizedÂ¶ *****
 Calcbench standardizes +1000 metrics to handle differences in filersâs
 tagging. The list of stardized points is @ https://www.calcbench.com/home/
 standardizedmetrics
   calcbench.standardized(company_identifiers=[], metrics=[], fiscal_year=None,
   fiscal_period=None, start_date=None, end_date=None, point_in_time=False,
-  filing_id=None, pit_V2=None, XBRL_only=False)Â¶
+  filing_id=None, pit_V2=None, XBRL_only=False, all_modifications=False)Â¶
       Standardized Numeric Data.
       The data behind the multi-company page, https://www.calcbench.com/multi.
       Example https://github.com/calcbench/notebooks/blob/master/
       python_client_api_demo.ipynb
         Parameters
                 * company_identifiers (Sequence[Union[str, int]]) â Tickers/
                   CIK codes. eg. [âmsftâ, âgoogâ, âapplâ,
@@ -47,14 +47,17 @@
                 * pit_V2 (Optional[bool]) â Defaults to True, use point in
                   time V2, this only makes sense when point_in_time = True.
                   This will go away at some point.
                 * XBRL_only (Optional[bool]) â Only get data that appeared in
                   an XBRL document. If supplied with start_date and end_date it
                   will filter by date_XBRL_confirmed, if a filing_id supplied
                   it will filter by confirming_XBRL_filing_ID.
+                * all_modifications (Optional[bool]) â Include data for which
+                  the metadata (XBRL confirmed) was modified in the specified
+                  date-range or filing_id.
         Returns
             Dataframe
       Standardized data with a timestamp when it was published by Calcbench.
       A record is returned for each filing in which a metric value changed (was
       revised).
       If the company files an 8-K with revenue = $100 then a week later files a
       10-K with revenue = $100 one record will be returned for that period. It
@@ -154,15 +157,15 @@
       >>> return_on_equity = d['NetIncome'] / d['StockholdersEquity']
   calcbench.standardized_raw(company_identifiers=[], metrics=[],
   start_year=None, start_period=None, end_year=None, end_period=None,
   entire_universe=False, point_in_time=False, include_trace=False,
   all_history=False, year=None, period=None, period_type=None,
   use_fiscal_period=False, all_face=False, all_footnotes=False, filing_id=None,
   all_non_GAAP=False, all_metrics=False, pit_V2=False, start_date=None,
-  end_date=None, XBRL_only=False)Â¶
+  end_date=None, XBRL_only=False, all_modifications=False)Â¶
       Standardized data.
       Get normalized data from Calcbench. Each point is normalized by economic
       concept and time period.
         Parameters
                 * company_identifiers (Sequence[Union[str, int]]) â a
                   sequence of tickers (or CIK codes), eg [âmsftâ,
                   âgoogâ, âapplâ]
@@ -200,14 +203,17 @@
                 * end_date (Union[datetime, date, None]) â points modified
                   until this date (exclusive). If not time is specified point
                   modified prior to this date are returned.
                 * XBRL_only (Optional[bool]) â Only get data that appeared in
                   an XBRL document. If supplied with start_date and end_date it
                   will filter by date_XBRL_confirmed, if a filing_id supplied
                   it will filter by confirming_XBRL_filing_ID.
+                * all_modifications (Optional[bool]) â Include data for which
+                  the metadata (XBRL confirmed) was modified in the specified
+                  date-range or filing_id.
         Return type
             Sequence[StandardizedPoint]
   classcalcbench.api_query_params.Period(value)
       An enumeration.
         Annual= 0
         Failure= -1
             Should be few and far between, indicates something went wrong
```

### Comparing `calcbench_api_client-9.0.1/docs/html/press-release.html` & `calcbench_api_client-9.1.0/docs/html/press-release.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/push-notification.html` & `calcbench_api_client-9.1.0/docs/html/push-notification.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/py-modindex.html` & `calcbench_api_client-9.1.0/docs/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/raw-numeric-XBRL.html` & `calcbench_api_client-9.1.0/docs/html/raw-numeric-XBRL.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/raw-numeric-non-XBRL.html` & `calcbench_api_client-9.1.0/docs/html/raw-numeric-non-XBRL.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/search.html` & `calcbench_api_client-9.1.0/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/html/searchindex.js` & `calcbench_api_client-9.1.0/docs/html/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -865,14 +865,15 @@
         aka: 5,
         all: [1, 2, 4, 5, 8, 11],
         all_docu: 2,
         all_fac: [3, 8, 10],
         all_footnot: [3, 8, 10],
         all_histori: [1, 2, 3, 4, 8],
         all_metr: 8,
+        all_modif: 8,
         all_non_gaap: 8,
         all_period: 4,
         all_text_block: 2,
         alloc: 7,
         also: 8,
         altern: 6,
         alwai: 10,
@@ -1526,14 +1527,15 @@
         managementsdiscussionandanalysi: 2,
         mani: 6,
         master: [6, 8, 10],
         md: 5,
         measur: 11,
         merger: 0,
         messag: 10,
+        metadata: 8,
         metric: [0, 1, 7, 8, 11],
         metric_id: 11,
         mfp: 5,
         mode: 3,
         modifi: 8,
         msd: 5,
         msdw: 5,
@@ -1695,15 +1697,15 @@
         quantit: [],
         quarter: 8,
         quarterli: [1, 2, 4, 8],
         queri: [2, 8],
         queryparsersyntax: 2,
         queue: 10,
         random: 3,
-        rang: 11,
+        rang: [8, 11],
         range_high: 11,
         range_high_valu: 9,
         range_low: 11,
         rare: 11,
         rate: [],
         rather: 1,
         raw: 7,
```

### Comparing `calcbench_api_client-9.0.1/docs/make.bat` & `calcbench_api_client-9.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/source/conf.py` & `calcbench_api_client-9.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/source/getting-started.rst` & `calcbench_api_client-9.1.0/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/source/index.rst` & `calcbench_api_client-9.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/source/numeric-data.rst` & `calcbench_api_client-9.1.0/docs/source/numeric-data.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/docs/source/push-notification.rst` & `calcbench_api_client-9.1.0/docs/source/push-notification.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.0.1/setup.py` & `calcbench_api_client-9.1.0/setup.py`

 * *Files identical despite different names*

