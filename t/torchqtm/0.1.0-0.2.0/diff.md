# Comparing `tmp/torchqtm-0.1.0.tar.gz` & `tmp/torchqtm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchqtm-0.1.0.tar", last modified: Sat Jun 10 15:56:28 2023, max compression
+gzip compressed data, was "torchqtm-0.2.0.tar", last modified: Thu Jul 13 09:16:54 2023, max compression
```

## Comparing `torchqtm-0.1.0.tar` & `torchqtm-0.2.0.tar`

### file list

```diff
@@ -1,94 +1,161 @@
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.422512 torchqtm-0.1.0/
--rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-05-21 08:16:14.000000 torchqtm-0.1.0/LICENSE
--rw-r--r--   0 nymath     (501) staff       (20)     2886 2023-06-10 15:56:28.422322 torchqtm-0.1.0/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     2431 2023-06-10 15:47:20.000000 torchqtm-0.1.0/README.md
--rw-r--r--   0 nymath     (501) staff       (20)       38 2023-06-10 15:56:28.422610 torchqtm-0.1.0/setup.cfg
--rw-r--r--   0 nymath     (501) staff       (20)     1312 2023-06-10 15:55:41.000000 torchqtm-0.1.0/setup.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.405187 torchqtm-0.1.0/test/
--rw-r--r--   0 nymath     (501) staff       (20)      505 2023-06-10 15:47:20.000000 torchqtm-0.1.0/test/testFunctional.py
--rw-r--r--   0 nymath     (501) staff       (20)     1216 2023-06-10 15:47:20.000000 torchqtm-0.1.0/test/testRolling.py
--rw-r--r--   0 nymath     (501) staff       (20)        2 2023-05-20 16:39:21.000000 torchqtm-0.1.0/test/test_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-08 06:45:36.000000 torchqtm-0.1.0/test/testfunc_.py
--rw-r--r--   0 nymath     (501) staff       (20)     1994 2023-06-08 06:45:36.000000 torchqtm-0.1.0/test/testgplearn.py
--rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-08 06:45:36.000000 torchqtm-0.1.0/test/testop.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.405685 torchqtm-0.1.0/torchqtm/
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.407438 torchqtm-0.1.0/torchqtm/_C/
--rw-r--r--   0 nymath     (501) staff       (20)   109379 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/_C/__init__.cpp
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/_C/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)   289927 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/_C/_functional.cpp
--rw-r--r--   0 nymath     (501) staff       (20)  1199949 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm/_C/_rolling.cpp
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.408267 torchqtm-0.1.0/torchqtm/_libs/
--rw-r--r--   0 nymath     (501) staff       (20)      323 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/_libs/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.410413 torchqtm-0.1.0/torchqtm/_libs/tslibs/
--rw-r--r--   0 nymath     (501) staff       (20)     1534 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/_libs/tslibs/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.410678 torchqtm-0.1.0/torchqtm/_libs/window/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/_libs/window/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.411714 torchqtm-0.1.0/torchqtm/alphas/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    21667 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/alpha101.py
--rw-r--r--   0 nymath     (501) staff       (20)     2093 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/alphas.py
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/chatgpt.py
--rw-r--r--   0 nymath     (501) staff       (20)      699 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/alphas/ml.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.411924 torchqtm-0.1.0/torchqtm/autoalpha/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.412028 torchqtm-0.1.0/torchqtm/autoalpha/boost/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/boost/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.412128 torchqtm-0.1.0/torchqtm/autoalpha/cnn/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/cnn/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.413639 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/
--rw-r--r--   0 nymath     (501) staff       (20)      218 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/_program.py
--rw-r--r--   0 nymath     (501) staff       (20)     6595 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/fitness.py
--rw-r--r--   0 nymath     (501) staff       (20)     7239 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/functions.py
--rw-r--r--   0 nymath     (501) staff       (20)    66949 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/genetic.py
--rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/autoalpha/gplearn/utils.py
--rw-r--r--   0 nymath     (501) staff       (20)     6459 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/base.py
--rw-r--r--   0 nymath     (501) staff       (20)      119 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/config.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.413833 torchqtm-0.1.0/torchqtm/core/
--rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-08 10:01:51.000000 torchqtm-0.1.0/torchqtm/core/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.414272 torchqtm-0.1.0/torchqtm/core/window/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 10:01:51.000000 torchqtm-0.1.0/torchqtm/core/window/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     6829 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/core/window/rolling.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.415626 torchqtm-0.1.0/torchqtm/edbt/
--rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     2143 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/account.py
--rw-r--r--   0 nymath     (501) staff       (20)     2231 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/backtest.py
--rw-r--r--   0 nymath     (501) staff       (20)     7015 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/datahandler.py
--rw-r--r--   0 nymath     (501) staff       (20)      144 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/setup.py
--rw-r--r--   0 nymath     (501) staff       (20)     3706 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/test.py
--rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/edbt/testsearch.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.416529 torchqtm-0.1.0/torchqtm/op/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/op/CrossSectionalOperators.py
--rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/op/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    11492 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/op/_numba.py
--rw-r--r--   0 nymath     (501) staff       (20)       68 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/op/algos.py
--rw-r--r--   0 nymath     (501) staff       (20)    20222 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/op/functional.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.417792 torchqtm-0.1.0/torchqtm/option/
--rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/Option.py
--rw-r--r--   0 nymath     (501) staff       (20)       97 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.418593 torchqtm-0.1.0/torchqtm/option/data/
--rw-r--r--   0 nymath     (501) staff       (20)       40 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/data/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      333 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/data/load_data.py
--rw-r--r--   0 nymath     (501) staff       (20)     2698 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/functional.py
--rw-r--r--   0 nymath     (501) staff       (20)      586 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/option/main.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.419167 torchqtm-0.1.0/torchqtm/uniquant/
--rw-r--r--   0 nymath     (501) staff       (20)       63 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/uniquant/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.421404 torchqtm-0.1.0/torchqtm/utils/
--rw-r--r--   0 nymath     (501) staff       (20)      626 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/utils/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/utils/benchmark.py
--rw-r--r--   0 nymath     (501) staff       (20)     2571 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/utils/rebalance.py
--rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/utils/stats.py
--rw-r--r--   0 nymath     (501) staff       (20)     1452 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/utils/universe.py
--rw-r--r--   0 nymath     (501) staff       (20)     1835 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/utils/visualization.py
--rw-r--r--   0 nymath     (501) staff       (20)     2675 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/utils/warnings.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.422007 torchqtm-0.1.0/torchqtm/vbt/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/vbt/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     5615 2023-06-10 15:47:20.000000 torchqtm-0.1.0/torchqtm/vbt/backtest.py
--rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-08 06:45:36.000000 torchqtm-0.1.0/torchqtm/vbt/dataset.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-10 15:56:28.406458 torchqtm-0.1.0/torchqtm.egg-info/
--rw-r--r--   0 nymath     (501) staff       (20)     2886 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     1895 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/SOURCES.txt
--rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/dependency_links.txt
--rw-r--r--   0 nymath     (501) staff       (20)       44 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/requires.txt
--rw-r--r--   0 nymath     (501) staff       (20)        9 2023-06-10 15:56:28.000000 torchqtm-0.1.0/torchqtm.egg-info/top_level.txt
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.398827 torchqtm-0.2.0/
+-rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-06-13 15:30:45.000000 torchqtm-0.2.0/LICENSE
+-rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-13 09:16:54.398575 torchqtm-0.2.0/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     3547 2023-07-13 06:59:46.000000 torchqtm-0.2.0/README.md
+-rw-r--r--   0 nymath     (501) staff       (20)       38 2023-07-13 09:16:54.398922 torchqtm-0.2.0/setup.cfg
+-rw-r--r--   0 nymath     (501) staff       (20)     1418 2023-07-13 09:16:36.000000 torchqtm-0.2.0/setup.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.358359 torchqtm-0.2.0/test/
+-rw-r--r--   0 nymath     (501) staff       (20)      505 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/testFunctional.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1216 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/testRolling.py
+-rw-r--r--   0 nymath     (501) staff       (20)        2 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/test_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/testfunc_.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1865 2023-06-28 01:46:48.000000 torchqtm-0.2.0/test/testgplearn.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/testop.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.359850 torchqtm-0.2.0/torchqtm/
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.362901 torchqtm-0.2.0/torchqtm/_C/
+-rw-r--r--   0 nymath     (501) staff       (20)   108947 2023-07-13 02:19:26.000000 torchqtm-0.2.0/torchqtm/_C/__init__.c
+-rw-r--r--   0 nymath     (501) staff       (20)   109379 2023-06-27 12:01:02.000000 torchqtm-0.2.0/torchqtm/_C/__init__.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/_C/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)   289603 2023-07-13 02:24:46.000000 torchqtm-0.2.0/torchqtm/_C/_functional.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)  1225596 2023-07-13 02:24:47.000000 torchqtm-0.2.0/torchqtm/_C/_rolling.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.365194 torchqtm-0.2.0/torchqtm/_libs/
+-rw-r--r--   0 nymath     (501) staff       (20)      323 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/_libs/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.365552 torchqtm-0.2.0/torchqtm/_libs/tslibs/
+-rw-r--r--   0 nymath     (501) staff       (20)     1534 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/_libs/tslibs/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.365852 torchqtm-0.2.0/torchqtm/_libs/window/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/_libs/window/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.368494 torchqtm-0.2.0/torchqtm/alphas/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    50043 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/alpha101.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2093 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/alphas.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.368804 torchqtm-0.2.0/torchqtm/alphas/autoalpha/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.368910 torchqtm-0.2.0/torchqtm/alphas/autoalpha/boost/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/boost/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.369014 torchqtm-0.2.0/torchqtm/alphas/autoalpha/cnn/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/cnn/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.371173 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/
+-rw-r--r--   0 nymath     (501) staff       (20)      218 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/_program.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6587 2023-06-26 08:02:51.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/fitness.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7231 2023-06-26 08:02:51.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/functions.py
+-rw-r--r--   0 nymath     (501) staff       (20)    66960 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/genetic.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1716 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/chatgpt.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1317 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/introduction.py
+-rw-r--r--   0 nymath     (501) staff       (20)      700 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/ml.py
+-rw-r--r--   0 nymath     (501) staff       (20)    28048 2023-06-19 13:01:39.000000 torchqtm-0.2.0/torchqtm/alphas/statistical.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9453 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/technical.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.371553 torchqtm-0.2.0/torchqtm/assets/
+-rw-r--r--   0 nymath     (501) staff       (20)       57 2023-07-04 07:03:05.000000 torchqtm-0.2.0/torchqtm/assets/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1430 2023-07-07 10:17:12.000000 torchqtm-0.2.0/torchqtm/assets/_assets.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6981 2023-06-19 12:57:55.000000 torchqtm-0.2.0/torchqtm/base.py
+-rw-r--r--   0 nymath     (501) staff       (20)      119 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/config.py
+-rw-r--r--   0 nymath     (501) staff       (20)      337 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/configurator.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6957 2023-07-11 03:47:35.000000 torchqtm-0.2.0/torchqtm/constants.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.371783 torchqtm-0.2.0/torchqtm/core/
+-rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/core/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.372036 torchqtm-0.2.0/torchqtm/core/window/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/core/window/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6854 2023-07-11 09:25:38.000000 torchqtm-0.2.0/torchqtm/core/window/rolling.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.372842 torchqtm-0.2.0/torchqtm/data/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:11:51.000000 torchqtm-0.2.0/torchqtm/data/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1477 2023-07-06 05:29:21.000000 torchqtm-0.2.0/torchqtm/data/bardata.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.373151 torchqtm-0.2.0/torchqtm/data/bundle/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-04 03:24:44.000000 torchqtm-0.2.0/torchqtm/data/bundle/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)       68 2023-07-04 03:26:41.000000 torchqtm-0.2.0/torchqtm/data/bundle/rqalpha.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7146 2023-07-13 06:47:38.000000 torchqtm-0.2.0/torchqtm/data/data_portal.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.374279 torchqtm-0.2.0/torchqtm/data/rq_data_source/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 10:32:43.000000 torchqtm-0.2.0/torchqtm/data/rq_data_source/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3214 2023-07-04 09:31:26.000000 torchqtm-0.2.0/torchqtm/data/rq_data_source/adjust.py
+-rw-r--r--   0 nymath     (501) staff       (20)    17792 2023-07-13 06:44:28.000000 torchqtm-0.2.0/torchqtm/data/rq_data_source/data_source.py
+-rw-r--r--   0 nymath     (501) staff       (20)    13906 2023-07-04 09:22:00.000000 torchqtm-0.2.0/torchqtm/data/rq_data_source/readers.py
+-rw-r--r--   0 nymath     (501) staff       (20)      885 2023-07-02 15:35:35.000000 torchqtm-0.2.0/torchqtm/data/sample.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.374540 torchqtm-0.2.0/torchqtm/derivatives/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:10:17.000000 torchqtm-0.2.0/torchqtm/derivatives/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.375073 torchqtm-0.2.0/torchqtm/derivatives/option/
+-rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/Option.py
+-rw-r--r--   0 nymath     (501) staff       (20)       97 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.375426 torchqtm-0.2.0/torchqtm/derivatives/option/data/
+-rw-r--r--   0 nymath     (501) staff       (20)       40 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/data/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      333 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/data/load_data.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2698 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/functional.py
+-rw-r--r--   0 nymath     (501) staff       (20)      598 2023-06-19 14:11:23.000000 torchqtm-0.2.0/torchqtm/derivatives/option/main.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.376435 torchqtm-0.2.0/torchqtm/edbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-27 14:16:32.000000 torchqtm-0.2.0/torchqtm/edbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    19847 2023-07-13 06:39:56.000000 torchqtm-0.2.0/torchqtm/edbt/algorithm.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.376771 torchqtm-0.2.0/torchqtm/edbt/gens/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:46:20.000000 torchqtm-0.2.0/torchqtm/edbt/gens/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2555 2023-07-11 09:33:34.000000 torchqtm-0.2.0/torchqtm/edbt/gens/sim_engine.py
+-rw-r--r--   0 nymath     (501) staff       (20)     4761 2023-07-13 06:48:14.000000 torchqtm-0.2.0/torchqtm/edbt/run_algo.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3458 2023-07-11 05:26:20.000000 torchqtm-0.2.0/torchqtm/edbt/sim_params.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.378387 torchqtm-0.2.0/torchqtm/edbt/temp/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:29:06.000000 torchqtm-0.2.0/torchqtm/edbt/temp/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2143 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/edbt/temp/account.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2269 2023-06-27 11:29:29.000000 torchqtm-0.2.0/torchqtm/edbt/temp/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7015 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/edbt/temp/datahandler.py
+-rw-r--r--   0 nymath     (501) staff       (20)      144 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/edbt/temp/setup.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-27 11:29:29.000000 torchqtm-0.2.0/torchqtm/edbt/temp/test.py
+-rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/edbt/temp/testsearch.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.381879 torchqtm-0.2.0/torchqtm/finance/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 14:28:45.000000 torchqtm-0.2.0/torchqtm/finance/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)   381269 2023-07-13 03:01:39.000000 torchqtm-0.2.0/torchqtm/finance/_finance_ext.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)    14758 2023-07-13 05:54:26.000000 torchqtm-0.2.0/torchqtm/finance/account.py
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 02:21:33.000000 torchqtm-0.2.0/torchqtm/finance/finance_ext.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.382955 torchqtm-0.2.0/torchqtm/finance/metrics/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:15:11.000000 torchqtm-0.2.0/torchqtm/finance/metrics/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      143 2023-07-12 07:38:30.000000 torchqtm-0.2.0/torchqtm/finance/metrics/loader.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7566 2023-07-13 05:53:29.000000 torchqtm-0.2.0/torchqtm/finance/metrics/metric.py
+-rw-r--r--   0 nymath     (501) staff       (20)     8929 2023-07-12 14:03:21.000000 torchqtm-0.2.0/torchqtm/finance/metrics/tracker.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.385124 torchqtm-0.2.0/torchqtm/finance/models/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:34.000000 torchqtm-0.2.0/torchqtm/finance/models/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      845 2023-07-12 01:43:27.000000 torchqtm-0.2.0/torchqtm/finance/models/cancel_policy.py
+-rw-r--r--   0 nymath     (501) staff       (20)    11967 2023-07-11 02:59:21.000000 torchqtm-0.2.0/torchqtm/finance/models/commission.py
+-rw-r--r--   0 nymath     (501) staff       (20)    20911 2023-07-13 06:01:13.000000 torchqtm-0.2.0/torchqtm/finance/models/slippage.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.388932 torchqtm-0.2.0/torchqtm/finance/orders/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:14:45.000000 torchqtm-0.2.0/torchqtm/finance/orders/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     8923 2023-07-12 08:40:39.000000 torchqtm-0.2.0/torchqtm/finance/orders/order.py
+-rw-r--r--   0 nymath     (501) staff       (20)    15141 2023-07-13 06:13:29.000000 torchqtm-0.2.0/torchqtm/finance/orders/tracker.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2466 2023-07-06 10:00:32.000000 torchqtm-0.2.0/torchqtm/finance/portfolio.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.389870 torchqtm-0.2.0/torchqtm/finance/positions/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:19.000000 torchqtm-0.2.0/torchqtm/finance/positions/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3384 2023-07-12 06:15:32.000000 torchqtm-0.2.0/torchqtm/finance/positions/position.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7469 2023-07-13 05:14:10.000000 torchqtm-0.2.0/torchqtm/finance/positions/tracker.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1319 2023-07-06 07:02:43.000000 torchqtm-0.2.0/torchqtm/finance/transaction.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2566 2023-07-06 03:42:02.000000 torchqtm-0.2.0/torchqtm/finance/zp_math.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.392231 torchqtm-0.2.0/torchqtm/op/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/op/CrossSectionalOperators.py
+-rw-r--r--   0 nymath     (501) staff       (20)      241 2023-06-19 12:58:39.000000 torchqtm-0.2.0/torchqtm/op/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    11492 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/op/_numba.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1965 2023-06-19 12:23:32.000000 torchqtm-0.2.0/torchqtm/op/algos.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.392696 torchqtm-0.2.0/torchqtm/op/filters/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 13:07:06.000000 torchqtm-0.2.0/torchqtm/op/filters/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    21852 2023-07-07 03:49:36.000000 torchqtm-0.2.0/torchqtm/op/functional.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.393859 torchqtm-0.2.0/torchqtm/tdbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/tdbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    12045 2023-06-23 23:59:52.000000 torchqtm-0.2.0/torchqtm/tdbt/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/tdbt/dataset.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1779 2023-07-11 03:00:28.000000 torchqtm-0.2.0/torchqtm/types.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.394071 torchqtm-0.2.0/torchqtm/uniquant/
+-rw-r--r--   0 nymath     (501) staff       (20)       63 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/uniquant/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.398205 torchqtm-0.2.0/torchqtm/utils/
+-rw-r--r--   0 nymath     (501) staff       (20)      626 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      431 2023-06-18 07:34:02.000000 torchqtm-0.2.0/torchqtm/utils/_decorators.py
+-rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/benchmark.py
+-rw-r--r--   0 nymath     (501) staff       (20)      219 2023-07-10 09:41:27.000000 torchqtm-0.2.0/torchqtm/utils/calendar_utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1459 2023-07-12 02:05:09.000000 torchqtm-0.2.0/torchqtm/utils/datetime_utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9078 2023-07-11 05:35:03.000000 torchqtm-0.2.0/torchqtm/utils/exchange_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2571 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/rebalance.py
+-rw-r--r--   0 nymath     (501) staff       (20)      114 2023-06-27 06:55:39.000000 torchqtm-0.2.0/torchqtm/utils/standards.py
+-rw-r--r--   0 nymath     (501) staff       (20)     4248 2023-06-18 06:26:04.000000 torchqtm-0.2.0/torchqtm/utils/stats.py
+-rw-r--r--   0 nymath     (501) staff       (20)      221 2023-07-04 05:59:26.000000 torchqtm-0.2.0/torchqtm/utils/trading_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1570 2023-07-06 16:31:56.000000 torchqtm-0.2.0/torchqtm/utils/universe.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1835 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/visualization.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2675 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/warnings.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.360611 torchqtm-0.2.0/torchqtm.egg-info/
+-rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     3794 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/SOURCES.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        1 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/dependency_links.txt
+-rw-r--r--   0 nymath     (501) staff       (20)       44 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/requires.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        9 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/top_level.txt
```

### Comparing `torchqtm-0.1.0/LICENSE` & `torchqtm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/PKG-INFO` & `torchqtm-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,12 @@
-Metadata-Version: 2.1
-Name: torchqtm
-Version: 0.1.0
-Summary: None
-Home-page: https://github.com/nymath/torchquantum/tree/main
-Download-URL: https://github.com/nymath/torchquantum/releases/tag/
-Author: ny
-Author-email: nymath@163.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img src="https://github.com/nymath/torchquantum/blob/main/src/fig/logo.png" align="right" width="196" />
+<img src="https://github.com/nymath/torchqtm/blob/main/resources/fig/logo.png" align="right" width="196" />
 
 # torchquantum
 
