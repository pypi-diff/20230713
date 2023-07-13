# Comparing `tmp/YYYTools-0.1.8.tar.gz` & `tmp/YYYTools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YYYTools-0.1.8.tar", last modified: Tue Jul 11 09:01:20 2023, max compression
+gzip compressed data, was "dist\YYYTools-0.1.9.tar", last modified: Wed Jul 12 01:19:44 2023, max compression
```

## Comparing `YYYTools-0.1.8.tar` & `YYYTools-0.1.9.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.345153 YYYTools-0.1.8/
--rw-rw-rw-   0        0        0     1059 2021-12-18 16:09:22.000000 YYYTools-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       41 2021-12-18 16:09:22.000000 YYYTools-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-11 09:01:20.344153 YYYTools-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0        8 2021-12-18 16:09:22.000000 YYYTools-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.245653 YYYTools-0.1.8/YTools/
--rw-rw-rw-   0        0        0      249 2023-07-11 08:33:57.000000 YYYTools-0.1.8/YTools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.248650 YYYTools-0.1.8/YTools/application/
--rw-rw-rw-   0        0        0       28 2023-07-11 08:33:56.000000 YYYTools-0.1.8/YTools/application/__init__.py
--rw-rw-rw-   0        0        0     4735 2023-07-11 08:29:10.000000 YYYTools-0.1.8/YTools/application/chord_analyze.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.251651 YYYTools-0.1.8/YTools/cg/
--rw-rw-rw-   0        0        0       25 2023-07-11 08:59:52.000000 YYYTools-0.1.8/YTools/cg/__init__.py
--rw-rw-rw-   0        0        0     5297 2021-12-18 16:09:52.000000 YYYTools-0.1.8/YTools/cg/glsl_use.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.253645 YYYTools-0.1.8/YTools/client/
--rw-rw-rw-   0        0        0       18 2023-07-11 08:29:33.000000 YYYTools-0.1.8/YTools/client/__init__.py
--rw-rw-rw-   0        0        0     3104 2021-12-18 16:09:46.000000 YYYTools-0.1.8/YTools/client/cui.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.256646 YYYTools-0.1.8/YTools/debug/
--rw-rw-rw-   0        0        0       30 2023-07-11 08:29:39.000000 YYYTools-0.1.8/YTools/debug/__init__.py
--rw-rw-rw-   0        0        0     6855 2021-12-18 16:09:45.000000 YYYTools-0.1.8/YTools/debug/debug_recursion.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.259646 YYYTools-0.1.8/YTools/deeplearning/
--rw-rw-rw-   0        0        0       41 2021-12-18 16:09:49.000000 YYYTools-0.1.8/YTools/deeplearning/__init__.py
--rw-rw-rw-   0        0        0     1655 2021-12-18 16:09:49.000000 YYYTools-0.1.8/YTools/deeplearning/composed_model.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.265659 YYYTools-0.1.8/YTools/experiment_helper/
--rw-rw-rw-   0        0        0      104 2021-12-18 16:09:24.000000 YYYTools-0.1.8/YTools/experiment_helper/__init__.py
--rw-rw-rw-   0        0        0     1822 2021-12-18 16:09:24.000000 YYYTools-0.1.8/YTools/experiment_helper/logger.py
--rw-rw-rw-   0        0        0      646 2021-12-18 16:09:24.000000 YYYTools-0.1.8/YTools/experiment_helper/random_seeder.py
--rw-rw-rw-   0        0        0      194 2021-12-18 16:09:24.000000 YYYTools-0.1.8/YTools/experiment_helper/watch_time.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.270657 YYYTools-0.1.8/YTools/magic/
--rw-rw-rw-   0        0        0       51 2023-07-11 08:30:17.000000 YYYTools-0.1.8/YTools/magic/__init__.py
--rw-rw-rw-   0        0        0     2468 2023-07-06 04:59:41.000000 YYYTools-0.1.8/YTools/magic/awss3.py
--rw-rw-rw-   0        0        0     1318 2023-07-11 08:40:42.000000 YYYTools-0.1.8/YTools/magic/chatgpt.py
--rw-rw-rw-   0        0        0      710 2023-07-06 04:57:10.000000 YYYTools-0.1.8/YTools/magic/egorov_awss3.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.274662 YYYTools-0.1.8/YTools/network/
--rw-rw-rw-   0        0        0       76 2023-07-11 08:30:33.000000 YYYTools-0.1.8/YTools/network/__init__.py
--rw-rw-rw-   0        0        0     3379 2021-12-18 16:09:47.000000 YYYTools-0.1.8/YTools/network/communicate.py
--rw-rw-rw-   0        0        0     4059 2021-12-18 16:09:47.000000 YYYTools-0.1.8/YTools/network/protocol.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.281158 YYYTools-0.1.8/YTools/network/server/
--rw-rw-rw-   0        0        0       46 2023-07-11 08:31:16.000000 YYYTools-0.1.8/YTools/network/server/__init__.py
--rw-rw-rw-   0        0        0      445 2021-12-18 16:09:48.000000 YYYTools-0.1.8/YTools/network/server/client.py
--rw-rw-rw-   0        0        0      751 2023-07-05 19:59:18.000000 YYYTools-0.1.8/YTools/network/server/server.py
--rw-rw-rw-   0        0        0      816 2021-12-18 16:09:48.000000 YYYTools-0.1.8/YTools/network/server/urlconf.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.289158 YYYTools-0.1.8/YTools/system/
--rw-rw-rw-   0        0        0      167 2023-07-11 08:42:50.000000 YYYTools-0.1.8/YTools/system/__init__.py
--rw-rw-rw-   0        0        0     2355 2021-12-18 16:09:25.000000 YYYTools-0.1.8/YTools/system/cmd_control.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.293159 YYYTools-0.1.8/YTools/system/fakepath/
--rw-rw-rw-   0        0        0       51 2021-12-18 16:09:25.000000 YYYTools-0.1.8/YTools/system/fakepath/__init__.py
--rw-rw-rw-   0        0        0      631 2021-12-18 16:09:25.000000 YYYTools-0.1.8/YTools/system/fakepath/fakepath.py
--rw-rw-rw-   0        0        0      376 2021-12-18 16:09:25.000000 YYYTools-0.1.8/YTools/system/fileintercept.py
--rw-rw-rw-   0        0        0      447 2021-12-18 16:09:25.000000 YYYTools-0.1.8/YTools/system/filewrite.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.298158 YYYTools-0.1.8/YTools/system/locker/
--rw-rw-rw-   0        0        0       42 2021-12-18 16:09:44.000000 YYYTools-0.1.8/YTools/system/locker/__init__.py
--rw-rw-rw-   0        0        0     2150 2021-12-18 16:09:44.000000 YYYTools-0.1.8/YTools/system/locker/filelock.py
--rw-rw-rw-   0        0        0     3783 2021-12-18 16:09:44.000000 YYYTools-0.1.8/YTools/system/locker/lock.py
--rw-rw-rw-   0        0        0    10671 2023-07-11 08:44:14.000000 YYYTools-0.1.8/YTools/system/static_hash.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.318154 YYYTools-0.1.8/YTools/universe/
--rw-rw-rw-   0        0        0      366 2023-07-11 08:32:40.000000 YYYTools-0.1.8/YTools/universe/__init__.py
--rw-rw-rw-   0        0        0     2275 2022-03-16 19:19:59.000000 YYYTools-0.1.8/YTools/universe/beautiful_str.py
--rw-rw-rw-   0        0        0     1779 2021-12-18 16:09:49.000000 YYYTools-0.1.8/YTools/universe/exceptions.py
--rw-rw-rw-   0        0        0     2159 2021-12-18 16:09:50.000000 YYYTools-0.1.8/YTools/universe/extra_type.py
--rw-rw-rw-   0        0        0     1169 2021-12-18 16:09:49.000000 YYYTools-0.1.8/YTools/universe/filename.py
--rw-rw-rw-   0        0        0      186 2021-12-18 16:09:50.000000 YYYTools-0.1.8/YTools/universe/myrandom.py
--rw-rw-rw-   0        0        0      478 2021-12-18 16:09:49.000000 YYYTools-0.1.8/YTools/universe/onexit.py
--rw-rw-rw-   0        0        0      112 2021-12-18 16:09:50.000000 YYYTools-0.1.8/YTools/universe/pather.py
--rw-rw-rw-   0        0        0      480 2021-12-18 16:09:50.000000 YYYTools-0.1.8/YTools/universe/save_load.py
--rw-rw-rw-   0        0        0      509 2022-03-16 19:15:25.000000 YYYTools-0.1.8/YTools/universe/strlen.py
--rw-rw-rw-   0        0        0      431 2021-12-18 16:09:49.000000 YYYTools-0.1.8/YTools/universe/temp_cwd.py
--rw-rw-rw-   0        0        0     1884 2021-12-18 16:09:50.000000 YYYTools-0.1.8/YTools/universe/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.341160 YYYTools-0.1.8/YYYTools.egg-info/
-drwxrwxrwx   0        0        0        0 2023-07-11 09:01:20.343152 YYYTools-0.1.8/YYYTools.egg-info/._DAV/
--rw-rw-rw-   0        0        0        0 2021-12-18 18:41:26.000000 YYYTools-0.1.8/YYYTools.egg-info/._DAV/.state_for_dir.dir
--rw-rw-rw-   0        0        0     1024 2021-12-18 18:41:26.000000 YYYTools-0.1.8/YYYTools.egg-info/._DAV/.state_for_dir.pag
--rw-rw-rw-   0        0        0      265 2023-07-11 09:01:20.000000 YYYTools-0.1.8/YYYTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1716 2023-07-11 09:01:20.000000 YYYTools-0.1.8/YYYTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 09:01:20.000000 YYYTools-0.1.8/YYYTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 09:01:20.000000 YYYTools-0.1.8/YYYTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 09:01:20.000000 YYYTools-0.1.8/YYYTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       47 2023-07-11 08:41:37.000000 YYYTools-0.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 09:01:20.346156 YYYTools-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-07-11 09:01:17.000000 YYYTools-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.595602 YYYTools-0.1.9/
+-rw-rw-rw-   0        0        0     1059 2021-12-18 16:09:22.000000 YYYTools-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       41 2021-12-18 16:09:22.000000 YYYTools-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-12 01:19:44.595602 YYYTools-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2021-12-18 16:09:22.000000 YYYTools-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.487580 YYYTools-0.1.9/YTools/
+-rw-rw-rw-   0        0        0      249 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.491580 YYYTools-0.1.9/YTools/application/
+-rw-rw-rw-   0        0        0       28 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/application/__init__.py
+-rw-rw-rw-   0        0        0     4735 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/application/chord_analyze.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.494580 YYYTools-0.1.9/YTools/cg/
+-rw-rw-rw-   0        0        0       25 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/cg/__init__.py
+-rw-rw-rw-   0        0        0     5297 2021-12-18 16:09:52.000000 YYYTools-0.1.9/YTools/cg/glsl_use.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.498581 YYYTools-0.1.9/YTools/client/
+-rw-rw-rw-   0        0        0       18 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/client/__init__.py
+-rw-rw-rw-   0        0        0     3104 2021-12-18 16:09:46.000000 YYYTools-0.1.9/YTools/client/cui.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.502582 YYYTools-0.1.9/YTools/debug/
+-rw-rw-rw-   0        0        0       30 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/debug/__init__.py
+-rw-rw-rw-   0        0        0     6855 2021-12-18 16:09:45.000000 YYYTools-0.1.9/YTools/debug/debug_recursion.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.506583 YYYTools-0.1.9/YTools/deeplearning/
+-rw-rw-rw-   0        0        0       41 2021-12-18 16:09:49.000000 YYYTools-0.1.9/YTools/deeplearning/__init__.py
+-rw-rw-rw-   0        0        0     1655 2021-12-18 16:09:49.000000 YYYTools-0.1.9/YTools/deeplearning/composed_model.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.517584 YYYTools-0.1.9/YTools/experiment_helper/
+-rw-rw-rw-   0        0        0      179 2023-07-12 01:17:16.000000 YYYTools-0.1.9/YTools/experiment_helper/__init__.py
+-rw-rw-rw-   0        0        0     2141 2023-07-12 01:18:51.000000 YYYTools-0.1.9/YTools/experiment_helper/globaldata.py
+-rw-rw-rw-   0        0        0     1755 2023-07-12 00:45:25.000000 YYYTools-0.1.9/YTools/experiment_helper/logger.py
+-rw-rw-rw-   0        0        0      684 2023-07-12 00:48:21.000000 YYYTools-0.1.9/YTools/experiment_helper/random_seeder.py
+-rw-rw-rw-   0        0        0      196 2023-07-12 00:47:09.000000 YYYTools-0.1.9/YTools/experiment_helper/watch_time.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.524586 YYYTools-0.1.9/YTools/magic/
+-rw-rw-rw-   0        0        0       75 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/magic/__init__.py
+-rw-rw-rw-   0        0        0     2468 2023-07-06 04:59:41.000000 YYYTools-0.1.9/YTools/magic/awss3.py
+-rw-rw-rw-   0        0        0     1318 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/magic/chatgpt.py
+-rw-rw-rw-   0        0        0      710 2023-07-06 04:57:10.000000 YYYTools-0.1.9/YTools/magic/egorov_awss3.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.530588 YYYTools-0.1.9/YTools/network/
+-rw-rw-rw-   0        0        0       76 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/network/__init__.py
+-rw-rw-rw-   0        0        0     3379 2021-12-18 16:09:47.000000 YYYTools-0.1.9/YTools/network/communicate.py
+-rw-rw-rw-   0        0        0     4059 2021-12-18 16:09:47.000000 YYYTools-0.1.9/YTools/network/protocol.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.537589 YYYTools-0.1.9/YTools/network/server/
+-rw-rw-rw-   0        0        0       46 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/network/server/__init__.py
+-rw-rw-rw-   0        0        0      445 2021-12-18 16:09:48.000000 YYYTools-0.1.9/YTools/network/server/client.py
+-rw-rw-rw-   0        0        0      751 2023-07-05 19:59:18.000000 YYYTools-0.1.9/YTools/network/server/server.py
+-rw-rw-rw-   0        0        0      816 2021-12-18 16:09:48.000000 YYYTools-0.1.9/YTools/network/server/urlconf.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.548592 YYYTools-0.1.9/YTools/system/
+-rw-rw-rw-   0        0        0      167 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/system/__init__.py
+-rw-rw-rw-   0        0        0     2355 2021-12-18 16:09:25.000000 YYYTools-0.1.9/YTools/system/cmd_control.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.552593 YYYTools-0.1.9/YTools/system/fakepath/
+-rw-rw-rw-   0        0        0       51 2021-12-18 16:09:25.000000 YYYTools-0.1.9/YTools/system/fakepath/__init__.py
+-rw-rw-rw-   0        0        0      631 2021-12-18 16:09:25.000000 YYYTools-0.1.9/YTools/system/fakepath/fakepath.py
+-rw-rw-rw-   0        0        0      376 2021-12-18 16:09:25.000000 YYYTools-0.1.9/YTools/system/fileintercept.py
+-rw-rw-rw-   0        0        0      447 2021-12-18 16:09:25.000000 YYYTools-0.1.9/YTools/system/filewrite.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.557594 YYYTools-0.1.9/YTools/system/locker/
+-rw-rw-rw-   0        0        0       42 2021-12-18 16:09:44.000000 YYYTools-0.1.9/YTools/system/locker/__init__.py
+-rw-rw-rw-   0        0        0     2150 2021-12-18 16:09:44.000000 YYYTools-0.1.9/YTools/system/locker/filelock.py
+-rw-rw-rw-   0        0        0     3783 2021-12-18 16:09:44.000000 YYYTools-0.1.9/YTools/system/locker/lock.py
+-rw-rw-rw-   0        0        0    10671 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/system/static_hash.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.582600 YYYTools-0.1.9/YTools/universe/
+-rw-rw-rw-   0        0        0      366 2023-07-12 00:14:41.000000 YYYTools-0.1.9/YTools/universe/__init__.py
+-rw-rw-rw-   0        0        0     2275 2022-03-16 19:19:59.000000 YYYTools-0.1.9/YTools/universe/beautiful_str.py
+-rw-rw-rw-   0        0        0     1782 2023-07-12 00:46:42.000000 YYYTools-0.1.9/YTools/universe/exceptions.py
+-rw-rw-rw-   0        0        0     2159 2021-12-18 16:09:50.000000 YYYTools-0.1.9/YTools/universe/extra_type.py
+-rw-rw-rw-   0        0        0     1169 2021-12-18 16:09:49.000000 YYYTools-0.1.9/YTools/universe/filename.py
+-rw-rw-rw-   0        0        0      186 2021-12-18 16:09:50.000000 YYYTools-0.1.9/YTools/universe/myrandom.py
+-rw-rw-rw-   0        0        0      478 2021-12-18 16:09:49.000000 YYYTools-0.1.9/YTools/universe/onexit.py
+-rw-rw-rw-   0        0        0      112 2021-12-18 16:09:50.000000 YYYTools-0.1.9/YTools/universe/pather.py
+-rw-rw-rw-   0        0        0      480 2021-12-18 16:09:50.000000 YYYTools-0.1.9/YTools/universe/save_load.py
+-rw-rw-rw-   0        0        0      509 2022-03-16 19:15:25.000000 YYYTools-0.1.9/YTools/universe/strlen.py
+-rw-rw-rw-   0        0        0      431 2021-12-18 16:09:49.000000 YYYTools-0.1.9/YTools/universe/temp_cwd.py
+-rw-rw-rw-   0        0        0     1884 2021-12-18 16:09:50.000000 YYYTools-0.1.9/YTools/universe/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.590601 YYYTools-0.1.9/YYYTools.egg-info/
+drwxrwxrwx   0        0        0        0 2023-07-12 01:19:44.593602 YYYTools-0.1.9/YYYTools.egg-info/._DAV/
+-rw-rw-rw-   0        0        0        0 2021-12-18 18:41:26.000000 YYYTools-0.1.9/YYYTools.egg-info/._DAV/.state_for_dir.dir
+-rw-rw-rw-   0        0        0     1024 2021-12-18 18:41:26.000000 YYYTools-0.1.9/YYYTools.egg-info/._DAV/.state_for_dir.pag
+-rw-rw-rw-   0        0        0      265 2023-07-12 01:19:44.000000 YYYTools-0.1.9/YYYTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2023-07-12 01:19:44.000000 YYYTools-0.1.9/YYYTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 01:19:44.000000 YYYTools-0.1.9/YYYTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-12 01:19:44.000000 YYYTools-0.1.9/YYYTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 01:19:44.000000 YYYTools-0.1.9/YYYTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       29 2023-07-12 01:19:09.000000 YYYTools-0.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 01:19:44.595602 YYYTools-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-07-12 01:19:15.000000 YYYTools-0.1.9/setup.py
```

### Comparing `YYYTools-0.1.8/LICENSE` & `YYYTools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/application/chord_analyze.py` & `YYYTools-0.1.9/YTools/application/chord_analyze.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/cg/glsl_use.py` & `YYYTools-0.1.9/YTools/cg/glsl_use.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/client/cui.py` & `YYYTools-0.1.9/YTools/client/cui.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/debug/debug_recursion.py` & `YYYTools-0.1.9/YTools/debug/debug_recursion.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/deeplearning/composed_model.py` & `YYYTools-0.1.9/YTools/deeplearning/composed_model.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/experiment_helper/logger.py` & `YYYTools-0.1.9/YTools/experiment_helper/logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .watch_time import my_clock
 from ..universe.strlen import last_len
 import time
