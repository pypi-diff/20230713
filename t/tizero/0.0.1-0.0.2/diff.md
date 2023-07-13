# Comparing `tmp/tizero-0.0.1.tar.gz` & `tmp/tizero-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tizero-0.0.1.tar", last modified: Mon Jun 26 11:20:39 2023, max compression
+gzip compressed data, was "tizero-0.0.2.tar", last modified: Thu Jul 13 03:44:38 2023, max compression
```

## Comparing `tizero-0.0.1.tar` & `tizero-0.0.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-26 11:20:39.226226 tizero-0.0.1/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-26 08:27:43.000000 tizero-0.0.1/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     3612 2023-06-26 11:20:39.226085 tizero-0.0.1/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     2521 2023-06-26 11:15:23.000000 tizero-0.0.1/README.md
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-06-26 11:20:39.226267 tizero-0.0.1/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2818 2023-06-26 11:19:04.000000 tizero-0.0.1/setup.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-26 11:20:39.216870 tizero-0.0.1/tizero/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1098 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-26 11:20:39.218104 tizero-0.0.1/tizero/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 tizero-0.0.1/tizero/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3014 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/cli/cli.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1354 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/cli/dump2video.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-26 11:20:39.218260 tizero-0.0.1/tizero/football_env/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 09:40:44.000000 tizero-0.0.1/tizero/football_env/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-26 11:20:39.220159 tizero-0.0.1/tizero/football_env/core/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 09:40:44.000000 tizero-0.0.1/tizero/football_env/core/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4883 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/core/config.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9417 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/core/football_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19248 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/core/football_env_core.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4766 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/core/scenario_builder.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-26 11:20:39.225149 tizero-0.0.1/tizero/football_env/scenarios/
--rw-r--r--   0 4paradigm   (501) staff       (20)     2468 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_determ_False.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2468 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_determ_True.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2810 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5989 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_diff.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2769 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_eval.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2808 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_new.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2739 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_reverse.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2764 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_v2.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2521 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_kaggle.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2381 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_stochastic.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1225 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1386 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_3_vs_1_with_keeper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2229 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_corner.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2296 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_counterattack_easy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2297 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_counterattack_hard.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1232 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_empty_goal.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_empty_goal_close.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1337 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_pass_and_shoot_with_keeper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1337 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_run_pass_and_shoot_with_keeper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1489 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_run_to_score.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1490 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/academy_run_to_score_with_keeper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2969 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/debug_football.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8119 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/football_scenario.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2649 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/football_env/scenarios/position_test.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-26 11:20:39.225778 tizero-0.0.1/tizero/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 tizero-0.0.1/tizero/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6779 2023-06-26 11:19:04.000000 tizero-0.0.1/tizero/utils/script_helpers.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1339 2023-06-26 11:18:17.000000 tizero-0.0.1/tizero/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-26 11:20:39.217591 tizero-0.0.1/tizero.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3612 2023-06-26 11:20:39.000000 tizero-0.0.1/tizero.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     1910 2023-06-26 11:20:39.000000 tizero-0.0.1/tizero.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-06-26 11:20:39.000000 tizero-0.0.1/tizero.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-06-26 11:20:39.000000 tizero-0.0.1/tizero.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      143 2023-06-26 11:20:39.000000 tizero-0.0.1/tizero.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        7 2023-06-26 11:20:39.000000 tizero-0.0.1/tizero.egg-info/top_level.txt
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-13 03:44:38.217216 tizero-0.0.2/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-26 08:27:43.000000 tizero-0.0.2/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3965 2023-07-13 03:44:38.217058 tizero-0.0.2/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2874 2023-07-13 03:30:57.000000 tizero-0.0.2/README.md
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-13 03:44:38.217260 tizero-0.0.2/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2818 2023-06-26 11:19:04.000000 tizero-0.0.2/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-13 03:44:38.207924 tizero-0.0.2/tizero/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1098 2023-07-13 03:44:18.000000 tizero-0.0.2/tizero/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-13 03:44:38.209456 tizero-0.0.2/tizero/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 tizero-0.0.2/tizero/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2624 2023-07-13 03:25:49.000000 tizero-0.0.2/tizero/cli/cli.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1354 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/cli/dump2video.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-13 03:44:38.209704 tizero-0.0.2/tizero/football_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 09:40:44.000000 tizero-0.0.2/tizero/football_env/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-13 03:44:38.211137 tizero-0.0.2/tizero/football_env/core/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 09:40:44.000000 tizero-0.0.2/tizero/football_env/core/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4883 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/core/config.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9417 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/core/football_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    19248 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/core/football_env_core.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4766 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/core/scenario_builder.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-13 03:44:38.216118 tizero-0.0.2/tizero/football_env/scenarios/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2468 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_determ_False.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2468 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_determ_True.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2810 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5989 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_diff.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2769 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_eval.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2808 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_new.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2739 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_reverse.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2764 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_v2.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2521 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_kaggle.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2381 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_stochastic.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1225 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1386 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_3_vs_1_with_keeper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2229 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_corner.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2296 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_counterattack_easy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2297 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_counterattack_hard.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1232 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_empty_goal.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_empty_goal_close.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1337 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_pass_and_shoot_with_keeper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1337 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_run_pass_and_shoot_with_keeper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1489 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_run_to_score.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1490 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/academy_run_to_score_with_keeper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2969 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/debug_football.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8119 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/football_scenario.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2649 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/football_env/scenarios/position_test.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-13 03:44:38.216704 tizero-0.0.2/tizero/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 tizero-0.0.2/tizero/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6779 2023-06-26 11:19:04.000000 tizero-0.0.2/tizero/utils/script_helpers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1339 2023-06-26 11:18:17.000000 tizero-0.0.2/tizero/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-13 03:44:38.208832 tizero-0.0.2/tizero.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3965 2023-07-13 03:44:38.000000 tizero-0.0.2/tizero.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1910 2023-07-13 03:44:38.000000 tizero-0.0.2/tizero.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-13 03:44:38.000000 tizero-0.0.2/tizero.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-13 03:44:38.000000 tizero-0.0.2/tizero.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      143 2023-07-13 03:44:38.000000 tizero-0.0.2/tizero.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        7 2023-07-13 03:44:38.000000 tizero-0.0.2/tizero.egg-info/top_level.txt
```

### Comparing `tizero-0.0.1/LICENSE` & `tizero-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/PKG-INFO` & `tizero-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tizero
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolkit and agents for Google Research Football
 Home-page: https://github.com/OpenRL-Lab/TiZero
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/TiZero
 Project-URL: Documentation, https://tizero.readthedocs.io/
 Keywords: reinforcement-learning multi-agent google research football