-TorchQuantum is a backtesting framework that integrates
+TorchQuantum is a backtesting framework that""" integrates
 the structure of PyTorch and WorldQuant's Operator for
 efficient quantitative financial analysis.
 
 ## Contents
 
 - [Installation](#installation)
 - [Features](#features)
@@ -29,16 +14,16 @@
 
 ## Installation
 
 for Unix:
 
 ```shell
 cd /path/to/your/directory
-git clone git@github.com:nymath/torchquantum.git
-cd ./torchquantum
+git clone git@github.com:nymath/torchqtm.git
+cd ./torchqtm
 ```
 
 Before running examples, you should compile the cython code.
 
 ```shell
 python setup.py build_ext --inplace
 ```
@@ -51,59 +36,99 @@
 
 If you are not downloading the dataset, then you should
 
 ```shell
 cd ./examples
 mkdir largedata
 cd ./largedata
-wget https://github.com/nymath/torchquantum/releases/download/V0.1/Stocks.pkl.zip
-unzip Stocks.pkl.zip
-rm Stocks.pkl.zip
+wget https://github.com/nymath/torchqtm/releases/download/V0.1/stocks_f64.pkl.zip
+unzip stocks_f64.pkl.zip
+rm stocks_f64.pkl.zip
 cd ../
 cd ../
+git checkout dev
+```
+As for the backtesting dataset, we use the bundle provided by [ricequant](https://www.ricequant.com/welcome/).
+We have wrapped the code into Makefile, you can just run the following command to download the bundle.
+```shell
+make rqalpha_download_bundle
 ```
 
-## Example
 
+for windows:
+We highly recommend you to use WSL2 to run torchquantum.
+
+## Examples
+
+### alpha mining
 You can easily create an alpha through torchquantum!
 
 ```python
 import torchqtm.op as op
 import torchqtm.op.functional as F
+
+
 class NeutralizePE(op.Fundamental):
     def __init__(self, env):
         super().__init__(env)
-        self.lag = op.Parameter(5, required_optim=False, feasible_region=None)
+        self.lag = op.Parameter(5, requires_optim=False, feasible_region=None)
 
     def forward(self):
         self.data = F.divide(1, self.env.PE)
         self.data = F.winsorize(self.data, 'std', 4)
         self.data = F.normalize(self.data)
         self.data = F.group_neutralize(self.data, self.env.Sector)
         self.data = F.regression_neut(self.data, self.env.MktVal)
         self.data = F.ts_mean(self.data, self.lag)
         return self.data
 ```
+
 - `F` is library that contains the operators defined by WorldQuant.
 - `op.Fundamental` implies the NeutralizePE belongs to fundamental alpha.
 - `self.lag` is the parameter of rolling mean, which can be optimized through grid search.
 
+### backtesting
+Here we create a buy and hold strategy for illustration.
 
+```python
+from torchqtm.edbt.algorithm import TradingAlgorithm
+from torchqtm.assets import Equity
+
+class BuyAndHold(TradingAlgorithm):
+    def initialize(self):
+        self.safe_set_attr("s0", Equity("000001.XSHE"))
+        self.safe_set_attr("count", 0)
+
+    def before_trading_start(self):
+        pass
+
+    def handle_data(self):
+        if self.count == 0:
+            self.order(self.s0, 10000)
+        self.count += 1
 
+    def analyze(self):
+        pass
+```
 
 ## Features
 
 - High-speed backtesting framework (most of the operators are implemented through cython)
 - A revised gplearn library that is compatible with Alpha mining.
 - CNN and other state of the art models for mining alphas.
 - Event Driven backtesting framework is available.
 
 ## Contribution
 
-For more information, we refer to [Documentation](https://nymath.github.io/torchquantum/navigate).
-
+For more information, we refer to [Documentation](https://nymath.github.io/torchqtm/navigate).
 
 ## Join us
 
-If you are interested in quantitative finance and are committed to devoting 
+If you are interested in quantitative finance and are committed to devoting
 your life to alpha mining, you can contact me through WeChat at Ny_math.
 
+## References
+
+[quantopian/alphalens](https://github1s.com/quantopian/alphalens/blob/HEAD/alphalens/performance.py)
+
+[quantopian/zipline](https://github1s.com/quantopian/zipline/blob/HEAD/zipline/performance.py)
+
```

### Comparing `torchqtm-0.1.0/setup.py` & `torchqtm-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from distutils.core import setup
 from setuptools import find_packages
 from Cython.Build import cythonize
 import numpy
 import glob
 
 extensions = glob.glob("torchqtm/_C/*.pyx")
+extensions.extend(glob.glob("torchqtm/window/*.pyx"))
+extensions.extend(glob.glob("torchqtm/finance/*.pyx"))
 
 install_requires = [
     'numpy',
     'pandas',
     'pandas_market_calendars',
     'cython',
 ]
 
 
 def main():
     setup(
-        ext_modules=cythonize(extensions, language='c++'),
+        ext_modules=cythonize(extensions, annotate=True),
         include_dirs=[numpy.get_include()],
         name="torchqtm",
-        version="0.1.0",
+        version="0.2.0",
         author="ny",
         author_email="nymath@163.com",
         install_requires=install_requires,
         description="None",
         long_description=open('README.md', 'r').read(),
         long_description_content_type="text/markdown",
-        url="https://github.com/nymath/torchquantum/tree/main",
-        download_url="https://github.com/nymath/torchquantum/releases/tag/",
+        url="https://github.com/nymath/torchqtm",
+        download_url="https://github.com/nymath/torchqtm/releases/tag/",
         packages=find_packages(),
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
             "Operating System :: Unix",
         ],
-        python_requires='>=3.6',
+        python_requires='>=3.9',
     )
 
 
 if __name__ == "__main__":
     main()
 
 ## setup cython
 # python setup.py build_ext --inplace
 ## setup package
 # pip install twine
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
 # twine upload --skip-existing dist/*
 
+# ny.math
+# xxx
```

### Comparing `torchqtm-0.1.0/test/testRolling.py` & `torchqtm-0.2.0/test/testRolling.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/test/testgplearn.py` & `torchqtm-0.2.0/test/testgplearn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-import pickle
-import os
-from torchqtm.autoalpha.gplearn import fitness
-from torchqtm.autoalpha.gplearn.genetic import SymbolicRegressor, SymbolicTransformer
-from datetime import datetime
-import graphviz
-from gplearn.functions import make_function
+from torchqtm.alphas.autoalpha.gplearn import fitness
+from torchqtm.alphas.autoalpha.gplearn import SymbolicRegressor
 import numpy as np
 
 
 def score_func_basic(y, y_pred, sample_weight):  # 适应度函数：策略评价指标
     rlt = np.sum((y - y_pred) ** 2)
     return rlt
```

### Comparing `torchqtm-0.1.0/test/testop.py` & `torchqtm-0.2.0/test/testop.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/_C/__init__.cpp` & `torchqtm-0.2.0/torchqtm/_C/__init__.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/_C/_functional.cpp` & `torchqtm-0.2.0/torchqtm/_C/_functional.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
 #define CYTHON_ABI "0_29_34"
 #define CYTHON_HEX_VERSION 0x001D22F0
-#define CYTHON_FUTURE_DIVISION 1
+#define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
@@ -1523,14 +1523,21 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
+/* StrEquals.proto */
+#if PY_MAJOR_VERSION >= 3
+#define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
+#else
+#define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
+#endif
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1876,15 +1883,15 @@
 static const char __pyx_k_torchqtm__C__functional_pyx[] = "torchqtm/_C/_functional.pyx";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static PyObject *__pyx_n_s_DataFrame;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_n_s_LinearRegression;
 static PyObject *__pyx_n_s_OP_MODE;
-static PyObject *__pyx_n_u_STABLE;
+static PyObject *__pyx_n_s_STABLE;
 static PyObject *__pyx_n_s_X;
 static PyObject *__pyx_n_s_Y;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_axis;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_columns;
 static PyObject *__pyx_n_s_concatenate;
@@ -1895,16 +1902,16 @@
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_model;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_nanmean;
 static PyObject *__pyx_n_s_nanvar;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+static PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
+static PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_others;
 static PyObject *__pyx_n_s_pandas;
 static PyObject *__pyx_n_s_pd;
 static PyObject *__pyx_n_s_predict;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_regression_neut;
 static PyObject *__pyx_n_s_regression_neut_2;
@@ -2390,15 +2397,15 @@
   PyObject *__pyx_v_result = NULL;
   Py_ssize_t __pyx_v_i;
   PyObject *__pyx_v_y = NULL;
   PyObject *__pyx_v_X = NULL;
   PyObject *__pyx_v_model = NULL;
   PyObject *__pyx_v_y_pred = NULL;
   PyObject *__pyx_v_residuals = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_x = NULL;
+  PyObject *__pyx_v_x = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
@@ -2461,80 +2468,72 @@
  *         model.fit(X, y)
  */
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_concatenate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    { /* enter inner scope */
-      __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L7_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      if (likely(PyList_CheckExact(__pyx_v_others)) || PyTuple_CheckExact(__pyx_v_others)) {
-        __pyx_t_6 = __pyx_v_others; __Pyx_INCREF(__pyx_t_6); __pyx_t_7 = 0;
-        __pyx_t_8 = NULL;
-      } else {
-        __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_others); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L7_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 37, __pyx_L7_error)
-      }
-      for (;;) {
-        if (likely(!__pyx_t_8)) {
-          if (likely(PyList_CheckExact(__pyx_t_6))) {
-            if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_6)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_9 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 37, __pyx_L7_error)
-            #else
-            __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_9);
-            #endif
-          } else {
-            if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 37, __pyx_L7_error)
-            #else
-            __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_9);
-            #endif
-          }
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (likely(PyList_CheckExact(__pyx_v_others)) || PyTuple_CheckExact(__pyx_v_others)) {
+      __pyx_t_6 = __pyx_v_others; __Pyx_INCREF(__pyx_t_6); __pyx_t_7 = 0;
+      __pyx_t_8 = NULL;
+    } else {
+      __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_others); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 37, __pyx_L1_error)
+    }
+    for (;;) {
+      if (likely(!__pyx_t_8)) {
+        if (likely(PyList_CheckExact(__pyx_t_6))) {
+          if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_6)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_9 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 37, __pyx_L1_error)
+          #else
+          __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_9);
+          #endif
         } else {
-          __pyx_t_9 = __pyx_t_8(__pyx_t_6);
-          if (unlikely(!__pyx_t_9)) {
-            PyObject* exc_type = PyErr_Occurred();
-            if (exc_type) {
-              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 37, __pyx_L7_error)
-            }
-            break;
-          }
+          if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 37, __pyx_L1_error)
+          #else
+          __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
+          #endif
+        }
+      } else {
+        __pyx_t_9 = __pyx_t_8(__pyx_t_6);
+        if (unlikely(!__pyx_t_9)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 37, __pyx_L1_error)
+          }
+          break;
         }
-        __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_x, __pyx_t_9);
-        __pyx_t_9 = 0;
-        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_x, __pyx_n_s_values); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L7_error)
-        __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_9, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 37, __pyx_L7_error)
-        __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_reshape); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 37, __pyx_L7_error)
-        __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_10))) __PYX_ERR(0, 37, __pyx_L7_error)
-        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x); __pyx_7genexpr__pyx_v_x = 0;
-      goto __pyx_L10_exit_scope;
-      __pyx_L7_error:;
-      __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x); __pyx_7genexpr__pyx_v_x = 0;
-      goto __pyx_L1_error;
-      __pyx_L10_exit_scope:;
-    } /* exit inner scope */
+      __Pyx_XDECREF_SET(__pyx_v_x, __pyx_t_9);
+      __pyx_t_9 = 0;
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_values); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_9, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 37, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_reshape); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 37, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 37, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_10))) __PYX_ERR(0, 37, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
@@ -2756,15 +2755,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_y);
   __Pyx_XDECREF(__pyx_v_X);
   __Pyx_XDECREF(__pyx_v_model);
   __Pyx_XDECREF(__pyx_v_y_pred);
   __Pyx_XDECREF(__pyx_v_residuals);
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x);
+  __Pyx_XDECREF(__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "torchqtm/_C/_functional.pyx":48
  * @cython.wraparound(False)
@@ -2962,15 +2961,15 @@
  *         if __OP_MODE__ == "STABLE":             # <<<<<<<<<<<<<<
  *             return _regression_neuts(Y, others)
  *         else:
  */
   /*else*/ {
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_OP_MODE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_STABLE, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_t_2, __pyx_n_s_STABLE, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_4) {
 
       /* "torchqtm/_C/_functional.pyx":54
  *     else:
  *         if __OP_MODE__ == "STABLE":
  *             return _regression_neuts(Y, others)             # <<<<<<<<<<<<<<
@@ -4136,15 +4135,15 @@
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_DataFrame, __pyx_k_DataFrame, sizeof(__pyx_k_DataFrame), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_n_s_LinearRegression, __pyx_k_LinearRegression, sizeof(__pyx_k_LinearRegression), 0, 0, 1, 1},
   {&__pyx_n_s_OP_MODE, __pyx_k_OP_MODE, sizeof(__pyx_k_OP_MODE), 0, 0, 1, 1},
-  {&__pyx_n_u_STABLE, __pyx_k_STABLE, sizeof(__pyx_k_STABLE), 0, 1, 0, 1},
+  {&__pyx_n_s_STABLE, __pyx_k_STABLE, sizeof(__pyx_k_STABLE), 0, 0, 1, 1},
   {&__pyx_n_s_X, __pyx_k_X, sizeof(__pyx_k_X), 0, 0, 1, 1},
   {&__pyx_n_s_Y, __pyx_k_Y, sizeof(__pyx_k_Y), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_axis, __pyx_k_axis, sizeof(__pyx_k_axis), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
   {&__pyx_n_s_concatenate, __pyx_k_concatenate, sizeof(__pyx_k_concatenate), 0, 0, 1, 1},
@@ -4155,16 +4154,16 @@
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_model, __pyx_k_model, sizeof(__pyx_k_model), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_nanmean, __pyx_k_nanmean, sizeof(__pyx_k_nanmean), 0, 0, 1, 1},
   {&__pyx_n_s_nanvar, __pyx_k_nanvar, sizeof(__pyx_k_nanvar), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-  {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+  {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
+  {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
   {&__pyx_n_s_others, __pyx_k_others, sizeof(__pyx_k_others), 0, 0, 1, 1},
   {&__pyx_n_s_pandas, __pyx_k_pandas, sizeof(__pyx_k_pandas), 0, 0, 1, 1},
   {&__pyx_n_s_pd, __pyx_k_pd, sizeof(__pyx_k_pd), 0, 0, 1, 1},
   {&__pyx_n_s_predict, __pyx_k_predict, sizeof(__pyx_k_predict), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_regression_neut, __pyx_k_regression_neut, sizeof(__pyx_k_regression_neut), 0, 0, 1, 1},
   {&__pyx_n_s_regression_neut_2, __pyx_k_regression_neut_2, sizeof(__pyx_k_regression_neut_2), 0, 0, 1, 1},
@@ -4211,26 +4210,26 @@
   /* "../../../opt/anaconda3/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "../../../opt/anaconda3/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "torchqtm/_C/_functional.pyx":19
  * @cython.wraparound(False)
  * @cython.boundscheck(False)
  * def _regression_neut(Y, X):             # <<<<<<<<<<<<<<
@@ -4616,27 +4615,27 @@
   /* "torchqtm/_C/_functional.pyx":4
  * # https://cython.readthedocs.io/en/stable/src/userguide/numpy_tutorial.html
  * cimport numpy
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport cython
  * import pandas as pd
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "torchqtm/_C/_functional.pyx":6
  * import numpy as np
  * cimport cython
  * import pandas as pd             # <<<<<<<<<<<<<<
  * from torchqtm.config import __OP_MODE__
  * from sklearn.linear_model import LinearRegression
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pandas, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pandas, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pd, __pyx_t_1) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "torchqtm/_C/_functional.pyx":7
  * cimport cython
  * import pandas as pd
@@ -4645,15 +4644,15 @@
  * 
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_OP_MODE);
   __Pyx_GIVEREF(__pyx_n_s_OP_MODE);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_OP_MODE);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_torchqtm_config, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_torchqtm_config, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_OP_MODE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_OP_MODE, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -4666,15 +4665,15 @@
  * ctypedef fused ArrayType:
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_LinearRegression);
   __Pyx_GIVEREF(__pyx_n_s_LinearRegression);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_LinearRegression);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_sklearn_linear_model, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_sklearn_linear_model, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_LinearRegression); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_LinearRegression, __pyx_t_2) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -4718,21 +4717,21 @@
   /* "torchqtm/_C/_functional.pyx":60
  * # roll_apply.pyx
  * cimport cython
  * import numpy as np             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "torchqtm/_C/_functional.pyx":1
- * # cython: language_level=3             # <<<<<<<<<<<<<<
+ * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # https://cython.readthedocs.io/en/stable/src/userguide/numpy_tutorial.html
  * cimport numpy
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `torchqtm-0.1.0/torchqtm/_C/_rolling.cpp` & `torchqtm-0.2.0/torchqtm/_C/_rolling.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
 #define CYTHON_ABI "0_29_34"
 #define CYTHON_HEX_VERSION 0x001D22F0
-#define CYTHON_FUTURE_DIVISION 1
+#define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
@@ -1463,15 +1463,15 @@
   int is_datetimelike;
 };
 struct __pyx_t_8torchqtm_2_C_8_rolling_node_t;
 typedef struct __pyx_t_8torchqtm_2_C_8_rolling_node_t __pyx_t_8torchqtm_2_C_8_rolling_node_t;
 struct __pyx_t_8torchqtm_2_C_8_rolling_skiplist_t;
 typedef struct __pyx_t_8torchqtm_2_C_8_rolling_skiplist_t __pyx_t_8torchqtm_2_C_8_rolling_skiplist_t;
 
-/* "torchqtm/_C/_rolling.pyx":60
+/* "torchqtm/_C/_rolling.pyx":59
  *     float64_t NaN = <float64_t>np.NaN
  * 
  * ctypedef struct node_t:             # <<<<<<<<<<<<<<
  *     node_t ** next
  *     int *width
  */
 struct __pyx_t_8torchqtm_2_C_8_rolling_node_t {
@@ -1479,15 +1479,15 @@
   int *width;
   double value;
   int is_nil;
   int levels;
   int ref_count;
 };
 
-/* "torchqtm/_C/_rolling.pyx":68
+/* "torchqtm/_C/_rolling.pyx":67
  *     int ref_count
  * 
  * ctypedef struct skiplist_t:             # <<<<<<<<<<<<<<
  *     node_t *head
  *     node_t ** tmp_chain
  */
 struct __pyx_t_8torchqtm_2_C_8_rolling_skiplist_t {
@@ -1792,14 +1792,20 @@
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* BufferFallbackError.proto */
 static void __Pyx_RaiseBufferFallbackError(void);
 
+/* BufferIndexError.proto */
+static void __Pyx_RaiseBufferIndexError(int axis);
+
+/* BufferIndexErrorNogil.proto */
+static void __Pyx_RaiseBufferIndexErrorNogil(int axis);
+
 #define __Pyx_BufPtrStrided1d(type, buf, i0, s0) (type)((char*)buf + i0 * s0)
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
@@ -1855,14 +1861,19 @@
 #define __pyx_get_slice_count_pointer(memview) (memview->acquisition_count_aligned_p)
 #define __pyx_get_slice_count(memview) (*__pyx_get_slice_count_pointer(memview))
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XDEC_MEMVIEW(slice, have_gil) __Pyx_XDEC_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *, int, int);
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
 #endif
 
@@ -2000,14 +2011,17 @@
 /* StrEquals.proto */
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
 #else
 #define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
 #endif
 
+/* DivInt[Py_ssize_t].proto */
+static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t, Py_ssize_t);
+
 /* UnaryNegOverflows.proto */
 #define UNARY_NEG_WOULD_OVERFLOW(x)\
         (((x) < 0) & ((unsigned long)(x) == 0-(unsigned long)(x)))
 
 static CYTHON_UNUSED int __pyx_array_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *); /*proto*/
 /* GetAttr.proto */
@@ -2121,14 +2135,17 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* DivInt[long].proto */
+static CYTHON_INLINE long __Pyx_div_long(long, long);
+
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* ImportFrom.proto */
@@ -2753,15 +2770,15 @@
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
-static PyObject *__pyx_n_u_C;
+static PyObject *__pyx_n_s_C;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_n_s_ImportError;
@@ -2842,16 +2859,16 @@
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_neg_ct;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_nobs;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+static PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
+static PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_output;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
@@ -3006,180 +3023,180 @@
 static PyObject *__pyx_codeobj__35;
 static PyObject *__pyx_codeobj__37;
 static PyObject *__pyx_codeobj__39;
 static PyObject *__pyx_codeobj__41;
 static PyObject *__pyx_codeobj__48;
 /* Late includes */
 
-/* "torchqtm/_C/_rolling.pyx":76
+/* "torchqtm/_C/_rolling.pyx":75
  * 
  * 
  * cdef bint isnan(float64_t x) nogil:             # <<<<<<<<<<<<<<
  *     return x != x
  * 
  */
 
 static int __pyx_f_8torchqtm_2_C_8_rolling_isnan(__pyx_t_5numpy_float64_t __pyx_v_x) {
   int __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":77
+  /* "torchqtm/_C/_rolling.pyx":76
  * 
  * cdef bint isnan(float64_t x) nogil:
  *     return x != x             # <<<<<<<<<<<<<<
  * 
  * cdef bint notnan(float64_t x) nogil:
  */
   __pyx_r = (__pyx_v_x != __pyx_v_x);
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":76
+  /* "torchqtm/_C/_rolling.pyx":75
  * 
  * 
  * cdef bint isnan(float64_t x) nogil:             # <<<<<<<<<<<<<<
  *     return x != x
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":79
+/* "torchqtm/_C/_rolling.pyx":78
  *     return x != x
  * 
  * cdef bint notnan(float64_t x) nogil:             # <<<<<<<<<<<<<<
  *     return x == x
  * 
  */
 
 static int __pyx_f_8torchqtm_2_C_8_rolling_notnan(__pyx_t_5numpy_float64_t __pyx_v_x) {
   int __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":80
+  /* "torchqtm/_C/_rolling.pyx":79
  * 
  * cdef bint notnan(float64_t x) nogil:
  *     return x == x             # <<<<<<<<<<<<<<
  * 
  * cdef bint signbit(float64_t x) nogil:
  */
   __pyx_r = (__pyx_v_x == __pyx_v_x);
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":79
+  /* "torchqtm/_C/_rolling.pyx":78
  *     return x != x
  * 
  * cdef bint notnan(float64_t x) nogil:             # <<<<<<<<<<<<<<
  *     return x == x
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":82
+/* "torchqtm/_C/_rolling.pyx":81
  *     return x == x
  * 
  * cdef bint signbit(float64_t x) nogil:             # <<<<<<<<<<<<<<
  *     if x < 0.0:
  *         return 1
  */
 
 static int __pyx_f_8torchqtm_2_C_8_rolling_signbit(__pyx_t_5numpy_float64_t __pyx_v_x) {
   int __pyx_r;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":83
+  /* "torchqtm/_C/_rolling.pyx":82
  * 
  * cdef bint signbit(float64_t x) nogil:
  *     if x < 0.0:             # <<<<<<<<<<<<<<
  *         return 1
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_x < 0.0) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":84
+    /* "torchqtm/_C/_rolling.pyx":83
  * cdef bint signbit(float64_t x) nogil:
  *     if x < 0.0:
  *         return 1             # <<<<<<<<<<<<<<
  *     else:
  *         return 0
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "torchqtm/_C/_rolling.pyx":83
+    /* "torchqtm/_C/_rolling.pyx":82
  * 
  * cdef bint signbit(float64_t x) nogil:
  *     if x < 0.0:             # <<<<<<<<<<<<<<
  *         return 1
  *     else:
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":86
+  /* "torchqtm/_C/_rolling.pyx":85
  *         return 1
  *     else:
  *         return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __pyx_r = 0;
     goto __pyx_L0;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":82
+  /* "torchqtm/_C/_rolling.pyx":81
  *     return x == x
  * 
  * cdef bint signbit(float64_t x) nogil:             # <<<<<<<<<<<<<<
  *     if x < 0.0:
  *         return 1
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":91
+/* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
 static CYTHON_INLINE __pyx_t_5numpy_int8_t __pyx_fuse_0__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_minp, CYTHON_UNUSED Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_int8_t __pyx_v_value) {
   __pyx_t_5numpy_int8_t __pyx_v_result;
   __pyx_t_5numpy_int8_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":102
+  /* "torchqtm/_C/_rolling.pyx":101
  *             result = NaN
  *     else:
  *         result = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __pyx_v_value;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3188,34 +3205,34 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_int16_t __pyx_fuse_1__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_minp, CYTHON_UNUSED Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_int16_t __pyx_v_value) {
   __pyx_t_5numpy_int16_t __pyx_v_result;
   __pyx_t_5numpy_int16_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":102
+  /* "torchqtm/_C/_rolling.pyx":101
  *             result = NaN
  *     else:
  *         result = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __pyx_v_value;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3224,34 +3241,34 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_int32_t __pyx_fuse_2__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_minp, CYTHON_UNUSED Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_int32_t __pyx_v_value) {
   __pyx_t_5numpy_int32_t __pyx_v_result;
   __pyx_t_5numpy_int32_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":102
+  /* "torchqtm/_C/_rolling.pyx":101
  *             result = NaN
  *     else:
  *         result = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __pyx_v_value;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3260,34 +3277,34 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_int64_t __pyx_fuse_3__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_minp, CYTHON_UNUSED Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_int64_t __pyx_v_value) {
   __pyx_t_5numpy_int64_t __pyx_v_result;
   __pyx_t_5numpy_int64_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":102
+  /* "torchqtm/_C/_rolling.pyx":101
  *             result = NaN
  *     else:
  *         result = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __pyx_v_value;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3296,34 +3313,34 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_uint8_t __pyx_fuse_4__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_minp, CYTHON_UNUSED Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_uint8_t __pyx_v_value) {
   __pyx_t_5numpy_uint8_t __pyx_v_result;
   __pyx_t_5numpy_uint8_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":102
+  /* "torchqtm/_C/_rolling.pyx":101
  *             result = NaN
  *     else:
  *         result = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __pyx_v_value;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3332,34 +3349,34 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_uint16_t __pyx_fuse_5__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_minp, CYTHON_UNUSED Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_uint16_t __pyx_v_value) {
   __pyx_t_5numpy_uint16_t __pyx_v_result;
   __pyx_t_5numpy_uint16_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":102
+  /* "torchqtm/_C/_rolling.pyx":101
  *             result = NaN
  *     else:
  *         result = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __pyx_v_value;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3368,34 +3385,34 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_uint32_t __pyx_fuse_6__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_minp, CYTHON_UNUSED Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_uint32_t __pyx_v_value) {
   __pyx_t_5numpy_uint32_t __pyx_v_result;
   __pyx_t_5numpy_uint32_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":102
+  /* "torchqtm/_C/_rolling.pyx":101
  *             result = NaN
  *     else:
  *         result = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __pyx_v_value;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3404,34 +3421,34 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_uint64_t __pyx_fuse_7__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_minp, CYTHON_UNUSED Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_uint64_t __pyx_v_value) {
   __pyx_t_5numpy_uint64_t __pyx_v_result;
   __pyx_t_5numpy_uint64_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":102
+  /* "torchqtm/_C/_rolling.pyx":101
  *             result = NaN
  *     else:
  *         result = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __pyx_v_value;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3441,66 +3458,66 @@
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_float32_t __pyx_fuse_8__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(__pyx_t_5numpy_int64_t __pyx_v_minp, Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_float32_t __pyx_v_value) {
   __pyx_t_5numpy_float32_t __pyx_v_result;
   __pyx_t_5numpy_float32_t __pyx_r;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":97
+  /* "torchqtm/_C/_rolling.pyx":96
  * 
  *     if numeric_t in cython.floating:
  *         if nobs >= minp:             # <<<<<<<<<<<<<<
  *             result = value
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_nobs >= __pyx_v_minp) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":98
+    /* "torchqtm/_C/_rolling.pyx":97
  *     if numeric_t in cython.floating:
  *         if nobs >= minp:
  *             result = value             # <<<<<<<<<<<<<<
  *         else:
  *             result = NaN
  */
     __pyx_v_result = __pyx_v_value;
 
-    /* "torchqtm/_C/_rolling.pyx":97
+    /* "torchqtm/_C/_rolling.pyx":96
  * 
  *     if numeric_t in cython.floating:
  *         if nobs >= minp:             # <<<<<<<<<<<<<<
  *             result = value
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":100
+  /* "torchqtm/_C/_rolling.pyx":99
  *             result = value
  *         else:
  *             result = NaN             # <<<<<<<<<<<<<<
  *     else:
  *         result = value
  */
   /*else*/ {
     __pyx_v_result = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
   }
   __pyx_L3:;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
@@ -3510,109 +3527,109 @@
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_float64_t __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(__pyx_t_5numpy_int64_t __pyx_v_minp, Py_ssize_t __pyx_v_nobs, __pyx_t_5numpy_float64_t __pyx_v_value) {
   __pyx_t_5numpy_float64_t __pyx_v_result;
   __pyx_t_5numpy_float64_t __pyx_r;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":97
+  /* "torchqtm/_C/_rolling.pyx":96
  * 
  *     if numeric_t in cython.floating:
  *         if nobs >= minp:             # <<<<<<<<<<<<<<
  *             result = value
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_nobs >= __pyx_v_minp) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":98
+    /* "torchqtm/_C/_rolling.pyx":97
  *     if numeric_t in cython.floating:
  *         if nobs >= minp:
  *             result = value             # <<<<<<<<<<<<<<
  *         else:
  *             result = NaN
  */
     __pyx_v_result = __pyx_v_value;
 
-    /* "torchqtm/_C/_rolling.pyx":97
+    /* "torchqtm/_C/_rolling.pyx":96
  * 
  *     if numeric_t in cython.floating:
  *         if nobs >= minp:             # <<<<<<<<<<<<<<
  *             result = value
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":100
+  /* "torchqtm/_C/_rolling.pyx":99
  *             result = value
  *         else:
  *             result = NaN             # <<<<<<<<<<<<<<
  *     else:
  *         result = value
  */
   /*else*/ {
     __pyx_v_result = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
   }
   __pyx_L3:;
 
-  /* "torchqtm/_C/_rolling.pyx":104
+  /* "torchqtm/_C/_rolling.pyx":103
  *         result = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":91
+  /* "torchqtm/_C/_rolling.pyx":90
  * #
  * #
  * cdef inline numeric_t calc_mm(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                               numeric_t value) nogil:
  *     cdef:
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":107
+/* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
 static CYTHON_INLINE __pyx_t_5numpy_int8_t __pyx_fuse_0__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_int8_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, CYTHON_UNUSED int __pyx_v_is_max) {
   __pyx_t_5numpy_int8_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":124
+  /* "torchqtm/_C/_rolling.pyx":123
  * 
  *     else:
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  * 
  *     return ai
  */
   (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3620,34 +3637,34 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_int16_t __pyx_fuse_1__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_int16_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, CYTHON_UNUSED int __pyx_v_is_max) {
   __pyx_t_5numpy_int16_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":124
+  /* "torchqtm/_C/_rolling.pyx":123
  * 
  *     else:
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  * 
  *     return ai
  */
   (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3655,34 +3672,34 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_int32_t __pyx_fuse_2__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_int32_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, CYTHON_UNUSED int __pyx_v_is_max) {
   __pyx_t_5numpy_int32_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":124
+  /* "torchqtm/_C/_rolling.pyx":123
  * 
  *     else:
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  * 
  *     return ai
  */
   (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3690,34 +3707,34 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_int64_t __pyx_fuse_3__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_int64_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, CYTHON_UNUSED int __pyx_v_is_max) {
   __pyx_t_5numpy_int64_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":124
+  /* "torchqtm/_C/_rolling.pyx":123
  * 
  *     else:
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  * 
  *     return ai
  */
   (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3725,34 +3742,34 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_uint8_t __pyx_fuse_4__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_uint8_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, CYTHON_UNUSED int __pyx_v_is_max) {
   __pyx_t_5numpy_uint8_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":124
+  /* "torchqtm/_C/_rolling.pyx":123
  * 
  *     else:
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  * 
  *     return ai
  */
   (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3760,34 +3777,34 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_uint16_t __pyx_fuse_5__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_uint16_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, CYTHON_UNUSED int __pyx_v_is_max) {
   __pyx_t_5numpy_uint16_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":124
+  /* "torchqtm/_C/_rolling.pyx":123
  * 
  *     else:
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  * 
  *     return ai
  */
   (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3795,34 +3812,34 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_uint32_t __pyx_fuse_6__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_uint32_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, CYTHON_UNUSED int __pyx_v_is_max) {
   __pyx_t_5numpy_uint32_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":124
+  /* "torchqtm/_C/_rolling.pyx":123
  * 
  *     else:
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  * 
  *     return ai
  */
   (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3830,34 +3847,34 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_uint64_t __pyx_fuse_7__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_uint64_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, CYTHON_UNUSED int __pyx_v_is_max) {
   __pyx_t_5numpy_uint64_t __pyx_r;
 
-  /* "torchqtm/_C/_rolling.pyx":124
+  /* "torchqtm/_C/_rolling.pyx":123
  * 
  *     else:
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  * 
  *     return ai
  */
   (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3866,103 +3883,103 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_float32_t __pyx_fuse_8__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_float32_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, int __pyx_v_is_max) {
   __pyx_t_5numpy_float32_t __pyx_r;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":110
+  /* "torchqtm/_C/_rolling.pyx":109
  * 
  *     if numeric_t in cython.floating:
  *         if ai == ai:             # <<<<<<<<<<<<<<
  *             nobs[0] = nobs[0] + 1
  *         elif is_max:
  */
   __pyx_t_1 = ((__pyx_v_ai == __pyx_v_ai) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":111
+    /* "torchqtm/_C/_rolling.pyx":110
  *     if numeric_t in cython.floating:
  *         if ai == ai:
  *             nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  *         elif is_max:
  *             if numeric_t == cython.float:
  */
     (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-    /* "torchqtm/_C/_rolling.pyx":110
+    /* "torchqtm/_C/_rolling.pyx":109
  * 
  *     if numeric_t in cython.floating:
  *         if ai == ai:             # <<<<<<<<<<<<<<
  *             nobs[0] = nobs[0] + 1
  *         elif is_max:
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":112
+  /* "torchqtm/_C/_rolling.pyx":111
  *         if ai == ai:
  *             nobs[0] = nobs[0] + 1
  *         elif is_max:             # <<<<<<<<<<<<<<
  *             if numeric_t == cython.float:
  *                 ai = MINfloat32
  */
   __pyx_t_1 = (__pyx_v_is_max != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":114
+    /* "torchqtm/_C/_rolling.pyx":113
  *         elif is_max:
  *             if numeric_t == cython.float:
  *                 ai = MINfloat32             # <<<<<<<<<<<<<<
  *             else:
  *                 ai = MINfloat64
  */
     __pyx_v_ai = __pyx_v_8torchqtm_2_C_8_rolling_MINfloat32;
 
-    /* "torchqtm/_C/_rolling.pyx":112
+    /* "torchqtm/_C/_rolling.pyx":111
  *         if ai == ai:
  *             nobs[0] = nobs[0] + 1
  *         elif is_max:             # <<<<<<<<<<<<<<
  *             if numeric_t == cython.float:
  *                 ai = MINfloat32
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":118
+  /* "torchqtm/_C/_rolling.pyx":117
  *                 ai = MINfloat64
  *         else:
  *             if numeric_t == cython.float:             # <<<<<<<<<<<<<<
  *                 ai = MAXfloat32
  *             else:
  */
   /*else*/ {
 
-    /* "torchqtm/_C/_rolling.pyx":119
+    /* "torchqtm/_C/_rolling.pyx":118
  *         else:
  *             if numeric_t == cython.float:
  *                 ai = MAXfloat32             # <<<<<<<<<<<<<<
  *             else:
  *                 ai = MAXfloat64
  */
     __pyx_v_ai = __pyx_v_8torchqtm_2_C_8_rolling_MAXfloat32;
   }
   __pyx_L3:;
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
@@ -3971,663 +3988,663 @@
   return __pyx_r;
 }
 
 static CYTHON_INLINE __pyx_t_5numpy_float64_t __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling_init_mm(__pyx_t_5numpy_float64_t __pyx_v_ai, Py_ssize_t *__pyx_v_nobs, int __pyx_v_is_max) {
   __pyx_t_5numpy_float64_t __pyx_r;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":110
+  /* "torchqtm/_C/_rolling.pyx":109
  * 
  *     if numeric_t in cython.floating:
  *         if ai == ai:             # <<<<<<<<<<<<<<
  *             nobs[0] = nobs[0] + 1
  *         elif is_max:
  */
   __pyx_t_1 = ((__pyx_v_ai == __pyx_v_ai) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":111
+    /* "torchqtm/_C/_rolling.pyx":110
  *     if numeric_t in cython.floating:
  *         if ai == ai:
  *             nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  *         elif is_max:
  *             if numeric_t == cython.float:
  */
     (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-    /* "torchqtm/_C/_rolling.pyx":110
+    /* "torchqtm/_C/_rolling.pyx":109
  * 
  *     if numeric_t in cython.floating:
  *         if ai == ai:             # <<<<<<<<<<<<<<
  *             nobs[0] = nobs[0] + 1
  *         elif is_max:
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":112
+  /* "torchqtm/_C/_rolling.pyx":111
  *         if ai == ai:
  *             nobs[0] = nobs[0] + 1
  *         elif is_max:             # <<<<<<<<<<<<<<
  *             if numeric_t == cython.float:
  *                 ai = MINfloat32
  */
   __pyx_t_1 = (__pyx_v_is_max != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":116
+    /* "torchqtm/_C/_rolling.pyx":115
  *                 ai = MINfloat32
  *             else:
  *                 ai = MINfloat64             # <<<<<<<<<<<<<<
  *         else:
  *             if numeric_t == cython.float:
  */
     __pyx_v_ai = __pyx_v_8torchqtm_2_C_8_rolling_MINfloat64;
 
-    /* "torchqtm/_C/_rolling.pyx":112
+    /* "torchqtm/_C/_rolling.pyx":111
  *         if ai == ai:
  *             nobs[0] = nobs[0] + 1
  *         elif is_max:             # <<<<<<<<<<<<<<
  *             if numeric_t == cython.float:
  *                 ai = MINfloat32
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":118
+  /* "torchqtm/_C/_rolling.pyx":117
  *                 ai = MINfloat64
  *         else:
  *             if numeric_t == cython.float:             # <<<<<<<<<<<<<<
  *                 ai = MAXfloat32
  *             else:
  */
   /*else*/ {
 
-    /* "torchqtm/_C/_rolling.pyx":121
+    /* "torchqtm/_C/_rolling.pyx":120
  *                 ai = MAXfloat32
  *             else:
  *                 ai = MAXfloat64             # <<<<<<<<<<<<<<
  * 
  *     else:
  */
     __pyx_v_ai = __pyx_v_8torchqtm_2_C_8_rolling_MAXfloat64;
   }
   __pyx_L3:;
 
-  /* "torchqtm/_C/_rolling.pyx":126
+  /* "torchqtm/_C/_rolling.pyx":125
  *         nobs[0] = nobs[0] + 1
  * 
  *     return ai             # <<<<<<<<<<<<<<
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  */
   __pyx_r = __pyx_v_ai;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":107
+  /* "torchqtm/_C/_rolling.pyx":106
  * 
  * 
  * cdef inline numeric_t init_mm(numeric_t ai, Py_ssize_t *nobs, bint is_max) nogil:             # <<<<<<<<<<<<<<
  * 
  *     if numeric_t in cython.floating:
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_0__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(CYTHON_UNUSED __pyx_t_5numpy_int8_t __pyx_v_aold, CYTHON_UNUSED Py_ssize_t *__pyx_v_nobs) {
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_1__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(CYTHON_UNUSED __pyx_t_5numpy_int16_t __pyx_v_aold, CYTHON_UNUSED Py_ssize_t *__pyx_v_nobs) {
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_2__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(CYTHON_UNUSED __pyx_t_5numpy_int32_t __pyx_v_aold, CYTHON_UNUSED Py_ssize_t *__pyx_v_nobs) {
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_3__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v_aold, CYTHON_UNUSED Py_ssize_t *__pyx_v_nobs) {
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_4__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(CYTHON_UNUSED __pyx_t_5numpy_uint8_t __pyx_v_aold, CYTHON_UNUSED Py_ssize_t *__pyx_v_nobs) {
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_5__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(CYTHON_UNUSED __pyx_t_5numpy_uint16_t __pyx_v_aold, CYTHON_UNUSED Py_ssize_t *__pyx_v_nobs) {
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_6__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(CYTHON_UNUSED __pyx_t_5numpy_uint32_t __pyx_v_aold, CYTHON_UNUSED Py_ssize_t *__pyx_v_nobs) {
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_7__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(CYTHON_UNUSED __pyx_t_5numpy_uint64_t __pyx_v_aold, CYTHON_UNUSED Py_ssize_t *__pyx_v_nobs) {
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":128
+/* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
 static CYTHON_INLINE void __pyx_fuse_8__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(__pyx_t_5numpy_float32_t __pyx_v_aold, Py_ssize_t *__pyx_v_nobs) {
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
   __pyx_t_1 = ((__pyx_v_aold == __pyx_v_aold) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":131
+    /* "torchqtm/_C/_rolling.pyx":130
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  *         nobs[0] = nobs[0] - 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) - 1);
 
-    /* "torchqtm/_C/_rolling.pyx":130
+    /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":128
+  /* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
   /* function exit code */
 }
 
 static CYTHON_INLINE void __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling_remove_mm(__pyx_t_5numpy_float64_t __pyx_v_aold, Py_ssize_t *__pyx_v_nobs) {
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":130
+  /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
   __pyx_t_1 = ((__pyx_v_aold == __pyx_v_aold) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":131
+    /* "torchqtm/_C/_rolling.pyx":130
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  *         nobs[0] = nobs[0] - 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) - 1);
 
-    /* "torchqtm/_C/_rolling.pyx":130
+    /* "torchqtm/_C/_rolling.pyx":129
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  * 
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":128
+  /* "torchqtm/_C/_rolling.pyx":127
  *     return ai
  * 
  * cdef inline void remove_mm(numeric_t aold, Py_ssize_t *nobs) nogil:             # <<<<<<<<<<<<<<
  *     """ remove a value from the mm calc """
  *     if numeric_t in cython.floating and aold == aold:
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":134
+/* "torchqtm/_C/_rolling.pyx":133
  * 
  * 
  * cdef inline float64_t calc_sum(int64_t minp, int64_t nobs, float64_t sum_x) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         float64_t result
  */
 
 static CYTHON_INLINE __pyx_t_5numpy_float64_t __pyx_f_8torchqtm_2_C_8_rolling_calc_sum(__pyx_t_5numpy_int64_t __pyx_v_minp, __pyx_t_5numpy_int64_t __pyx_v_nobs, __pyx_t_5numpy_float64_t __pyx_v_sum_x) {
   __pyx_t_5numpy_float64_t __pyx_v_result;
   __pyx_t_5numpy_float64_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
 
-  /* "torchqtm/_C/_rolling.pyx":138
+  /* "torchqtm/_C/_rolling.pyx":137
  *         float64_t result
  * 
  *     if nobs == 0 == minp:             # <<<<<<<<<<<<<<
  *         result = 0
  *     elif nobs >= minp:
  */
   __pyx_t_1 = (__pyx_v_nobs == 0);
   if (__pyx_t_1) {
     __pyx_t_1 = (0 == __pyx_v_minp);
   }
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "torchqtm/_C/_rolling.pyx":139
+    /* "torchqtm/_C/_rolling.pyx":138
  * 
  *     if nobs == 0 == minp:
  *         result = 0             # <<<<<<<<<<<<<<
  *     elif nobs >= minp:
  *         result = sum_x
  */
     __pyx_v_result = 0.0;
 
-    /* "torchqtm/_C/_rolling.pyx":138
+    /* "torchqtm/_C/_rolling.pyx":137
  *         float64_t result
  * 
  *     if nobs == 0 == minp:             # <<<<<<<<<<<<<<
  *         result = 0
  *     elif nobs >= minp:
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":140
+  /* "torchqtm/_C/_rolling.pyx":139
  *     if nobs == 0 == minp:
  *         result = 0
  *     elif nobs >= minp:             # <<<<<<<<<<<<<<
  *         result = sum_x
  *     else:
  */
   __pyx_t_2 = ((__pyx_v_nobs >= __pyx_v_minp) != 0);
   if (__pyx_t_2) {
 
-    /* "torchqtm/_C/_rolling.pyx":141
+    /* "torchqtm/_C/_rolling.pyx":140
  *         result = 0
  *     elif nobs >= minp:
  *         result = sum_x             # <<<<<<<<<<<<<<
  *     else:
  *         result = NaN
  */
     __pyx_v_result = __pyx_v_sum_x;
 
-    /* "torchqtm/_C/_rolling.pyx":140
+    /* "torchqtm/_C/_rolling.pyx":139
  *     if nobs == 0 == minp:
  *         result = 0
  *     elif nobs >= minp:             # <<<<<<<<<<<<<<
  *         result = sum_x
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":143
+  /* "torchqtm/_C/_rolling.pyx":142
  *         result = sum_x
  *     else:
  *         result = NaN             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   /*else*/ {
     __pyx_v_result = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
   }
   __pyx_L3:;
 
-  /* "torchqtm/_C/_rolling.pyx":145
+  /* "torchqtm/_C/_rolling.pyx":144
  *         result = NaN
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":134
+  /* "torchqtm/_C/_rolling.pyx":133
  * 
  * 
  * cdef inline float64_t calc_sum(int64_t minp, int64_t nobs, float64_t sum_x) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         float64_t result
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":148
+/* "torchqtm/_C/_rolling.pyx":147
  * 
  * 
  * cdef inline void add_sum(float64_t val, int64_t *nobs, float64_t *sum_x,             # <<<<<<<<<<<<<<
  *                          float64_t *compensation) nogil:
  *     """ add a value from the sum calc using Kahan summation """
  */
 
 static CYTHON_INLINE void __pyx_f_8torchqtm_2_C_8_rolling_add_sum(__pyx_t_5numpy_float64_t __pyx_v_val, __pyx_t_5numpy_int64_t *__pyx_v_nobs, __pyx_t_5numpy_float64_t *__pyx_v_sum_x, __pyx_t_5numpy_float64_t *__pyx_v_compensation) {
   __pyx_t_5numpy_float64_t __pyx_v_y;
   __pyx_t_5numpy_float64_t __pyx_v_t;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":156
+  /* "torchqtm/_C/_rolling.pyx":155
  * 
  *     # Not NaN
  *     if notnan(val):             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] + 1
  *         y = val - compensation[0]
  */
   __pyx_t_1 = (__pyx_f_8torchqtm_2_C_8_rolling_notnan(__pyx_v_val) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":157
+    /* "torchqtm/_C/_rolling.pyx":156
  *     # Not NaN
  *     if notnan(val):
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  *         y = val - compensation[0]
  *         t = sum_x[0] + y
  */
     (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-    /* "torchqtm/_C/_rolling.pyx":158
+    /* "torchqtm/_C/_rolling.pyx":157
  *     if notnan(val):
  *         nobs[0] = nobs[0] + 1
  *         y = val - compensation[0]             # <<<<<<<<<<<<<<
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y
  */
     __pyx_v_y = (__pyx_v_val - (__pyx_v_compensation[0]));
 
-    /* "torchqtm/_C/_rolling.pyx":159
+    /* "torchqtm/_C/_rolling.pyx":158
  *         nobs[0] = nobs[0] + 1
  *         y = val - compensation[0]
  *         t = sum_x[0] + y             # <<<<<<<<<<<<<<
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t
  */
     __pyx_v_t = ((__pyx_v_sum_x[0]) + __pyx_v_y);
 
-    /* "torchqtm/_C/_rolling.pyx":160
+    /* "torchqtm/_C/_rolling.pyx":159
  *         y = val - compensation[0]
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y             # <<<<<<<<<<<<<<
  *         sum_x[0] = t
  * 
  */
     (__pyx_v_compensation[0]) = ((__pyx_v_t - (__pyx_v_sum_x[0])) - __pyx_v_y);
 
-    /* "torchqtm/_C/_rolling.pyx":161
+    /* "torchqtm/_C/_rolling.pyx":160
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_sum_x[0]) = __pyx_v_t;
 
-    /* "torchqtm/_C/_rolling.pyx":156
+    /* "torchqtm/_C/_rolling.pyx":155
  * 
  *     # Not NaN
  *     if notnan(val):             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] + 1
  *         y = val - compensation[0]
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":148
+  /* "torchqtm/_C/_rolling.pyx":147
  * 
  * 
  * cdef inline void add_sum(float64_t val, int64_t *nobs, float64_t *sum_x,             # <<<<<<<<<<<<<<
  *                          float64_t *compensation) nogil:
  *     """ add a value from the sum calc using Kahan summation """
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":164
+/* "torchqtm/_C/_rolling.pyx":163
  * 
  * 
  * cdef inline void remove_sum(float64_t val, int64_t *nobs, float64_t *sum_x,             # <<<<<<<<<<<<<<
  *                             float64_t *compensation) nogil:
  *     """ remove a value from the sum calc using Kahan summation """
  */
 
 static CYTHON_INLINE void __pyx_f_8torchqtm_2_C_8_rolling_remove_sum(__pyx_t_5numpy_float64_t __pyx_v_val, __pyx_t_5numpy_int64_t *__pyx_v_nobs, __pyx_t_5numpy_float64_t *__pyx_v_sum_x, __pyx_t_5numpy_float64_t *__pyx_v_compensation) {
   __pyx_t_5numpy_float64_t __pyx_v_y;
   __pyx_t_5numpy_float64_t __pyx_v_t;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":172
+  /* "torchqtm/_C/_rolling.pyx":171
  * 
  *     # Not NaN
  *     if notnan(val):             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  *         y = - val - compensation[0]
  */
   __pyx_t_1 = (__pyx_f_8torchqtm_2_C_8_rolling_notnan(__pyx_v_val) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":173
+    /* "torchqtm/_C/_rolling.pyx":172
  *     # Not NaN
  *     if notnan(val):
  *         nobs[0] = nobs[0] - 1             # <<<<<<<<<<<<<<
  *         y = - val - compensation[0]
  *         t = sum_x[0] + y
  */
     (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) - 1);
 
-    /* "torchqtm/_C/_rolling.pyx":174
+    /* "torchqtm/_C/_rolling.pyx":173
  *     if notnan(val):
  *         nobs[0] = nobs[0] - 1
  *         y = - val - compensation[0]             # <<<<<<<<<<<<<<
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y
  */
     __pyx_v_y = ((-__pyx_v_val) - (__pyx_v_compensation[0]));
 
-    /* "torchqtm/_C/_rolling.pyx":175
+    /* "torchqtm/_C/_rolling.pyx":174
  *         nobs[0] = nobs[0] - 1
  *         y = - val - compensation[0]
  *         t = sum_x[0] + y             # <<<<<<<<<<<<<<
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t
  */
     __pyx_v_t = ((__pyx_v_sum_x[0]) + __pyx_v_y);
 
-    /* "torchqtm/_C/_rolling.pyx":176
+    /* "torchqtm/_C/_rolling.pyx":175
  *         y = - val - compensation[0]
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y             # <<<<<<<<<<<<<<
  *         sum_x[0] = t
  * 
  */
     (__pyx_v_compensation[0]) = ((__pyx_v_t - (__pyx_v_sum_x[0])) - __pyx_v_y);
 
-    /* "torchqtm/_C/_rolling.pyx":177
+    /* "torchqtm/_C/_rolling.pyx":176
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_sum_x[0]) = __pyx_v_t;
 
-    /* "torchqtm/_C/_rolling.pyx":172
+    /* "torchqtm/_C/_rolling.pyx":171
  * 
  *     # Not NaN
  *     if notnan(val):             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  *         y = - val - compensation[0]
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":164
+  /* "torchqtm/_C/_rolling.pyx":163
  * 
  * 
  * cdef inline void remove_sum(float64_t val, int64_t *nobs, float64_t *sum_x,             # <<<<<<<<<<<<<<
  *                             float64_t *compensation) nogil:
  *     """ remove a value from the sum calc using Kahan summation """
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":180
+/* "torchqtm/_C/_rolling.pyx":179
  * 
  * 
  * def roll_sum(const float64_t[:] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     cdef:
  */
 
@@ -4668,55 +4685,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_sum", 1, 4, 4, 1); __PYX_ERR(0, 180, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_sum", 1, 4, 4, 1); __PYX_ERR(0, 179, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_sum", 1, 4, 4, 2); __PYX_ERR(0, 180, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_sum", 1, 4, 4, 2); __PYX_ERR(0, 179, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_sum", 1, 4, 4, 3); __PYX_ERR(0, 180, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_sum", 1, 4, 4, 3); __PYX_ERR(0, 179, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_sum") < 0)) __PYX_ERR(0, 180, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_sum") < 0)) __PYX_ERR(0, 179, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
-    __pyx_v_values = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[0], 0); if (unlikely(!__pyx_v_values.memview)) __PYX_ERR(0, 180, __pyx_L3_error)
+    __pyx_v_values = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[0], 0); if (unlikely(!__pyx_v_values.memview)) __PYX_ERR(0, 179, __pyx_L3_error)
     __pyx_v_start = ((PyArrayObject *)values[1]);
     __pyx_v_end = ((PyArrayObject *)values[2]);
-    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_sum", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 180, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_sum", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 179, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_sum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 180, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 181, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 180, __pyx_L1_error)
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_roll_sum(__pyx_self, __pyx_v_values, __pyx_v_start, __pyx_v_end, __pyx_v_minp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4778,77 +4795,77 @@
   __pyx_pybuffernd_start.rcbuffer = &__pyx_pybuffer_start;
   __pyx_pybuffer_end.pybuffer.buf = NULL;
   __pyx_pybuffer_end.refcount = 0;
   __pyx_pybuffernd_end.data = NULL;
   __pyx_pybuffernd_end.rcbuffer = &__pyx_pybuffer_end;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 180, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 179, __pyx_L1_error)
   }
   __pyx_pybuffernd_start.diminfo[0].strides = __pyx_pybuffernd_start.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_start.diminfo[0].shape = __pyx_pybuffernd_start.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 180, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 179, __pyx_L1_error)
   }
   __pyx_pybuffernd_end.diminfo[0].strides = __pyx_pybuffernd_end.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_end.diminfo[0].shape = __pyx_pybuffernd_end.rcbuffer->pybuffer.shape[0];
 
-  /* "torchqtm/_C/_rolling.pyx":186
+  /* "torchqtm/_C/_rolling.pyx":185
  *         float64_t sum_x, compensation_add, compensation_remove
  *         int64_t s, e
  *         int64_t nobs = 0, N = len(start)             # <<<<<<<<<<<<<<
  *         ndarray[float64_t] output
  *         bint is_monotonic_increasing_bounds
  */
   __pyx_v_nobs = 0;
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 185, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":190
+  /* "torchqtm/_C/_rolling.pyx":189
  *         bint is_monotonic_increasing_bounds
  * 
  *     is_monotonic_increasing_bounds = True             # <<<<<<<<<<<<<<
  * 
  *     output = np.empty(N, dtype=np.float64)
  */
   __pyx_v_is_monotonic_increasing_bounds = 1;
 
-  /* "torchqtm/_C/_rolling.pyx":192
+  /* "torchqtm/_C/_rolling.pyx":191
  *     is_monotonic_increasing_bounds = True
  * 
  *     output = np.empty(N, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_npy_int64(__pyx_v_N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_npy_int64(__pyx_v_N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 192, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output.rcbuffer->pybuffer);
     __pyx_t_8 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_8 < 0)) {
       PyErr_Fetch(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
@@ -4857,68 +4874,86 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_9, __pyx_t_10, __pyx_t_11);
       }
       __pyx_t_9 = __pyx_t_10 = __pyx_t_11 = 0;
     }
     __pyx_pybuffernd_output.diminfo[0].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output.diminfo[0].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 191, __pyx_L1_error)
   }
   __pyx_t_7 = 0;
   __pyx_v_output = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":194
+  /* "torchqtm/_C/_rolling.pyx":193
  *     output = np.empty(N, dtype=np.float64)
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  * 
  *         for i in range(0, N):
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "torchqtm/_C/_rolling.pyx":196
+        /* "torchqtm/_C/_rolling.pyx":195
  *     with nogil:
  * 
  *         for i in range(0, N):             # <<<<<<<<<<<<<<
  *             s = start[i]
  *             e = end[i]
  */
         __pyx_t_12 = __pyx_v_N;
         __pyx_t_13 = __pyx_t_12;
         for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_13; __pyx_t_1+=1) {
           __pyx_v_i = __pyx_t_1;
 
-          /* "torchqtm/_C/_rolling.pyx":197
+          /* "torchqtm/_C/_rolling.pyx":196
  * 
  *         for i in range(0, N):
  *             s = start[i]             # <<<<<<<<<<<<<<
  *             e = end[i]
  * 
  */
           __pyx_t_14 = __pyx_v_i;
+          __pyx_t_8 = -1;
+          if (__pyx_t_14 < 0) {
+            __pyx_t_14 += __pyx_pybuffernd_start.diminfo[0].shape;
+            if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+          } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_start.diminfo[0].shape)) __pyx_t_8 = 0;
+          if (unlikely(__pyx_t_8 != -1)) {
+            __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+            __PYX_ERR(0, 196, __pyx_L4_error)
+          }
           __pyx_v_s = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_start.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_start.diminfo[0].strides));
 
-          /* "torchqtm/_C/_rolling.pyx":198
+          /* "torchqtm/_C/_rolling.pyx":197
  *         for i in range(0, N):
  *             s = start[i]
  *             e = end[i]             # <<<<<<<<<<<<<<
  * 
  *             if i == 0 or not is_monotonic_increasing_bounds or s >= end[i - 1]:
  */
           __pyx_t_14 = __pyx_v_i;
+          __pyx_t_8 = -1;
+          if (__pyx_t_14 < 0) {
+            __pyx_t_14 += __pyx_pybuffernd_end.diminfo[0].shape;
+            if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+          } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_end.diminfo[0].shape)) __pyx_t_8 = 0;
+          if (unlikely(__pyx_t_8 != -1)) {
+            __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+            __PYX_ERR(0, 197, __pyx_L4_error)
+          }
           __pyx_v_e = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_end.diminfo[0].strides));
 
-          /* "torchqtm/_C/_rolling.pyx":200
+          /* "torchqtm/_C/_rolling.pyx":199
  *             e = end[i]
  * 
  *             if i == 0 or not is_monotonic_increasing_bounds or s >= end[i - 1]:             # <<<<<<<<<<<<<<
  * 
  *                 # setup
  */
           __pyx_t_16 = ((__pyx_v_i == 0) != 0);
@@ -4930,213 +4965,283 @@
           __pyx_t_16 = ((!(__pyx_v_is_monotonic_increasing_bounds != 0)) != 0);
           if (!__pyx_t_16) {
           } else {
             __pyx_t_15 = __pyx_t_16;
             goto __pyx_L9_bool_binop_done;
           }
           __pyx_t_14 = (__pyx_v_i - 1);
+          __pyx_t_8 = -1;
+          if (__pyx_t_14 < 0) {
+            __pyx_t_14 += __pyx_pybuffernd_end.diminfo[0].shape;
+            if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+          } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_end.diminfo[0].shape)) __pyx_t_8 = 0;
+          if (unlikely(__pyx_t_8 != -1)) {
+            __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+            __PYX_ERR(0, 199, __pyx_L4_error)
+          }
           __pyx_t_16 = ((__pyx_v_s >= (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_end.diminfo[0].strides))) != 0);
           __pyx_t_15 = __pyx_t_16;
           __pyx_L9_bool_binop_done:;
           if (__pyx_t_15) {
 
-            /* "torchqtm/_C/_rolling.pyx":204
+            /* "torchqtm/_C/_rolling.pyx":203
  *                 # setup
  * 
  *                 sum_x = compensation_add = compensation_remove = 0             # <<<<<<<<<<<<<<
  *                 nobs = 0
  *                 for j in range(s, e):
  */
             __pyx_v_sum_x = 0.0;
             __pyx_v_compensation_add = 0.0;
             __pyx_v_compensation_remove = 0.0;
 
-            /* "torchqtm/_C/_rolling.pyx":205
+            /* "torchqtm/_C/_rolling.pyx":204
  * 
  *                 sum_x = compensation_add = compensation_remove = 0
  *                 nobs = 0             # <<<<<<<<<<<<<<
  *                 for j in range(s, e):
  *                     add_sum(values[j], &nobs, &sum_x, &compensation_add)
  */
             __pyx_v_nobs = 0;
 
-            /* "torchqtm/_C/_rolling.pyx":206
+            /* "torchqtm/_C/_rolling.pyx":205
  *                 sum_x = compensation_add = compensation_remove = 0
  *                 nobs = 0
  *                 for j in range(s, e):             # <<<<<<<<<<<<<<
  *                     add_sum(values[j], &nobs, &sum_x, &compensation_add)
  * 
  */
             __pyx_t_17 = __pyx_v_e;
             __pyx_t_18 = __pyx_t_17;
             for (__pyx_t_19 = __pyx_v_s; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
               __pyx_v_j = __pyx_t_19;
 
-              /* "torchqtm/_C/_rolling.pyx":207
+              /* "torchqtm/_C/_rolling.pyx":206
  *                 nobs = 0
  *                 for j in range(s, e):
  *                     add_sum(values[j], &nobs, &sum_x, &compensation_add)             # <<<<<<<<<<<<<<
  * 
  *             else:
  */
               __pyx_t_14 = __pyx_v_j;
+              __pyx_t_8 = -1;
+              if (__pyx_t_14 < 0) {
+                __pyx_t_14 += __pyx_v_values.shape[0];
+                if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+              } else if (unlikely(__pyx_t_14 >= __pyx_v_values.shape[0])) __pyx_t_8 = 0;
+              if (unlikely(__pyx_t_8 != -1)) {
+                __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                __PYX_ERR(0, 206, __pyx_L4_error)
+              }
               __pyx_f_8torchqtm_2_C_8_rolling_add_sum((*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_values.data + __pyx_t_14 * __pyx_v_values.strides[0]) ))), (&__pyx_v_nobs), (&__pyx_v_sum_x), (&__pyx_v_compensation_add));
             }
 
-            /* "torchqtm/_C/_rolling.pyx":200
+            /* "torchqtm/_C/_rolling.pyx":199
  *             e = end[i]
  * 
  *             if i == 0 or not is_monotonic_increasing_bounds or s >= end[i - 1]:             # <<<<<<<<<<<<<<
  * 
  *                 # setup
  */
             goto __pyx_L8;
           }
 
-          /* "torchqtm/_C/_rolling.pyx":212
+          /* "torchqtm/_C/_rolling.pyx":211
  * 
  *                 # calculate deletes
  *                 for j in range(start[i - 1], s):             # <<<<<<<<<<<<<<
  *                     remove_sum(values[j], &nobs, &sum_x, &compensation_remove)
  * 
  */
           /*else*/ {
             __pyx_t_17 = __pyx_v_s;
             __pyx_t_14 = (__pyx_v_i - 1);
+            __pyx_t_8 = -1;
+            if (__pyx_t_14 < 0) {
+              __pyx_t_14 += __pyx_pybuffernd_start.diminfo[0].shape;
+              if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_start.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 211, __pyx_L4_error)
+            }
             __pyx_t_18 = __pyx_t_17;
             for (__pyx_t_19 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_start.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_start.diminfo[0].strides)); __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
               __pyx_v_j = __pyx_t_19;
 
-              /* "torchqtm/_C/_rolling.pyx":213
+              /* "torchqtm/_C/_rolling.pyx":212
  *                 # calculate deletes
  *                 for j in range(start[i - 1], s):
  *                     remove_sum(values[j], &nobs, &sum_x, &compensation_remove)             # <<<<<<<<<<<<<<
  * 
  *                 # calculate adds
  */
               __pyx_t_20 = __pyx_v_j;
+              __pyx_t_8 = -1;
+              if (__pyx_t_20 < 0) {
+                __pyx_t_20 += __pyx_v_values.shape[0];
+                if (unlikely(__pyx_t_20 < 0)) __pyx_t_8 = 0;
+              } else if (unlikely(__pyx_t_20 >= __pyx_v_values.shape[0])) __pyx_t_8 = 0;
+              if (unlikely(__pyx_t_8 != -1)) {
+                __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                __PYX_ERR(0, 212, __pyx_L4_error)
+              }
               __pyx_f_8torchqtm_2_C_8_rolling_remove_sum((*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_values.data + __pyx_t_20 * __pyx_v_values.strides[0]) ))), (&__pyx_v_nobs), (&__pyx_v_sum_x), (&__pyx_v_compensation_remove));
             }
 
-            /* "torchqtm/_C/_rolling.pyx":216
+            /* "torchqtm/_C/_rolling.pyx":215
  * 
  *                 # calculate adds
  *                 for j in range(end[i - 1], e):             # <<<<<<<<<<<<<<
  *                     add_sum(values[j], &nobs, &sum_x, &compensation_add)
  * 
  */
             __pyx_t_17 = __pyx_v_e;
             __pyx_t_14 = (__pyx_v_i - 1);
+            __pyx_t_8 = -1;
+            if (__pyx_t_14 < 0) {
+              __pyx_t_14 += __pyx_pybuffernd_end.diminfo[0].shape;
+              if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_end.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 215, __pyx_L4_error)
+            }
             __pyx_t_18 = __pyx_t_17;
             for (__pyx_t_19 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_end.diminfo[0].strides)); __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
               __pyx_v_j = __pyx_t_19;
 
-              /* "torchqtm/_C/_rolling.pyx":217
+              /* "torchqtm/_C/_rolling.pyx":216
  *                 # calculate adds
  *                 for j in range(end[i - 1], e):
  *                     add_sum(values[j], &nobs, &sum_x, &compensation_add)             # <<<<<<<<<<<<<<
  * 
  *             output[i] = calc_sum(minp, nobs, sum_x)
  */
               __pyx_t_20 = __pyx_v_j;
+              __pyx_t_8 = -1;
+              if (__pyx_t_20 < 0) {
+                __pyx_t_20 += __pyx_v_values.shape[0];
+                if (unlikely(__pyx_t_20 < 0)) __pyx_t_8 = 0;
+              } else if (unlikely(__pyx_t_20 >= __pyx_v_values.shape[0])) __pyx_t_8 = 0;
+              if (unlikely(__pyx_t_8 != -1)) {
+                __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                __PYX_ERR(0, 216, __pyx_L4_error)
+              }
               __pyx_f_8torchqtm_2_C_8_rolling_add_sum((*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_values.data + __pyx_t_20 * __pyx_v_values.strides[0]) ))), (&__pyx_v_nobs), (&__pyx_v_sum_x), (&__pyx_v_compensation_add));
             }
           }
           __pyx_L8:;
 
-          /* "torchqtm/_C/_rolling.pyx":219
+          /* "torchqtm/_C/_rolling.pyx":218
  *                     add_sum(values[j], &nobs, &sum_x, &compensation_add)
  * 
  *             output[i] = calc_sum(minp, nobs, sum_x)             # <<<<<<<<<<<<<<
  * 
  *             if not is_monotonic_increasing_bounds:
  */
           __pyx_t_14 = __pyx_v_i;
+          __pyx_t_8 = -1;
+          if (__pyx_t_14 < 0) {
+            __pyx_t_14 += __pyx_pybuffernd_output.diminfo[0].shape;
+            if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+          } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_output.diminfo[0].shape)) __pyx_t_8 = 0;
+          if (unlikely(__pyx_t_8 != -1)) {
+            __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+            __PYX_ERR(0, 218, __pyx_L4_error)
+          }
           *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_output.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_output.diminfo[0].strides) = __pyx_f_8torchqtm_2_C_8_rolling_calc_sum(__pyx_v_minp, __pyx_v_nobs, __pyx_v_sum_x);
 
-          /* "torchqtm/_C/_rolling.pyx":221
+          /* "torchqtm/_C/_rolling.pyx":220
  *             output[i] = calc_sum(minp, nobs, sum_x)
  * 
  *             if not is_monotonic_increasing_bounds:             # <<<<<<<<<<<<<<
  *                 nobs = 0
  *                 sum_x = 0.0
  */
           __pyx_t_15 = ((!(__pyx_v_is_monotonic_increasing_bounds != 0)) != 0);
           if (__pyx_t_15) {
 
-            /* "torchqtm/_C/_rolling.pyx":222
+            /* "torchqtm/_C/_rolling.pyx":221
  * 
  *             if not is_monotonic_increasing_bounds:
  *                 nobs = 0             # <<<<<<<<<<<<<<
  *                 sum_x = 0.0
  *                 compensation_remove = 0.0
  */
             __pyx_v_nobs = 0;
 
-            /* "torchqtm/_C/_rolling.pyx":223
+            /* "torchqtm/_C/_rolling.pyx":222
  *             if not is_monotonic_increasing_bounds:
  *                 nobs = 0
  *                 sum_x = 0.0             # <<<<<<<<<<<<<<
  *                 compensation_remove = 0.0
  * 
  */
             __pyx_v_sum_x = 0.0;
 
-            /* "torchqtm/_C/_rolling.pyx":224
+            /* "torchqtm/_C/_rolling.pyx":223
  *                 nobs = 0
  *                 sum_x = 0.0
  *                 compensation_remove = 0.0             # <<<<<<<<<<<<<<
  * 
  *     return output
  */
             __pyx_v_compensation_remove = 0.0;
 
-            /* "torchqtm/_C/_rolling.pyx":221
+            /* "torchqtm/_C/_rolling.pyx":220
  *             output[i] = calc_sum(minp, nobs, sum_x)
  * 
  *             if not is_monotonic_increasing_bounds:             # <<<<<<<<<<<<<<
  *                 nobs = 0
  *                 sum_x = 0.0
  */
           }
         }
       }
 
-      /* "torchqtm/_C/_rolling.pyx":194
+      /* "torchqtm/_C/_rolling.pyx":193
  *     output = np.empty(N, dtype=np.float64)
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  * 
  *         for i in range(0, N):
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
           __Pyx_FastGIL_Forget();
           Py_BLOCK_THREADS
           #endif
           goto __pyx_L5;
         }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L1_error;
+        }
         __pyx_L5:;
       }
   }
 
-  /* "torchqtm/_C/_rolling.pyx":226
+  /* "torchqtm/_C/_rolling.pyx":225
  *                 compensation_remove = 0.0
  * 
  *     return output             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_output));
   __pyx_r = ((PyObject *)__pyx_v_output);
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":180
+  /* "torchqtm/_C/_rolling.pyx":179
  * 
  * 
  * def roll_sum(const float64_t[:] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     cdef:
  */
 
@@ -5166,15 +5271,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_output);
   __PYX_XDEC_MEMVIEW(&__pyx_v_values, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":229
+/* "torchqtm/_C/_rolling.pyx":228
  * 
  * 
  * def roll_max(ndarray[float64_t] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     """
  */
 