+from typing import Union
 
 class Logger:
 	'''自动日志。
 
 	参数：
 	mode：一个函数，代表输出方向。"write"表示向文件写
 	log_path：日志文件的位置。如果选了"write"的话必须填此项。如果打开了文件最后一定要调用close()
@@ -12,61 +13,60 @@
 
 
 	方法：
 	log：输出一个字符串
 	close：关闭文件
 	
 	'''
-	def __init__(self , mode = [print] , log_path = None , append = ["clock"] , line_length = 90):
+	def __init__(self , mode = [print] , log_path = None ,  extra = ["clock"]):
 		if log_path:
 			self.log_fil = open(log_path , "w" , encoding = "utf-8")
 		else:
 			self.log_fil = None
 
 		self.mode = mode
 
 		if ("write" in mode) and (not log_path):
 			raise Exception("Should have a log_path")
 
-		self.append 	= append
-		self.line_length = line_length
+		self.extra 	= extra
 
 	def close(self):
 		if self.log_fil:
 			self.log_fil.close()
 
-	def log(self , content = ""):
+	def log(self , content: str = ""):
 
-		content = self.pre_process(content)
+		if isinstance(content , str):
 
-		for x in self.mode:
-			if x == "write":
-				self.log_fil.write(content + "\n")
-				self.log_fil.flush()
-			else:
-				x(str(content))
+			content = self.pre_process(content)
+
+			for md in self.mode:
+				if md == "write" and self.log_fil:
+					self.log_fil.write(content + "\n")
+					self.log_fil.flush()
+				else:
+					md(str(content))
 