@@ -29,15 +29,16 @@
 </div>
 
 <div align="center">
 <img height="300px" height="auto" src="./docs/figures/screen_800.png">
 </div>
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
+[![PyPI](https://img.shields.io/pypi/v/tizero)](https://pypi.org/project/tizero/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tizero)
 [![Documentation Status](https://readthedocs.org/projects/tizero/badge/?version=latest)](https://tizero.readthedocs.io/en/latest/?badge=latest)
 
 
 ### Introduction
 
 Reinforcement learning agent for Google Research Football.
 
@@ -54,28 +55,30 @@
 - `pip install gfootball`
 - `pip install tizero` (or clone this repo and `pip install -e .`).
 - test the installation by `python3 -m gfootball.play_game --action_set=full`.
 
 ### Convert dump file to video
 
 After the installation, you can use tizero to convert a dump file to a video file.
+The usage is `tizero dump2video <dump_file> <output_dir> --episode_length <the length> --render_type <2d/3d>`.
+
 You can download an example dump file from [here](http://jidiai.cn/daily_6484285/daily_6484285.dump). 
-And then execute `tizero --tool dump2video --input daily_6484285.dump --output ./` in your terminal.
+And then execute `tizero dump2video daily_6484285.dump ./` in your terminal. By default, the episode length is 3000 and the render type is 2d.
 Wait a minute, you will get a video file named `daily_6484285.avi` in your current directory.
 
 ### Submit TiZero to JIDI(及第评测平台)
 
 <div align="center">
 <img height="400px" height="auto" src="./docs/figures/jidi.png">
 </div>
 
 
 JIDI is a public evaluation platform for RL agents. You can submit your agent of GRF at: [http://www.jidiai.cn/env_detail?envid=34](http://www.jidiai.cn/env_detail?envid=34).
 
-We provide two agents under `./submission/` directory:
+We provide several agents under `./submission/` directory,  which can be submitted to JIDI directly:
 
 - `./submission/tizero`: the final model of TiZero for JIDI submission, which ranked 1st on October 28th, 2022.
 - `./submission/random_agent`: the random agent for JIDI submission.
 
 
 ### Cite
```

### Comparing `tizero-0.0.1/README.md` & `tizero-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 </div>
 
 <div align="center">
 <img height="300px" height="auto" src="./docs/figures/screen_800.png">
 </div>
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
+[![PyPI](https://img.shields.io/pypi/v/tizero)](https://pypi.org/project/tizero/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tizero)
 [![Documentation Status](https://readthedocs.org/projects/tizero/badge/?version=latest)](https://tizero.readthedocs.io/en/latest/?badge=latest)
 
 
 ### Introduction
 
 Reinforcement learning agent for Google Research Football.
 
@@ -28,28 +29,30 @@
 - `pip install gfootball`
 - `pip install tizero` (or clone this repo and `pip install -e .`).
 - test the installation by `python3 -m gfootball.play_game --action_set=full`.
 
 ### Convert dump file to video
 
 After the installation, you can use tizero to convert a dump file to a video file.
+The usage is `tizero dump2video <dump_file> <output_dir> --episode_length <the length> --render_type <2d/3d>`.
+
 You can download an example dump file from [here](http://jidiai.cn/daily_6484285/daily_6484285.dump). 
-And then execute `tizero --tool dump2video --input daily_6484285.dump --output ./` in your terminal.
+And then execute `tizero dump2video daily_6484285.dump ./` in your terminal. By default, the episode length is 3000 and the render type is 2d.
 Wait a minute, you will get a video file named `daily_6484285.avi` in your current directory.
 
 ### Submit TiZero to JIDI(及第评测平台)
 
 <div align="center">
 <img height="400px" height="auto" src="./docs/figures/jidi.png">
 </div>
 
 
 JIDI is a public evaluation platform for RL agents. You can submit your agent of GRF at: [http://www.jidiai.cn/env_detail?envid=34](http://www.jidiai.cn/env_detail?envid=34).
 
-We provide two agents under `./submission/` directory:
+We provide several agents under `./submission/` directory,  which can be submitted to JIDI directly:
 
 - `./submission/tizero`: the final model of TiZero for JIDI submission, which ranked 1st on October 28th, 2022.
 - `./submission/random_agent`: the random agent for JIDI submission.
 
 
 ### Cite
```

### Comparing `tizero-0.0.1/setup.py` & `tizero-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/__init__.py` & `tizero-0.0.2/tizero/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "tizero"
-__VERSION__ = "v0.0.1"
+__VERSION__ = "v0.0.2"
 __DESCRIPTION__ = "Toolkit and Agents for Google Research Football"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
 
 python_version_list = list(map(int, platform.python_version_tuple()))
 assert python_version_list >= [
     3,
     8,
     0,
 ], (
-    "OpenRL requires Python 3.8 or newer, but your Python is"
+    "tizero requires Python 3.8 or newer, but your Python is"
     f" {platform.python_version()}"
 )
```

### Comparing `tizero-0.0.1/tizero/cli/__init__.py` & `tizero-0.0.2/tizero/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/cli/cli.py` & `tizero-0.0.2/tizero/cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         click.secho(f"- {key}: {red(value)}")
     ctx.exit()
 
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
-@click.command(context_settings=CONTEXT_SETTINGS)
+@click.group(invoke_without_command=True)
 @click.option(
     "--version",
     is_flag=True,
     callback=print_version,
     expose_value=False,
     is_eager=True,
     help="Show package's version information.",
@@ -69,36 +69,25 @@
     "--system_info",
     is_flag=True,
     callback=print_system_info,
     expose_value=False,
     is_eager=True,
     help="Show system information.",
 )
-@click.option(
-    "--tool",
-    prompt="Choose a tool to use",
-    type=click.Choice(
-        [
-            "dump2video",
-        ]
-    ),
-    help="tool name",
-)
-@click.option(
-    "--input",
-    prompt="Please enter input file path or directory",
-    type=str,
-    help="input file path or directory",
-)
-@click.option(
-    "--output",
-    prompt="Please enter output file path or directory",
-    type=str,
-    help="output file path or directory",
-)
+@click.pass_context
+def run(ctx):
+    if ctx.invoked_subcommand is None:
+        pass
+    else:
+        pass
+
+
+@run.command()
+@click.argument("input")
+@click.argument("output")
 @click.option(
     "--episode_length",
     type=int,
     default=None,
     help="episode length",
 )
 @click.option(
@@ -108,19 +97,16 @@
             "2d",
             "3d",
         ]
     ),
     default="2d",
     help="render type",
 )
-def run(tool: str, input: str, output: str, episode_length: int, render_type: str):
-    if tool == "dump2video":
-        from tizero.cli.dump2video import dump2video
-
-        dump2video(
-            input=input,
-            output=output,
-            episode_length=episode_length,
-            render_type=render_type,
-        )
-    else:
-        raise NotImplementedError
+def dump2video(input: str, output: str, episode_length: int, render_type: str):
+    from tizero.cli.dump2video import dump2video
+
+    dump2video(
+        input=input,
+        output=output,
+        episode_length=episode_length,
+        render_type=render_type,
+    )
```

### Comparing `tizero-0.0.1/tizero/cli/dump2video.py` & `tizero-0.0.2/tizero/cli/dump2video.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/__init__.py` & `tizero-0.0.2/tizero/football_env/__init__.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/core/__init__.py` & `tizero-0.0.2/tizero/football_env/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/core/config.py` & `tizero-0.0.2/tizero/football_env/core/config.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/core/football_env.py` & `tizero-0.0.2/tizero/football_env/core/football_env.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/core/football_env_core.py` & `tizero-0.0.2/tizero/football_env/core/football_env_core.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/core/scenario_builder.py` & `tizero-0.0.2/tizero/football_env/core/scenario_builder.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_determ_False.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_determ_False.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_determ_True.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_determ_True.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_diff.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_diff.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_eval.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_eval.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_new.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_new.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_reverse.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_reverse.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_jidi_v2.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_jidi_v2.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_kaggle.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_kaggle.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/11_vs_11_stochastic.py` & `tizero-0.0.2/tizero/football_env/scenarios/11_vs_11_stochastic.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/__init__.py` & `tizero-0.0.2/tizero/football_env/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_3_vs_1_with_keeper.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_3_vs_1_with_keeper.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_corner.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_corner.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_counterattack_easy.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_counterattack_easy.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_counterattack_hard.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_counterattack_hard.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_empty_goal.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_empty_goal.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_empty_goal_close.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_empty_goal_close.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_pass_and_shoot_with_keeper.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_pass_and_shoot_with_keeper.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_run_pass_and_shoot_with_keeper.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_run_pass_and_shoot_with_keeper.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_run_to_score.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_run_to_score.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/academy_run_to_score_with_keeper.py` & `tizero-0.0.2/tizero/football_env/scenarios/academy_run_to_score_with_keeper.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/debug_football.py` & `tizero-0.0.2/tizero/football_env/scenarios/debug_football.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/football_scenario.py` & `tizero-0.0.2/tizero/football_env/scenarios/football_scenario.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/football_env/scenarios/position_test.py` & `tizero-0.0.2/tizero/football_env/scenarios/position_test.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/utils/__init__.py` & `tizero-0.0.2/tizero/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/utils/script_helpers.py` & `tizero-0.0.2/tizero/utils/script_helpers.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero/utils/util.py` & `tizero-0.0.2/tizero/utils/util.py`

 * *Files identical despite different names*

### Comparing `tizero-0.0.1/tizero.egg-info/PKG-INFO` & `tizero-0.0.2/tizero.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tizero
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolkit and agents for Google Research Football
 Home-page: https://github.com/OpenRL-Lab/TiZero
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/TiZero
 Project-URL: Documentation, https://tizero.readthedocs.io/
 Keywords: reinforcement-learning multi-agent google research football
@@ -29,15 +29,16 @@
 </div>
 
 <div align="center">
 <img height="300px" height="auto" src="./docs/figures/screen_800.png">
 </div>
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
+[![PyPI](https://img.shields.io/pypi/v/tizero)](https://pypi.org/project/tizero/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tizero)
 [![Documentation Status](https://readthedocs.org/projects/tizero/badge/?version=latest)](https://tizero.readthedocs.io/en/latest/?badge=latest)
 
 
 ### Introduction
 
 Reinforcement learning agent for Google Research Football.
 
@@ -54,28 +55,30 @@
 - `pip install gfootball`
 - `pip install tizero` (or clone this repo and `pip install -e .`).
 - test the installation by `python3 -m gfootball.play_game --action_set=full`.
 
 ### Convert dump file to video
 
 After the installation, you can use tizero to convert a dump file to a video file.
+The usage is `tizero dump2video <dump_file> <output_dir> --episode_length <the length> --render_type <2d/3d>`.
+
 You can download an example dump file from [here](http://jidiai.cn/daily_6484285/daily_6484285.dump). 
-And then execute `tizero --tool dump2video --input daily_6484285.dump --output ./` in your terminal.
+And then execute `tizero dump2video daily_6484285.dump ./` in your terminal. By default, the episode length is 3000 and the render type is 2d.
 Wait a minute, you will get a video file named `daily_6484285.avi` in your current directory.
 
 ### Submit TiZero to JIDI(及第评测平台)
 
 <div align="center">
 <img height="400px" height="auto" src="./docs/figures/jidi.png">
 </div>
 
 
 JIDI is a public evaluation platform for RL agents. You can submit your agent of GRF at: [http://www.jidiai.cn/env_detail?envid=34](http://www.jidiai.cn/env_detail?envid=34).
 
-We provide two agents under `./submission/` directory:
+We provide several agents under `./submission/` directory,  which can be submitted to JIDI directly:
 
 - `./submission/tizero`: the final model of TiZero for JIDI submission, which ranked 1st on October 28th, 2022.
 - `./submission/random_agent`: the random agent for JIDI submission.
 
 
 ### Cite
```

### Comparing `tizero-0.0.1/tizero.egg-info/SOURCES.txt` & `tizero-0.0.2/tizero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