@@ -5216,56 +5321,56 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_max", 1, 4, 4, 1); __PYX_ERR(0, 229, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_max", 1, 4, 4, 1); __PYX_ERR(0, 228, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_max", 1, 4, 4, 2); __PYX_ERR(0, 229, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_max", 1, 4, 4, 2); __PYX_ERR(0, 228, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_max", 1, 4, 4, 3); __PYX_ERR(0, 229, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_max", 1, 4, 4, 3); __PYX_ERR(0, 228, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_max") < 0)) __PYX_ERR(0, 229, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_max") < 0)) __PYX_ERR(0, 228, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_values = ((PyArrayObject *)values[0]);
     __pyx_v_start = ((PyArrayObject *)values[1]);
     __pyx_v_end = ((PyArrayObject *)values[2]);
-    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 229, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_max", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 229, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_max", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 228, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_max", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_values), __pyx_ptype_5numpy_ndarray, 1, "values", 0))) __PYX_ERR(0, 229, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 229, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 230, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_values), __pyx_ptype_5numpy_ndarray, 1, "values", 0))) __PYX_ERR(0, 228, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 228, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 229, __pyx_L1_error)
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_2roll_max(__pyx_self, __pyx_v_values, __pyx_v_start, __pyx_v_end, __pyx_v_minp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5297,43 +5402,43 @@
   __pyx_pybuffernd_start.rcbuffer = &__pyx_pybuffer_start;
   __pyx_pybuffer_end.pybuffer.buf = NULL;
   __pyx_pybuffer_end.refcount = 0;
   __pyx_pybuffernd_end.data = NULL;
   __pyx_pybuffernd_end.rcbuffer = &__pyx_pybuffer_end;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 229, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 228, __pyx_L1_error)
   }
   __pyx_pybuffernd_values.diminfo[0].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_values.diminfo[0].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 229, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 228, __pyx_L1_error)
   }
   __pyx_pybuffernd_start.diminfo[0].strides = __pyx_pybuffernd_start.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_start.diminfo[0].shape = __pyx_pybuffernd_start.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 229, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 228, __pyx_L1_error)
   }
   __pyx_pybuffernd_end.diminfo[0].strides = __pyx_pybuffernd_end.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_end.diminfo[0].shape = __pyx_pybuffernd_end.rcbuffer->pybuffer.shape[0];
 
-  /* "torchqtm/_C/_rolling.pyx":250
+  /* "torchqtm/_C/_rolling.pyx":249
  *     np.ndarray[float]
  *     """
  *     return _roll_min_max(values, start, end, minp, is_max=1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling__roll_min_max(((PyArrayObject *)__pyx_v_values), ((PyArrayObject *)__pyx_v_start), ((PyArrayObject *)__pyx_v_end), __pyx_v_minp, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_1 = __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling__roll_min_max(((PyArrayObject *)__pyx_v_values), ((PyArrayObject *)__pyx_v_start), ((PyArrayObject *)__pyx_v_end), __pyx_v_minp, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":229
+  /* "torchqtm/_C/_rolling.pyx":228
  * 
  * 
  * def roll_max(ndarray[float64_t] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     """
  */
 
@@ -5357,15 +5462,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_values.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":253
+/* "torchqtm/_C/_rolling.pyx":252
  * 
  * 
  * def roll_min(ndarray[float64_t] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     """
  */
 
@@ -5407,56 +5512,56 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_min", 1, 4, 4, 1); __PYX_ERR(0, 253, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_min", 1, 4, 4, 1); __PYX_ERR(0, 252, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_min", 1, 4, 4, 2); __PYX_ERR(0, 253, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_min", 1, 4, 4, 2); __PYX_ERR(0, 252, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_min", 1, 4, 4, 3); __PYX_ERR(0, 253, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_min", 1, 4, 4, 3); __PYX_ERR(0, 252, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_min") < 0)) __PYX_ERR(0, 253, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_min") < 0)) __PYX_ERR(0, 252, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_values = ((PyArrayObject *)values[0]);
     __pyx_v_start = ((PyArrayObject *)values[1]);
     __pyx_v_end = ((PyArrayObject *)values[2]);
-    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 254, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_min", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 253, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_min", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 252, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_min", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_values), __pyx_ptype_5numpy_ndarray, 1, "values", 0))) __PYX_ERR(0, 253, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 253, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 254, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_values), __pyx_ptype_5numpy_ndarray, 1, "values", 0))) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 253, __pyx_L1_error)
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_4roll_min(__pyx_self, __pyx_v_values, __pyx_v_start, __pyx_v_end, __pyx_v_minp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5488,43 +5593,43 @@
   __pyx_pybuffernd_start.rcbuffer = &__pyx_pybuffer_start;
   __pyx_pybuffer_end.pybuffer.buf = NULL;
   __pyx_pybuffer_end.refcount = 0;
   __pyx_pybuffernd_end.data = NULL;
   __pyx_pybuffernd_end.rcbuffer = &__pyx_pybuffer_end;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 253, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 252, __pyx_L1_error)
   }
   __pyx_pybuffernd_values.diminfo[0].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_values.diminfo[0].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 253, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 252, __pyx_L1_error)
   }
   __pyx_pybuffernd_start.diminfo[0].strides = __pyx_pybuffernd_start.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_start.diminfo[0].shape = __pyx_pybuffernd_start.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 253, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 252, __pyx_L1_error)
   }
   __pyx_pybuffernd_end.diminfo[0].strides = __pyx_pybuffernd_end.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_end.diminfo[0].shape = __pyx_pybuffernd_end.rcbuffer->pybuffer.shape[0];
 
-  /* "torchqtm/_C/_rolling.pyx":271
+  /* "torchqtm/_C/_rolling.pyx":270
  *     np.ndarray[float]
  *     """
  *     return _roll_min_max(values, start, end, minp, is_max=0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling__roll_min_max(((PyArrayObject *)__pyx_v_values), ((PyArrayObject *)__pyx_v_start), ((PyArrayObject *)__pyx_v_end), __pyx_v_minp, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_1 = __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling__roll_min_max(((PyArrayObject *)__pyx_v_values), ((PyArrayObject *)__pyx_v_start), ((PyArrayObject *)__pyx_v_end), __pyx_v_minp, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":253
+  /* "torchqtm/_C/_rolling.pyx":252
  * 
  * 
  * def roll_min(ndarray[float64_t] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     """
  */
 
@@ -5548,15 +5653,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_values.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":274
+/* "torchqtm/_C/_rolling.pyx":273
  * 
  * 
  * cdef _roll_min_max(ndarray[numeric_t] values,             # <<<<<<<<<<<<<<
  *                    ndarray[int64_t] starti,
  *                    ndarray[int64_t] endi,
  */
 
@@ -5622,73 +5727,73 @@
   __pyx_pybuffernd_starti.rcbuffer = &__pyx_pybuffer_starti;
   __pyx_pybuffer_endi.pybuffer.buf = NULL;
   __pyx_pybuffer_endi.refcount = 0;
   __pyx_pybuffernd_endi.data = NULL;
   __pyx_pybuffernd_endi.rcbuffer = &__pyx_pybuffer_endi;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 274, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 273, __pyx_L1_error)
   }
   __pyx_pybuffernd_values.diminfo[0].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_values.diminfo[0].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_starti.rcbuffer->pybuffer, (PyObject*)__pyx_v_starti, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 274, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_starti.rcbuffer->pybuffer, (PyObject*)__pyx_v_starti, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 273, __pyx_L1_error)
   }
   __pyx_pybuffernd_starti.diminfo[0].strides = __pyx_pybuffernd_starti.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_starti.diminfo[0].shape = __pyx_pybuffernd_starti.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_endi.rcbuffer->pybuffer, (PyObject*)__pyx_v_endi, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 274, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_endi.rcbuffer->pybuffer, (PyObject*)__pyx_v_endi, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 273, __pyx_L1_error)
   }
   __pyx_pybuffernd_endi.diminfo[0].strides = __pyx_pybuffernd_endi.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_endi.diminfo[0].shape = __pyx_pybuffernd_endi.rcbuffer->pybuffer.shape[0];
 
-  /* "torchqtm/_C/_rolling.pyx":282
+  /* "torchqtm/_C/_rolling.pyx":281
  *         numeric_t ai
  *         int64_t curr_win_size, start
  *         Py_ssize_t i, k, nobs = 0, N = len(starti)             # <<<<<<<<<<<<<<
  *         deque Q[int64_t]  # min/max always the front
  *         deque W[int64_t]  # track the whole window for nobs compute
  */
   __pyx_v_nobs = 0;
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_starti)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_starti)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":287
+  /* "torchqtm/_C/_rolling.pyx":286
  *         ndarray[float64_t, ndim=1] output
  * 
  *     output = np.empty(N, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     Q = deque[int64_t]()
  *     W = deque[int64_t]()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 287, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 286, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output.rcbuffer->pybuffer);
     __pyx_t_8 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_8 < 0)) {
       PyErr_Fetch(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
@@ -5697,232 +5802,331 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_9, __pyx_t_10, __pyx_t_11);
       }
       __pyx_t_9 = __pyx_t_10 = __pyx_t_11 = 0;
     }
     __pyx_pybuffernd_output.diminfo[0].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output.diminfo[0].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 287, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 286, __pyx_L1_error)
   }
   __pyx_t_7 = 0;
   __pyx_v_output = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":288
+  /* "torchqtm/_C/_rolling.pyx":287
  * 
  *     output = np.empty(N, dtype=np.float64)
  *     Q = deque[int64_t]()             # <<<<<<<<<<<<<<
  *     W = deque[int64_t]()
  * 
  */
   try {
     __pyx_t_12 = std::deque<__pyx_t_5numpy_int64_t> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 288, __pyx_L1_error)
+    __PYX_ERR(0, 287, __pyx_L1_error)
   }
   __pyx_v_Q = __pyx_t_12;
 
-  /* "torchqtm/_C/_rolling.pyx":289
+  /* "torchqtm/_C/_rolling.pyx":288
  *     output = np.empty(N, dtype=np.float64)
  *     Q = deque[int64_t]()
  *     W = deque[int64_t]()             # <<<<<<<<<<<<<<
  * 
  *     with nogil:
  */
   try {
     __pyx_t_12 = std::deque<__pyx_t_5numpy_int64_t> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 289, __pyx_L1_error)
+    __PYX_ERR(0, 288, __pyx_L1_error)
   }
   __pyx_v_W = __pyx_t_12;
 
-  /* "torchqtm/_C/_rolling.pyx":291
+  /* "torchqtm/_C/_rolling.pyx":290
  *     W = deque[int64_t]()
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  * 
  *         # This is using a modified version of the C++ code in this
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "torchqtm/_C/_rolling.pyx":299
+        /* "torchqtm/_C/_rolling.pyx":298
  * 
  *         # first window's size
  *         curr_win_size = endi[0] - starti[0]             # <<<<<<<<<<<<<<
  *         # GH 32865
  *         # Anchor output index to values index to provide custom
  */
         __pyx_t_13 = 0;
+        __pyx_t_8 = -1;
+        if (__pyx_t_13 < 0) {
+          __pyx_t_13 += __pyx_pybuffernd_endi.diminfo[0].shape;
+          if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+        } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_endi.diminfo[0].shape)) __pyx_t_8 = 0;
+        if (unlikely(__pyx_t_8 != -1)) {
+          __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+          __PYX_ERR(0, 298, __pyx_L4_error)
+        }
         __pyx_t_14 = 0;
+        __pyx_t_8 = -1;
+        if (__pyx_t_14 < 0) {
+          __pyx_t_14 += __pyx_pybuffernd_starti.diminfo[0].shape;
+          if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+        } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_starti.diminfo[0].shape)) __pyx_t_8 = 0;
+        if (unlikely(__pyx_t_8 != -1)) {
+          __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+          __PYX_ERR(0, 298, __pyx_L4_error)
+        }
         __pyx_v_curr_win_size = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_endi.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_endi.diminfo[0].strides)) - (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_starti.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_starti.diminfo[0].strides)));
 
-        /* "torchqtm/_C/_rolling.pyx":303
+        /* "torchqtm/_C/_rolling.pyx":302
  *         # Anchor output index to values index to provide custom
  *         # BaseIndexer support
  *         for i in range(N):             # <<<<<<<<<<<<<<
  * 
  *             curr_win_size = endi[i] - starti[i]
  */
         __pyx_t_1 = __pyx_v_N;
         __pyx_t_15 = __pyx_t_1;
         for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
           __pyx_v_i = __pyx_t_16;
 
-          /* "torchqtm/_C/_rolling.pyx":305
+          /* "torchqtm/_C/_rolling.pyx":304
  *         for i in range(N):
  * 
  *             curr_win_size = endi[i] - starti[i]             # <<<<<<<<<<<<<<
  *             if i == 0:
  *                 start = starti[i]
  */
           __pyx_t_14 = __pyx_v_i;
+          __pyx_t_8 = -1;
+          if (__pyx_t_14 < 0) {
+            __pyx_t_14 += __pyx_pybuffernd_endi.diminfo[0].shape;
+            if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
+          } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_endi.diminfo[0].shape)) __pyx_t_8 = 0;
+          if (unlikely(__pyx_t_8 != -1)) {
+            __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+            __PYX_ERR(0, 304, __pyx_L4_error)
+          }
           __pyx_t_13 = __pyx_v_i;
+          __pyx_t_8 = -1;
+          if (__pyx_t_13 < 0) {
+            __pyx_t_13 += __pyx_pybuffernd_starti.diminfo[0].shape;
+            if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+          } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_starti.diminfo[0].shape)) __pyx_t_8 = 0;
+          if (unlikely(__pyx_t_8 != -1)) {
+            __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+            __PYX_ERR(0, 304, __pyx_L4_error)
+          }
           __pyx_v_curr_win_size = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_endi.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_endi.diminfo[0].strides)) - (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_starti.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_starti.diminfo[0].strides)));
 
-          /* "torchqtm/_C/_rolling.pyx":306
+          /* "torchqtm/_C/_rolling.pyx":305
  * 
  *             curr_win_size = endi[i] - starti[i]
  *             if i == 0:             # <<<<<<<<<<<<<<
  *                 start = starti[i]
  *             else:
  */
           __pyx_t_17 = ((__pyx_v_i == 0) != 0);
           if (__pyx_t_17) {
 
-            /* "torchqtm/_C/_rolling.pyx":307
+            /* "torchqtm/_C/_rolling.pyx":306
  *             curr_win_size = endi[i] - starti[i]
  *             if i == 0:
  *                 start = starti[i]             # <<<<<<<<<<<<<<
  *             else:
  *                 start = endi[i - 1]
  */
             __pyx_t_13 = __pyx_v_i;
+            __pyx_t_8 = -1;
+            if (__pyx_t_13 < 0) {
+              __pyx_t_13 += __pyx_pybuffernd_starti.diminfo[0].shape;
+              if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_starti.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 306, __pyx_L4_error)
+            }
             __pyx_v_start = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_starti.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_starti.diminfo[0].strides));
 
-            /* "torchqtm/_C/_rolling.pyx":306
+            /* "torchqtm/_C/_rolling.pyx":305
  * 
  *             curr_win_size = endi[i] - starti[i]
  *             if i == 0:             # <<<<<<<<<<<<<<
  *                 start = starti[i]
  *             else:
  */
             goto __pyx_L8;
           }
 
-          /* "torchqtm/_C/_rolling.pyx":309
+          /* "torchqtm/_C/_rolling.pyx":308
  *                 start = starti[i]
  *             else:
  *                 start = endi[i - 1]             # <<<<<<<<<<<<<<
  * 
  *             for k in range(start, endi[i]):
  */
           /*else*/ {
             __pyx_t_13 = (__pyx_v_i - 1);
+            __pyx_t_8 = -1;
+            if (__pyx_t_13 < 0) {
+              __pyx_t_13 += __pyx_pybuffernd_endi.diminfo[0].shape;
+              if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_endi.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 308, __pyx_L4_error)
+            }
             __pyx_v_start = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_endi.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_endi.diminfo[0].strides));
           }
           __pyx_L8:;
 
-          /* "torchqtm/_C/_rolling.pyx":311
+          /* "torchqtm/_C/_rolling.pyx":310
  *                 start = endi[i - 1]
  * 
  *             for k in range(start, endi[i]):             # <<<<<<<<<<<<<<
  *                 ai = init_mm(values[k], &nobs, is_max)
  *                 # Discard previous entries if we find new min or max
  */
           __pyx_t_13 = __pyx_v_i;
+          __pyx_t_8 = -1;
+          if (__pyx_t_13 < 0) {
+            __pyx_t_13 += __pyx_pybuffernd_endi.diminfo[0].shape;
+            if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+          } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_endi.diminfo[0].shape)) __pyx_t_8 = 0;
+          if (unlikely(__pyx_t_8 != -1)) {
+            __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+            __PYX_ERR(0, 310, __pyx_L4_error)
+          }
           __pyx_t_18 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_endi.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_endi.diminfo[0].strides));
           __pyx_t_19 = __pyx_t_18;
           for (__pyx_t_20 = __pyx_v_start; __pyx_t_20 < __pyx_t_19; __pyx_t_20+=1) {
             __pyx_v_k = __pyx_t_20;
 
-            /* "torchqtm/_C/_rolling.pyx":312
+            /* "torchqtm/_C/_rolling.pyx":311
  * 
  *             for k in range(start, endi[i]):
  *                 ai = init_mm(values[k], &nobs, is_max)             # <<<<<<<<<<<<<<
  *                 # Discard previous entries if we find new min or max
  *                 if is_max:
  */
             __pyx_t_13 = __pyx_v_k;
+            __pyx_t_8 = -1;
+            if (__pyx_t_13 < 0) {
+              __pyx_t_13 += __pyx_pybuffernd_values.diminfo[0].shape;
+              if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 311, __pyx_L4_error)
+            }
             __pyx_v_ai = __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling_init_mm((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_values.diminfo[0].strides)), (&__pyx_v_nobs), __pyx_v_is_max);
 
-            /* "torchqtm/_C/_rolling.pyx":314
+            /* "torchqtm/_C/_rolling.pyx":313
  *                 ai = init_mm(values[k], &nobs, is_max)
  *                 # Discard previous entries if we find new min or max
  *                 if is_max:             # <<<<<<<<<<<<<<
  *                     while not Q.empty() and ((ai >= values[Q.back()]) or
  *                                              values[Q.back()] != values[Q.back()]):
  */
             __pyx_t_17 = (__pyx_v_is_max != 0);
             if (__pyx_t_17) {
 
-              /* "torchqtm/_C/_rolling.pyx":315
+              /* "torchqtm/_C/_rolling.pyx":314
  *                 # Discard previous entries if we find new min or max
  *                 if is_max:
  *                     while not Q.empty() and ((ai >= values[Q.back()]) or             # <<<<<<<<<<<<<<
  *                                              values[Q.back()] != values[Q.back()]):
  *                         Q.pop_back()
  */
               while (1) {
                 __pyx_t_21 = ((!(__pyx_v_Q.empty() != 0)) != 0);
                 if (__pyx_t_21) {
                 } else {
                   __pyx_t_17 = __pyx_t_21;
                   goto __pyx_L14_bool_binop_done;
                 }
                 __pyx_t_22 = __pyx_v_Q.back();
+                __pyx_t_8 = -1;
+                if (__pyx_t_22 < 0) {
+                  __pyx_t_22 += __pyx_pybuffernd_values.diminfo[0].shape;
+                  if (unlikely(__pyx_t_22 < 0)) __pyx_t_8 = 0;
+                } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+                if (unlikely(__pyx_t_8 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                  __PYX_ERR(0, 314, __pyx_L4_error)
+                }
                 __pyx_t_21 = ((__pyx_v_ai >= (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_values.diminfo[0].strides))) != 0);
                 if (!__pyx_t_21) {
                 } else {
                   __pyx_t_17 = __pyx_t_21;
                   goto __pyx_L14_bool_binop_done;
                 }
 
-                /* "torchqtm/_C/_rolling.pyx":316
+                /* "torchqtm/_C/_rolling.pyx":315
  *                 if is_max:
  *                     while not Q.empty() and ((ai >= values[Q.back()]) or
  *                                              values[Q.back()] != values[Q.back()]):             # <<<<<<<<<<<<<<
  *                         Q.pop_back()
  *                 else:
  */
                 __pyx_t_22 = __pyx_v_Q.back();
+                __pyx_t_8 = -1;
+                if (__pyx_t_22 < 0) {
+                  __pyx_t_22 += __pyx_pybuffernd_values.diminfo[0].shape;
+                  if (unlikely(__pyx_t_22 < 0)) __pyx_t_8 = 0;
+                } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+                if (unlikely(__pyx_t_8 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                  __PYX_ERR(0, 315, __pyx_L4_error)
+                }
                 __pyx_t_23 = __pyx_v_Q.back();
+                __pyx_t_8 = -1;
+                if (__pyx_t_23 < 0) {
+                  __pyx_t_23 += __pyx_pybuffernd_values.diminfo[0].shape;
+                  if (unlikely(__pyx_t_23 < 0)) __pyx_t_8 = 0;
+                } else if (unlikely(__pyx_t_23 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+                if (unlikely(__pyx_t_8 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                  __PYX_ERR(0, 315, __pyx_L4_error)
+                }
                 __pyx_t_21 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_values.diminfo[0].strides)) != (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_23, __pyx_pybuffernd_values.diminfo[0].strides))) != 0);
                 __pyx_t_17 = __pyx_t_21;
                 __pyx_L14_bool_binop_done:;
                 if (!__pyx_t_17) break;
 
-                /* "torchqtm/_C/_rolling.pyx":317
+                /* "torchqtm/_C/_rolling.pyx":316
  *                     while not Q.empty() and ((ai >= values[Q.back()]) or
  *                                              values[Q.back()] != values[Q.back()]):
  *                         Q.pop_back()             # <<<<<<<<<<<<<<
  *                 else:
  *                     while not Q.empty() and ((ai <= values[Q.back()]) or
  */
                 __pyx_v_Q.pop_back();
               }
 