-	def add_line(self , num = -1 , char = "-"):
+	def add_line(self , num: int = 90 , char: str = "-"):
 		'''输出num个char , 如果num<0则默认line_length个
 		'''
-		if num < 0:
-			num = self.line_length
 		self.log(char * num)
 
 	def pre_process(self , content):
-		insert_space = self.line_length - last_len(content) #补全到line_length 
-		content += " " * insert_space
 
-		for x in self.append: #要往末尾添加哪些东西
+		for ex in self.extra: #要往开头添加哪些东西
 
-			y = ""
-			if x == "clock":
-				y = "%.2fs" % (my_clock())
-			elif x == "time":
-				y = time.strftime("%Y-%m-%d %H:%M:%S" , time.localtime() )
+			to_add = ""
+
+			if ex == "clock":
+				to_add = "%.2fs" % (my_clock())
+			elif ex == "time":
+				to_add = time.strftime("%Y-%m-%d %H:%M:%S" , time.localtime() )
 			else:
-				y = x()
+				to_add = ex()
 
-			content += "| " + y + " "
+			content = f"[{to_add}] {content}"
 
 
-		return content
+		return content
+
```

### Comparing `YYYTools-0.1.8/YTools/experiment_helper/random_seeder.py` & `YYYTools-0.1.9/YTools/experiment_helper/random_seeder.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 	if "random" in modules:
 		random.seed(seed)
 	if "numpy" in modules:
 		import numpy as np
 		np.random.seed(seed)
 	if "torch" in modules:
 		import torch as tc