-              /* "torchqtm/_C/_rolling.pyx":314
+              /* "torchqtm/_C/_rolling.pyx":313
  *                 ai = init_mm(values[k], &nobs, is_max)
  *                 # Discard previous entries if we find new min or max
  *                 if is_max:             # <<<<<<<<<<<<<<
  *                     while not Q.empty() and ((ai >= values[Q.back()]) or
  *                                              values[Q.back()] != values[Q.back()]):
  */
               goto __pyx_L11;
             }
 
-            /* "torchqtm/_C/_rolling.pyx":319
+            /* "torchqtm/_C/_rolling.pyx":318
  *                         Q.pop_back()
  *                 else:
  *                     while not Q.empty() and ((ai <= values[Q.back()]) or             # <<<<<<<<<<<<<<
  *                                              values[Q.back()] != values[Q.back()]):
  *                         Q.pop_back()
  */
             /*else*/ {
@@ -5930,137 +6134,191 @@
                 __pyx_t_21 = ((!(__pyx_v_Q.empty() != 0)) != 0);
                 if (__pyx_t_21) {
                 } else {
                   __pyx_t_17 = __pyx_t_21;
                   goto __pyx_L19_bool_binop_done;
                 }
                 __pyx_t_23 = __pyx_v_Q.back();
+                __pyx_t_8 = -1;
+                if (__pyx_t_23 < 0) {
+                  __pyx_t_23 += __pyx_pybuffernd_values.diminfo[0].shape;
+                  if (unlikely(__pyx_t_23 < 0)) __pyx_t_8 = 0;
+                } else if (unlikely(__pyx_t_23 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+                if (unlikely(__pyx_t_8 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                  __PYX_ERR(0, 318, __pyx_L4_error)
+                }
                 __pyx_t_21 = ((__pyx_v_ai <= (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_23, __pyx_pybuffernd_values.diminfo[0].strides))) != 0);
                 if (!__pyx_t_21) {
                 } else {
                   __pyx_t_17 = __pyx_t_21;
                   goto __pyx_L19_bool_binop_done;
                 }
 
-                /* "torchqtm/_C/_rolling.pyx":320
+                /* "torchqtm/_C/_rolling.pyx":319
  *                 else:
  *                     while not Q.empty() and ((ai <= values[Q.back()]) or
  *                                              values[Q.back()] != values[Q.back()]):             # <<<<<<<<<<<<<<
  *                         Q.pop_back()
  *                 Q.push_back(k)
  */
                 __pyx_t_23 = __pyx_v_Q.back();
+                __pyx_t_8 = -1;
+                if (__pyx_t_23 < 0) {
+                  __pyx_t_23 += __pyx_pybuffernd_values.diminfo[0].shape;
+                  if (unlikely(__pyx_t_23 < 0)) __pyx_t_8 = 0;
+                } else if (unlikely(__pyx_t_23 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+                if (unlikely(__pyx_t_8 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                  __PYX_ERR(0, 319, __pyx_L4_error)
+                }
                 __pyx_t_22 = __pyx_v_Q.back();
+                __pyx_t_8 = -1;
+                if (__pyx_t_22 < 0) {
+                  __pyx_t_22 += __pyx_pybuffernd_values.diminfo[0].shape;
+                  if (unlikely(__pyx_t_22 < 0)) __pyx_t_8 = 0;
+                } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+                if (unlikely(__pyx_t_8 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+                  __PYX_ERR(0, 319, __pyx_L4_error)
+                }
                 __pyx_t_21 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_23, __pyx_pybuffernd_values.diminfo[0].strides)) != (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_values.diminfo[0].strides))) != 0);
                 __pyx_t_17 = __pyx_t_21;
                 __pyx_L19_bool_binop_done:;
                 if (!__pyx_t_17) break;
 
-                /* "torchqtm/_C/_rolling.pyx":321
+                /* "torchqtm/_C/_rolling.pyx":320
  *                     while not Q.empty() and ((ai <= values[Q.back()]) or
  *                                              values[Q.back()] != values[Q.back()]):
  *                         Q.pop_back()             # <<<<<<<<<<<<<<
  *                 Q.push_back(k)
  *                 W.push_back(k)
  */
                 __pyx_v_Q.pop_back();
               }
             }
             __pyx_L11:;
 
-            /* "torchqtm/_C/_rolling.pyx":322
+            /* "torchqtm/_C/_rolling.pyx":321
  *                                              values[Q.back()] != values[Q.back()]):
  *                         Q.pop_back()
  *                 Q.push_back(k)             # <<<<<<<<<<<<<<
  *                 W.push_back(k)
  * 
  */
             __pyx_v_Q.push_back(__pyx_v_k);
 
-            /* "torchqtm/_C/_rolling.pyx":323
+            /* "torchqtm/_C/_rolling.pyx":322
  *                         Q.pop_back()
  *                 Q.push_back(k)
  *                 W.push_back(k)             # <<<<<<<<<<<<<<
  * 
  *             # Discard entries outside and left of current window
  */
             __pyx_v_W.push_back(__pyx_v_k);
           }
 
-          /* "torchqtm/_C/_rolling.pyx":326
+          /* "torchqtm/_C/_rolling.pyx":325
  * 
  *             # Discard entries outside and left of current window
  *             while not Q.empty() and Q.front() <= starti[i] - 1:             # <<<<<<<<<<<<<<
  *                 Q.pop_front()
  *             while not W.empty() and W.front() <= starti[i] - 1:
  */
           while (1) {
             __pyx_t_21 = ((!(__pyx_v_Q.empty() != 0)) != 0);
             if (__pyx_t_21) {
             } else {
               __pyx_t_17 = __pyx_t_21;
               goto __pyx_L24_bool_binop_done;
             }
             __pyx_t_13 = __pyx_v_i;
+            __pyx_t_8 = -1;
+            if (__pyx_t_13 < 0) {
+              __pyx_t_13 += __pyx_pybuffernd_starti.diminfo[0].shape;
+              if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_starti.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 325, __pyx_L4_error)
+            }
             __pyx_t_21 = ((__pyx_v_Q.front() <= ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_starti.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_starti.diminfo[0].strides)) - 1)) != 0);
             __pyx_t_17 = __pyx_t_21;
             __pyx_L24_bool_binop_done:;
             if (!__pyx_t_17) break;
 
-            /* "torchqtm/_C/_rolling.pyx":327
+            /* "torchqtm/_C/_rolling.pyx":326
  *             # Discard entries outside and left of current window
  *             while not Q.empty() and Q.front() <= starti[i] - 1:
  *                 Q.pop_front()             # <<<<<<<<<<<<<<
  *             while not W.empty() and W.front() <= starti[i] - 1:
  *                 remove_mm(values[W.front()], &nobs)
  */
             __pyx_v_Q.pop_front();
           }
 
-          /* "torchqtm/_C/_rolling.pyx":328
+          /* "torchqtm/_C/_rolling.pyx":327
  *             while not Q.empty() and Q.front() <= starti[i] - 1:
  *                 Q.pop_front()
  *             while not W.empty() and W.front() <= starti[i] - 1:             # <<<<<<<<<<<<<<
  *                 remove_mm(values[W.front()], &nobs)
  *                 W.pop_front()
  */
           while (1) {
             __pyx_t_21 = ((!(__pyx_v_W.empty() != 0)) != 0);
             if (__pyx_t_21) {
             } else {
               __pyx_t_17 = __pyx_t_21;
               goto __pyx_L28_bool_binop_done;
             }
             __pyx_t_13 = __pyx_v_i;
+            __pyx_t_8 = -1;
+            if (__pyx_t_13 < 0) {
+              __pyx_t_13 += __pyx_pybuffernd_starti.diminfo[0].shape;
+              if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_starti.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 327, __pyx_L4_error)
+            }
             __pyx_t_21 = ((__pyx_v_W.front() <= ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_starti.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_starti.diminfo[0].strides)) - 1)) != 0);
             __pyx_t_17 = __pyx_t_21;
             __pyx_L28_bool_binop_done:;
             if (!__pyx_t_17) break;
 
-            /* "torchqtm/_C/_rolling.pyx":329
+            /* "torchqtm/_C/_rolling.pyx":328
  *                 Q.pop_front()
  *             while not W.empty() and W.front() <= starti[i] - 1:
  *                 remove_mm(values[W.front()], &nobs)             # <<<<<<<<<<<<<<
  *                 W.pop_front()
  * 
  */
             __pyx_t_18 = __pyx_v_W.front();
+            __pyx_t_8 = -1;
+            if (__pyx_t_18 < 0) {
+              __pyx_t_18 += __pyx_pybuffernd_values.diminfo[0].shape;
+              if (unlikely(__pyx_t_18 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 328, __pyx_L4_error)
+            }
             __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling_remove_mm((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_values.diminfo[0].strides)), (&__pyx_v_nobs));
 
-            /* "torchqtm/_C/_rolling.pyx":330
+            /* "torchqtm/_C/_rolling.pyx":329
  *             while not W.empty() and W.front() <= starti[i] - 1:
  *                 remove_mm(values[W.front()], &nobs)
  *                 W.pop_front()             # <<<<<<<<<<<<<<
  * 
  *             # Save output based on index in input value array
  */
             __pyx_v_W.pop_front();
           }
 
-          /* "torchqtm/_C/_rolling.pyx":333
+          /* "torchqtm/_C/_rolling.pyx":332
  * 
  *             # Save output based on index in input value array
  *             if not Q.empty() and curr_win_size > 0:             # <<<<<<<<<<<<<<
  *                 output[i] = calc_mm(minp, nobs, values[Q.front()])
  *             else:
  */
           __pyx_t_21 = ((!(__pyx_v_Q.empty() != 0)) != 0);
@@ -6070,82 +6328,116 @@
             goto __pyx_L31_bool_binop_done;
           }
           __pyx_t_21 = ((__pyx_v_curr_win_size > 0) != 0);
           __pyx_t_17 = __pyx_t_21;
           __pyx_L31_bool_binop_done:;
           if (__pyx_t_17) {
 
-            /* "torchqtm/_C/_rolling.pyx":334
+            /* "torchqtm/_C/_rolling.pyx":333
  *             # Save output based on index in input value array
  *             if not Q.empty() and curr_win_size > 0:
  *                 output[i] = calc_mm(minp, nobs, values[Q.front()])             # <<<<<<<<<<<<<<
  *             else:
  *                 output[i] = NaN
  */
             __pyx_t_18 = __pyx_v_Q.front();
+            __pyx_t_8 = -1;
+            if (__pyx_t_18 < 0) {
+              __pyx_t_18 += __pyx_pybuffernd_values.diminfo[0].shape;
+              if (unlikely(__pyx_t_18 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_values.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 333, __pyx_L4_error)
+            }
             __pyx_t_13 = __pyx_v_i;
+            __pyx_t_8 = -1;
+            if (__pyx_t_13 < 0) {
+              __pyx_t_13 += __pyx_pybuffernd_output.diminfo[0].shape;
+              if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_output.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 333, __pyx_L4_error)
+            }
             *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_output.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_output.diminfo[0].strides) = __pyx_fuse_9__pyx_f_8torchqtm_2_C_8_rolling_calc_mm(__pyx_v_minp, __pyx_v_nobs, (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_values.diminfo[0].strides)));
 
-            /* "torchqtm/_C/_rolling.pyx":333
+            /* "torchqtm/_C/_rolling.pyx":332
  * 
  *             # Save output based on index in input value array
  *             if not Q.empty() and curr_win_size > 0:             # <<<<<<<<<<<<<<
  *                 output[i] = calc_mm(minp, nobs, values[Q.front()])
  *             else:
  */
             goto __pyx_L30;
           }
 
-          /* "torchqtm/_C/_rolling.pyx":336
+          /* "torchqtm/_C/_rolling.pyx":335
  *                 output[i] = calc_mm(minp, nobs, values[Q.front()])
  *             else:
  *                 output[i] = NaN             # <<<<<<<<<<<<<<
  * 
  *     return output
  */
           /*else*/ {
             __pyx_t_13 = __pyx_v_i;
+            __pyx_t_8 = -1;
+            if (__pyx_t_13 < 0) {
+              __pyx_t_13 += __pyx_pybuffernd_output.diminfo[0].shape;
+              if (unlikely(__pyx_t_13 < 0)) __pyx_t_8 = 0;
+            } else if (unlikely(__pyx_t_13 >= __pyx_pybuffernd_output.diminfo[0].shape)) __pyx_t_8 = 0;
+            if (unlikely(__pyx_t_8 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_8);
+              __PYX_ERR(0, 335, __pyx_L4_error)
+            }
             *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_output.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_output.diminfo[0].strides) = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
           }
           __pyx_L30:;
         }
       }
 
-      /* "torchqtm/_C/_rolling.pyx":291
+      /* "torchqtm/_C/_rolling.pyx":290
  *     W = deque[int64_t]()
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  * 
  *         # This is using a modified version of the C++ code in this
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
           __Pyx_FastGIL_Forget();
           Py_BLOCK_THREADS
           #endif
           goto __pyx_L5;
         }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L1_error;
+        }
         __pyx_L5:;
       }
   }
 
-  /* "torchqtm/_C/_rolling.pyx":338
+  /* "torchqtm/_C/_rolling.pyx":337
  *                 output[i] = NaN
  * 
  *     return output             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_output));
   __pyx_r = ((PyObject *)__pyx_v_output);
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":274
+  /* "torchqtm/_C/_rolling.pyx":273
  * 
  * 
  * cdef _roll_min_max(ndarray[numeric_t] values,             # <<<<<<<<<<<<<<
  *                    ndarray[int64_t] starti,
  *                    ndarray[int64_t] endi,
  */
 
@@ -6176,29 +6468,32 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_output);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":341
+/* "torchqtm/_C/_rolling.pyx":340
  * 
  * 
  * cdef inline float64_t calc_mean(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                                 Py_ssize_t neg_ct, float64_t sum_x) nogil:
  *     cdef:
  */
 
 static CYTHON_INLINE __pyx_t_5numpy_float64_t __pyx_f_8torchqtm_2_C_8_rolling_calc_mean(__pyx_t_5numpy_int64_t __pyx_v_minp, Py_ssize_t __pyx_v_nobs, Py_ssize_t __pyx_v_neg_ct, __pyx_t_5numpy_float64_t __pyx_v_sum_x) {
   __pyx_t_5numpy_float64_t __pyx_v_result;
   __pyx_t_5numpy_float64_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":346
+  /* "torchqtm/_C/_rolling.pyx":345
  *         float64_t result
  * 
  *     if nobs >= minp and nobs > 0:             # <<<<<<<<<<<<<<
  *         result = sum_x / <float64_t>nobs
  *         if neg_ct == 0 and result < 0:
  */
   __pyx_t_2 = ((__pyx_v_nobs >= __pyx_v_minp) != 0);
@@ -6208,24 +6503,34 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_nobs > 0) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":347
+    /* "torchqtm/_C/_rolling.pyx":346
  * 
  *     if nobs >= minp and nobs > 0:
  *         result = sum_x / <float64_t>nobs             # <<<<<<<<<<<<<<
  *         if neg_ct == 0 and result < 0:
  *             # all positive
  */
+    if (unlikely(((__pyx_t_5numpy_float64_t)__pyx_v_nobs) == 0)) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 346, __pyx_L1_error)
+    }
     __pyx_v_result = (__pyx_v_sum_x / ((__pyx_t_5numpy_float64_t)__pyx_v_nobs));
 
-    /* "torchqtm/_C/_rolling.pyx":348
+    /* "torchqtm/_C/_rolling.pyx":347
  *     if nobs >= minp and nobs > 0:
  *         result = sum_x / <float64_t>nobs
  *         if neg_ct == 0 and result < 0:             # <<<<<<<<<<<<<<
  *             # all positive
  *             result = 0
  */
     __pyx_t_2 = ((__pyx_v_neg_ct == 0) != 0);
@@ -6235,34 +6540,34 @@
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_2 = ((__pyx_v_result < 0.0) != 0);
     __pyx_t_1 = __pyx_t_2;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_1) {
 
-      /* "torchqtm/_C/_rolling.pyx":350
+      /* "torchqtm/_C/_rolling.pyx":349
  *         if neg_ct == 0 and result < 0:
  *             # all positive
  *             result = 0             # <<<<<<<<<<<<<<
  *         elif neg_ct == nobs and result > 0:
  *             # all negative
  */
       __pyx_v_result = 0.0;
 
-      /* "torchqtm/_C/_rolling.pyx":348
+      /* "torchqtm/_C/_rolling.pyx":347
  *     if nobs >= minp and nobs > 0:
  *         result = sum_x / <float64_t>nobs
  *         if neg_ct == 0 and result < 0:             # <<<<<<<<<<<<<<
  *             # all positive
  *             result = 0
  */
       goto __pyx_L6;
     }
 
-    /* "torchqtm/_C/_rolling.pyx":351
+    /* "torchqtm/_C/_rolling.pyx":350
  *             # all positive
  *             result = 0
  *         elif neg_ct == nobs and result > 0:             # <<<<<<<<<<<<<<
  *             # all negative
  *             result = 0
  */
     __pyx_t_2 = ((__pyx_v_neg_ct == __pyx_v_nobs) != 0);
@@ -6272,324 +6577,327 @@
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_2 = ((__pyx_v_result > 0.0) != 0);
     __pyx_t_1 = __pyx_t_2;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_1) {
 
-      /* "torchqtm/_C/_rolling.pyx":353
+      /* "torchqtm/_C/_rolling.pyx":352
  *         elif neg_ct == nobs and result > 0:
  *             # all negative
  *             result = 0             # <<<<<<<<<<<<<<
  *         else:
  *             pass
  */
       __pyx_v_result = 0.0;
 
-      /* "torchqtm/_C/_rolling.pyx":351
+      /* "torchqtm/_C/_rolling.pyx":350
  *             # all positive
  *             result = 0
  *         elif neg_ct == nobs and result > 0:             # <<<<<<<<<<<<<<
  *             # all negative
  *             result = 0
  */
       goto __pyx_L6;
     }
 
-    /* "torchqtm/_C/_rolling.pyx":355
+    /* "torchqtm/_C/_rolling.pyx":354
  *             result = 0
  *         else:
  *             pass             # <<<<<<<<<<<<<<
  *     else:
  *         result = NaN
  */
     /*else*/ {
     }
     __pyx_L6:;
 
-    /* "torchqtm/_C/_rolling.pyx":346
+    /* "torchqtm/_C/_rolling.pyx":345
  *         float64_t result
  * 
  *     if nobs >= minp and nobs > 0:             # <<<<<<<<<<<<<<
  *         result = sum_x / <float64_t>nobs
  *         if neg_ct == 0 and result < 0:
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":357
+  /* "torchqtm/_C/_rolling.pyx":356
  *             pass
  *     else:
  *         result = NaN             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   /*else*/ {
     __pyx_v_result = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
   }
   __pyx_L3:;
 
-  /* "torchqtm/_C/_rolling.pyx":358
+  /* "torchqtm/_C/_rolling.pyx":357
  *     else:
  *         result = NaN
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":341
+  /* "torchqtm/_C/_rolling.pyx":340
  * 
  * 
  * cdef inline float64_t calc_mean(int64_t minp, Py_ssize_t nobs,             # <<<<<<<<<<<<<<
  *                                 Py_ssize_t neg_ct, float64_t sum_x) nogil:
  *     cdef:
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("torchqtm._C._rolling.calc_mean", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
+  __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":361
+/* "torchqtm/_C/_rolling.pyx":360
  * 
  * 
  * cdef inline void add_mean(float64_t val, Py_ssize_t *nobs, float64_t *sum_x,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t *neg_ct, float64_t *compensation) nogil:
  *     """ add a value from the mean calc using Kahan summation """
  */
 
 static CYTHON_INLINE void __pyx_f_8torchqtm_2_C_8_rolling_add_mean(__pyx_t_5numpy_float64_t __pyx_v_val, Py_ssize_t *__pyx_v_nobs, __pyx_t_5numpy_float64_t *__pyx_v_sum_x, Py_ssize_t *__pyx_v_neg_ct, __pyx_t_5numpy_float64_t *__pyx_v_compensation) {
   __pyx_t_5numpy_float64_t __pyx_v_y;
   __pyx_t_5numpy_float64_t __pyx_v_t;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":368
+  /* "torchqtm/_C/_rolling.pyx":367
  * 
  *     # Not NaN
  *     if notnan(val):             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] + 1
  *         y = val - compensation[0]
  */
   __pyx_t_1 = (__pyx_f_8torchqtm_2_C_8_rolling_notnan(__pyx_v_val) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":369
+    /* "torchqtm/_C/_rolling.pyx":368
  *     # Not NaN
  *     if notnan(val):
  *         nobs[0] = nobs[0] + 1             # <<<<<<<<<<<<<<
  *         y = val - compensation[0]
  *         t = sum_x[0] + y
  */
     (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) + 1);
 
-    /* "torchqtm/_C/_rolling.pyx":370
+    /* "torchqtm/_C/_rolling.pyx":369
  *     if notnan(val):
  *         nobs[0] = nobs[0] + 1
  *         y = val - compensation[0]             # <<<<<<<<<<<<<<
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y
  */
     __pyx_v_y = (__pyx_v_val - (__pyx_v_compensation[0]));
 
-    /* "torchqtm/_C/_rolling.pyx":371
+    /* "torchqtm/_C/_rolling.pyx":370
  *         nobs[0] = nobs[0] + 1
  *         y = val - compensation[0]
  *         t = sum_x[0] + y             # <<<<<<<<<<<<<<
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t
  */
     __pyx_v_t = ((__pyx_v_sum_x[0]) + __pyx_v_y);
 
-    /* "torchqtm/_C/_rolling.pyx":372
+    /* "torchqtm/_C/_rolling.pyx":371
  *         y = val - compensation[0]
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y             # <<<<<<<<<<<<<<
  *         sum_x[0] = t
  *         if signbit(val):
  */
     (__pyx_v_compensation[0]) = ((__pyx_v_t - (__pyx_v_sum_x[0])) - __pyx_v_y);
 
-    /* "torchqtm/_C/_rolling.pyx":373
+    /* "torchqtm/_C/_rolling.pyx":372
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t             # <<<<<<<<<<<<<<
  *         if signbit(val):
  *             neg_ct[0] = neg_ct[0] + 1
  */
     (__pyx_v_sum_x[0]) = __pyx_v_t;
 
-    /* "torchqtm/_C/_rolling.pyx":374
+    /* "torchqtm/_C/_rolling.pyx":373
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t
  *         if signbit(val):             # <<<<<<<<<<<<<<
  *             neg_ct[0] = neg_ct[0] + 1
  * 
  */
     __pyx_t_1 = (__pyx_f_8torchqtm_2_C_8_rolling_signbit(__pyx_v_val) != 0);
     if (__pyx_t_1) {
 
-      /* "torchqtm/_C/_rolling.pyx":375
+      /* "torchqtm/_C/_rolling.pyx":374
  *         sum_x[0] = t
  *         if signbit(val):
  *             neg_ct[0] = neg_ct[0] + 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       (__pyx_v_neg_ct[0]) = ((__pyx_v_neg_ct[0]) + 1);
 
-      /* "torchqtm/_C/_rolling.pyx":374
+      /* "torchqtm/_C/_rolling.pyx":373
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t
  *         if signbit(val):             # <<<<<<<<<<<<<<
  *             neg_ct[0] = neg_ct[0] + 1
  * 
  */
     }
 
-    /* "torchqtm/_C/_rolling.pyx":368
+    /* "torchqtm/_C/_rolling.pyx":367
  * 
  *     # Not NaN
  *     if notnan(val):             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] + 1
  *         y = val - compensation[0]
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":361
+  /* "torchqtm/_C/_rolling.pyx":360
  * 
  * 
  * cdef inline void add_mean(float64_t val, Py_ssize_t *nobs, float64_t *sum_x,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t *neg_ct, float64_t *compensation) nogil:
  *     """ add a value from the mean calc using Kahan summation """
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":378
+/* "torchqtm/_C/_rolling.pyx":377
  * 
  * 
  * cdef inline void remove_mean(float64_t val, Py_ssize_t *nobs, float64_t *sum_x,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t *neg_ct, float64_t *compensation) nogil:
  *     """ remove a value from the mean calc using Kahan summation """
  */
 
 static CYTHON_INLINE void __pyx_f_8torchqtm_2_C_8_rolling_remove_mean(__pyx_t_5numpy_float64_t __pyx_v_val, Py_ssize_t *__pyx_v_nobs, __pyx_t_5numpy_float64_t *__pyx_v_sum_x, Py_ssize_t *__pyx_v_neg_ct, __pyx_t_5numpy_float64_t *__pyx_v_compensation) {
   __pyx_t_5numpy_float64_t __pyx_v_y;
   __pyx_t_5numpy_float64_t __pyx_v_t;
   int __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":384
+  /* "torchqtm/_C/_rolling.pyx":383
  *         float64_t y, t
  * 
  *     if notnan(val):             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  *         y = - val - compensation[0]
  */
   __pyx_t_1 = (__pyx_f_8torchqtm_2_C_8_rolling_notnan(__pyx_v_val) != 0);
   if (__pyx_t_1) {
 
-    /* "torchqtm/_C/_rolling.pyx":385
+    /* "torchqtm/_C/_rolling.pyx":384
  * 
  *     if notnan(val):
  *         nobs[0] = nobs[0] - 1             # <<<<<<<<<<<<<<
  *         y = - val - compensation[0]
  *         t = sum_x[0] + y
  */
     (__pyx_v_nobs[0]) = ((__pyx_v_nobs[0]) - 1);
 
-    /* "torchqtm/_C/_rolling.pyx":386
+    /* "torchqtm/_C/_rolling.pyx":385
  *     if notnan(val):
  *         nobs[0] = nobs[0] - 1
  *         y = - val - compensation[0]             # <<<<<<<<<<<<<<
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y
  */
     __pyx_v_y = ((-__pyx_v_val) - (__pyx_v_compensation[0]));
 
-    /* "torchqtm/_C/_rolling.pyx":387
+    /* "torchqtm/_C/_rolling.pyx":386
  *         nobs[0] = nobs[0] - 1
  *         y = - val - compensation[0]
  *         t = sum_x[0] + y             # <<<<<<<<<<<<<<
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t
  */
     __pyx_v_t = ((__pyx_v_sum_x[0]) + __pyx_v_y);
 
-    /* "torchqtm/_C/_rolling.pyx":388
+    /* "torchqtm/_C/_rolling.pyx":387
  *         y = - val - compensation[0]
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y             # <<<<<<<<<<<<<<
  *         sum_x[0] = t
  *         if signbit(val):
  */
     (__pyx_v_compensation[0]) = ((__pyx_v_t - (__pyx_v_sum_x[0])) - __pyx_v_y);
 
-    /* "torchqtm/_C/_rolling.pyx":389
+    /* "torchqtm/_C/_rolling.pyx":388
  *         t = sum_x[0] + y
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t             # <<<<<<<<<<<<<<
  *         if signbit(val):
  *             neg_ct[0] = neg_ct[0] - 1
  */
     (__pyx_v_sum_x[0]) = __pyx_v_t;
 
-    /* "torchqtm/_C/_rolling.pyx":390
+    /* "torchqtm/_C/_rolling.pyx":389
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t
  *         if signbit(val):             # <<<<<<<<<<<<<<
  *             neg_ct[0] = neg_ct[0] - 1
  * 
  */
     __pyx_t_1 = (__pyx_f_8torchqtm_2_C_8_rolling_signbit(__pyx_v_val) != 0);
     if (__pyx_t_1) {
 
-      /* "torchqtm/_C/_rolling.pyx":391
+      /* "torchqtm/_C/_rolling.pyx":390
  *         sum_x[0] = t
  *         if signbit(val):
  *             neg_ct[0] = neg_ct[0] - 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       (__pyx_v_neg_ct[0]) = ((__pyx_v_neg_ct[0]) - 1);
 
-      /* "torchqtm/_C/_rolling.pyx":390
+      /* "torchqtm/_C/_rolling.pyx":389
  *         compensation[0] = t - sum_x[0] - y
  *         sum_x[0] = t
  *         if signbit(val):             # <<<<<<<<<<<<<<
  *             neg_ct[0] = neg_ct[0] - 1
  * 
  */
     }
 
-    /* "torchqtm/_C/_rolling.pyx":384
+    /* "torchqtm/_C/_rolling.pyx":383
  *         float64_t y, t
  * 
  *     if notnan(val):             # <<<<<<<<<<<<<<
  *         nobs[0] = nobs[0] - 1
  *         y = - val - compensation[0]
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":378
+  /* "torchqtm/_C/_rolling.pyx":377
  * 
  * 
  * cdef inline void remove_mean(float64_t val, Py_ssize_t *nobs, float64_t *sum_x,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t *neg_ct, float64_t *compensation) nogil:
  *     """ remove a value from the mean calc using Kahan summation """
  */
 
   /* function exit code */
 }
 
-/* "torchqtm/_C/_rolling.pyx":394
- * 
- * 
+/* "torchqtm/_C/_rolling.pyx":395
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_mean(const float64_t[:] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *               ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     cdef:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8torchqtm_2_C_8_rolling_7roll_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -6628,55 +6936,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_mean", 1, 4, 4, 1); __PYX_ERR(0, 394, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_mean", 1, 4, 4, 1); __PYX_ERR(0, 395, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_mean", 1, 4, 4, 2); __PYX_ERR(0, 394, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_mean", 1, 4, 4, 2); __PYX_ERR(0, 395, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_mean", 1, 4, 4, 3); __PYX_ERR(0, 394, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_mean", 1, 4, 4, 3); __PYX_ERR(0, 395, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_mean") < 0)) __PYX_ERR(0, 394, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_mean") < 0)) __PYX_ERR(0, 395, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
-    __pyx_v_values = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[0], 0); if (unlikely(!__pyx_v_values.memview)) __PYX_ERR(0, 394, __pyx_L3_error)
+    __pyx_v_values = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[0], 0); if (unlikely(!__pyx_v_values.memview)) __PYX_ERR(0, 395, __pyx_L3_error)
     __pyx_v_start = ((PyArrayObject *)values[1]);
     __pyx_v_end = ((PyArrayObject *)values[2]);
-    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 395, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 396, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_mean", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 394, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_mean", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 395, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 394, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 395, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 395, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 396, __pyx_L1_error)
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_6roll_mean(__pyx_self, __pyx_v_values, __pyx_v_start, __pyx_v_end, __pyx_v_minp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6740,76 +7048,76 @@
   __pyx_pybuffernd_start.rcbuffer = &__pyx_pybuffer_start;
   __pyx_pybuffer_end.pybuffer.buf = NULL;
   __pyx_pybuffer_end.refcount = 0;
   __pyx_pybuffernd_end.data = NULL;
   __pyx_pybuffernd_end.rcbuffer = &__pyx_pybuffer_end;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 394, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 395, __pyx_L1_error)
   }
   __pyx_pybuffernd_start.diminfo[0].strides = __pyx_pybuffernd_start.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_start.diminfo[0].shape = __pyx_pybuffernd_start.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 394, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 395, __pyx_L1_error)
   }
   __pyx_pybuffernd_end.diminfo[0].strides = __pyx_pybuffernd_end.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_end.diminfo[0].shape = __pyx_pybuffernd_end.rcbuffer->pybuffer.shape[0];
 
-  /* "torchqtm/_C/_rolling.pyx":399
+  /* "torchqtm/_C/_rolling.pyx":400
  *         float64_t val, compensation_add, compensation_remove, sum_x
  *         int64_t s, e
  *         Py_ssize_t nobs, i, j, neg_ct, N = len(start)             # <<<<<<<<<<<<<<
  *         ndarray[float64_t] output
  *         bint is_monotonic_increasing_bounds
  */
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 400, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":403
+  /* "torchqtm/_C/_rolling.pyx":404
  *         bint is_monotonic_increasing_bounds
  * 
  *     is_monotonic_increasing_bounds = True             # <<<<<<<<<<<<<<
  * 
  *     output = np.empty(N, dtype=np.float64)
  */
   __pyx_v_is_monotonic_increasing_bounds = 1;
 
-  /* "torchqtm/_C/_rolling.pyx":405
+  /* "torchqtm/_C/_rolling.pyx":406
  *     is_monotonic_increasing_bounds = True
  * 
  *     output = np.empty(N, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 405, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 405, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 406, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output.rcbuffer->pybuffer);
     __pyx_t_8 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_8 < 0)) {
       PyErr_Fetch(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
@@ -6818,68 +7126,68 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_9, __pyx_t_10, __pyx_t_11);
       }
       __pyx_t_9 = __pyx_t_10 = __pyx_t_11 = 0;
     }
     __pyx_pybuffernd_output.diminfo[0].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output.diminfo[0].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 405, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
   }
   __pyx_t_7 = 0;
   __pyx_v_output = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":407
+  /* "torchqtm/_C/_rolling.pyx":408
  *     output = np.empty(N, dtype=np.float64)
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  * 
  *         for i in range(0, N):
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "torchqtm/_C/_rolling.pyx":409
+        /* "torchqtm/_C/_rolling.pyx":410
  *     with nogil:
  * 
  *         for i in range(0, N):             # <<<<<<<<<<<<<<
  *             s = start[i]
  *             e = end[i]
  */
         __pyx_t_1 = __pyx_v_N;
         __pyx_t_12 = __pyx_t_1;
         for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
           __pyx_v_i = __pyx_t_13;
 
-          /* "torchqtm/_C/_rolling.pyx":410
+          /* "torchqtm/_C/_rolling.pyx":411
  * 
  *         for i in range(0, N):
  *             s = start[i]             # <<<<<<<<<<<<<<
  *             e = end[i]
  * 
  */
           __pyx_t_14 = __pyx_v_i;
           __pyx_v_s = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_start.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_start.diminfo[0].strides));
 
-          /* "torchqtm/_C/_rolling.pyx":411
+          /* "torchqtm/_C/_rolling.pyx":412
  *         for i in range(0, N):
  *             s = start[i]
  *             e = end[i]             # <<<<<<<<<<<<<<
  * 
  *             if i == 0 or not is_monotonic_increasing_bounds or s >= end[i - 1]:
  */
           __pyx_t_14 = __pyx_v_i;
           __pyx_v_e = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_end.diminfo[0].strides));
 
-          /* "torchqtm/_C/_rolling.pyx":413
+          /* "torchqtm/_C/_rolling.pyx":414
  *             e = end[i]
  * 
  *             if i == 0 or not is_monotonic_increasing_bounds or s >= end[i - 1]:             # <<<<<<<<<<<<<<
  * 
  *                 compensation_add = compensation_remove = sum_x = 0
  */
           __pyx_t_16 = ((__pyx_v_i == 0) != 0);
@@ -6896,214 +7204,214 @@
           }
           __pyx_t_14 = (__pyx_v_i - 1);
           __pyx_t_16 = ((__pyx_v_s >= (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_end.diminfo[0].strides))) != 0);
           __pyx_t_15 = __pyx_t_16;
           __pyx_L9_bool_binop_done:;
           if (__pyx_t_15) {
 
-            /* "torchqtm/_C/_rolling.pyx":415
+            /* "torchqtm/_C/_rolling.pyx":416
  *             if i == 0 or not is_monotonic_increasing_bounds or s >= end[i - 1]:
  * 
  *                 compensation_add = compensation_remove = sum_x = 0             # <<<<<<<<<<<<<<
  *                 nobs = neg_ct = 0
  *                 # setup
  */
             __pyx_v_compensation_add = 0.0;
             __pyx_v_compensation_remove = 0.0;
             __pyx_v_sum_x = 0.0;
 
-            /* "torchqtm/_C/_rolling.pyx":416
+            /* "torchqtm/_C/_rolling.pyx":417
  * 
  *                 compensation_add = compensation_remove = sum_x = 0
  *                 nobs = neg_ct = 0             # <<<<<<<<<<<<<<
  *                 # setup
  *                 for j in range(s, e):
  */
             __pyx_v_nobs = 0;
             __pyx_v_neg_ct = 0;
 
-            /* "torchqtm/_C/_rolling.pyx":418
+            /* "torchqtm/_C/_rolling.pyx":419
  *                 nobs = neg_ct = 0
  *                 # setup
  *                 for j in range(s, e):             # <<<<<<<<<<<<<<
  *                     val = values[j]
  *                     add_mean(val, &nobs, &sum_x, &neg_ct, &compensation_add)
  */
             __pyx_t_17 = __pyx_v_e;
             __pyx_t_18 = __pyx_t_17;
             for (__pyx_t_19 = __pyx_v_s; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
               __pyx_v_j = __pyx_t_19;
 
-              /* "torchqtm/_C/_rolling.pyx":419
+              /* "torchqtm/_C/_rolling.pyx":420
  *                 # setup
  *                 for j in range(s, e):
  *                     val = values[j]             # <<<<<<<<<<<<<<
  *                     add_mean(val, &nobs, &sum_x, &neg_ct, &compensation_add)
  * 
  */
               __pyx_t_14 = __pyx_v_j;
               __pyx_v_val = (*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_values.data + __pyx_t_14 * __pyx_v_values.strides[0]) )));
 