+		import torch.backends.cudnn 
 		tc.manual_seed(seed)
 		tc.cuda.manual_seed_all(seed)
-		tc.backends.cudnn.deterministic = True
-		tc.backends.cudnn.benchmark = False
+		torch.backends.cudnn.deterministic = True
+		torch.backends.cudnn.benchmark = False
```

### Comparing `YYYTools-0.1.8/YTools/magic/awss3.py` & `YYYTools-0.1.9/YTools/magic/awss3.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/magic/chatgpt.py` & `YYYTools-0.1.9/YTools/magic/chatgpt.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/magic/egorov_awss3.py` & `YYYTools-0.1.9/YTools/magic/egorov_awss3.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/network/communicate.py` & `YYYTools-0.1.9/YTools/network/communicate.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/network/protocol.py` & `YYYTools-0.1.9/YTools/network/protocol.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/network/server/server.py` & `YYYTools-0.1.9/YTools/network/server/server.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/network/server/urlconf.py` & `YYYTools-0.1.9/YTools/network/server/urlconf.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/system/cmd_control.py` & `YYYTools-0.1.9/YTools/system/cmd_control.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/system/fakepath/fakepath.py` & `YYYTools-0.1.9/YTools/system/fakepath/fakepath.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/system/locker/filelock.py` & `YYYTools-0.1.9/YTools/system/locker/filelock.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/system/locker/lock.py` & `YYYTools-0.1.9/YTools/system/locker/lock.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/system/static_hash.py` & `YYYTools-0.1.9/YTools/system/static_hash.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/universe/beautiful_str.py` & `YYYTools-0.1.9/YTools/universe/beautiful_str.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/universe/exceptions.py` & `YYYTools-0.1.9/YTools/universe/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 		if note_str is None:
 			note_str = "Invalid argument value"
 		
 		var_str = ""
 		if var_name is not None:
 			var_str = ": {var_name} can not be {var_val}".format(var_name = var_name , var_val = var_val)
 		