-              /* "torchqtm/_C/_rolling.pyx":420
+              /* "torchqtm/_C/_rolling.pyx":421
  *                 for j in range(s, e):
  *                     val = values[j]
  *                     add_mean(val, &nobs, &sum_x, &neg_ct, &compensation_add)             # <<<<<<<<<<<<<<
  * 
  *             else:
  */
               __pyx_f_8torchqtm_2_C_8_rolling_add_mean(__pyx_v_val, (&__pyx_v_nobs), (&__pyx_v_sum_x), (&__pyx_v_neg_ct), (&__pyx_v_compensation_add));
             }
 
-            /* "torchqtm/_C/_rolling.pyx":413
+            /* "torchqtm/_C/_rolling.pyx":414
  *             e = end[i]
  * 
  *             if i == 0 or not is_monotonic_increasing_bounds or s >= end[i - 1]:             # <<<<<<<<<<<<<<
  * 
  *                 compensation_add = compensation_remove = sum_x = 0
  */
             goto __pyx_L8;
           }
 
-          /* "torchqtm/_C/_rolling.pyx":425
+          /* "torchqtm/_C/_rolling.pyx":426
  * 
  *                 # calculate deletes
  *                 for j in range(start[i - 1], s):             # <<<<<<<<<<<<<<
  *                     val = values[j]
  *                     remove_mean(val, &nobs, &sum_x, &neg_ct, &compensation_remove)
  */
           /*else*/ {
             __pyx_t_17 = __pyx_v_s;
             __pyx_t_14 = (__pyx_v_i - 1);
             __pyx_t_18 = __pyx_t_17;
             for (__pyx_t_19 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_start.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_start.diminfo[0].strides)); __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
               __pyx_v_j = __pyx_t_19;
 
-              /* "torchqtm/_C/_rolling.pyx":426
+              /* "torchqtm/_C/_rolling.pyx":427
  *                 # calculate deletes
  *                 for j in range(start[i - 1], s):
  *                     val = values[j]             # <<<<<<<<<<<<<<
  *                     remove_mean(val, &nobs, &sum_x, &neg_ct, &compensation_remove)
  * 
  */
               __pyx_t_20 = __pyx_v_j;
               __pyx_v_val = (*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_values.data + __pyx_t_20 * __pyx_v_values.strides[0]) )));
 
-              /* "torchqtm/_C/_rolling.pyx":427
+              /* "torchqtm/_C/_rolling.pyx":428
  *                 for j in range(start[i - 1], s):
  *                     val = values[j]
  *                     remove_mean(val, &nobs, &sum_x, &neg_ct, &compensation_remove)             # <<<<<<<<<<<<<<
  * 
  *                 # calculate adds
  */
               __pyx_f_8torchqtm_2_C_8_rolling_remove_mean(__pyx_v_val, (&__pyx_v_nobs), (&__pyx_v_sum_x), (&__pyx_v_neg_ct), (&__pyx_v_compensation_remove));
             }
 
-            /* "torchqtm/_C/_rolling.pyx":430
+            /* "torchqtm/_C/_rolling.pyx":431
  * 
  *                 # calculate adds
  *                 for j in range(end[i - 1], e):             # <<<<<<<<<<<<<<
  *                     val = values[j]
  *                     add_mean(val, &nobs, &sum_x, &neg_ct, &compensation_add)
  */
             __pyx_t_17 = __pyx_v_e;
             __pyx_t_14 = (__pyx_v_i - 1);
             __pyx_t_18 = __pyx_t_17;
             for (__pyx_t_19 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_end.diminfo[0].strides)); __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
               __pyx_v_j = __pyx_t_19;
 
-              /* "torchqtm/_C/_rolling.pyx":431
+              /* "torchqtm/_C/_rolling.pyx":432
  *                 # calculate adds
  *                 for j in range(end[i - 1], e):
  *                     val = values[j]             # <<<<<<<<<<<<<<
  *                     add_mean(val, &nobs, &sum_x, &neg_ct, &compensation_add)
  * 
  */
               __pyx_t_20 = __pyx_v_j;
               __pyx_v_val = (*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_values.data + __pyx_t_20 * __pyx_v_values.strides[0]) )));
 
-              /* "torchqtm/_C/_rolling.pyx":432
+              /* "torchqtm/_C/_rolling.pyx":433
  *                 for j in range(end[i - 1], e):
  *                     val = values[j]
  *                     add_mean(val, &nobs, &sum_x, &neg_ct, &compensation_add)             # <<<<<<<<<<<<<<
  * 
  *             output[i] = calc_mean(minp, nobs, neg_ct, sum_x)
  */
               __pyx_f_8torchqtm_2_C_8_rolling_add_mean(__pyx_v_val, (&__pyx_v_nobs), (&__pyx_v_sum_x), (&__pyx_v_neg_ct), (&__pyx_v_compensation_add));
             }
           }
           __pyx_L8:;
 
-          /* "torchqtm/_C/_rolling.pyx":434
+          /* "torchqtm/_C/_rolling.pyx":435
  *                     add_mean(val, &nobs, &sum_x, &neg_ct, &compensation_add)
  * 
  *             output[i] = calc_mean(minp, nobs, neg_ct, sum_x)             # <<<<<<<<<<<<<<
  * 
  *             if not is_monotonic_increasing_bounds:
  */
           __pyx_t_14 = __pyx_v_i;
           *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_output.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_output.diminfo[0].strides) = __pyx_f_8torchqtm_2_C_8_rolling_calc_mean(__pyx_v_minp, __pyx_v_nobs, __pyx_v_neg_ct, __pyx_v_sum_x);
 
-          /* "torchqtm/_C/_rolling.pyx":436
+          /* "torchqtm/_C/_rolling.pyx":437
  *             output[i] = calc_mean(minp, nobs, neg_ct, sum_x)
  * 
  *             if not is_monotonic_increasing_bounds:             # <<<<<<<<<<<<<<
  *                 nobs = 0
  *                 neg_ct = 0
  */
           __pyx_t_15 = ((!(__pyx_v_is_monotonic_increasing_bounds != 0)) != 0);
           if (__pyx_t_15) {
 
-            /* "torchqtm/_C/_rolling.pyx":437
+            /* "torchqtm/_C/_rolling.pyx":438
  * 
  *             if not is_monotonic_increasing_bounds:
  *                 nobs = 0             # <<<<<<<<<<<<<<
  *                 neg_ct = 0
  *                 sum_x = 0.0
  */
             __pyx_v_nobs = 0;
 
-            /* "torchqtm/_C/_rolling.pyx":438
+            /* "torchqtm/_C/_rolling.pyx":439
  *             if not is_monotonic_increasing_bounds:
  *                 nobs = 0
  *                 neg_ct = 0             # <<<<<<<<<<<<<<
  *                 sum_x = 0.0
  *                 compensation_remove = 0.0
  */
             __pyx_v_neg_ct = 0;
 
-            /* "torchqtm/_C/_rolling.pyx":439
+            /* "torchqtm/_C/_rolling.pyx":440
  *                 nobs = 0
  *                 neg_ct = 0
  *                 sum_x = 0.0             # <<<<<<<<<<<<<<
  *                 compensation_remove = 0.0
  *     return output
  */
             __pyx_v_sum_x = 0.0;
 
-            /* "torchqtm/_C/_rolling.pyx":440
+            /* "torchqtm/_C/_rolling.pyx":441
  *                 neg_ct = 0
  *                 sum_x = 0.0
  *                 compensation_remove = 0.0             # <<<<<<<<<<<<<<
  *     return output
  * 
  */
             __pyx_v_compensation_remove = 0.0;
 
-            /* "torchqtm/_C/_rolling.pyx":436
+            /* "torchqtm/_C/_rolling.pyx":437
  *             output[i] = calc_mean(minp, nobs, neg_ct, sum_x)
  * 
  *             if not is_monotonic_increasing_bounds:             # <<<<<<<<<<<<<<
  *                 nobs = 0
  *                 neg_ct = 0
  */
           }
         }
       }
 
-      /* "torchqtm/_C/_rolling.pyx":407
+      /* "torchqtm/_C/_rolling.pyx":408
  *     output = np.empty(N, dtype=np.float64)
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  * 
  *         for i in range(0, N):
  */
       /*finally:*/ {
@@ -7114,29 +7422,29 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "torchqtm/_C/_rolling.pyx":441
+  /* "torchqtm/_C/_rolling.pyx":442
  *                 sum_x = 0.0
  *                 compensation_remove = 0.0
  *     return output             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_output));
   __pyx_r = ((PyObject *)__pyx_v_output);
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":394
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":395
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_mean(const float64_t[:] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *               ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     cdef:
  */
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7164,17 +7472,17 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_output);
   __PYX_XDEC_MEMVIEW(&__pyx_v_values, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":444
- * 
- * 
+/* "torchqtm/_C/_rolling.pyx":447
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_1D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8torchqtm_2_C_8_rolling_9roll_apply_1D(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -7222,49 +7530,49 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 1); __PYX_ERR(0, 444, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 1); __PYX_ERR(0, 447, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 2); __PYX_ERR(0, 444, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 2); __PYX_ERR(0, 447, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 3); __PYX_ERR(0, 444, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 3); __PYX_ERR(0, 447, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_function)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 4); __PYX_ERR(0, 444, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 4); __PYX_ERR(0, 447, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 5); __PYX_ERR(0, 444, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 5); __PYX_ERR(0, 447, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 6); __PYX_ERR(0, 444, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, 6); __PYX_ERR(0, 447, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_apply_1D") < 0)) __PYX_ERR(0, 444, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_apply_1D") < 0)) __PYX_ERR(0, 447, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -7272,31 +7580,31 @@
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
     __pyx_v_obj = values[0];
     __pyx_v_start = ((PyArrayObject *)values[1]);
     __pyx_v_end = ((PyArrayObject *)values[2]);
-    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 447, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 450, __pyx_L3_error)
     __pyx_v_function = values[4];
     __pyx_v_args = ((PyObject*)values[5]);
     __pyx_v_kwargs = ((PyObject*)values[6]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 444, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_apply_1D", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 447, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_apply_1D", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 445, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 446, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyTuple_Type), 1, "args", 1))) __PYX_ERR(0, 449, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyDict_Type), 1, "kwargs", 1))) __PYX_ERR(0, 450, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 448, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 449, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyTuple_Type), 1, "args", 1))) __PYX_ERR(0, 452, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyDict_Type), 1, "kwargs", 1))) __PYX_ERR(0, 453, __pyx_L1_error)
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_8roll_apply_1D(__pyx_self, __pyx_v_obj, __pyx_v_start, __pyx_v_end, __pyx_v_minp, __pyx_v_function, __pyx_v_args, __pyx_v_kwargs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7366,128 +7674,128 @@
   __pyx_pybuffernd_start.rcbuffer = &__pyx_pybuffer_start;
   __pyx_pybuffer_end.pybuffer.buf = NULL;
   __pyx_pybuffer_end.refcount = 0;
   __pyx_pybuffernd_end.data = NULL;
   __pyx_pybuffernd_end.rcbuffer = &__pyx_pybuffer_end;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 444, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 447, __pyx_L1_error)
   }
   __pyx_pybuffernd_start.diminfo[0].strides = __pyx_pybuffernd_start.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_start.diminfo[0].shape = __pyx_pybuffernd_start.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 444, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 447, __pyx_L1_error)
   }
   __pyx_pybuffernd_end.diminfo[0].strides = __pyx_pybuffernd_end.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_end.diminfo[0].shape = __pyx_pybuffernd_end.rcbuffer->pybuffer.shape[0];
 
-  /* "torchqtm/_C/_rolling.pyx":455
+  /* "torchqtm/_C/_rolling.pyx":458
  *         ndarray[float64_t, cast=True] arr
  *         Py_ssize_t i, s, e,
  *         Py_ssize_t N = len(start)             # <<<<<<<<<<<<<<
  *         Py_ssize_t n = len(obj)
  * 
  */
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 458, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":456
+  /* "torchqtm/_C/_rolling.pyx":459
  *         Py_ssize_t i, s, e,
  *         Py_ssize_t N = len(start)
  *         Py_ssize_t n = len(obj)             # <<<<<<<<<<<<<<
  * 
  *     if n == 0:
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_obj); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 456, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_obj); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 459, __pyx_L1_error)
   __pyx_v_n = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":458
+  /* "torchqtm/_C/_rolling.pyx":461
  *         Py_ssize_t n = len(obj)
  * 
  *     if n == 0:             # <<<<<<<<<<<<<<
  *         return np.array([], dtype=np.float64)
  * 
  */
   __pyx_t_2 = ((__pyx_v_n == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "torchqtm/_C/_rolling.pyx":459
+    /* "torchqtm/_C/_rolling.pyx":462
  * 
  *     if n == 0:
  *         return np.array([], dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     arr = np.asarray(obj)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 459, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_7;
     __pyx_t_7 = 0;
     goto __pyx_L0;
 
-    /* "torchqtm/_C/_rolling.pyx":458
+    /* "torchqtm/_C/_rolling.pyx":461
  *         Py_ssize_t n = len(obj)
  * 
  *     if n == 0:             # <<<<<<<<<<<<<<
  *         return np.array([], dtype=np.float64)
  * 
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":461
+  /* "torchqtm/_C/_rolling.pyx":464
  *         return np.array([], dtype=np.float64)
  * 
  *     arr = np.asarray(obj)             # <<<<<<<<<<<<<<
  * 
  *     # ndarray input
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_7 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_v_obj) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_obj);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 461, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 461, __pyx_L1_error)
+  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 464, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_7);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_arr.rcbuffer->pybuffer);
     __pyx_t_9 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 1, __pyx_stack);
     if (unlikely(__pyx_t_9 < 0)) {
       PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
@@ -7496,62 +7804,62 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
       }
       __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
     }
     __pyx_pybuffernd_arr.diminfo[0].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_arr.diminfo[0].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 461, __pyx_L1_error)
+    if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 464, __pyx_L1_error)
   }
   __pyx_t_8 = 0;
   __pyx_v_arr = ((PyArrayObject *)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":464
+  /* "torchqtm/_C/_rolling.pyx":467
  * 
  *     # ndarray input
  *     if not arr.flags.c_contiguous:             # <<<<<<<<<<<<<<
  *         arr = arr.copy('C')
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_flags); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_flags); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_c_contiguous); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_c_contiguous); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_13 = ((!__pyx_t_2) != 0);
   if (__pyx_t_13) {
 
-    /* "torchqtm/_C/_rolling.pyx":465
+    /* "torchqtm/_C/_rolling.pyx":468
  *     # ndarray input
  *     if not arr.flags.c_contiguous:
  *         arr = arr.copy('C')             # <<<<<<<<<<<<<<
  * 
  *     counts = roll_sum(np.isfinite(arr).astype(float), start, end, minp)
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_copy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 465, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_copy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_3, __pyx_n_u_C) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_n_u_C);
+    __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_3, __pyx_n_s_C) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_n_s_C);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 465, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 465, __pyx_L1_error)
+    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 468, __pyx_L1_error)
     __pyx_t_8 = ((PyArrayObject *)__pyx_t_5);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_arr.rcbuffer->pybuffer);
       __pyx_t_9 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 1, __pyx_stack);
       if (unlikely(__pyx_t_9 < 0)) {
         PyErr_Fetch(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
@@ -7560,77 +7868,77 @@
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_12, __pyx_t_11, __pyx_t_10);
         }
         __pyx_t_12 = __pyx_t_11 = __pyx_t_10 = 0;
       }
       __pyx_pybuffernd_arr.diminfo[0].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_arr.diminfo[0].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 465, __pyx_L1_error)
+      if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 468, __pyx_L1_error)
     }
     __pyx_t_8 = 0;
     __Pyx_DECREF_SET(__pyx_v_arr, ((PyArrayObject *)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "torchqtm/_C/_rolling.pyx":464
+    /* "torchqtm/_C/_rolling.pyx":467
  * 
  *     # ndarray input
  *     if not arr.flags.c_contiguous:             # <<<<<<<<<<<<<<
  *         arr = arr.copy('C')
  * 
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":467
+  /* "torchqtm/_C/_rolling.pyx":470
  *         arr = arr.copy('C')
  * 
  *     counts = roll_sum(np.isfinite(arr).astype(float), start, end, minp)             # <<<<<<<<<<<<<<
  * 
  *     output = np.empty(N, dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_roll_sum); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_roll_sum); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_6, ((PyObject *)__pyx_v_arr)) : __Pyx_PyObject_CallOneArg(__pyx_t_14, ((PyObject *)__pyx_v_arr));
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_astype); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_astype); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_4, ((PyObject *)(&PyFloat_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_14, ((PyObject *)(&PyFloat_Type)));
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 467, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  __pyx_t_14 = __Pyx_PyInt_From_npy_int64(__pyx_v_minp); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyInt_From_npy_int64(__pyx_v_minp); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __pyx_t_4 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -7639,33 +7947,33 @@
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[5] = {__pyx_t_4, __pyx_t_3, ((PyObject *)__pyx_v_start), ((PyObject *)__pyx_v_end), __pyx_t_14};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[5] = {__pyx_t_4, __pyx_t_3, ((PyObject *)__pyx_v_start), ((PyObject *)__pyx_v_end), __pyx_t_14};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 4+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(4+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(4+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_9, __pyx_t_3);
     __Pyx_INCREF(((PyObject *)__pyx_v_start));
@@ -7674,20 +7982,20 @@
     __Pyx_INCREF(((PyObject *)__pyx_v_end));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_end));
     PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_9, ((PyObject *)__pyx_v_end));
     __Pyx_GIVEREF(__pyx_t_14);
     PyTuple_SET_ITEM(__pyx_t_6, 3+__pyx_t_9, __pyx_t_14);
     __pyx_t_3 = 0;
     __pyx_t_14 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 467, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 470, __pyx_L1_error)
   __pyx_t_15 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_counts.rcbuffer->pybuffer);
     __pyx_t_9 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_counts.rcbuffer->pybuffer, (PyObject*)__pyx_t_15, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_9 < 0)) {
       PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
@@ -7696,54 +8004,54 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
       }
       __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
     }
     __pyx_pybuffernd_counts.diminfo[0].strides = __pyx_pybuffernd_counts.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_counts.diminfo[0].shape = __pyx_pybuffernd_counts.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 467, __pyx_L1_error)
+    if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 470, __pyx_L1_error)
   }
   __pyx_t_15 = 0;
   __pyx_v_counts = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":469
+  /* "torchqtm/_C/_rolling.pyx":472
  *     counts = roll_sum(np.isfinite(arr).astype(float), start, end, minp)
  * 
  *     output = np.empty(N, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(N):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 469, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 472, __pyx_L1_error)
   __pyx_t_15 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output.rcbuffer->pybuffer);
     __pyx_t_9 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output.rcbuffer->pybuffer, (PyObject*)__pyx_t_15, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_9 < 0)) {
       PyErr_Fetch(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
@@ -7752,147 +8060,147 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_12, __pyx_t_11, __pyx_t_10);
       }
       __pyx_t_12 = __pyx_t_11 = __pyx_t_10 = 0;
     }
     __pyx_pybuffernd_output.diminfo[0].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output.diminfo[0].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 469, __pyx_L1_error)
+    if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 472, __pyx_L1_error)
   }
   __pyx_t_15 = 0;
   __pyx_v_output = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":471
+  /* "torchqtm/_C/_rolling.pyx":474
  *     output = np.empty(N, dtype=np.float64)
  * 
  *     for i in range(N):             # <<<<<<<<<<<<<<
  * 
  *         s = start[i]
  */
   __pyx_t_1 = __pyx_v_N;
   __pyx_t_16 = __pyx_t_1;
   for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
     __pyx_v_i = __pyx_t_17;
 
-    /* "torchqtm/_C/_rolling.pyx":473
+    /* "torchqtm/_C/_rolling.pyx":476
  *     for i in range(N):
  * 
  *         s = start[i]             # <<<<<<<<<<<<<<
  *         e = end[i]
  * 
  */
     __pyx_t_18 = __pyx_v_i;
     __pyx_v_s = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_start.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_start.diminfo[0].strides));
 
-    /* "torchqtm/_C/_rolling.pyx":474
+    /* "torchqtm/_C/_rolling.pyx":477
  * 
  *         s = start[i]
  *         e = end[i]             # <<<<<<<<<<<<<<
  * 
  *         if counts[i] >= minp:
  */
     __pyx_t_18 = __pyx_v_i;
     __pyx_v_e = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_end.diminfo[0].strides));
 
-    /* "torchqtm/_C/_rolling.pyx":476
+    /* "torchqtm/_C/_rolling.pyx":479
  *         e = end[i]
  * 
  *         if counts[i] >= minp:             # <<<<<<<<<<<<<<
  *                 output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  */
     __pyx_t_18 = __pyx_v_i;
     __pyx_t_13 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_counts.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_counts.diminfo[0].strides)) >= __pyx_v_minp) != 0);
     if (__pyx_t_13) {
 
-      /* "torchqtm/_C/_rolling.pyx":477
+      /* "torchqtm/_C/_rolling.pyx":480
  * 
  *         if counts[i] >= minp:
  *                 output[i] = function(arr[s:e], *args, **kwargs)             # <<<<<<<<<<<<<<
  *         else:
  *             output[i] = NaN
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_s); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_s); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_e); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_e); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PySlice_New(__pyx_t_3, __pyx_t_5, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_6 = PySlice_New(__pyx_t_3, __pyx_t_5, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
       __pyx_t_5 = 0;
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 477, __pyx_L1_error)
+        __PYX_ERR(0, 480, __pyx_L1_error)
       }
-      __pyx_t_5 = PyNumber_Add(__pyx_t_6, __pyx_v_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_5 = PyNumber_Add(__pyx_t_6, __pyx_v_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-        __PYX_ERR(0, 477, __pyx_L1_error)
+        __PYX_ERR(0, 480, __pyx_L1_error)
       }
-      __pyx_t_6 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_6 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_v_function, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_v_function, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_19 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_19 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 477, __pyx_L1_error)
+      __pyx_t_19 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_19 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_18 = __pyx_v_i;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_output.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_output.diminfo[0].strides) = __pyx_t_19;
 
-      /* "torchqtm/_C/_rolling.pyx":476
+      /* "torchqtm/_C/_rolling.pyx":479
  *         e = end[i]
  * 
  *         if counts[i] >= minp:             # <<<<<<<<<<<<<<
  *                 output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  */
       goto __pyx_L7;
     }
 
-    /* "torchqtm/_C/_rolling.pyx":479
+    /* "torchqtm/_C/_rolling.pyx":482
  *                 output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  *             output[i] = NaN             # <<<<<<<<<<<<<<
  * 
  *     return output
  */
     /*else*/ {
       __pyx_t_18 = __pyx_v_i;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_output.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_output.diminfo[0].strides) = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
     }
     __pyx_L7:;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":481
+  /* "torchqtm/_C/_rolling.pyx":484
  *             output[i] = NaN
  * 
  *     return output             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_output));
   __pyx_r = ((PyObject *)__pyx_v_output);
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":444
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":447
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_1D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7926,17 +8234,17 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_counts);
   __Pyx_XDECREF((PyObject *)__pyx_v_arr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":484
- * 
- * 
+/* "torchqtm/_C/_rolling.pyx":489
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_2D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8torchqtm_2_C_8_rolling_11roll_apply_2D(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -7984,49 +8292,49 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 1); __PYX_ERR(0, 484, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 1); __PYX_ERR(0, 489, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 2); __PYX_ERR(0, 484, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 2); __PYX_ERR(0, 489, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 3); __PYX_ERR(0, 484, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 3); __PYX_ERR(0, 489, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_function)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 4); __PYX_ERR(0, 484, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 4); __PYX_ERR(0, 489, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 5); __PYX_ERR(0, 484, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 5); __PYX_ERR(0, 489, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 6); __PYX_ERR(0, 484, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, 6); __PYX_ERR(0, 489, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_apply_2D") < 0)) __PYX_ERR(0, 484, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_apply_2D") < 0)) __PYX_ERR(0, 489, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -8034,31 +8342,31 @@
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
     __pyx_v_obj = values[0];
     __pyx_v_start = ((PyArrayObject *)values[1]);
     __pyx_v_end = ((PyArrayObject *)values[2]);
-    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 487, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 492, __pyx_L3_error)
     __pyx_v_function = values[4];
     __pyx_v_args = ((PyObject*)values[5]);
     __pyx_v_kwargs = ((PyObject*)values[6]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 484, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_apply_2D", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 489, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_apply_2D", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 485, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 486, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyTuple_Type), 1, "args", 1))) __PYX_ERR(0, 489, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyDict_Type), 1, "kwargs", 1))) __PYX_ERR(0, 490, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 490, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 491, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyTuple_Type), 1, "args", 1))) __PYX_ERR(0, 494, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyDict_Type), 1, "kwargs", 1))) __PYX_ERR(0, 495, __pyx_L1_error)
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_10roll_apply_2D(__pyx_self, __pyx_v_obj, __pyx_v_start, __pyx_v_end, __pyx_v_minp, __pyx_v_function, __pyx_v_args, __pyx_v_kwargs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8130,87 +8438,87 @@
   __pyx_pybuffernd_start.rcbuffer = &__pyx_pybuffer_start;
   __pyx_pybuffer_end.pybuffer.buf = NULL;
   __pyx_pybuffer_end.refcount = 0;
   __pyx_pybuffernd_end.data = NULL;
   __pyx_pybuffernd_end.rcbuffer = &__pyx_pybuffer_end;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 484, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 489, __pyx_L1_error)
   }
   __pyx_pybuffernd_start.diminfo[0].strides = __pyx_pybuffernd_start.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_start.diminfo[0].shape = __pyx_pybuffernd_start.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 484, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 489, __pyx_L1_error)
   }
   __pyx_pybuffernd_end.diminfo[0].strides = __pyx_pybuffernd_end.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_end.diminfo[0].shape = __pyx_pybuffernd_end.rcbuffer->pybuffer.shape[0];
 
-  /* "torchqtm/_C/_rolling.pyx":496
+  /* "torchqtm/_C/_rolling.pyx":501
  *         ndarray[float64_t, ndim=2, cast=True] arr
  *         Py_ssize_t i, s, e,
  *         Py_ssize_t N = len(start)             # <<<<<<<<<<<<<<
  *         Py_ssize_t n = len(obj)
  *         Py_ssize_t n_col = obj.shape[1]
  */
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 496, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 501, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":497
+  /* "torchqtm/_C/_rolling.pyx":502
  *         Py_ssize_t i, s, e,
  *         Py_ssize_t N = len(start)
  *         Py_ssize_t n = len(obj)             # <<<<<<<<<<<<<<
  *         Py_ssize_t n_col = obj.shape[1]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_obj); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 497, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_obj); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 502, __pyx_L1_error)
   __pyx_v_n = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":498
+  /* "torchqtm/_C/_rolling.pyx":503
  *         Py_ssize_t N = len(start)
  *         Py_ssize_t n = len(obj)
  *         Py_ssize_t n_col = obj.shape[1]             # <<<<<<<<<<<<<<
  * 
  *     # if n == 0:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 498, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_n_col = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":503
+  /* "torchqtm/_C/_rolling.pyx":508
  *     #     return np.array([], dtype=np.float64)
  * 
  *     arr = np.asarray(obj)             # <<<<<<<<<<<<<<
  * 
  *     # ndarray input
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_v_obj) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_obj);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 503, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 503, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 508, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_arr.rcbuffer->pybuffer);
     __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 1, __pyx_stack);
     if (unlikely(__pyx_t_6 < 0)) {
       PyErr_Fetch(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
@@ -8219,62 +8527,62 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       }
       __pyx_t_7 = __pyx_t_8 = __pyx_t_9 = 0;
     }
     __pyx_pybuffernd_arr.diminfo[0].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_arr.diminfo[0].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_arr.diminfo[1].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_arr.diminfo[1].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 503, __pyx_L1_error)
+    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 508, __pyx_L1_error)
   }
   __pyx_t_5 = 0;
   __pyx_v_arr = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":506
+  /* "torchqtm/_C/_rolling.pyx":511
  * 
  *     # ndarray input
  *     if not arr.flags.c_contiguous:             # <<<<<<<<<<<<<<
  *         arr = arr.copy('C')
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_c_contiguous); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_c_contiguous); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_11 = ((!__pyx_t_10) != 0);
   if (__pyx_t_11) {
 
-    /* "torchqtm/_C/_rolling.pyx":507
+    /* "torchqtm/_C/_rolling.pyx":512
  *     # ndarray input
  *     if not arr.flags.c_contiguous:
  *         arr = arr.copy('C')             # <<<<<<<<<<<<<<
  * 
  *     counts = roll_sum(np.isfinite(arr[:, 0]).astype(float), start, end, minp)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_copy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 507, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_copy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_n_u_C) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_C);
+    __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_n_s_C) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_C);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 507, __pyx_L1_error)
+    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 512, __pyx_L1_error)
     __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_arr.rcbuffer->pybuffer);
       __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 1, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_9, &__pyx_t_8, &__pyx_t_7);
@@ -8283,80 +8591,80 @@
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_9, __pyx_t_8, __pyx_t_7);
         }
         __pyx_t_9 = __pyx_t_8 = __pyx_t_7 = 0;
       }
       __pyx_pybuffernd_arr.diminfo[0].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_arr.diminfo[0].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_arr.diminfo[1].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_arr.diminfo[1].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[1];
-      if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 507, __pyx_L1_error)
+      if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 512, __pyx_L1_error)
     }
     __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_arr, ((PyArrayObject *)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "torchqtm/_C/_rolling.pyx":506
+    /* "torchqtm/_C/_rolling.pyx":511
  * 
  *     # ndarray input
  *     if not arr.flags.c_contiguous:             # <<<<<<<<<<<<<<
  *         arr = arr.copy('C')
  * 
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":509
+  /* "torchqtm/_C/_rolling.pyx":514
  *         arr = arr.copy('C')
  * 
  *     counts = roll_sum(np.isfinite(arr[:, 0]).astype(float), start, end, minp)             # <<<<<<<<<<<<<<
  * 
  *     output = np.empty((N, n_col), dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_roll_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_roll_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_np); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_np); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_13 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_tuple__2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_tuple__2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
   __pyx_t_12 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_15, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_13);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_astype); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_astype); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_t_12 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_12);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
   __pyx_t_2 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_12, ((PyObject *)(&PyFloat_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_14, ((PyObject *)(&PyFloat_Type)));
   __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  __pyx_t_14 = __Pyx_PyInt_From_npy_int64(__pyx_v_minp); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyInt_From_npy_int64(__pyx_v_minp); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __pyx_t_12 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -8365,33 +8673,33 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[5] = {__pyx_t_12, __pyx_t_2, ((PyObject *)__pyx_v_start), ((PyObject *)__pyx_v_end), __pyx_t_14};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 509, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[5] = {__pyx_t_12, __pyx_t_2, ((PyObject *)__pyx_v_start), ((PyObject *)__pyx_v_end), __pyx_t_14};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 509, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   } else
   #endif
   {
-    __pyx_t_13 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 509, __pyx_L1_error)
+    __pyx_t_13 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     if (__pyx_t_12) {
       __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_12); __pyx_t_12 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_6, __pyx_t_2);
     __Pyx_INCREF(((PyObject *)__pyx_v_start));
@@ -8400,20 +8708,20 @@
     __Pyx_INCREF(((PyObject *)__pyx_v_end));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_end));
     PyTuple_SET_ITEM(__pyx_t_13, 2+__pyx_t_6, ((PyObject *)__pyx_v_end));
     __Pyx_GIVEREF(__pyx_t_14);
     PyTuple_SET_ITEM(__pyx_t_13, 3+__pyx_t_6, __pyx_t_14);
     __pyx_t_2 = 0;
     __pyx_t_14 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 509, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 514, __pyx_L1_error)
   __pyx_t_16 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_counts.rcbuffer->pybuffer);
     __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_counts.rcbuffer->pybuffer, (PyObject*)__pyx_t_16, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_6 < 0)) {
       PyErr_Fetch(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
@@ -8422,64 +8730,64 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       }
       __pyx_t_7 = __pyx_t_8 = __pyx_t_9 = 0;
     }
     __pyx_pybuffernd_counts.diminfo[0].strides = __pyx_pybuffernd_counts.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_counts.diminfo[0].shape = __pyx_pybuffernd_counts.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 509, __pyx_L1_error)
+    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 514, __pyx_L1_error)
   }
   __pyx_t_16 = 0;
   __pyx_v_counts = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":511
+  /* "torchqtm/_C/_rolling.pyx":516
  *     counts = roll_sum(np.isfinite(arr[:, 0]).astype(float), start, end, minp)
  * 
  *     output = np.empty((N, n_col), dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(N):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_13 = PyInt_FromSsize_t(__pyx_v_n_col); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_13 = PyInt_FromSsize_t(__pyx_v_n_col); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_13);
   PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_13);
   __pyx_t_4 = 0;
   __pyx_t_13 = 0;
-  __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_14);
   PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_14);
   __pyx_t_14 = 0;
-  __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, __pyx_t_14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, __pyx_t_14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 511, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 516, __pyx_L1_error)
   __pyx_t_17 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output.rcbuffer->pybuffer);
     __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output.rcbuffer->pybuffer, (PyObject*)__pyx_t_17, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_6 < 0)) {
       PyErr_Fetch(&__pyx_t_9, &__pyx_t_8, &__pyx_t_7);
@@ -8488,147 +8796,147 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_9, __pyx_t_8, __pyx_t_7);
       }
       __pyx_t_9 = __pyx_t_8 = __pyx_t_7 = 0;
     }
     __pyx_pybuffernd_output.diminfo[0].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output.diminfo[0].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_output.diminfo[1].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_output.diminfo[1].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 511, __pyx_L1_error)
+    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 516, __pyx_L1_error)
   }
   __pyx_t_17 = 0;
   __pyx_v_output = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":513
+  /* "torchqtm/_C/_rolling.pyx":518
  *     output = np.empty((N, n_col), dtype=np.float64)
  * 
  *     for i in range(N):             # <<<<<<<<<<<<<<
  * 
  *         s = start[i]
  */
   __pyx_t_1 = __pyx_v_N;
   __pyx_t_18 = __pyx_t_1;
   for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
     __pyx_v_i = __pyx_t_19;
 
-    /* "torchqtm/_C/_rolling.pyx":515
+    /* "torchqtm/_C/_rolling.pyx":520
  *     for i in range(N):
  * 
  *         s = start[i]             # <<<<<<<<<<<<<<
  *         e = end[i]
  * 
  */
     __pyx_t_20 = __pyx_v_i;
     __pyx_v_s = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_start.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_start.diminfo[0].strides));
 
-    /* "torchqtm/_C/_rolling.pyx":516
+    /* "torchqtm/_C/_rolling.pyx":521
  * 
  *         s = start[i]
  *         e = end[i]             # <<<<<<<<<<<<<<
  * 
  *         if counts[i] >= minp:
  */
     __pyx_t_20 = __pyx_v_i;
     __pyx_v_e = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_end.diminfo[0].strides));
 
-    /* "torchqtm/_C/_rolling.pyx":518
+    /* "torchqtm/_C/_rolling.pyx":523
  *         e = end[i]
  * 
  *         if counts[i] >= minp:             # <<<<<<<<<<<<<<
  *             output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  */
     __pyx_t_20 = __pyx_v_i;
     __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_counts.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_counts.diminfo[0].strides)) >= __pyx_v_minp) != 0);
     if (__pyx_t_11) {
 
-      /* "torchqtm/_C/_rolling.pyx":519
+      /* "torchqtm/_C/_rolling.pyx":524
  * 
  *         if counts[i] >= minp:
  *             output[i] = function(arr[s:e], *args, **kwargs)             # <<<<<<<<<<<<<<
  *         else:
  *             output[i] = NaN
  */
-      __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
+      __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_14 = PyInt_FromSsize_t(__pyx_v_e); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 519, __pyx_L1_error)
+      __pyx_t_14 = PyInt_FromSsize_t(__pyx_v_e); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
-      __pyx_t_13 = PySlice_New(__pyx_t_2, __pyx_t_14, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 519, __pyx_L1_error)
+      __pyx_t_13 = PySlice_New(__pyx_t_2, __pyx_t_14, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      __pyx_t_14 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 519, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 519, __pyx_L1_error)
+      __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_GIVEREF(__pyx_t_14);
       PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_14);
       __pyx_t_14 = 0;
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 519, __pyx_L1_error)
+        __PYX_ERR(0, 524, __pyx_L1_error)
       }
-      __pyx_t_14 = PyNumber_Add(__pyx_t_13, __pyx_v_args); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 519, __pyx_L1_error)
+      __pyx_t_14 = PyNumber_Add(__pyx_t_13, __pyx_v_args); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-        __PYX_ERR(0, 519, __pyx_L1_error)
+        __PYX_ERR(0, 524, __pyx_L1_error)
       }
-      __pyx_t_13 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 519, __pyx_L1_error)
+      __pyx_t_13 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_v_function, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_v_function, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_output), __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 519, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_output), __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "torchqtm/_C/_rolling.pyx":518
+      /* "torchqtm/_C/_rolling.pyx":523
  *         e = end[i]
  * 
  *         if counts[i] >= minp:             # <<<<<<<<<<<<<<
  *             output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  */
       goto __pyx_L6;
     }
 
-    /* "torchqtm/_C/_rolling.pyx":521
+    /* "torchqtm/_C/_rolling.pyx":526
  *             output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  *             output[i] = NaN             # <<<<<<<<<<<<<<
  * 
  *     return output
  */
     /*else*/ {
-      __pyx_t_2 = PyFloat_FromDouble(__pyx_v_8torchqtm_2_C_8_rolling_NaN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
+      __pyx_t_2 = PyFloat_FromDouble(__pyx_v_8torchqtm_2_C_8_rolling_NaN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 526, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_output), __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 521, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_output), __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 526, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L6:;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":523
+  /* "torchqtm/_C/_rolling.pyx":528
  *             output[i] = NaN
  * 
  *     return output             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_output));
   __pyx_r = ((PyObject *)__pyx_v_output);
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":484
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":489
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_2D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8663,17 +8971,17 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_counts);
   __Pyx_XDECREF((PyObject *)__pyx_v_arr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":526
- * 
- * 
+/* "torchqtm/_C/_rolling.pyx":533
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_3D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8torchqtm_2_C_8_rolling_13roll_apply_3D(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -8721,49 +9029,49 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 1); __PYX_ERR(0, 526, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 1); __PYX_ERR(0, 533, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 2); __PYX_ERR(0, 526, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 2); __PYX_ERR(0, 533, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 3); __PYX_ERR(0, 526, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 3); __PYX_ERR(0, 533, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_function)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 4); __PYX_ERR(0, 526, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 4); __PYX_ERR(0, 533, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 5); __PYX_ERR(0, 526, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 5); __PYX_ERR(0, 533, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 6); __PYX_ERR(0, 526, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, 6); __PYX_ERR(0, 533, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_apply_3D") < 0)) __PYX_ERR(0, 526, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_apply_3D") < 0)) __PYX_ERR(0, 533, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -8771,31 +9079,31 @@
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
     __pyx_v_obj = values[0];
     __pyx_v_start = ((PyArrayObject *)values[1]);
     __pyx_v_end = ((PyArrayObject *)values[2]);
-    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 529, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minp == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 536, __pyx_L3_error)
     __pyx_v_function = values[4];
     __pyx_v_args = ((PyObject*)values[5]);
     __pyx_v_kwargs = ((PyObject*)values[6]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 526, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_apply_3D", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 533, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_apply_3D", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 527, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 528, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyTuple_Type), 1, "args", 1))) __PYX_ERR(0, 531, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyDict_Type), 1, "kwargs", 1))) __PYX_ERR(0, 532, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), __pyx_ptype_5numpy_ndarray, 1, "start", 0))) __PYX_ERR(0, 534, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), __pyx_ptype_5numpy_ndarray, 1, "end", 0))) __PYX_ERR(0, 535, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyTuple_Type), 1, "args", 1))) __PYX_ERR(0, 538, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyDict_Type), 1, "kwargs", 1))) __PYX_ERR(0, 539, __pyx_L1_error)
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_12roll_apply_3D(__pyx_self, __pyx_v_obj, __pyx_v_start, __pyx_v_end, __pyx_v_minp, __pyx_v_function, __pyx_v_args, __pyx_v_kwargs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8868,103 +9176,103 @@
   __pyx_pybuffernd_start.rcbuffer = &__pyx_pybuffer_start;
   __pyx_pybuffer_end.pybuffer.buf = NULL;
   __pyx_pybuffer_end.refcount = 0;
   __pyx_pybuffernd_end.data = NULL;
   __pyx_pybuffernd_end.rcbuffer = &__pyx_pybuffer_end;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 526, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_start.rcbuffer->pybuffer, (PyObject*)__pyx_v_start, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 533, __pyx_L1_error)
   }
   __pyx_pybuffernd_start.diminfo[0].strides = __pyx_pybuffernd_start.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_start.diminfo[0].shape = __pyx_pybuffernd_start.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 526, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_end.rcbuffer->pybuffer, (PyObject*)__pyx_v_end, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 533, __pyx_L1_error)
   }
   __pyx_pybuffernd_end.diminfo[0].strides = __pyx_pybuffernd_end.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_end.diminfo[0].shape = __pyx_pybuffernd_end.rcbuffer->pybuffer.shape[0];
 
-  /* "torchqtm/_C/_rolling.pyx":538
+  /* "torchqtm/_C/_rolling.pyx":545
  *         ndarray[float64_t, ndim=3, cast=True] arr
  *         Py_ssize_t i, s, e,
  *         Py_ssize_t N = len(start)             # <<<<<<<<<<<<<<
  *         Py_ssize_t n = len(obj)
  *         Py_ssize_t n_stocks = obj.shape[1]
  */
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 538, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_start)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 545, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":539
+  /* "torchqtm/_C/_rolling.pyx":546
  *         Py_ssize_t i, s, e,
  *         Py_ssize_t N = len(start)
  *         Py_ssize_t n = len(obj)             # <<<<<<<<<<<<<<
  *         Py_ssize_t n_stocks = obj.shape[1]
  *         Py_ssize_t n_features = obj.shape[2]
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_obj); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 539, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_obj); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 546, __pyx_L1_error)
   __pyx_v_n = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":540
+  /* "torchqtm/_C/_rolling.pyx":547
  *         Py_ssize_t N = len(start)
  *         Py_ssize_t n = len(obj)
  *         Py_ssize_t n_stocks = obj.shape[1]             # <<<<<<<<<<<<<<
  *         Py_ssize_t n_features = obj.shape[2]
  *     # if n == 0:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_n_stocks = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":541
+  /* "torchqtm/_C/_rolling.pyx":548
  *         Py_ssize_t n = len(obj)
  *         Py_ssize_t n_stocks = obj.shape[1]
  *         Py_ssize_t n_features = obj.shape[2]             # <<<<<<<<<<<<<<
  *     # if n == 0:
  *     #     return np.array([], dtype=np.float64)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_n_features = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":545
+  /* "torchqtm/_C/_rolling.pyx":552
  *     #     return np.array([], dtype=np.float64)
  * 
  *     arr = np.asarray(obj)             # <<<<<<<<<<<<<<
  *     # ndarray input
  *     if not arr.flags.c_contiguous:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 552, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 552, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_obj) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_obj);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 545, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 545, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 552, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_arr.rcbuffer->pybuffer);
     __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 1, __pyx_stack);
     if (unlikely(__pyx_t_6 < 0)) {
       PyErr_Fetch(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
@@ -8973,62 +9281,62 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       }
       __pyx_t_7 = __pyx_t_8 = __pyx_t_9 = 0;
     }
     __pyx_pybuffernd_arr.diminfo[0].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_arr.diminfo[0].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_arr.diminfo[1].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_arr.diminfo[1].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_arr.diminfo[2].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_arr.diminfo[2].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[2];
-    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 545, __pyx_L1_error)
+    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 552, __pyx_L1_error)
   }
   __pyx_t_5 = 0;
   __pyx_v_arr = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":547
+  /* "torchqtm/_C/_rolling.pyx":554
  *     arr = np.asarray(obj)
  *     # ndarray input
  *     if not arr.flags.c_contiguous:             # <<<<<<<<<<<<<<
  *         arr = arr.copy('C')
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_c_contiguous); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 547, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_c_contiguous); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 547, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_11 = ((!__pyx_t_10) != 0);
   if (__pyx_t_11) {
 
-    /* "torchqtm/_C/_rolling.pyx":548
+    /* "torchqtm/_C/_rolling.pyx":555
  *     # ndarray input
  *     if not arr.flags.c_contiguous:
  *         arr = arr.copy('C')             # <<<<<<<<<<<<<<
  * 
  *     counts = roll_sum(np.isfinite(arr[:, 0, 0]).astype(float), start, end, minp)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_arr), __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_u_C) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_C);
+    __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_s_C) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_C);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 548, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 548, __pyx_L1_error)
+    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 555, __pyx_L1_error)
     __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_arr.rcbuffer->pybuffer);
       __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 1, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_9, &__pyx_t_8, &__pyx_t_7);
@@ -9037,80 +9345,80 @@
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_9, __pyx_t_8, __pyx_t_7);
         }
         __pyx_t_9 = __pyx_t_8 = __pyx_t_7 = 0;
       }
       __pyx_pybuffernd_arr.diminfo[0].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_arr.diminfo[0].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_arr.diminfo[1].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_arr.diminfo[1].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_arr.diminfo[2].strides = __pyx_pybuffernd_arr.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_arr.diminfo[2].shape = __pyx_pybuffernd_arr.rcbuffer->pybuffer.shape[2];
-      if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 548, __pyx_L1_error)
+      if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 555, __pyx_L1_error)
     }
     __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_arr, ((PyArrayObject *)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "torchqtm/_C/_rolling.pyx":547
+    /* "torchqtm/_C/_rolling.pyx":554
  *     arr = np.asarray(obj)
  *     # ndarray input
  *     if not arr.flags.c_contiguous:             # <<<<<<<<<<<<<<
  *         arr = arr.copy('C')
  * 
  */
   }
 
-  /* "torchqtm/_C/_rolling.pyx":550
+  /* "torchqtm/_C/_rolling.pyx":557
  *         arr = arr.copy('C')
  * 
  *     counts = roll_sum(np.isfinite(arr[:, 0, 0]).astype(float), start, end, minp)             # <<<<<<<<<<<<<<
  *     output = np.empty((N, n_stocks), dtype=np.float64)
  *     for i in range(N):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_roll_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_roll_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_np); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_np); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_13 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_tuple__3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_tuple__3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
   __pyx_t_12 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_15, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_13);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 550, __pyx_L1_error)
+  if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_astype); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_astype); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_t_12 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_14);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
       __Pyx_INCREF(__pyx_t_12);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_14, function);
     }
   }
   __pyx_t_3 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_12, ((PyObject *)(&PyFloat_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_14, ((PyObject *)(&PyFloat_Type)));
   __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 550, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  __pyx_t_14 = __Pyx_PyInt_From_npy_int64(__pyx_v_minp); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyInt_From_npy_int64(__pyx_v_minp); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __pyx_t_12 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9119,33 +9427,33 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_12, __pyx_t_3, ((PyObject *)__pyx_v_start), ((PyObject *)__pyx_v_end), __pyx_t_14};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 550, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 557, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_12, __pyx_t_3, ((PyObject *)__pyx_v_start), ((PyObject *)__pyx_v_end), __pyx_t_14};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 550, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 557, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   } else
   #endif
   {
-    __pyx_t_13 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 550, __pyx_L1_error)
+    __pyx_t_13 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 557, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     if (__pyx_t_12) {
       __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_12); __pyx_t_12 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_6, __pyx_t_3);
     __Pyx_INCREF(((PyObject *)__pyx_v_start));
@@ -9154,20 +9462,20 @@
     __Pyx_INCREF(((PyObject *)__pyx_v_end));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_end));
     PyTuple_SET_ITEM(__pyx_t_13, 2+__pyx_t_6, ((PyObject *)__pyx_v_end));
     __Pyx_GIVEREF(__pyx_t_14);
     PyTuple_SET_ITEM(__pyx_t_13, 3+__pyx_t_6, __pyx_t_14);
     __pyx_t_3 = 0;
     __pyx_t_14 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_13, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 550, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_13, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 557, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 550, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 557, __pyx_L1_error)
   __pyx_t_16 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_counts.rcbuffer->pybuffer);
     __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_counts.rcbuffer->pybuffer, (PyObject*)__pyx_t_16, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_6 < 0)) {
       PyErr_Fetch(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
@@ -9176,64 +9484,64 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       }
       __pyx_t_7 = __pyx_t_8 = __pyx_t_9 = 0;
     }
     __pyx_pybuffernd_counts.diminfo[0].strides = __pyx_pybuffernd_counts.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_counts.diminfo[0].shape = __pyx_pybuffernd_counts.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 550, __pyx_L1_error)
+    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 557, __pyx_L1_error)
   }
   __pyx_t_16 = 0;
   __pyx_v_counts = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":551
+  /* "torchqtm/_C/_rolling.pyx":558
  * 
  *     counts = roll_sum(np.isfinite(arr[:, 0, 0]).astype(float), start, end, minp)
  *     output = np.empty((N, n_stocks), dtype=np.float64)             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         s = start[i]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_13 = PyInt_FromSsize_t(__pyx_v_n_stocks); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_13 = PyInt_FromSsize_t(__pyx_v_n_stocks); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_13);
   PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_13);
   __pyx_t_4 = 0;
   __pyx_t_13 = 0;
-  __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_14);
   PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_14);
   __pyx_t_14 = 0;
-  __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_13, __pyx_t_14); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_13, __pyx_t_14); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 558, __pyx_L1_error)
   __pyx_t_17 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output.rcbuffer->pybuffer);
     __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output.rcbuffer->pybuffer, (PyObject*)__pyx_t_17, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_6 < 0)) {
       PyErr_Fetch(&__pyx_t_9, &__pyx_t_8, &__pyx_t_7);
@@ -9242,147 +9550,147 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_9, __pyx_t_8, __pyx_t_7);
       }
       __pyx_t_9 = __pyx_t_8 = __pyx_t_7 = 0;
     }
     __pyx_pybuffernd_output.diminfo[0].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output.diminfo[0].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_output.diminfo[1].strides = __pyx_pybuffernd_output.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_output.diminfo[1].shape = __pyx_pybuffernd_output.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 551, __pyx_L1_error)
+    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 558, __pyx_L1_error)
   }
   __pyx_t_17 = 0;
   __pyx_v_output = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":552
+  /* "torchqtm/_C/_rolling.pyx":559
  *     counts = roll_sum(np.isfinite(arr[:, 0, 0]).astype(float), start, end, minp)
  *     output = np.empty((N, n_stocks), dtype=np.float64)
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         s = start[i]
  *         e = end[i]
  */
   __pyx_t_1 = __pyx_v_N;
   __pyx_t_18 = __pyx_t_1;
   for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
     __pyx_v_i = __pyx_t_19;
 
-    /* "torchqtm/_C/_rolling.pyx":553
+    /* "torchqtm/_C/_rolling.pyx":560
  *     output = np.empty((N, n_stocks), dtype=np.float64)
  *     for i in range(N):
  *         s = start[i]             # <<<<<<<<<<<<<<
  *         e = end[i]
  * 
  */
     __pyx_t_20 = __pyx_v_i;
     __pyx_v_s = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_start.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_start.diminfo[0].strides));
 
-    /* "torchqtm/_C/_rolling.pyx":554
+    /* "torchqtm/_C/_rolling.pyx":561
  *     for i in range(N):
  *         s = start[i]
  *         e = end[i]             # <<<<<<<<<<<<<<
  * 
  *         if counts[i] >= minp:
  */
     __pyx_t_20 = __pyx_v_i;
     __pyx_v_e = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_end.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_end.diminfo[0].strides));
 
-    /* "torchqtm/_C/_rolling.pyx":556
+    /* "torchqtm/_C/_rolling.pyx":563
  *         e = end[i]
  * 
  *         if counts[i] >= minp:             # <<<<<<<<<<<<<<
  *             output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  */
     __pyx_t_20 = __pyx_v_i;
     __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_counts.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_counts.diminfo[0].strides)) >= __pyx_v_minp) != 0);
     if (__pyx_t_11) {
 
-      /* "torchqtm/_C/_rolling.pyx":557
+      /* "torchqtm/_C/_rolling.pyx":564
  * 
  *         if counts[i] >= minp:
  *             output[i] = function(arr[s:e], *args, **kwargs)             # <<<<<<<<<<<<<<
  *         else:
  *             output[i] = NaN
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_s); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_s); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_14 = PyInt_FromSsize_t(__pyx_v_e); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 557, __pyx_L1_error)
+      __pyx_t_14 = PyInt_FromSsize_t(__pyx_v_e); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
-      __pyx_t_13 = PySlice_New(__pyx_t_3, __pyx_t_14, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 557, __pyx_L1_error)
+      __pyx_t_13 = PySlice_New(__pyx_t_3, __pyx_t_14, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      __pyx_t_14 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 557, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_arr), __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 557, __pyx_L1_error)
+      __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_GIVEREF(__pyx_t_14);
       PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_14);
       __pyx_t_14 = 0;
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 557, __pyx_L1_error)
+        __PYX_ERR(0, 564, __pyx_L1_error)
       }
-      __pyx_t_14 = PyNumber_Add(__pyx_t_13, __pyx_v_args); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 557, __pyx_L1_error)
+      __pyx_t_14 = PyNumber_Add(__pyx_t_13, __pyx_v_args); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-        __PYX_ERR(0, 557, __pyx_L1_error)
+        __PYX_ERR(0, 564, __pyx_L1_error)
       }
-      __pyx_t_13 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 557, __pyx_L1_error)
+      __pyx_t_13 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_v_function, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_v_function, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_output), __pyx_v_i, __pyx_t_3, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 557, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_output), __pyx_v_i, __pyx_t_3, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 564, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "torchqtm/_C/_rolling.pyx":556
+      /* "torchqtm/_C/_rolling.pyx":563
  *         e = end[i]
  * 
  *         if counts[i] >= minp:             # <<<<<<<<<<<<<<
  *             output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  */
       goto __pyx_L6;
     }
 
-    /* "torchqtm/_C/_rolling.pyx":559
+    /* "torchqtm/_C/_rolling.pyx":566
  *             output[i] = function(arr[s:e], *args, **kwargs)
  *         else:
  *             output[i] = NaN             # <<<<<<<<<<<<<<
  *     return output
  * 
  */
     /*else*/ {
-      __pyx_t_3 = PyFloat_FromDouble(__pyx_v_8torchqtm_2_C_8_rolling_NaN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 559, __pyx_L1_error)
+      __pyx_t_3 = PyFloat_FromDouble(__pyx_v_8torchqtm_2_C_8_rolling_NaN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 566, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_output), __pyx_v_i, __pyx_t_3, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 559, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_output), __pyx_v_i, __pyx_t_3, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 566, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_L6:;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":560
+  /* "torchqtm/_C/_rolling.pyx":567
  *         else:
  *             output[i] = NaN
  *     return output             # <<<<<<<<<<<<<<
  * 
- * def roll_weighted_sum(
+ * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_output));
   __pyx_r = ((PyObject *)__pyx_v_output);
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":526
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":533
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_3D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9417,17 +9725,17 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_counts);
   __Pyx_XDECREF((PyObject *)__pyx_v_arr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":562
- *     return output
- * 
+/* "torchqtm/_C/_rolling.pyx":572
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_weighted_sum(             # <<<<<<<<<<<<<<
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8torchqtm_2_C_8_rolling_15roll_weighted_sum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -9463,40 +9771,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_weights)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_weighted_sum", 1, 3, 3, 1); __PYX_ERR(0, 562, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_weighted_sum", 1, 3, 3, 1); __PYX_ERR(0, 572, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_weighted_sum", 1, 3, 3, 2); __PYX_ERR(0, 562, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_weighted_sum", 1, 3, 3, 2); __PYX_ERR(0, 572, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_weighted_sum") < 0)) __PYX_ERR(0, 562, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_weighted_sum") < 0)) __PYX_ERR(0, 572, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_values = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[0], 0); if (unlikely(!__pyx_v_values.memview)) __PYX_ERR(0, 563, __pyx_L3_error)
-    __pyx_v_weights = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[1], 0); if (unlikely(!__pyx_v_weights.memview)) __PYX_ERR(0, 563, __pyx_L3_error)
-    __pyx_v_minp = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_minp == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 563, __pyx_L3_error)
+    __pyx_v_values = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[0], 0); if (unlikely(!__pyx_v_values.memview)) __PYX_ERR(0, 573, __pyx_L3_error)
+    __pyx_v_weights = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[1], 0); if (unlikely(!__pyx_v_weights.memview)) __PYX_ERR(0, 573, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_minp == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 573, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_weighted_sum", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 562, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_weighted_sum", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 572, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_weighted_sum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_14roll_weighted_sum(__pyx_self, __pyx_v_values, __pyx_v_weights, __pyx_v_minp);
 
@@ -9511,35 +9819,35 @@
   __Pyx_memviewslice __pyx_t_1 = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("roll_weighted_sum", 0);
 
-  /* "torchqtm/_C/_rolling.pyx":565
+  /* "torchqtm/_C/_rolling.pyx":575
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  *     return _roll_weighted_sum_mean(values, weights, minp, avg=0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8torchqtm_2_C_8_rolling__roll_weighted_sum_mean(__pyx_v_values, __pyx_v_weights, __pyx_v_minp, 0); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 565, __pyx_L1_error)
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_t_1, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8torchqtm_2_C_8_rolling__roll_weighted_sum_mean(__pyx_v_values, __pyx_v_weights, __pyx_v_minp, 0); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_t_1, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __PYX_XDEC_MEMVIEW(&__pyx_t_1, 1);
   __pyx_t_1.memview = NULL;
   __pyx_t_1.data = NULL;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":562
- *     return output
- * 
+  /* "torchqtm/_C/_rolling.pyx":572
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_weighted_sum(             # <<<<<<<<<<<<<<
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  */
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9551,17 +9859,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_values, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_weights, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":568
- * 
- * 
+/* "torchqtm/_C/_rolling.pyx":580
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_weighted_mean(             # <<<<<<<<<<<<<<
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8torchqtm_2_C_8_rolling_17roll_weighted_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -9597,40 +9905,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_weights)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_weighted_mean", 1, 3, 3, 1); __PYX_ERR(0, 568, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_weighted_mean", 1, 3, 3, 1); __PYX_ERR(0, 580, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("roll_weighted_mean", 1, 3, 3, 2); __PYX_ERR(0, 568, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("roll_weighted_mean", 1, 3, 3, 2); __PYX_ERR(0, 580, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_weighted_mean") < 0)) __PYX_ERR(0, 568, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "roll_weighted_mean") < 0)) __PYX_ERR(0, 580, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_values = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[0], 0); if (unlikely(!__pyx_v_values.memview)) __PYX_ERR(0, 569, __pyx_L3_error)
-    __pyx_v_weights = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[1], 0); if (unlikely(!__pyx_v_weights.memview)) __PYX_ERR(0, 569, __pyx_L3_error)
-    __pyx_v_minp = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_minp == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 569, __pyx_L3_error)
+    __pyx_v_values = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[0], 0); if (unlikely(!__pyx_v_values.memview)) __PYX_ERR(0, 581, __pyx_L3_error)
+    __pyx_v_weights = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t__const__(values[1], 0); if (unlikely(!__pyx_v_weights.memview)) __PYX_ERR(0, 581, __pyx_L3_error)
+    __pyx_v_minp = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_minp == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 581, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("roll_weighted_mean", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 568, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("roll_weighted_mean", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 580, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("torchqtm._C._rolling.roll_weighted_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8torchqtm_2_C_8_rolling_16roll_weighted_mean(__pyx_self, __pyx_v_values, __pyx_v_weights, __pyx_v_minp);
 
@@ -9645,35 +9953,35 @@
   __Pyx_memviewslice __pyx_t_1 = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("roll_weighted_mean", 0);
 
-  /* "torchqtm/_C/_rolling.pyx":571
+  /* "torchqtm/_C/_rolling.pyx":583
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  *     return _roll_weighted_sum_mean(values, weights, minp, avg=1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8torchqtm_2_C_8_rolling__roll_weighted_sum_mean(__pyx_v_values, __pyx_v_weights, __pyx_v_minp, 1); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 571, __pyx_L1_error)
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_t_1, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 571, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8torchqtm_2_C_8_rolling__roll_weighted_sum_mean(__pyx_v_values, __pyx_v_weights, __pyx_v_minp, 1); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_t_1, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __PYX_XDEC_MEMVIEW(&__pyx_t_1, 1);
   __pyx_t_1.memview = NULL;
   __pyx_t_1.data = NULL;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":568
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":580
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_weighted_mean(             # <<<<<<<<<<<<<<
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  */
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9685,15 +9993,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_values, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_weights, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "torchqtm/_C/_rolling.pyx":574
+/* "torchqtm/_C/_rolling.pyx":586
  * 
  * 
  * cdef float64_t[:] _roll_weighted_sum_mean(const float64_t[:] values,             # <<<<<<<<<<<<<<
  *                                           const float64_t[:] weights,
  *                                           int minp, bint avg):
  */
 
@@ -9731,201 +10039,201 @@
   Py_ssize_t __pyx_t_18;
   Py_ssize_t __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_roll_weighted_sum_mean", 0);
 
-  /* "torchqtm/_C/_rolling.pyx":585
+  /* "torchqtm/_C/_rolling.pyx":597
  *         float64_t val_in, val_win, c, w
  * 
  *     in_n = len(values)             # <<<<<<<<<<<<<<
  *     win_n = len(weights)
  * 
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_values); 
   __pyx_v_in_n = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":586
+  /* "torchqtm/_C/_rolling.pyx":598
  * 
  *     in_n = len(values)
  *     win_n = len(weights)             # <<<<<<<<<<<<<<
  * 
  *     output = np.zeros(in_n, dtype=np.float64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_weights); 
   __pyx_v_win_n = __pyx_t_1;
 
-  /* "torchqtm/_C/_rolling.pyx":588
+  /* "torchqtm/_C/_rolling.pyx":600
  *     win_n = len(weights)
  * 
  *     output = np.zeros(in_n, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     counts = np.zeros(in_n, dtype=np.float64)
  *     if avg:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_in_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_in_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 588, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_output = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "torchqtm/_C/_rolling.pyx":589
+  /* "torchqtm/_C/_rolling.pyx":601
  * 
  *     output = np.zeros(in_n, dtype=np.float64)
  *     counts = np.zeros(in_n, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     if avg:
  *         tot_wgt = np.zeros(in_n, dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_in_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_in_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 589, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_counts = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "torchqtm/_C/_rolling.pyx":590
+  /* "torchqtm/_C/_rolling.pyx":602
  *     output = np.zeros(in_n, dtype=np.float64)
  *     counts = np.zeros(in_n, dtype=np.float64)
  *     if avg:             # <<<<<<<<<<<<<<
  *         tot_wgt = np.zeros(in_n, dtype=np.float64)
  * 
  */
   __pyx_t_8 = (__pyx_v_avg != 0);
   if (__pyx_t_8) {
 
-    /* "torchqtm/_C/_rolling.pyx":591
+    /* "torchqtm/_C/_rolling.pyx":603
  *     counts = np.zeros(in_n, dtype=np.float64)
  *     if avg:
  *         tot_wgt = np.zeros(in_n, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     elif minp > in_n:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_in_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_in_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 591, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(__pyx_t_3, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(__pyx_t_3, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_tot_wgt = __pyx_t_7;
     __pyx_t_7.memview = NULL;
     __pyx_t_7.data = NULL;
 
-    /* "torchqtm/_C/_rolling.pyx":590
+    /* "torchqtm/_C/_rolling.pyx":602
  *     output = np.zeros(in_n, dtype=np.float64)
  *     counts = np.zeros(in_n, dtype=np.float64)
  *     if avg:             # <<<<<<<<<<<<<<
  *         tot_wgt = np.zeros(in_n, dtype=np.float64)
  * 
  */
     goto __pyx_L3;
   }
 
-  /* "torchqtm/_C/_rolling.pyx":593
+  /* "torchqtm/_C/_rolling.pyx":605
  *         tot_wgt = np.zeros(in_n, dtype=np.float64)
  * 
  *     elif minp > in_n:             # <<<<<<<<<<<<<<
  *         minp = in_n + 1
  * 
  */
   __pyx_t_8 = ((__pyx_v_minp > __pyx_v_in_n) != 0);
   if (__pyx_t_8) {
 
-    /* "torchqtm/_C/_rolling.pyx":594
+    /* "torchqtm/_C/_rolling.pyx":606
  * 
  *     elif minp > in_n:
  *         minp = in_n + 1             # <<<<<<<<<<<<<<
  * 
  *     minp = max(minp, 1)
  */
     __pyx_v_minp = (__pyx_v_in_n + 1);
 
-    /* "torchqtm/_C/_rolling.pyx":593
+    /* "torchqtm/_C/_rolling.pyx":605
  *         tot_wgt = np.zeros(in_n, dtype=np.float64)
  * 
  *     elif minp > in_n:             # <<<<<<<<<<<<<<
  *         minp = in_n + 1
  * 
  */
   }
   __pyx_L3:;
 
-  /* "torchqtm/_C/_rolling.pyx":596
+  /* "torchqtm/_C/_rolling.pyx":608
  *         minp = in_n + 1
  * 
  *     minp = max(minp, 1)             # <<<<<<<<<<<<<<
  * 
  *     with nogil:
  */
   __pyx_t_9 = 1;
@@ -9933,457 +10241,610 @@
   if (((__pyx_t_9 > __pyx_t_10) != 0)) {
     __pyx_t_11 = __pyx_t_9;
   } else {
     __pyx_t_11 = __pyx_t_10;
   }
   __pyx_v_minp = __pyx_t_11;
 
-  /* "torchqtm/_C/_rolling.pyx":598
+  /* "torchqtm/_C/_rolling.pyx":610
  *     minp = max(minp, 1)
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  *         if avg:
  *             for win_i in range(win_n):
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "torchqtm/_C/_rolling.pyx":599
+        /* "torchqtm/_C/_rolling.pyx":611
  * 
  *     with nogil:
  *         if avg:             # <<<<<<<<<<<<<<
  *             for win_i in range(win_n):
  *                 val_win = weights[win_i]
  */
         __pyx_t_8 = (__pyx_v_avg != 0);
         if (__pyx_t_8) {
 
-          /* "torchqtm/_C/_rolling.pyx":600
+          /* "torchqtm/_C/_rolling.pyx":612
  *     with nogil:
  *         if avg:
  *             for win_i in range(win_n):             # <<<<<<<<<<<<<<
  *                 val_win = weights[win_i]
  *                 if val_win != val_win:
  */
           __pyx_t_12 = __pyx_v_win_n;
           __pyx_t_13 = __pyx_t_12;
           for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
             __pyx_v_win_i = __pyx_t_14;
 
-            /* "torchqtm/_C/_rolling.pyx":601
+            /* "torchqtm/_C/_rolling.pyx":613
  *         if avg:
  *             for win_i in range(win_n):
  *                 val_win = weights[win_i]             # <<<<<<<<<<<<<<
  *                 if val_win != val_win:
  *                     continue
  */
             __pyx_t_15 = __pyx_v_win_i;
+            __pyx_t_10 = -1;
+            if (__pyx_t_15 < 0) {
+              __pyx_t_15 += __pyx_v_weights.shape[0];
+              if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+            } else if (unlikely(__pyx_t_15 >= __pyx_v_weights.shape[0])) __pyx_t_10 = 0;
+            if (unlikely(__pyx_t_10 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+              __PYX_ERR(0, 613, __pyx_L5_error)
+            }
             __pyx_v_val_win = (*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_weights.data + __pyx_t_15 * __pyx_v_weights.strides[0]) )));
 
-            /* "torchqtm/_C/_rolling.pyx":602
+            /* "torchqtm/_C/_rolling.pyx":614
  *             for win_i in range(win_n):
  *                 val_win = weights[win_i]
  *                 if val_win != val_win:             # <<<<<<<<<<<<<<
  *                     continue
  * 
  */
             __pyx_t_8 = ((__pyx_v_val_win != __pyx_v_val_win) != 0);
             if (__pyx_t_8) {
 
-              /* "torchqtm/_C/_rolling.pyx":603
+              /* "torchqtm/_C/_rolling.pyx":615
  *                 val_win = weights[win_i]
  *                 if val_win != val_win:
  *                     continue             # <<<<<<<<<<<<<<
  * 
  *                 for in_i in range(in_n - (win_n - win_i) + 1):
  */
               goto __pyx_L8_continue;
 
-              /* "torchqtm/_C/_rolling.pyx":602
+              /* "torchqtm/_C/_rolling.pyx":614
  *             for win_i in range(win_n):
  *                 val_win = weights[win_i]
  *                 if val_win != val_win:             # <<<<<<<<<<<<<<
  *                     continue
  * 
  */
             }
 
-            /* "torchqtm/_C/_rolling.pyx":605
+            /* "torchqtm/_C/_rolling.pyx":617
  *                     continue
  * 
  *                 for in_i in range(in_n - (win_n - win_i) + 1):             # <<<<<<<<<<<<<<
  *                     val_in = values[in_i]
  *                     if val_in == val_in:
  */
             __pyx_t_16 = ((__pyx_v_in_n - (__pyx_v_win_n - __pyx_v_win_i)) + 1);
             __pyx_t_17 = __pyx_t_16;
             for (__pyx_t_18 = 0; __pyx_t_18 < __pyx_t_17; __pyx_t_18+=1) {
               __pyx_v_in_i = __pyx_t_18;
 
-              /* "torchqtm/_C/_rolling.pyx":606
+              /* "torchqtm/_C/_rolling.pyx":618
  * 
  *                 for in_i in range(in_n - (win_n - win_i) + 1):
  *                     val_in = values[in_i]             # <<<<<<<<<<<<<<
  *                     if val_in == val_in:
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win
  */
               __pyx_t_15 = __pyx_v_in_i;
+              __pyx_t_10 = -1;
+              if (__pyx_t_15 < 0) {
+                __pyx_t_15 += __pyx_v_values.shape[0];
+                if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+              } else if (unlikely(__pyx_t_15 >= __pyx_v_values.shape[0])) __pyx_t_10 = 0;
+              if (unlikely(__pyx_t_10 != -1)) {
+                __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                __PYX_ERR(0, 618, __pyx_L5_error)
+              }
               __pyx_v_val_in = (*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_values.data + __pyx_t_15 * __pyx_v_values.strides[0]) )));
 
-              /* "torchqtm/_C/_rolling.pyx":607
+              /* "torchqtm/_C/_rolling.pyx":619
  *                 for in_i in range(in_n - (win_n - win_i) + 1):
  *                     val_in = values[in_i]
  *                     if val_in == val_in:             # <<<<<<<<<<<<<<
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win
  *                         counts[in_i + (win_n - win_i) - 1] += 1
  */
               __pyx_t_8 = ((__pyx_v_val_in == __pyx_v_val_in) != 0);
               if (__pyx_t_8) {
 
-                /* "torchqtm/_C/_rolling.pyx":608
+                /* "torchqtm/_C/_rolling.pyx":620
  *                     val_in = values[in_i]
  *                     if val_in == val_in:
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win             # <<<<<<<<<<<<<<
  *                         counts[in_i + (win_n - win_i) - 1] += 1
  *                         tot_wgt[in_i + (win_n - win_i) - 1] += val_win
  */
                 __pyx_t_15 = ((__pyx_v_in_i + (__pyx_v_win_n - __pyx_v_win_i)) - 1);
+                __pyx_t_10 = -1;
+                if (__pyx_t_15 < 0) {
+                  __pyx_t_15 += __pyx_v_output.shape[0];
+                  if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+                } else if (unlikely(__pyx_t_15 >= __pyx_v_output.shape[0])) __pyx_t_10 = 0;
+                if (unlikely(__pyx_t_10 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                  __PYX_ERR(0, 620, __pyx_L5_error)
+                }
                 *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_15 * __pyx_v_output.strides[0]) )) += (__pyx_v_val_in * __pyx_v_val_win);
 
-                /* "torchqtm/_C/_rolling.pyx":609
+                /* "torchqtm/_C/_rolling.pyx":621
  *                     if val_in == val_in:
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win
  *                         counts[in_i + (win_n - win_i) - 1] += 1             # <<<<<<<<<<<<<<
  *                         tot_wgt[in_i + (win_n - win_i) - 1] += val_win
  * 
  */
                 __pyx_t_15 = ((__pyx_v_in_i + (__pyx_v_win_n - __pyx_v_win_i)) - 1);
+                __pyx_t_10 = -1;
+                if (__pyx_t_15 < 0) {
+                  __pyx_t_15 += __pyx_v_counts.shape[0];
+                  if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+                } else if (unlikely(__pyx_t_15 >= __pyx_v_counts.shape[0])) __pyx_t_10 = 0;
+                if (unlikely(__pyx_t_10 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                  __PYX_ERR(0, 621, __pyx_L5_error)
+                }
                 *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_counts.data + __pyx_t_15 * __pyx_v_counts.strides[0]) )) += 1.0;
 
-                /* "torchqtm/_C/_rolling.pyx":610
+                /* "torchqtm/_C/_rolling.pyx":622
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win
  *                         counts[in_i + (win_n - win_i) - 1] += 1
  *                         tot_wgt[in_i + (win_n - win_i) - 1] += val_win             # <<<<<<<<<<<<<<
  * 
  *             for in_i in range(in_n):
  */
-                if (unlikely(!__pyx_v_tot_wgt.memview)) { __Pyx_RaiseUnboundMemoryviewSliceNogil("tot_wgt"); __PYX_ERR(0, 610, __pyx_L5_error) }
+                if (unlikely(!__pyx_v_tot_wgt.memview)) { __Pyx_RaiseUnboundMemoryviewSliceNogil("tot_wgt"); __PYX_ERR(0, 622, __pyx_L5_error) }
                 __pyx_t_15 = ((__pyx_v_in_i + (__pyx_v_win_n - __pyx_v_win_i)) - 1);
+                __pyx_t_10 = -1;
+                if (__pyx_t_15 < 0) {
+                  __pyx_t_15 += __pyx_v_tot_wgt.shape[0];
+                  if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+                } else if (unlikely(__pyx_t_15 >= __pyx_v_tot_wgt.shape[0])) __pyx_t_10 = 0;
+                if (unlikely(__pyx_t_10 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                  __PYX_ERR(0, 622, __pyx_L5_error)
+                }
                 *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_tot_wgt.data + __pyx_t_15 * __pyx_v_tot_wgt.strides[0]) )) += __pyx_v_val_win;
 