-		self.args = ["{func_name}: {note_str}{var_str}".format(
+		self.args = ("{func_name}: {note_str}{var_str}".format(
 			func_name = func_name , note_str = note_str , var_str = var_str
-		)]
+		), )
 		
 class YAttributeError(Exception):
 	'''函数的参数不符合要求'''
 	def __init__(self, func_name , var_name = None , var_val = None , class_name = None , note_str = None):
 		''' 
 		参数：
 			func_name： 字符串。抛出异常的位置
@@ -40,10 +40,10 @@
 		if note_str is None:
 			note_str = "Invalid artribute value"
 		
 		var_str = ""
 		if var_name is not None:
 			var_str = ": {var_name} can not be {var_val}".format(var_name = var_name , var_val = var_val)
 		
-		self.args = ["{func_name}: {note_str}{var_str}".format(
+		self.args = ("{func_name}: {note_str}{var_str}".format(
 			func_name = func_name , note_str = note_str , var_str = var_str
-		)]
+		),)
```

### Comparing `YYYTools-0.1.8/YTools/universe/extra_type.py` & `YYYTools-0.1.9/YTools/universe/extra_type.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/universe/filename.py` & `YYYTools-0.1.9/YTools/universe/filename.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YTools/universe/timer.py` & `YYYTools-0.1.9/YTools/universe/timer.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YYYTools.egg-info/._DAV/.state_for_dir.pag` & `YYYTools-0.1.9/YYYTools.egg-info/._DAV/.state_for_dir.pag`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.8/YYYTools.egg-info/SOURCES.txt` & `YYYTools-0.1.9/YYYTools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 YTools/client/__init__.py
 YTools/client/cui.py
 YTools/debug/__init__.py
 YTools/debug/debug_recursion.py
 YTools/deeplearning/__init__.py
 YTools/deeplearning/composed_model.py
 YTools/experiment_helper/__init__.py
+YTools/experiment_helper/globaldata.py
 YTools/experiment_helper/logger.py
 YTools/experiment_helper/random_seeder.py
 YTools/experiment_helper/watch_time.py
 YTools/magic/__init__.py
 YTools/magic/awss3.py
 YTools/magic/chatgpt.py
 YTools/magic/egorov_awss3.py
```

### Comparing `YYYTools-0.1.8/setup.py` & `YYYTools-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     reqs = f.read()
 
 pkgs = [p for p in find_packages() if p.startswith('YTools')]
 print(pkgs)
 
 setup(
     name='YYYTools',
-    version='0.1.8',
+    version='0.1.9',
     url='http://github.com/FFTYYY/YTools',
     description='',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='MIT',
     author = 'Yongyi Yang',
 	author_email = 'yongyi@umich.edu',
```