-                /* "torchqtm/_C/_rolling.pyx":607
+                /* "torchqtm/_C/_rolling.pyx":619
  *                 for in_i in range(in_n - (win_n - win_i) + 1):
  *                     val_in = values[in_i]
  *                     if val_in == val_in:             # <<<<<<<<<<<<<<
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win
  *                         counts[in_i + (win_n - win_i) - 1] += 1
  */
               }
             }
             __pyx_L8_continue:;
           }
 
-          /* "torchqtm/_C/_rolling.pyx":612
+          /* "torchqtm/_C/_rolling.pyx":624
  *                         tot_wgt[in_i + (win_n - win_i) - 1] += val_win
  * 
  *             for in_i in range(in_n):             # <<<<<<<<<<<<<<
  *                 c = counts[in_i]
  *                 if c < minp:
  */
           __pyx_t_12 = __pyx_v_in_n;
           __pyx_t_13 = __pyx_t_12;
           for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
             __pyx_v_in_i = __pyx_t_14;
 
-            /* "torchqtm/_C/_rolling.pyx":613
+            /* "torchqtm/_C/_rolling.pyx":625
  * 
  *             for in_i in range(in_n):
  *                 c = counts[in_i]             # <<<<<<<<<<<<<<
  *                 if c < minp:
  *                     output[in_i] = NaN
  */
             __pyx_t_15 = __pyx_v_in_i;
+            __pyx_t_10 = -1;
+            if (__pyx_t_15 < 0) {
+              __pyx_t_15 += __pyx_v_counts.shape[0];
+              if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+            } else if (unlikely(__pyx_t_15 >= __pyx_v_counts.shape[0])) __pyx_t_10 = 0;
+            if (unlikely(__pyx_t_10 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+              __PYX_ERR(0, 625, __pyx_L5_error)
+            }
             __pyx_v_c = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_counts.data + __pyx_t_15 * __pyx_v_counts.strides[0]) )));
 
-            /* "torchqtm/_C/_rolling.pyx":614
+            /* "torchqtm/_C/_rolling.pyx":626
  *             for in_i in range(in_n):
  *                 c = counts[in_i]
  *                 if c < minp:             # <<<<<<<<<<<<<<
  *                     output[in_i] = NaN
  *                 else:
  */
             __pyx_t_8 = ((__pyx_v_c < __pyx_v_minp) != 0);
             if (__pyx_t_8) {
 
-              /* "torchqtm/_C/_rolling.pyx":615
+              /* "torchqtm/_C/_rolling.pyx":627
  *                 c = counts[in_i]
  *                 if c < minp:
  *                     output[in_i] = NaN             # <<<<<<<<<<<<<<
  *                 else:
  *                     w = tot_wgt[in_i]
  */
               __pyx_t_15 = __pyx_v_in_i;
+              __pyx_t_10 = -1;
+              if (__pyx_t_15 < 0) {
+                __pyx_t_15 += __pyx_v_output.shape[0];
+                if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+              } else if (unlikely(__pyx_t_15 >= __pyx_v_output.shape[0])) __pyx_t_10 = 0;
+              if (unlikely(__pyx_t_10 != -1)) {
+                __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                __PYX_ERR(0, 627, __pyx_L5_error)
+              }
               *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_15 * __pyx_v_output.strides[0]) )) = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
 
-              /* "torchqtm/_C/_rolling.pyx":614
+              /* "torchqtm/_C/_rolling.pyx":626
  *             for in_i in range(in_n):
  *                 c = counts[in_i]
  *                 if c < minp:             # <<<<<<<<<<<<<<
  *                     output[in_i] = NaN
  *                 else:
  */
               goto __pyx_L16;
             }
 
-            /* "torchqtm/_C/_rolling.pyx":617
+            /* "torchqtm/_C/_rolling.pyx":629
  *                     output[in_i] = NaN
  *                 else:
  *                     w = tot_wgt[in_i]             # <<<<<<<<<<<<<<
  *                     if w == 0:
  *                         output[in_i] = NaN
  */
             /*else*/ {
-              if (unlikely(!__pyx_v_tot_wgt.memview)) { __Pyx_RaiseUnboundMemoryviewSliceNogil("tot_wgt"); __PYX_ERR(0, 617, __pyx_L5_error) }
+              if (unlikely(!__pyx_v_tot_wgt.memview)) { __Pyx_RaiseUnboundMemoryviewSliceNogil("tot_wgt"); __PYX_ERR(0, 629, __pyx_L5_error) }
               __pyx_t_15 = __pyx_v_in_i;
+              __pyx_t_10 = -1;
+              if (__pyx_t_15 < 0) {
+                __pyx_t_15 += __pyx_v_tot_wgt.shape[0];
+                if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+              } else if (unlikely(__pyx_t_15 >= __pyx_v_tot_wgt.shape[0])) __pyx_t_10 = 0;
+              if (unlikely(__pyx_t_10 != -1)) {
+                __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                __PYX_ERR(0, 629, __pyx_L5_error)
+              }
               __pyx_v_w = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_tot_wgt.data + __pyx_t_15 * __pyx_v_tot_wgt.strides[0]) )));
 
-              /* "torchqtm/_C/_rolling.pyx":618
+              /* "torchqtm/_C/_rolling.pyx":630
  *                 else:
  *                     w = tot_wgt[in_i]
  *                     if w == 0:             # <<<<<<<<<<<<<<
  *                         output[in_i] = NaN
  *                     else:
  */
               __pyx_t_8 = ((__pyx_v_w == 0.0) != 0);
               if (__pyx_t_8) {
 
-                /* "torchqtm/_C/_rolling.pyx":619
+                /* "torchqtm/_C/_rolling.pyx":631
  *                     w = tot_wgt[in_i]
  *                     if w == 0:
  *                         output[in_i] = NaN             # <<<<<<<<<<<<<<
  *                     else:
  *                         output[in_i] /= tot_wgt[in_i]
  */
                 __pyx_t_15 = __pyx_v_in_i;
+                __pyx_t_10 = -1;
+                if (__pyx_t_15 < 0) {
+                  __pyx_t_15 += __pyx_v_output.shape[0];
+                  if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+                } else if (unlikely(__pyx_t_15 >= __pyx_v_output.shape[0])) __pyx_t_10 = 0;
+                if (unlikely(__pyx_t_10 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                  __PYX_ERR(0, 631, __pyx_L5_error)
+                }
                 *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_15 * __pyx_v_output.strides[0]) )) = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
 
-                /* "torchqtm/_C/_rolling.pyx":618
+                /* "torchqtm/_C/_rolling.pyx":630
  *                 else:
  *                     w = tot_wgt[in_i]
  *                     if w == 0:             # <<<<<<<<<<<<<<
  *                         output[in_i] = NaN
  *                     else:
  */
                 goto __pyx_L17;
               }
 
-              /* "torchqtm/_C/_rolling.pyx":621
+              /* "torchqtm/_C/_rolling.pyx":633
  *                         output[in_i] = NaN
  *                     else:
  *                         output[in_i] /= tot_wgt[in_i]             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
               /*else*/ {
-                if (unlikely(!__pyx_v_tot_wgt.memview)) { __Pyx_RaiseUnboundMemoryviewSliceNogil("tot_wgt"); __PYX_ERR(0, 621, __pyx_L5_error) }
+                if (unlikely(!__pyx_v_tot_wgt.memview)) { __Pyx_RaiseUnboundMemoryviewSliceNogil("tot_wgt"); __PYX_ERR(0, 633, __pyx_L5_error) }
                 __pyx_t_15 = __pyx_v_in_i;
+                __pyx_t_10 = -1;
+                if (__pyx_t_15 < 0) {
+                  __pyx_t_15 += __pyx_v_tot_wgt.shape[0];
+                  if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+                } else if (unlikely(__pyx_t_15 >= __pyx_v_tot_wgt.shape[0])) __pyx_t_10 = 0;
+                if (unlikely(__pyx_t_10 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                  __PYX_ERR(0, 633, __pyx_L5_error)
+                }
                 __pyx_t_19 = __pyx_v_in_i;
+                __pyx_t_10 = -1;
+                if (__pyx_t_19 < 0) {
+                  __pyx_t_19 += __pyx_v_output.shape[0];
+                  if (unlikely(__pyx_t_19 < 0)) __pyx_t_10 = 0;
+                } else if (unlikely(__pyx_t_19 >= __pyx_v_output.shape[0])) __pyx_t_10 = 0;
+                if (unlikely(__pyx_t_10 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                  __PYX_ERR(0, 633, __pyx_L5_error)
+                }
                 *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_19 * __pyx_v_output.strides[0]) )) /= (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_tot_wgt.data + __pyx_t_15 * __pyx_v_tot_wgt.strides[0]) )));
               }
               __pyx_L17:;
             }
             __pyx_L16:;
           }
 
-          /* "torchqtm/_C/_rolling.pyx":599
+          /* "torchqtm/_C/_rolling.pyx":611
  * 
  *     with nogil:
  *         if avg:             # <<<<<<<<<<<<<<
  *             for win_i in range(win_n):
  *                 val_win = weights[win_i]
  */
           goto __pyx_L7;
         }
 
-        /* "torchqtm/_C/_rolling.pyx":624
+        /* "torchqtm/_C/_rolling.pyx":636
  * 
  *         else:
  *             for win_i in range(win_n):             # <<<<<<<<<<<<<<
  *                 val_win = weights[win_i]
  *                 if val_win != val_win:
  */
         /*else*/ {
           __pyx_t_12 = __pyx_v_win_n;
           __pyx_t_13 = __pyx_t_12;
           for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
             __pyx_v_win_i = __pyx_t_14;
 
-            /* "torchqtm/_C/_rolling.pyx":625
+            /* "torchqtm/_C/_rolling.pyx":637
  *         else:
  *             for win_i in range(win_n):
  *                 val_win = weights[win_i]             # <<<<<<<<<<<<<<
  *                 if val_win != val_win:
  *                     continue
  */
             __pyx_t_15 = __pyx_v_win_i;
+            __pyx_t_10 = -1;
+            if (__pyx_t_15 < 0) {
+              __pyx_t_15 += __pyx_v_weights.shape[0];
+              if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+            } else if (unlikely(__pyx_t_15 >= __pyx_v_weights.shape[0])) __pyx_t_10 = 0;
+            if (unlikely(__pyx_t_10 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+              __PYX_ERR(0, 637, __pyx_L5_error)
+            }
             __pyx_v_val_win = (*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_weights.data + __pyx_t_15 * __pyx_v_weights.strides[0]) )));
 
-            /* "torchqtm/_C/_rolling.pyx":626
+            /* "torchqtm/_C/_rolling.pyx":638
  *             for win_i in range(win_n):
  *                 val_win = weights[win_i]
  *                 if val_win != val_win:             # <<<<<<<<<<<<<<
  *                     continue
  * 
  */
             __pyx_t_8 = ((__pyx_v_val_win != __pyx_v_val_win) != 0);
             if (__pyx_t_8) {
 
-              /* "torchqtm/_C/_rolling.pyx":627
+              /* "torchqtm/_C/_rolling.pyx":639
  *                 val_win = weights[win_i]
  *                 if val_win != val_win:
  *                     continue             # <<<<<<<<<<<<<<
  * 
  *                 for in_i in range(in_n - (win_n - win_i) + 1):
  */
               goto __pyx_L18_continue;
 
-              /* "torchqtm/_C/_rolling.pyx":626
+              /* "torchqtm/_C/_rolling.pyx":638
  *             for win_i in range(win_n):
  *                 val_win = weights[win_i]
  *                 if val_win != val_win:             # <<<<<<<<<<<<<<
  *                     continue
  * 
  */
             }
 
-            /* "torchqtm/_C/_rolling.pyx":629
+            /* "torchqtm/_C/_rolling.pyx":641
  *                     continue
  * 
  *                 for in_i in range(in_n - (win_n - win_i) + 1):             # <<<<<<<<<<<<<<
  *                     val_in = values[in_i]
  * 
  */
             __pyx_t_16 = ((__pyx_v_in_n - (__pyx_v_win_n - __pyx_v_win_i)) + 1);
             __pyx_t_17 = __pyx_t_16;
             for (__pyx_t_18 = 0; __pyx_t_18 < __pyx_t_17; __pyx_t_18+=1) {
               __pyx_v_in_i = __pyx_t_18;
 
-              /* "torchqtm/_C/_rolling.pyx":630
+              /* "torchqtm/_C/_rolling.pyx":642
  * 
  *                 for in_i in range(in_n - (win_n - win_i) + 1):
  *                     val_in = values[in_i]             # <<<<<<<<<<<<<<
  * 
  *                     if val_in == val_in:
  */
               __pyx_t_15 = __pyx_v_in_i;
+              __pyx_t_10 = -1;
+              if (__pyx_t_15 < 0) {
+                __pyx_t_15 += __pyx_v_values.shape[0];
+                if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+              } else if (unlikely(__pyx_t_15 >= __pyx_v_values.shape[0])) __pyx_t_10 = 0;
+              if (unlikely(__pyx_t_10 != -1)) {
+                __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                __PYX_ERR(0, 642, __pyx_L5_error)
+              }
               __pyx_v_val_in = (*((__pyx_t_5numpy_float64_t const  *) ( /* dim=0 */ (__pyx_v_values.data + __pyx_t_15 * __pyx_v_values.strides[0]) )));
 
-              /* "torchqtm/_C/_rolling.pyx":632
+              /* "torchqtm/_C/_rolling.pyx":644
  *                     val_in = values[in_i]
  * 
  *                     if val_in == val_in:             # <<<<<<<<<<<<<<
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win
  *                         counts[in_i + (win_n - win_i) - 1] += 1
  */
               __pyx_t_8 = ((__pyx_v_val_in == __pyx_v_val_in) != 0);
               if (__pyx_t_8) {
 
-                /* "torchqtm/_C/_rolling.pyx":633
+                /* "torchqtm/_C/_rolling.pyx":645
  * 
  *                     if val_in == val_in:
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win             # <<<<<<<<<<<<<<
  *                         counts[in_i + (win_n - win_i) - 1] += 1
  * 
  */
                 __pyx_t_15 = ((__pyx_v_in_i + (__pyx_v_win_n - __pyx_v_win_i)) - 1);
+                __pyx_t_10 = -1;
+                if (__pyx_t_15 < 0) {
+                  __pyx_t_15 += __pyx_v_output.shape[0];
+                  if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+                } else if (unlikely(__pyx_t_15 >= __pyx_v_output.shape[0])) __pyx_t_10 = 0;
+                if (unlikely(__pyx_t_10 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                  __PYX_ERR(0, 645, __pyx_L5_error)
+                }
                 *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_15 * __pyx_v_output.strides[0]) )) += (__pyx_v_val_in * __pyx_v_val_win);
 
-                /* "torchqtm/_C/_rolling.pyx":634
+                /* "torchqtm/_C/_rolling.pyx":646
  *                     if val_in == val_in:
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win
  *                         counts[in_i + (win_n - win_i) - 1] += 1             # <<<<<<<<<<<<<<
  * 
  *             for in_i in range(in_n):
  */
                 __pyx_t_15 = ((__pyx_v_in_i + (__pyx_v_win_n - __pyx_v_win_i)) - 1);
+                __pyx_t_10 = -1;
+                if (__pyx_t_15 < 0) {
+                  __pyx_t_15 += __pyx_v_counts.shape[0];
+                  if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+                } else if (unlikely(__pyx_t_15 >= __pyx_v_counts.shape[0])) __pyx_t_10 = 0;
+                if (unlikely(__pyx_t_10 != -1)) {
+                  __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                  __PYX_ERR(0, 646, __pyx_L5_error)
+                }
                 *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_counts.data + __pyx_t_15 * __pyx_v_counts.strides[0]) )) += 1.0;
 
-                /* "torchqtm/_C/_rolling.pyx":632
+                /* "torchqtm/_C/_rolling.pyx":644
  *                     val_in = values[in_i]
  * 
  *                     if val_in == val_in:             # <<<<<<<<<<<<<<
  *                         output[in_i + (win_n - win_i) - 1] += val_in * val_win
  *                         counts[in_i + (win_n - win_i) - 1] += 1
  */
               }
             }
             __pyx_L18_continue:;
           }
 
-          /* "torchqtm/_C/_rolling.pyx":636
+          /* "torchqtm/_C/_rolling.pyx":648
  *                         counts[in_i + (win_n - win_i) - 1] += 1
  * 
  *             for in_i in range(in_n):             # <<<<<<<<<<<<<<
  *                 c = counts[in_i]
  *                 if c < minp:
  */
           __pyx_t_12 = __pyx_v_in_n;
           __pyx_t_13 = __pyx_t_12;
           for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
             __pyx_v_in_i = __pyx_t_14;
 
-            /* "torchqtm/_C/_rolling.pyx":637
+            /* "torchqtm/_C/_rolling.pyx":649
  * 
  *             for in_i in range(in_n):
  *                 c = counts[in_i]             # <<<<<<<<<<<<<<
  *                 if c < minp:
  *                     output[in_i] = NaN
  */
             __pyx_t_15 = __pyx_v_in_i;
+            __pyx_t_10 = -1;
+            if (__pyx_t_15 < 0) {
+              __pyx_t_15 += __pyx_v_counts.shape[0];
+              if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+            } else if (unlikely(__pyx_t_15 >= __pyx_v_counts.shape[0])) __pyx_t_10 = 0;
+            if (unlikely(__pyx_t_10 != -1)) {
+              __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+              __PYX_ERR(0, 649, __pyx_L5_error)
+            }
             __pyx_v_c = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_counts.data + __pyx_t_15 * __pyx_v_counts.strides[0]) )));
 
-            /* "torchqtm/_C/_rolling.pyx":638
+            /* "torchqtm/_C/_rolling.pyx":650
  *             for in_i in range(in_n):
  *                 c = counts[in_i]
  *                 if c < minp:             # <<<<<<<<<<<<<<
  *                     output[in_i] = NaN
  * 
  */
             __pyx_t_8 = ((__pyx_v_c < __pyx_v_minp) != 0);
             if (__pyx_t_8) {
 
-              /* "torchqtm/_C/_rolling.pyx":639
+              /* "torchqtm/_C/_rolling.pyx":651
  *                 c = counts[in_i]
  *                 if c < minp:
  *                     output[in_i] = NaN             # <<<<<<<<<<<<<<
  * 
  *     return output
  */
               __pyx_t_15 = __pyx_v_in_i;
+              __pyx_t_10 = -1;
+              if (__pyx_t_15 < 0) {
+                __pyx_t_15 += __pyx_v_output.shape[0];
+                if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
+              } else if (unlikely(__pyx_t_15 >= __pyx_v_output.shape[0])) __pyx_t_10 = 0;
+              if (unlikely(__pyx_t_10 != -1)) {
+                __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_10);
+                __PYX_ERR(0, 651, __pyx_L5_error)
+              }
               *((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_15 * __pyx_v_output.strides[0]) )) = __pyx_v_8torchqtm_2_C_8_rolling_NaN;
 
-              /* "torchqtm/_C/_rolling.pyx":638
+              /* "torchqtm/_C/_rolling.pyx":650
  *             for in_i in range(in_n):
  *                 c = counts[in_i]
  *                 if c < minp:             # <<<<<<<<<<<<<<
  *                     output[in_i] = NaN
  * 
  */
             }
           }
         }
         __pyx_L7:;
       }
 
-      /* "torchqtm/_C/_rolling.pyx":598
+      /* "torchqtm/_C/_rolling.pyx":610
  *     minp = max(minp, 1)
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  *         if avg:
  *             for win_i in range(win_n):
  */
       /*finally:*/ {
@@ -10401,24 +10862,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L6:;
       }
   }
 
-  /* "torchqtm/_C/_rolling.pyx":641
+  /* "torchqtm/_C/_rolling.pyx":653
  *                     output[in_i] = NaN
  * 
  *     return output             # <<<<<<<<<<<<<<
  */
   __PYX_INC_MEMVIEW(&__pyx_v_output, 0);
   __pyx_r = __pyx_v_output;
   goto __pyx_L0;
 
-  /* "torchqtm/_C/_rolling.pyx":574
+  /* "torchqtm/_C/_rolling.pyx":586
  * 
  * 
  * cdef float64_t[:] _roll_weighted_sum_mean(const float64_t[:] values,             # <<<<<<<<<<<<<<
  *                                           const float64_t[:] weights,
  *                                           int minp, bint avg):
  */
 
@@ -12144,15 +12605,15 @@
         PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
         __PYX_ERR(2, 181, __pyx_L1_error)
       }
       else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_self->len))) {
         PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
         __PYX_ERR(2, 181, __pyx_L1_error)
       }
-      __pyx_t_1 = (__pyx_v_self->len / __pyx_v_itemsize);
+      __pyx_t_1 = __Pyx_div_Py_ssize_t(__pyx_v_self->len, __pyx_v_itemsize);
       __pyx_t_9 = __pyx_t_1;
       for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_9; __pyx_t_11+=1) {
         __pyx_v_i = __pyx_t_11;
 
         /* "View.MemoryView":182
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
@@ -15844,15 +16305,15 @@
  *         else:
  *             if len(self.view.format) == 1:
  *                 return result[0]             # <<<<<<<<<<<<<<
  *             return result
  * 
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 500, __pyx_L5_except_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 500, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L6_except_return;
 
         /* "View.MemoryView":499
  *             raise ValueError("Unable to convert item to object")
@@ -20159,15 +20620,15 @@
       PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
       __PYX_ERR(2, 919, __pyx_L1_error)
     }
     else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_view->len))) {
       PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
       __PYX_ERR(2, 919, __pyx_L1_error)
     }
-    __pyx_v_shape = (__pyx_v_view->len / __pyx_v_itemsize);
+    __pyx_v_shape = __Pyx_div_Py_ssize_t(__pyx_v_view->len, __pyx_v_itemsize);
 
     /* "View.MemoryView":920
  *     if view.ndim == 0:
  *         shape = view.len / itemsize
  *         stride = itemsize             # <<<<<<<<<<<<<<
  *     else:
  *         shape = view.shape[dim]
@@ -20464,15 +20925,15 @@
   /* "View.MemoryView":953
  * 
  *     cdef int i, j
  *     for i in range(ndim / 2):             # <<<<<<<<<<<<<<
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  */
-  __pyx_t_3 = (__pyx_v_ndim / 2);
+  __pyx_t_3 = __Pyx_div_long(__pyx_v_ndim, 2);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_4; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
     /* "View.MemoryView":954
  *     cdef int i, j
  *     for i in range(ndim / 2):
@@ -24403,15 +24864,15 @@
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[1])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->name);
   __Pyx_DECREF(__pyx_v___pyx_result->name);
   __pyx_v___pyx_result->name = __pyx_t_1;
   __pyx_t_1 = 0;
 
@@ -24448,15 +24909,15 @@
     __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v___pyx_state == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(2, 14, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 14, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
@@ -25275,15 +25736,15 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_ASCII, __pyx_k_ASCII, sizeof(__pyx_k_ASCII), 0, 0, 1, 1},
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
-  {&__pyx_n_u_C, __pyx_k_C, sizeof(__pyx_k_C), 0, 1, 0, 1},
+  {&__pyx_n_s_C, __pyx_k_C, sizeof(__pyx_k_C), 0, 0, 1, 1},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
@@ -25364,16 +25825,16 @@
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_neg_ct, __pyx_k_neg_ct, sizeof(__pyx_k_neg_ct), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_nobs, __pyx_k_nobs, sizeof(__pyx_k_nobs), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-  {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+  {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
+  {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_output, __pyx_k_output, sizeof(__pyx_k_output), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
@@ -25420,15 +25881,15 @@
   {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {&__pyx_n_s_weights, __pyx_k_weights, sizeof(__pyx_k_weights), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 195, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
@@ -25438,58 +25899,58 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "torchqtm/_C/_rolling.pyx":509
+  /* "torchqtm/_C/_rolling.pyx":514
  *         arr = arr.copy('C')
  * 
  *     counts = roll_sum(np.isfinite(arr[:, 0]).astype(float), start, end, minp)             # <<<<<<<<<<<<<<
  * 
  *     output = np.empty((N, n_col), dtype=np.float64)
  */
-  __pyx_slice_ = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_slice_ = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_slice_, __pyx_int_0); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_slice_, __pyx_int_0); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "torchqtm/_C/_rolling.pyx":550
+  /* "torchqtm/_C/_rolling.pyx":557
  *         arr = arr.copy('C')
  * 
  *     counts = roll_sum(np.isfinite(arr[:, 0, 0]).astype(float), start, end, minp)             # <<<<<<<<<<<<<<
  *     output = np.empty((N, n_stocks), dtype=np.float64)
  *     for i in range(N):
  */
-  __pyx_tuple__3 = PyTuple_Pack(3, __pyx_slice_, __pyx_int_0, __pyx_int_0); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(3, __pyx_slice_, __pyx_int_0, __pyx_int_0); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "../../../opt/anaconda3/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "../../../opt/anaconda3/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -25669,121 +26130,121 @@
   __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
   __pyx_tuple__23 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "torchqtm/_C/_rolling.pyx":180
+  /* "torchqtm/_C/_rolling.pyx":179
  * 
  * 
  * def roll_sum(const float64_t[:] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     cdef:
  */
-  __pyx_tuple__24 = PyTuple_Pack(15, __pyx_n_s_values, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_sum_x, __pyx_n_s_compensation_add, __pyx_n_s_compensation_remove, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_nobs, __pyx_n_s_N, __pyx_n_s_output, __pyx_n_s_is_monotonic_increasing_bounds); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(15, __pyx_n_s_values, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_sum_x, __pyx_n_s_compensation_add, __pyx_n_s_compensation_remove, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_nobs, __pyx_n_s_N, __pyx_n_s_output, __pyx_n_s_is_monotonic_increasing_bounds); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(4, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_sum, 180, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(4, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_sum, 179, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "torchqtm/_C/_rolling.pyx":229
+  /* "torchqtm/_C/_rolling.pyx":228
  * 
  * 
  * def roll_max(ndarray[float64_t] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     """
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_values, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_values, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_max, 229, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_max, 228, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 228, __pyx_L1_error)
 
-  /* "torchqtm/_C/_rolling.pyx":253
+  /* "torchqtm/_C/_rolling.pyx":252
  * 
  * 
  * def roll_min(ndarray[float64_t] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     """
  */
-  __pyx_tuple__28 = PyTuple_Pack(4, __pyx_n_s_values, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(4, __pyx_n_s_values, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_min, 253, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_min, 252, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 252, __pyx_L1_error)
 
-  /* "torchqtm/_C/_rolling.pyx":394
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":395
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_mean(const float64_t[:] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *               ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     cdef:
  */
-  __pyx_tuple__30 = PyTuple_Pack(17, __pyx_n_s_values, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_val, __pyx_n_s_compensation_add, __pyx_n_s_compensation_remove, __pyx_n_s_sum_x, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_nobs, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_neg_ct, __pyx_n_s_N, __pyx_n_s_output, __pyx_n_s_is_monotonic_increasing_bounds); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 394, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(17, __pyx_n_s_values, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_val, __pyx_n_s_compensation_add, __pyx_n_s_compensation_remove, __pyx_n_s_sum_x, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_nobs, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_neg_ct, __pyx_n_s_N, __pyx_n_s_output, __pyx_n_s_is_monotonic_increasing_bounds); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(4, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_mean, 394, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 394, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(4, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_mean, 395, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 395, __pyx_L1_error)
 
-  /* "torchqtm/_C/_rolling.pyx":444
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":447
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_1D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
-  __pyx_tuple__32 = PyTuple_Pack(15, __pyx_n_s_obj, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_function, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_output, __pyx_n_s_counts, __pyx_n_s_arr, __pyx_n_s_i, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_N, __pyx_n_s_n); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(15, __pyx_n_s_obj, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_function, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_output, __pyx_n_s_counts, __pyx_n_s_arr, __pyx_n_s_i, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_N, __pyx_n_s_n); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__32);
   __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(7, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_apply_1D, 444, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(7, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_apply_1D, 447, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 447, __pyx_L1_error)
 
-  /* "torchqtm/_C/_rolling.pyx":484
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":489
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_2D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
-  __pyx_tuple__34 = PyTuple_Pack(16, __pyx_n_s_obj, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_function, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_output, __pyx_n_s_counts, __pyx_n_s_arr, __pyx_n_s_i, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_N, __pyx_n_s_n, __pyx_n_s_n_col); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(16, __pyx_n_s_obj, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_function, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_output, __pyx_n_s_counts, __pyx_n_s_arr, __pyx_n_s_i, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_N, __pyx_n_s_n, __pyx_n_s_n_col); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 489, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(7, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_apply_2D, 484, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(7, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_apply_2D, 489, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 489, __pyx_L1_error)
 
-  /* "torchqtm/_C/_rolling.pyx":526
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":533
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_3D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
-  __pyx_tuple__36 = PyTuple_Pack(17, __pyx_n_s_obj, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_function, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_output, __pyx_n_s_counts, __pyx_n_s_arr, __pyx_n_s_i, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_N, __pyx_n_s_n, __pyx_n_s_n_stocks, __pyx_n_s_n_features); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 526, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(17, __pyx_n_s_obj, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_minp, __pyx_n_s_function, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_output, __pyx_n_s_counts, __pyx_n_s_arr, __pyx_n_s_i, __pyx_n_s_s, __pyx_n_s_e, __pyx_n_s_N, __pyx_n_s_n, __pyx_n_s_n_stocks, __pyx_n_s_n_features); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(7, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_apply_3D, 526, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 526, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(7, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_apply_3D, 533, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 533, __pyx_L1_error)
 
-  /* "torchqtm/_C/_rolling.pyx":562
- *     return output
- * 
+  /* "torchqtm/_C/_rolling.pyx":572
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_weighted_sum(             # <<<<<<<<<<<<<<
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  */
-  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_values, __pyx_n_s_weights, __pyx_n_s_minp); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_values, __pyx_n_s_weights, __pyx_n_s_minp); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_weighted_sum, 562, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_weighted_sum, 572, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 572, __pyx_L1_error)
 
-  /* "torchqtm/_C/_rolling.pyx":568
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":580
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_weighted_mean(             # <<<<<<<<<<<<<<
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  */
-  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_n_s_values, __pyx_n_s_weights, __pyx_n_s_minp); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_n_s_values, __pyx_n_s_weights, __pyx_n_s_minp); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_weighted_mean, 568, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_torchqtm__C__rolling_pyx, __pyx_n_s_roll_weighted_mean, 580, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 580, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -26258,239 +26719,238 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "torchqtm/_C/_rolling.pyx":3
- * # cython: boundscheck=False, wraparound=False, cdivision=True, language_level=3,
+  /* "torchqtm/_C/_rolling.pyx":2
  * # distutils: language=c++
  * from typing import Type             # <<<<<<<<<<<<<<
  * 
  * import numpy as np
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Type);
   __Pyx_GIVEREF(__pyx_n_s_Type);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Type);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Type, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Type, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":5
+  /* "torchqtm/_C/_rolling.pyx":4
  * from typing import Type
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as cnp
  * import cython
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":52
+  /* "torchqtm/_C/_rolling.pyx":51
  * 
  * cdef:
  *     float32_t MINfloat32 = np.NINF             # <<<<<<<<<<<<<<
  *     float64_t MINfloat64 = np.NINF
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NINF); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NINF); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __pyx_PyFloat_AsFloat(__pyx_t_1); if (unlikely((__pyx_t_3 == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_3 = __pyx_PyFloat_AsFloat(__pyx_t_1); if (unlikely((__pyx_t_3 == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_8torchqtm_2_C_8_rolling_MINfloat32 = __pyx_t_3;
 
-  /* "torchqtm/_C/_rolling.pyx":53
+  /* "torchqtm/_C/_rolling.pyx":52
  * cdef:
  *     float32_t MINfloat32 = np.NINF
  *     float64_t MINfloat64 = np.NINF             # <<<<<<<<<<<<<<
  * 
  *     float32_t MAXfloat32 = np.inf
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NINF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NINF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_8torchqtm_2_C_8_rolling_MINfloat64 = __pyx_t_4;
 
-  /* "torchqtm/_C/_rolling.pyx":55
+  /* "torchqtm/_C/_rolling.pyx":54
  *     float64_t MINfloat64 = np.NINF
  * 
  *     float32_t MAXfloat32 = np.inf             # <<<<<<<<<<<<<<
  *     float64_t MAXfloat64 = np.inf
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_inf); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_inf); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __pyx_PyFloat_AsFloat(__pyx_t_1); if (unlikely((__pyx_t_3 == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_3 = __pyx_PyFloat_AsFloat(__pyx_t_1); if (unlikely((__pyx_t_3 == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_8torchqtm_2_C_8_rolling_MAXfloat32 = __pyx_t_3;
 
-  /* "torchqtm/_C/_rolling.pyx":56
+  /* "torchqtm/_C/_rolling.pyx":55
  * 
  *     float32_t MAXfloat32 = np.inf
  *     float64_t MAXfloat64 = np.inf             # <<<<<<<<<<<<<<
  * 
  *     float64_t NaN = <float64_t>np.NaN
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_inf); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_inf); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_8torchqtm_2_C_8_rolling_MAXfloat64 = __pyx_t_4;
 
-  /* "torchqtm/_C/_rolling.pyx":58
+  /* "torchqtm/_C/_rolling.pyx":57
  *     float64_t MAXfloat64 = np.inf
  * 
  *     float64_t NaN = <float64_t>np.NaN             # <<<<<<<<<<<<<<
  * 
  * ctypedef struct node_t:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NaN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NaN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_8torchqtm_2_C_8_rolling_NaN = ((__pyx_t_5numpy_float64_t)__pyx_t_4);
 
-  /* "torchqtm/_C/_rolling.pyx":180
+  /* "torchqtm/_C/_rolling.pyx":179
  * 
  * 
  * def roll_sum(const float64_t[:] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     cdef:
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_1roll_sum, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_1roll_sum, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_sum, __pyx_t_1) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_sum, __pyx_t_1) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":229
+  /* "torchqtm/_C/_rolling.pyx":228
  * 
  * 
  * def roll_max(ndarray[float64_t] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     """
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_3roll_max, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_3roll_max, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_max, __pyx_t_1) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_max, __pyx_t_1) < 0) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":253
+  /* "torchqtm/_C/_rolling.pyx":252
  * 
  * 
  * def roll_min(ndarray[float64_t] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *              ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     """
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_5roll_min, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_5roll_min, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_min, __pyx_t_1) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_min, __pyx_t_1) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":394
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":395
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_mean(const float64_t[:] values, ndarray[int64_t] start,             # <<<<<<<<<<<<<<
  *               ndarray[int64_t] end, int64_t minp) -> np.ndarray:
  *     cdef:
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_7roll_mean, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_7roll_mean, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_mean, __pyx_t_1) < 0) __PYX_ERR(0, 394, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_mean, __pyx_t_1) < 0) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":444
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":447
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_1D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_9roll_apply_1D, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_9roll_apply_1D, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_apply_1D, __pyx_t_1) < 0) __PYX_ERR(0, 444, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_apply_1D, __pyx_t_1) < 0) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":484
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":489
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_2D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_11roll_apply_2D, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_11roll_apply_2D, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 489, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_apply_2D, __pyx_t_1) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_apply_2D, __pyx_t_1) < 0) __PYX_ERR(0, 489, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":526
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":533
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_apply_3D(object obj,             # <<<<<<<<<<<<<<
  *                   ndarray[int64_t] start,
  *                   ndarray[int64_t] end,
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_13roll_apply_3D, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 526, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_13roll_apply_3D, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_apply_3D, __pyx_t_1) < 0) __PYX_ERR(0, 526, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_apply_3D, __pyx_t_1) < 0) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":562
- *     return output
- * 
+  /* "torchqtm/_C/_rolling.pyx":572
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_weighted_sum(             # <<<<<<<<<<<<<<
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_15roll_weighted_sum, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_15roll_weighted_sum, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_weighted_sum, __pyx_t_1) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_weighted_sum, __pyx_t_1) < 0) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "torchqtm/_C/_rolling.pyx":568
- * 
- * 
+  /* "torchqtm/_C/_rolling.pyx":580
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
  * def roll_weighted_mean(             # <<<<<<<<<<<<<<
  *     const float64_t[:] values, const float64_t[:] weights, int minp
  * ) -> np.ndaray:
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_17roll_weighted_mean, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8torchqtm_2_C_8_rolling_17roll_weighted_mean, NULL, __pyx_n_s_torchqtm__C__rolling); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_weighted_mean, __pyx_t_1) < 0) __PYX_ERR(0, 568, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_roll_weighted_mean, __pyx_t_1) < 0) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "torchqtm/_C/_rolling.pyx":1
- * # cython: boundscheck=False, wraparound=False, cdivision=True, language_level=3,             # <<<<<<<<<<<<<<
- * # distutils: language=c++
+ * # distutils: language=c++             # <<<<<<<<<<<<<<
  * from typing import Type
+ * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "View.MemoryView":210
@@ -27536,14 +27996,31 @@
 
 /* BufferFallbackError */
   static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
 }
 
+/* BufferIndexError */
+  static void __Pyx_RaiseBufferIndexError(int axis) {
+  PyErr_Format(PyExc_IndexError,
+     "Out of bounds on buffer access (axis %d)", axis);
+}
+
+/* BufferIndexErrorNogil */
+  static void __Pyx_RaiseBufferIndexErrorNogil(int axis) {
+    #ifdef WITH_THREAD
+    PyGILState_STATE gilstate = PyGILState_Ensure();
+    #endif
+    __Pyx_RaiseBufferIndexError(axis);
+    #ifdef WITH_THREAD
+    PyGILState_Release(gilstate);
+    #endif
+}
+
 /* PyErrFetchRestore */
   #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
@@ -27692,14 +28169,54 @@
             PyGILState_Release(_gilstate);
         }
     } else {
         memslice->memview = NULL;
     }
 }
 
+/* WriteUnraisableException */
+  static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* PyCFunctionFastCall */
   #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
     PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
     PyCFunction meth = PyCFunction_GET_FUNCTION(func);
     PyObject *self = PyCFunction_GET_SELF(func);
     int flags = PyCFunction_GET_FLAGS(func);
@@ -28567,14 +29084,22 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
+/* DivInt[Py_ssize_t] */
+  static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t a, Py_ssize_t b) {
+    Py_ssize_t q = a / b;
+    Py_ssize_t r = a - q*b;
+    q -= ((r != 0) & ((r ^ b) < 0));
+    return q;
+}
+
 /* GetAttr */
   static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
 #if CYTHON_USE_TYPE_SLOTS
 #if PY_MAJOR_VERSION >= 3
     if (likely(PyUnicode_Check(n)))
 #else
     if (likely(PyString_Check(n)))
@@ -28970,14 +29495,22 @@
             PyFPE_END_PROTECT(result)
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
+/* DivInt[long] */
+  static CYTHON_INLINE long __Pyx_div_long(long a, long b) {
+    long q = a / b;
+    long r = a - q*b;
+    q -= ((r != 0) & ((r ^ b) < 0));
+    return q;
+}
+
 /* ImportFrom */
   static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
     PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
     if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Format(PyExc_ImportError,
         #if PY_MAJOR_VERSION < 3
             "cannot import name %.230s", PyString_AS_STRING(name));
```

### Comparing `torchqtm-0.1.0/torchqtm/_libs/tslibs/__init__.py` & `torchqtm-0.2.0/torchqtm/_libs/tslibs/__init__.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/alphas/alphas.py` & `torchqtm-0.2.0/torchqtm/alphas/alphas.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/alphas/ml.py` & `torchqtm-0.2.0/torchqtm/alphas/ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torchqtm.op as op
 import torchqtm.op.functional as F
 from torchqtm.op.functional import *
 import pandas as pd
 import numpy as np
 from abc import ABCMeta, abstractmethod
-from torchqtm.vbt.backtest import BackTestEnv
+from torchqtm.tdbt.backtest import BackTestEnv
 from torchqtm.base import BaseAlpha
 
 
 class MLAlpha(BaseAlpha):
     def __init__(self, env: BackTestEnv, model=None, *args, **kwargs):
         super().__init__(env, *args, **kwargs)
         self.type = 'machine learning alpha'
```

### Comparing `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/_program.py` & `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/_program.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/fitness.py` & `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/fitness.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 __all__ = ['make_fitness']
 
 
 class _Fitness(object):
 
     """A metric to measure the fitness of a program.
 
-    This object is able to be called with NumPy torchquantum arguments and return
+    This object is able to be called with NumPy torchqtm arguments and return
     a resulting floating point score quantifying the quality of the program's
     representation of the true relationship.
 
     Parameters
     ----------
     function : callable
         A function with signature function(y, y_pred, sample_weight) that
@@ -51,15 +51,15 @@
 
 def make_fitness(*, function, greater_is_better, wrap=True):
     """Make a fitness measure, a metric scoring the quality of a program's fit.
 
     This factory function creates a fitness measure object which measures the
     quality of a program's fit and thus its likelihood to undergo genetic
     operations into the next generation. The resulting object is able to be
-    called with NumPy torchquantum arguments and return a resulting floating
+    called with NumPy torchqtm arguments and return a resulting floating
     point score quantifying the quality of the program's representation of the
     true relationship.
 
     Parameters
     ----------
     function : callable
         A function with signature function(y, y_pred, sample_weight) that
```

### Comparing `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/functions.py` & `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 __all__ = ['make_function']
 
 
 class _Function(object):
     """A representation of a mathematical relationship, a node in a program.
 
-    This object is able to be called with NumPy torchquantum arguments and return
+    This object is able to be called with NumPy torchqtm arguments and return
     a resulting vector based on a mathematical relationship.
 
     Parameters
     ----------
     function : callable
         A function with signature function(x1, *args) that returns a Numpy
         array of the same shape as its arguments.
@@ -48,15 +48,15 @@
         return self.function(*args)
 
 
 def make_function(*, function, name, arity, wrap=True):
     """Make a function node, a representation of a mathematical relationship.
 
     This factory function creates a function node, one of the core nodes in any
-    program. The resulting object is able to be called with NumPy torchquantum
+    program. The resulting object is able to be called with NumPy torchqtm
     arguments and return a resulting vector based on a mathematical
     relationship.
 
     Parameters
     ----------
     function : callable
         A function with signature `function(x1, *args)` that returns a Numpy
```

### Comparing `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/genetic.py` & `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/genetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from ._program import _Program
 from .fitness import _fitness_map, _Fitness
 from .functions import _function_map, _Function, sig1 as sigmoid
 from .utils import _partition_estimators
 from .utils import check_random_state
 import copy
-from torchqtm.vbt.backtest import BaseTest
+from torchqtm.tdbt.backtest import BaseTester
 
 __all__ = ['SymbolicRegressor', 'SymbolicClassifier', 'SymbolicTransformer']
 
 MAX_INT = np.iinfo(np.int32).max
 
 
 def _parallel_evolve(n_programs, parents, X, y, sample_weight, seeds, params):
@@ -50,15 +50,15 @@
     metric = params['_metric']
     transformer = params['_transformer']
     parsimony_coefficient = params['parsimony_coefficient']
     method_probs = params['method_probs']
     p_point_replace = params['p_point_replace']
     max_samples = params['max_samples']
     feature_names = params['feature_names']
-    strategy: BaseTest = params['strategy']
+    strategy: BaseTester = params['strategy']
     max_samples = int(max_samples * n_samples)
 
     def _tournament():
         """Find the fittest individual from a sub-population."""
         contenders = random_state.randint(0, len(parents), tournament_size)
         fitness = [parents[p].fitness_ for p in contenders]
         if metric.greater_is_better:
@@ -190,15 +190,15 @@
                  class_weight=None,
                  feature_names=None,
                  warm_start=False,
                  low_memory=False,
                  n_jobs=1,
                  verbose=0,
                  random_state=None,
-                 strategy: BaseTest = None,
+                 strategy: BaseTester = None,
                  ):
         self.population_size = population_size
         self.hall_of_fame = hall_of_fame
         self.n_components = n_components
         self.generations = generations
         self.tournament_size = tournament_size
         self.stopping_criteria = stopping_criteria
@@ -218,15 +218,15 @@
         self.class_weight = class_weight
         self.feature_names = feature_names
         self.warm_start = warm_start
         self.low_memory = low_memory
         self.n_jobs = n_jobs
         self.verbose = verbose
         self.random_state = random_state
-        self.strategy: BaseTest = strategy
+        self.strategy: BaseTester = strategy
         self.n_features_in_ = ...
         self._function_set = ...
         self._arities = ...
 
     def _verbose_reporter(self, run_details=None):
         """A report of the progress of the evolution process.
 
@@ -815,15 +815,15 @@
                  max_samples=1.0,
                  feature_names=None,
                  warm_start=False,
                  low_memory=False,
                  n_jobs=1,
                  verbose=0,
                  random_state=None,
-                 strategy: BaseTest = None):
+                 strategy: BaseTester = None):
         super(SymbolicRegressor, self).__init__(
             population_size=population_size,
             generations=generations,
             tournament_size=tournament_size,
             stopping_criteria=stopping_criteria,
             const_range=const_range,
             init_depth=init_depth,
```

### Comparing `torchqtm-0.1.0/torchqtm/autoalpha/gplearn/utils.py` & `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/utils.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/base.py` & `torchqtm-0.2.0/torchqtm/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from abc import ABCMeta, abstractmethod
 from torchqtm.utils.universe import Universe
 import pandas as pd
 import numpy as np
 from typing import Dict, Hashable
 from abc import ABCMeta, abstractmethod
-from typing import Iterable
+from typing import Iterable, Callable
+from collections import OrderedDict
+from torchqtm.utils._decorators import ContextManager
+from torchqtm.utils.warnings import catch_warnings
 
 
 class BackTestEnv(object):
     """
     # We can create two different BackTestEnvs
     # 1. For Op, we create env with trade_dates
     # 2. For backtest, we create env with rebalance_dates
@@ -35,78 +38,83 @@
         self.Close = None
         self.Volume = None
         self.Returns = None
         self.Vwap = None
         self.MktVal = None
         self.PE = None
         self.Sector = None
-        self._FutureReturn = None
+        self.forward_returns = None
         self._create_datas()
         self._create_features()
 
     def _check_dfs(self):
         """
         check is dfs is a valid dict
         :return: None
         """
         # assert 'close' in self.dfs
         assert 'MktVal' in self.dfs
         assert 'Sector' in self.dfs
 
     def _create_datas(self):
-        self.datas = {}
+        self.data = {}
         for key in self.dfs:
             if isinstance(self.dfs[key], pd.DataFrame):
-                self.datas[key] = self.dfs[key].loc[self.dates, self.symbols]
+                self.data[key] = self.dfs[key].loc[self.dates, self.symbols]
             else:
-                self.datas[key] = self.dfs[key]
-        self.datas['_FutureReturn'] = self.datas['Close'].pct_change().shift(-1)
+                self.data[key] = self.dfs[key]
+
+    def create_forward_returns(self, D=1):
+        forward_returns = self.data['Close'].pct_change().shift(-1)
+        return forward_returns
 
     def _create_features(self):
         """
         Create the reference to the dict values
         :return:
         """
-        for key in self.datas.keys():
-            setattr(self, key, self.datas[key])
-        setattr(self, '_FutureReturn', self.datas['_FutureReturn'])
+        for key in self.data.keys():
+            setattr(self, key, self.data[key])
 
     def __getitem__(self, item):
         """
         Keep the operator[]
         :param item:
         :return:
         """
-        return self.datas[item]
+        return self.data[item]
 
     def __setitem__(self, item, value):
         """
         Keep the operator[]
         :param item:
         :return:
         """
         assert isinstance(value, pd.DataFrame)
-        self.datas[item] = value
+        self.data[item] = value
         setattr(self, item, value)
 
     def __delitem__(self, item):
-        del self.datas[item]
+        del self.data[item]
         delattr(self, item)
 
     def __contains__(self, item):
-        return item in self.datas
+        return item in self.data
 
-    def match_env(self, factor):
+    def match(self, factor):
         return factor.loc[self.dates, self.symbols]
 
 
 class Parameter(np.ndarray, metaclass=ABCMeta):
-    def __new__(cls, data: int, required_optim: bool = False, feasible_region: Iterable[int] = None):
+    def __new__(cls,
+                data: int,
+                requires_optim: bool = False,
+                feasible_region: Iterable[int] = None):
         obj = np.asarray(data).view(cls)
-        obj.required_optim = required_optim
+        obj.required_optim = requires_optim
         obj.feasible_region = feasible_region
         obj._check_data()
         return obj
 
     def __array_finalize__(self, obj):
         if obj is None: return
         self.required_optim = getattr(obj, 'required_optim', None)
@@ -117,14 +125,17 @@
             raise ValueError("must provide possible values for search")
 
 
 __TYPES = ['momentum', 'reversion']
 
 
 class BaseOperator(object, metaclass=ABCMeta):
+
+    catch_warnings = False
+
     def __init__(self, *args, **kwargs):
         pass
 
     @abstractmethod
     def forward(self, *args, **kwargs):
         """assign self.rawdata and return"""
         raise NotImplementedError
@@ -132,25 +143,25 @@
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
 
 
 class BaseAlpha(BaseOperator, metaclass=ABCMeta):
 
     __DATA_AVAILABLE__ = ['open', 'high', 'low', 'close', 'volume',
-                          'return', 'vwap', 'adv20', 'sector']
+                          'returns', 'vwap', 'adv20', 'sector']
 
     def __init__(self, env: BackTestEnv, *args, **kwargs):
 
         super().__init__(*args, **kwargs)
         self.env = env
         self.args = args
         self.kwargs = kwargs
         self.data = None
         self.type = None
-        self.USED = True  # default to be used
+        self.Enabled = True  # default to be used
 
     @abstractmethod
     def forward(self, *args, **kwargs):
         """assign self.rawdata and return"""
         raise NotImplementedError
 
     def __eq__(self, other):
@@ -233,10 +244,20 @@
 
     @abstractmethod
     def forward(self, *args, **kwargs):
         """assign self.rawdata and return"""
         raise NotImplementedError
 
 
+class Technical(BaseAlpha):
+    def __init__(self, env: BackTestEnv, *args, **kwargs):
+        super().__init__(env, *args, **kwargs)
+        self.type = 'technical'
+
+    @abstractmethod
+    def forward(self, *args, **kwargs):
+        """assign self.rawdata and return"""
+        raise NotImplementedError
+
```

### Comparing `torchqtm-0.1.0/torchqtm/core/window/rolling.py` & `torchqtm-0.2.0/torchqtm/core/window/rolling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from torchqtm._C._rolling import *
-from torchqtm._libs.window.aggregations import (
+from pandas._libs.window.aggregations import (
     roll_rank,
     roll_quantile,
     roll_kurt,
     roll_var,
-    roll_weighted_sum)
+    roll_weighted_sum
+)
+from pandas._libs.algos import rank_1d, rank_2d
 import numpy as np
 from typing import Callable, Union
 from numpy.typing import NDArray
 import datetime
 import functools
-from pandas._libs.algos import rank_1d, rank_2d
+
 
 # PythonScalar = Union[str, float, bool]
 # DatetimeLikeScalar = Union["Period", "Timestamp", "Timedelta"]
 # PandasScalar = Union["Period", "Timestamp", "Timedelta", "Interval"]
 # Scalar = Union[PythonScalar, PandasScalar, np.datetime64, np.timedelta64, datetime]
 
 
-@functools.lru_cache(maxsize=None)
+# @functools.lru_cache(maxsize=None)
 def get_window_bounds(num_values, window_size):
     offset = 0
     end = np.arange(1 + offset, num_values + 1 + offset, 1, dtype=np.int64)
     start = end - window_size
     end = np.clip(end, 0, num_values)
     start = np.clip(start, 0, num_values)
     return start, end
@@ -85,15 +87,15 @@
     aux_func = roll_mean
     helper_func = lambda x: np.nanmean(x, axis=0)
 
     if array.ndim == 1:
         return aux_func(array, start, end, window_size)
     if mode == "auto":
         if array.ndim == 2:
-            if window_size > 10:  # 这里使用500是个经验法则了吧
+            if window_size > 20 or array.shape[1] < 20:  # 这里使用500是个经验法则了吧
                 rlt = np.empty_like(array)
                 for i in range(array.shape[1]):
                     rlt[:, i] = aux_func(array[:, i], start, end, window_size)
                 return rlt
             else:
                 return roll_apply_2D(array, start, end, window_size, helper_func, (), {})
         else:
```

### Comparing `torchqtm-0.1.0/torchqtm/edbt/account.py` & `torchqtm-0.2.0/torchqtm/edbt/temp/account.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/edbt/backtest.py` & `torchqtm-0.2.0/torchqtm/edbt/temp/backtest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from account import VirtualAccount
+from torchqtm.edbt.temp.account import VirtualAccount
 from abc import ABCMeta, abstractmethod
 from collections.abc import Iterable
-from datahandler import BarData
+from torchqtm.edbt.temp.datahandler import BarData
 from mycalendar import Calendar
 import pandas as pd
 
 
 class BacktestEngine(object, metaclass=ABCMeta):
 
     def __init__(self, bars: BarData, accounts_names: Iterable[str]):
```

### Comparing `torchqtm-0.1.0/torchqtm/edbt/datahandler.py` & `torchqtm-0.2.0/torchqtm/edbt/temp/datahandler.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/edbt/test.py` & `torchqtm-0.2.0/torchqtm/edbt/temp/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from matplotlib import gridspec
 import numpy as np
 import pandas as pd
-from datahandler import BarData, MultiBarData, ModifiedBarData
-from backtest import BacktestEngine
+from torchqtm.edbt.temp.datahandler import BarData
+from torchqtm.edbt.temp.backtest import BacktestEngine
 from sklearn.linear_model import LinearRegression
 import statsmodels.api as sm
 
 lm = LinearRegression()
 factor_name = 'fom123_mean'
```

### Comparing `torchqtm-0.1.0/torchqtm/op/_numba.py` & `torchqtm-0.2.0/torchqtm/op/_numba.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/op/functional.py` & `torchqtm-0.2.0/torchqtm/op/functional.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,31 @@
 from sklearn.linear_model import LinearRegression
 
 from ..config import __OP_MODE__
 from typing import overload
 from .algos import rank_1d, rank_2d
 from scipy.stats import norm
 import talib
+import typing
+
+CORR_METHOD = typing.Literal["pearson", "spearman"]
+
 
 # Arithmetic Operators
 
 
+def revert_type(raw, target):
+    if isinstance(target, np.ndarray):
+        return raw.values
+    elif isinstance(target, pd.Series):
+        return pd.Series(raw, index=target.index, name=target.name)
+    elif isinstance(target, pd.DataFrame):
+        return pd.DataFrame(raw, index=target.index, columns=target.columns)
+
+
 def abs(x):
     """absolute value of x"""
     if isinstance(x, pd.DataFrame):
         return np.abs(x)
     elif isinstance(x, np.ndarray):
         return np.abs(x)
 
@@ -85,28 +98,42 @@
     return np.log(X)
 
 
 def log_diff(X):
     return np.log(X / ts_delay(X, 1))
 
 
+def max(X, Y):
+    condition = X > Y
+    value_if_true = X
+    value_if_false = Y
+    return if_else(condition, value_if_true, value_if_false)
+
+
+def min(X, Y):
+    condition = X <= Y
+    value_if_true = X
+    value_if_false = Y
+    return if_else(condition, value_if_true, value_if_false)
+
+
 def nan_out(X, lower=-0.1, upper=0.1):
     """set returns outside of [lower, upper] to nan"""
     rlt = np.where(((X < lower) + (X > upper)) > 0, np.nan, X)
     if isinstance(rlt, np.ndarray):
         return rlt
     elif isinstance(rlt, pd.DataFrame):
         return pd.DataFrame(rlt, index=X.index, columns=X.columns)
 
 
 def purify(X):
     rlt = np.where(np.isinf(X), np.nan, X)
-    if isinstance(rlt, np.ndarray):
+    if isinstance(X, np.ndarray):
         return rlt
-    elif isinstance(rlt, pd.DataFrame):
+    elif isinstance(X, pd.DataFrame):
         return pd.DataFrame(rlt, index=X.index, columns=X.columns)
 
 
 def sign(X):
     rlt = np.where(X > 0, 1, X)
     rlt = np.where(X < 0, -1, rlt)
     rlt = np.where(X == 0, 0, rlt)
@@ -136,17 +163,17 @@
     pass
 
 
 # Logical Operators
 # TODO: 1231
 def if_else(condition, value_if_true, value_if_false):
     rlt = np.where(condition, value_if_true, value_if_false)
-    if isinstance(rlt, np.ndarray):
+    if isinstance(condition, np.ndarray):
         return rlt
-    elif isinstance(rlt, pd.DataFrame):
+    elif isinstance(condition, pd.DataFrame):
         return pd.DataFrame(rlt, index=condition.index, columns=condition.columns)
 
 
 def logical_and(x, y):
     return np.logical_and(x, y)
 
 
@@ -252,15 +279,15 @@
 
 
 def days_from_last_change(x, d):
     pass
 
 
 def ts_weighted_delay(x, k=0.5):
-    return add(k * x, (1-k) * ts_delay(x, 1))
+    return add(k * x, (1 - k) * ts_delay(x, 1))
 
 
 # 这俩函数有点抽象, 后边想想怎么实现
 # def hump(x, hump=0.01):
 #     """
 #     This operator limits amount and magnitude of changes in input
 #     (thus reducing turnover). If input changed by less than a threshold
@@ -282,28 +309,41 @@
 
 
 def jump_decay(x, d, sensitivity=0.5, force=0.1):
     """
     If there is a huge jump in current data compare to previous one, apply force:
     我认为作用是滤平变动
     """
-    cond = abs(x-ts_delay(x, 1) > sensitivity * ts_std_dev(x, d))
+    cond = abs(x - ts_delay(x, 1) > sensitivity * ts_std_dev(x, d))
     value_if_true = ts_delay(x, 1) + ts_delta(x, 1) * force
     value_if_false = x
     return if_else(cond, value_if_true, value_if_false)
 
 
 def kth_element(x, d, k):
     pass
 
 
 def last_diff_value(x, d):
     pass
 
 
+# def ts_arg_min(x, d):
+#     def aux_func(t):
+#         return np.nanargmin(t[::-1], axis=0)
+#     if len(x.shape) == 2 and x.shape[1] <= 301:
+#         raw = pd.DataFrame(x).rolling(d).argmin()
+#         return convert_type(raw, x)
+#     elif len(x.shape) == 1:
+#         raw = pd.Series(x).rolling(d).argmin()
+#         return convert_type(raw, x)
+#     else:
+#         return ts_apply(x, d, aux_func)
+
+
 def ts_arg_min(x, d):
     def aux_func(t):
         return np.nanargmin(t[::-1], axis=0)
 
     return ts_apply(x, d, aux_func)
 
 
@@ -326,22 +366,31 @@
     pass
 
 
 def _ts_corr_single(x, y, d):
     pass
 
 
-def ts_corr(x, y, d):
+def ts_corr(x, y, d: int, method: CORR_METHOD = "pearson"):
     """
     Pearson correlation of x, y in the past d days.
     """
-    if len(x.shape) == 2:
-        rlt = pd.DataFrame(x).rolling(d).corr(pd.DataFrame(y))
+    if method == "pearson":
+        if len(x.shape) == 2:
+            rlt = pd.DataFrame(x).rolling(d).corr(pd.DataFrame(y))
+        else:
+            rlt = pd.Series(x).rolling(d).corr(pd.Series(y))
+    elif method == "spearman":
+        if len(x.shape) == 2:
+            rlt = pd.DataFrame(x).rank().rolling(d).corr(pd.DataFrame(y).rank())
+        else:
+            rlt = pd.Series(x).rank().rolling(d).corr(pd.Series(y).rank())
     else:
-        rlt = pd.Series(x).rolling(d).corr(pd.Series(y))
+        raise ValueError
+
     if isinstance(x, np.ndarray):
         return rlt.values
     elif isinstance(x, pd.Series):
         return pd.Series(rlt.values, index=x.index, name=x.name)
     elif isinstance(x, pd.DataFrame):
         return pd.DataFrame(rlt.values, index=x.index, columns=x.columns)
 
@@ -364,16 +413,17 @@
 def ts_decay_exp_window(x, d, factor):
     pass
 
 
 def ts_decay_linear(x, d, dense=False):
     # TODO: 想想怎么改进这个矩阵乘法, 目前会产生大量的NA
     def aux_func(data_slice):
-        filters = np.arange(1, d+1) / ( d * (d + 2) / 2 )
+        filters = np.arange(1, d + 1) / (d * (d + 2) / 2)
         return np.matmul(data_slice.T, filters)
+
     return ts_apply(x, d, aux_func)
 
 
 def ts_std_dev(x, d):
     def aux_func(t):
         return np.nanstd(t, axis=0)
 
@@ -391,14 +441,15 @@
 def ts_max_diff(x, d):
     return sub(x, ts_max(x, d))
 
 
 def ts_median(x, d):
     def aux_func(t):
         return np.nanmedian(x, axis=0)
+
     return ts_apply(x, d, aux_func)
 
 
 def ts_min_diff(x, d):
     return x - ts_min(x, d)
 
 
@@ -434,25 +485,32 @@
         return np.nanprod(x, axis=0)
 
     return ts_apply(x, d, aux_func)
 
 
 def ts_rank(x, d, mode="auto"):
     def aux_func(array, window_size):
-        return roll_apply_rank(array, window_size, method=mode)
+        return roll_apply_rank(array, window_size, mode=mode)
 
     if isinstance(x, np.ndarray):
         return aux_func(x, d)
     elif isinstance(x, pd.Series):
         return pd.Series(aux_func(x.values, d), index=x.index, name=x.name)
     elif isinstance(x, pd.DataFrame):
         return pd.DataFrame(aux_func(x.values, d), index=x.index, columns=x.columns)
 
 
-def ts_regression(y, x, d, lag=0, rettype=0):
+def ts_beta(y, x, d, lag=0):
+    """
+    y 允许 多个纬度, x只能有一个纬度, 否则不是well-defined
+    """
+    pass
+
+
+def ts_regression(y, d, lag=0, rettype=0):
     pass
 
 
 def ts_returns(x, d):
     return (x - ts_delay(x, d)) / ts_delay(x, d)
 
 
@@ -614,26 +672,26 @@
 
 
 def _winsorize(X, method, param):
     assert isinstance(X, np.ndarray)
     n_stocks = X.shape[-1]
     n_axis = len(X.shape)
     if method == 'quantile':
-        lower_bound = np.nanquantile(X, param, axis=n_axis-1, keepdims=True)
-        upper_bound = np.nanquantile(X, 1-param, axis=n_axis-1, keepdims=True)
+        lower_bound = np.nanquantile(X, param, axis=n_axis - 1, keepdims=True)
+        upper_bound = np.nanquantile(X, 1 - param, axis=n_axis - 1, keepdims=True)
     elif method == 'std':
-        mean = np.nanmean(X, axis=n_axis-1, keepdims=True)
-        std = np.nanstd(X, axis=n_axis-1, keepdims=True)
+        mean = np.nanmean(X, axis=n_axis - 1, keepdims=True)
+        std = np.nanstd(X, axis=n_axis - 1, keepdims=True)
         lower_bound = mean - std * param
         upper_bound = mean + std * param
     else:
         raise ValueError('Unknown method')
     return np.clip(a=X,
-                   a_min=np.repeat(lower_bound, n_stocks, axis=n_axis-1),
-                   a_max=np.repeat(upper_bound, n_stocks, axis=n_axis-1))
+                   a_min=np.repeat(lower_bound, n_stocks, axis=n_axis - 1),
+                   a_max=np.repeat(upper_bound, n_stocks, axis=n_axis - 1))
 
 
 def winsorize(X, method='quantile', param=0.05):
     aux_func = _winsorize
     if isinstance(X, np.ndarray):
         return aux_func(X, method, param)
     elif isinstance(X, pd.Series):
@@ -642,20 +700,20 @@
         return pd.DataFrame(aux_func(X.values, method, param), index=X.index, columns=X.columns)
 
 
 def _normalize(X, useStd):
     assert isinstance(X, np.ndarray)
     n_axis = len(X.shape)
     n_stocks = X.shape[-1]
-    x_mean = np.nanmean(X, axis=n_axis-1, keepdims=True)
-    s_std = np.nanstd(X, axis=n_axis-1, keepdims=True)
+    x_mean = np.nanmean(X, axis=n_axis - 1, keepdims=True)
+    s_std = np.nanstd(X, axis=n_axis - 1, keepdims=True)
     if useStd:
-        return (X - np.repeat(x_mean, n_stocks, axis=n_axis-1)) / np.repeat(s_std, n_stocks, axis=n_axis-1)
+        return (X - np.repeat(x_mean, n_stocks, axis=n_axis - 1)) / np.repeat(s_std, n_stocks, axis=n_axis - 1)
     else:
-        return X - np.repeat(x_mean, n_stocks, axis=n_axis-1)
+        return X - np.repeat(x_mean, n_stocks, axis=n_axis - 1)
 
 
 def normalize(X, useStd=True):
     aux_func = _normalize
     if isinstance(X, np.ndarray):
         return aux_func(X, useStd)
     elif isinstance(X, pd.Series):
@@ -773,15 +831,15 @@
     return np.arctan(x)
 
 
 # def bucket(rank(x), range="0, 1, 0.1" or buckets = "2,5,6,7,10")
 
 # def clamp(x, lower = 0, upper = 0, inverse = False, mask = ")
 
-def filter(x, h = "1, 2, 3, 4", t="0.5"):
+def filter(x, h="1, 2, 3, 4", t="0.5"):
     pass
 
 
 def keep(x, f, period=5):
     pass
 
 
@@ -808,15 +866,16 @@
 
 
 def tail(x, lower=0, upper=0.5, newval=np.nan):
     cond = logical_or(less(x, lower), more(x, upper))
     return if_else(cond, x, np.nan)
 
 
-# TODO: 保持变量类型封闭
+# TODO: 保持变量类型封闭, 目前有一堆BUG
+# BUG:
 def trade_when(trigger: np.ndarray[bool],
                alpha: np.ndarray[np.float64],
                exit_cond: np.ndarray[bool]):
     rlt = if_else(exit_cond, np.nan, alpha)
     rlt = if_else(trigger, rlt, ts_delay(rlt, 1))
     if isinstance(alpha, np.ndarray):
         return rlt
```

### Comparing `torchqtm-0.1.0/torchqtm/option/functional.py` & `torchqtm-0.2.0/torchqtm/derivatives/option/functional.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/utils/__init__.py` & `torchqtm-0.2.0/torchqtm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/utils/benchmark.py` & `torchqtm-0.2.0/torchqtm/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/utils/rebalance.py` & `torchqtm-0.2.0/torchqtm/utils/rebalance.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/utils/stats.py` & `torchqtm-0.2.0/torchqtm/utils/stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import torchqtm.op.functional as F
 from typing import Optional
 import matplotlib.pyplot as plt
+from scipy import stats
 
 
 class RiskEvaluator(object):
     def __init__(self,
                  returns: pd.Series,
                  weights: pd.DataFrame = None,
                  freq=None,
@@ -122,12 +123,25 @@
 
     mean = returns.mean()
     std = returns.std()
     _annf = freq
     return mean / std * _annf ** 0.5
 
 
+def information_table(ic_data):
+    ic_summary_table = pd.DataFrame()
+    ic_summary_table["IC Mean"] = ic_data.mean()
+    ic_summary_table["IC Std."] = ic_data.std()
+    ic_summary_table["Risk-Adjusted IC"] = \
+        ic_data.mean() / ic_data.std()
+    t_stat, p_value = stats.ttest_1samp(ic_data, 0)
+    ic_summary_table["t-stat(IC)"] = t_stat
+    ic_summary_table["p-value(IC)"] = p_value
+    ic_summary_table["IC Skew"] = stats.skew(ic_data)
+    ic_summary_table["IC Kurtosis"] = stats.kurtosis(ic_data)
+
+
```

### Comparing `torchqtm-0.1.0/torchqtm/utils/universe.py` & `torchqtm-0.2.0/torchqtm/utils/universe.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,29 @@
 import tushare as ts
 import numpy as np
 from torchqtm.config import __TS_API__
 from torchqtm.utils import relativedelta, datetime
 pro = ts.pro_api(__TS_API__)
 from typing import Iterable, Union, List
 from abc import abstractmethod, ABCMeta
+import joblib
 
 
 class Universe(object, metaclass=ABCMeta):
     def __init__(self):
         pass
 
     @abstractmethod
     def get_symbols(self, trade_date: Union[str, datetime, pd.Timestamp]):
         raise NotImplementedError
 
+    @abstractmethod
+    def data(self):
+        pass
+
 
 class StaticUniverse(Universe):
     def __init__(self, symbols: Iterable[str]):
         super().__init__()
         self.symbols = symbols
 
     def get_symbols(self, trade_date=None):
@@ -30,22 +35,23 @@
         return self.symbols
 
 
 class DynamicUniverse(object):
     pass
 
 
+# @joblib.Memory('./.cache', verbose=0).cache
 class IndexComponents(object):
     def __init__(self,
                  index_code: str,
                  in_date: str):
         self.index_code = index_code
         self.in_date = in_date
         self.data = self._get_components()
 
     def _get_components(self) -> List[str]:
         end = datetime.strptime(self.in_date, "%Y%m%d")
         start = end - relativedelta(months=1)
-        df = pro.index_weight(index_code='399300.SZ', start_date=start.strftime("%Y%m%d"), end_date=end.strftime("%Y%m%d"))
+        df = pro.index_weight(index_code=self.index_code, start_date=start.strftime("%Y%m%d"), end_date=end.strftime("%Y%m%d"))
         rlt = df[df['trade_date'] == max(np.unique(df['trade_date']))]['con_code']
         rlt = sorted(list(rlt.apply(lambda x: x[:-3])))
         return rlt
```

### Comparing `torchqtm-0.1.0/torchqtm/utils/visualization.py` & `torchqtm-0.2.0/torchqtm/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm/utils/warnings.py` & `torchqtm-0.2.0/torchqtm/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.1.0/torchqtm.egg-info/PKG-INFO` & `torchqtm-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: torchqtm
-Version: 0.1.0
+Version: 0.2.0
 Summary: None
-Home-page: https://github.com/nymath/torchquantum/tree/main
-Download-URL: https://github.com/nymath/torchquantum/releases/tag/
+Home-page: https://github.com/nymath/torchqtm
+Download-URL: https://github.com/nymath/torchqtm/releases/tag/
 Author: ny
 Author-email: nymath@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src="https://github.com/nymath/torchquantum/blob/main/src/fig/logo.png" align="right" width="196" />
+<img src="https://github.com/nymath/torchqtm/blob/main/resources/fig/logo.png" align="right" width="196" />
 
 # torchquantum
 
-TorchQuantum is a backtesting framework that integrates
+TorchQuantum is a backtesting framework that""" integrates
 the structure of PyTorch and WorldQuant's Operator for
 efficient quantitative financial analysis.
 
 ## Contents
 
 - [Installation](#installation)
 - [Features](#features)
@@ -29,16 +29,16 @@
 
 ## Installation
 
 for Unix:
 
 ```shell
 cd /path/to/your/directory
-git clone git@github.com:nymath/torchquantum.git
-cd ./torchquantum
+git clone git@github.com:nymath/torchqtm.git
+cd ./torchqtm
 ```
 
 Before running examples, you should compile the cython code.
 
 ```shell
 python setup.py build_ext --inplace
 ```
@@ -51,59 +51,99 @@
 
 If you are not downloading the dataset, then you should
 
 ```shell
 cd ./examples
 mkdir largedata
 cd ./largedata
-wget https://github.com/nymath/torchquantum/releases/download/V0.1/Stocks.pkl.zip
-unzip Stocks.pkl.zip
-rm Stocks.pkl.zip
+wget https://github.com/nymath/torchqtm/releases/download/V0.1/stocks_f64.pkl.zip
+unzip stocks_f64.pkl.zip
+rm stocks_f64.pkl.zip
 cd ../
 cd ../
+git checkout dev
 ```
+As for the backtesting dataset, we use the bundle provided by [ricequant](https://www.ricequant.com/welcome/).
+We have wrapped the code into Makefile, you can just run the following command to download the bundle.
+```shell
+make rqalpha_download_bundle
+```
+
+
+for windows:
+We highly recommend you to use WSL2 to run torchquantum.
 
-## Example
+## Examples
 
+### alpha mining
 You can easily create an alpha through torchquantum!
 
 ```python
 import torchqtm.op as op
 import torchqtm.op.functional as F
+
+
 class NeutralizePE(op.Fundamental):
     def __init__(self, env):
         super().__init__(env)
-        self.lag = op.Parameter(5, required_optim=False, feasible_region=None)
+        self.lag = op.Parameter(5, requires_optim=False, feasible_region=None)
 
     def forward(self):
         self.data = F.divide(1, self.env.PE)
         self.data = F.winsorize(self.data, 'std', 4)
         self.data = F.normalize(self.data)
         self.data = F.group_neutralize(self.data, self.env.Sector)
         self.data = F.regression_neut(self.data, self.env.MktVal)
         self.data = F.ts_mean(self.data, self.lag)
         return self.data
 ```
+
 - `F` is library that contains the operators defined by WorldQuant.
 - `op.Fundamental` implies the NeutralizePE belongs to fundamental alpha.
 - `self.lag` is the parameter of rolling mean, which can be optimized through grid search.
 
+### backtesting
+Here we create a buy and hold strategy for illustration.
 
+```python
+from torchqtm.edbt.algorithm import TradingAlgorithm
+from torchqtm.assets import Equity
+
+class BuyAndHold(TradingAlgorithm):
+    def initialize(self):
+        self.safe_set_attr("s0", Equity("000001.XSHE"))
+        self.safe_set_attr("count", 0)
+
+    def before_trading_start(self):
+        pass
+
+    def handle_data(self):
+        if self.count == 0:
+            self.order(self.s0, 10000)
+        self.count += 1
 
+    def analyze(self):
+        pass
+```
 
 ## Features
 
 - High-speed backtesting framework (most of the operators are implemented through cython)
 - A revised gplearn library that is compatible with Alpha mining.
 - CNN and other state of the art models for mining alphas.
 - Event Driven backtesting framework is available.
 
 ## Contribution
 
-For more information, we refer to [Documentation](https://nymath.github.io/torchquantum/navigate).
-
+For more information, we refer to [Documentation](https://nymath.github.io/torchqtm/navigate).
 
 ## Join us
 
-If you are interested in quantitative finance and are committed to devoting 
+If you are interested in quantitative finance and are committed to devoting
 your life to alpha mining, you can contact me through WeChat at Ny_math.
 
+## References
+
+[quantopian/alphalens](https://github1s.com/quantopian/alphalens/blob/HEAD/alphalens/performance.py)
+
+[quantopian/zipline](https://github1s.com/quantopian/zipline/blob/HEAD/zipline/performance.py)
+
```

