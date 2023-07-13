# Comparing `tmp/emdbg-1.0.1.tar.gz` & `tmp/emdbg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emdbg-1.0.1.tar", last modified: Wed Jul 12 12:13:30 2023, max compression
+gzip compressed data, was "emdbg-1.0.2.tar", last modified: Thu Jul 13 14:17:56 2023, max compression
```

## Comparing `emdbg-1.0.1.tar` & `emdbg-1.0.2.tar`

### file list

```diff
@@ -1,87 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.574667 emdbg-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-12 12:13:15.000000 emdbg-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-12 12:13:30.574667 emdbg-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-12 12:13:15.000000 emdbg-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-12 12:13:15.000000 emdbg-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:13:30.574667 emdbg-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.558667 emdbg-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.558667 emdbg-1.0.1/src/emdbg/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.562667 emdbg-1.0.1/src/emdbg/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/analyze/backtrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/analyze/callgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/analyze/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/analyze/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/analyze/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.562667 emdbg-1.0.1/src/emdbg/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.570667 emdbg-1.0.1/src/emdbg/bench/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2501281 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/data/STM32F7x5.svd
--rw-r--r--   0 runner    (1001) docker     (123)  4087801 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/data/STM32H753x.svd
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/data/fmu.gdb
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/data/fmu_v5x.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/data/fmu_v6x.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/data/fmu_v6x.jlinkscript
--rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/data/orbuculum.gdb
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/fmu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/bench/skynode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.570667 emdbg-1.0.1/src/emdbg/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/crashdebug.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/jlink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/openocd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.570667 emdbg-1.0.1/src/emdbg/debug/px4/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/pinout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/system_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/px4/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.570667 emdbg-1.0.1/src/emdbg/debug/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/remote/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/remote/gdb_api_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/remote/mi.py
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/remote/px4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/remote/rpyc.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/debug/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.570667 emdbg-1.0.1/src/emdbg/io/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/io/digilent.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.570667 emdbg-1.0.1/src/emdbg/patch/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.574667 emdbg-1.0.1/src/emdbg/patch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/data/disable_uavcan_v5x.patch
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/data/itm.h
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/data/itm_Make.defs
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/data/itm_nuttx_Makefile.patch
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/data/nuttx_tracing_itm.patch
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/data/sem_boostlog.c
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/data/semaphore_boostlog.h
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/data/semaphore_boostlog.patch
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/patch/set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.574667 emdbg-1.0.1/src/emdbg/power/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/power/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/power/yocto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.574667 emdbg-1.0.1/src/emdbg/serial/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/serial/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/serial/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-12 12:13:15.000000 emdbg-1.0.1/src/emdbg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:13:30.558667 emdbg-1.0.1/src/emdbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-12 12:13:30.000000 emdbg-1.0.1/src/emdbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-12 12:13:30.000000 emdbg-1.0.1/src/emdbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:13:30.000000 emdbg-1.0.1/src/emdbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:13:30.000000 emdbg-1.0.1/src/emdbg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 12:13:30.000000 emdbg-1.0.1/src/emdbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 12:13:30.000000 emdbg-1.0.1/src/emdbg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.509517 emdbg-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-13 14:17:38.000000 emdbg-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-13 14:17:56.509517 emdbg-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-13 14:17:38.000000 emdbg-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-13 14:17:38.000000 emdbg-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:17:56.509517 emdbg-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.489516 emdbg-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.489516 emdbg-1.0.2/src/emdbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.493516 emdbg-1.0.2/src/emdbg/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/callgraph.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/callgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/calltrace.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.493516 emdbg-1.0.2/src/emdbg/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.501516 emdbg-1.0.2/src/emdbg/bench/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2501281 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/STM32F7x5.svd
+-rw-r--r--   0 runner    (1001) docker     (123)  4087801 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/STM32H753x.svd
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/fmu.gdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/fmu_v5x.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/fmu_v6x.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/fmu_v6x.jlinkscript
+-rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/orbuculum.gdb
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/fmu.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/fmu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/skynode.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/skynode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/crashdebug.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/crashdebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31384 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/gdb.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/jlink.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/jlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/openocd.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/openocd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/debug/px4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/pinout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/system_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/debug/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/gdb_api_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/mi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/px4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/rpyc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/io/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/io/digilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.509517 emdbg-1.0.2/src/emdbg/patch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/disable_uavcan_v5x.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/itm.h
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/itm_Make.defs
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/itm_nuttx_Makefile.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/nuttx_tracing_itm.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/sem_boostlog.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/semaphore_boostlog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/semaphore_boostlog.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.509517 emdbg-1.0.2/src/emdbg/power/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/power/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/power/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/power/yocto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.509517 emdbg-1.0.2/src/emdbg/serial/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/serial/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/serial/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/serial/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.493516 emdbg-1.0.2/src/emdbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/top_level.txt
```

### Comparing `emdbg-1.0.1/LICENSE` & `emdbg-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/PKG-INFO` & `emdbg-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdbg
-Version: 1.0.1
+Version: 1.0.2
 Summary: Embedded Debug Tools
 Author-email: Auterion <success@auterion.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/auterion/embedded-debug-tools
 Keywords: embedded,debug,gdb,stm32,px4
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `emdbg-1.0.1/README.md` & `emdbg-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/pyproject.toml` & `emdbg-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # yocto = ["yoctopuce"]
 # rpyc = ["rpyc"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-emdbg = ["*.md"]
+emdbg = ["*.md", "*/*.md", "*/*/*.md", "*/*/*/*.md"]
 "emdbg.patch.data" = ["*"]
 "emdbg.bench.data" = ["*"]
 
 [tool.setuptools]
 # GDB expects plain text config files!
 zip-safe = false
```

### Comparing `emdbg-1.0.1/src/emdbg/__init__.py` & `emdbg-1.0.2/src/emdbg/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/analyze/backtrace.py` & `emdbg-1.0.2/src/emdbg/analyze/backtrace.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/analyze/callgraph.py` & `emdbg-1.0.2/src/emdbg/analyze/callgraph.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/analyze/calltrace.py` & `emdbg-1.0.2/src/emdbg/analyze/calltrace.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/analyze/priority.py` & `emdbg-1.0.2/src/emdbg/analyze/priority.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/bench/data/STM32F7x5.svd` & `emdbg-1.0.2/src/emdbg/bench/data/STM32F7x5.svd`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/bench/data/STM32H753x.svd` & `emdbg-1.0.2/src/emdbg/bench/data/STM32H753x.svd`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/bench/data/fmu.gdb` & `emdbg-1.0.2/src/emdbg/bench/data/fmu.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/bench/data/fmu_v6x.jlinkscript` & `emdbg-1.0.2/src/emdbg/bench/data/fmu_v6x.jlinkscript`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/bench/data/orbuculum.gdb` & `emdbg-1.0.2/src/emdbg/bench/data/orbuculum.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/bench/fmu.py` & `emdbg-1.0.2/src/emdbg/bench/fmu.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/bench/skynode.py` & `emdbg-1.0.2/src/emdbg/bench/skynode.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/__init__.py` & `emdbg-1.0.2/src/emdbg/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/backend.py` & `emdbg-1.0.2/src/emdbg/debug/backend.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/crashdebug.py` & `emdbg-1.0.2/src/emdbg/debug/crashdebug.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/gdb.py` & `emdbg-1.0.2/src/emdbg/debug/gdb.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/jlink.py` & `emdbg-1.0.2/src/emdbg/debug/jlink.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/openocd.py` & `emdbg-1.0.2/src/emdbg/debug/openocd.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/__init__.py` & `emdbg-1.0.2/src/emdbg/debug/px4/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/base.py` & `emdbg-1.0.2/src/emdbg/debug/px4/base.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/device.py` & `emdbg-1.0.2/src/emdbg/debug/px4/device.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/pinout.py` & `emdbg-1.0.2/src/emdbg/debug/px4/pinout.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/semaphore.py` & `emdbg-1.0.2/src/emdbg/debug/px4/semaphore.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/svd.py` & `emdbg-1.0.2/src/emdbg/debug/px4/svd.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/system_load.py` & `emdbg-1.0.2/src/emdbg/debug/px4/system_load.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/task.py` & `emdbg-1.0.2/src/emdbg/debug/px4/task.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/px4/utils.py` & `emdbg-1.0.2/src/emdbg/debug/px4/utils.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/remote/__init__.py` & `emdbg-1.0.2/src/emdbg/debug/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/remote/gdb.py` & `emdbg-1.0.2/src/emdbg/debug/remote/gdb.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/remote/gdb_api_bridge.py` & `emdbg-1.0.2/src/emdbg/debug/remote/gdb_api_bridge.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/remote/mi.py` & `emdbg-1.0.2/src/emdbg/debug/remote/mi.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/remote/px4.py` & `emdbg-1.0.2/src/emdbg/debug/remote/px4.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/remote/rpyc.py` & `emdbg-1.0.2/src/emdbg/debug/remote/rpyc.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/debug/utils.py` & `emdbg-1.0.2/src/emdbg/debug/utils.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/io/digilent.py` & `emdbg-1.0.2/src/emdbg/io/digilent.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/logger.py` & `emdbg-1.0.2/src/emdbg/logger.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/__main__.py` & `emdbg-1.0.2/src/emdbg/patch/__main__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/data/disable_uavcan_v5x.patch` & `emdbg-1.0.2/src/emdbg/patch/data/disable_uavcan_v5x.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/data/itm.h` & `emdbg-1.0.2/src/emdbg/patch/data/itm.h`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/data/itm_nuttx_Makefile.patch` & `emdbg-1.0.2/src/emdbg/patch/data/itm_nuttx_Makefile.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/data/nuttx_tracing_itm.patch` & `emdbg-1.0.2/src/emdbg/patch/data/nuttx_tracing_itm.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/data/sem_boostlog.c` & `emdbg-1.0.2/src/emdbg/patch/data/sem_boostlog.c`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/data/semaphore_boostlog.h` & `emdbg-1.0.2/src/emdbg/patch/data/semaphore_boostlog.h`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/data/semaphore_boostlog.patch` & `emdbg-1.0.2/src/emdbg/patch/data/semaphore_boostlog.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/operation.py` & `emdbg-1.0.2/src/emdbg/patch/operation.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/patch/set.py` & `emdbg-1.0.2/src/emdbg/patch/set.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/power/base.py` & `emdbg-1.0.2/src/emdbg/power/base.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/power/yocto.py` & `emdbg-1.0.2/src/emdbg/power/yocto.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/serial/protocol.py` & `emdbg-1.0.2/src/emdbg/serial/protocol.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg/serial/utils.py` & `emdbg-1.0.2/src/emdbg/serial/utils.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.1/src/emdbg.egg-info/PKG-INFO` & `emdbg-1.0.2/src/emdbg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdbg
-Version: 1.0.1
+Version: 1.0.2
 Summary: Embedded Debug Tools
 Author-email: Auterion <success@auterion.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/auterion/embedded-debug-tools
 Keywords: embedded,debug,gdb,stm32,px4
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `emdbg-1.0.1/src/emdbg.egg-info/SOURCES.txt` & `emdbg-1.0.2/src/emdbg.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,33 +8,41 @@
 src/emdbg.egg-info/SOURCES.txt
 src/emdbg.egg-info/dependency_links.txt
 src/emdbg.egg-info/not-zip-safe
 src/emdbg.egg-info/requires.txt
 src/emdbg.egg-info/top_level.txt
 src/emdbg/analyze/__init__.py
 src/emdbg/analyze/backtrace.py
+src/emdbg/analyze/callgraph.md
 src/emdbg/analyze/callgraph.py
+src/emdbg/analyze/calltrace.md
 src/emdbg/analyze/calltrace.py
 src/emdbg/analyze/priority.py
 src/emdbg/analyze/utils.py
 src/emdbg/bench/__init__.py
+src/emdbg/bench/fmu.md
 src/emdbg/bench/fmu.py
+src/emdbg/bench/skynode.md
 src/emdbg/bench/skynode.py
 src/emdbg/bench/data/STM32F7x5.svd
 src/emdbg/bench/data/STM32H753x.svd
 src/emdbg/bench/data/fmu.gdb
 src/emdbg/bench/data/fmu_v5x.cfg
 src/emdbg/bench/data/fmu_v6x.cfg
 src/emdbg/bench/data/fmu_v6x.jlinkscript
 src/emdbg/bench/data/orbuculum.gdb
 src/emdbg/debug/__init__.py
 src/emdbg/debug/backend.py
+src/emdbg/debug/crashdebug.md
 src/emdbg/debug/crashdebug.py
+src/emdbg/debug/gdb.md
 src/emdbg/debug/gdb.py
+src/emdbg/debug/jlink.md
 src/emdbg/debug/jlink.py
+src/emdbg/debug/openocd.md
 src/emdbg/debug/openocd.py
 src/emdbg/debug/utils.py
 src/emdbg/debug/px4/__init__.py
 src/emdbg/debug/px4/base.py
 src/emdbg/debug/px4/device.py
 src/emdbg/debug/px4/pinout.py
 src/emdbg/debug/px4/semaphore.py
@@ -44,27 +52,31 @@
 src/emdbg/debug/px4/utils.py
 src/emdbg/debug/remote/__init__.py
 src/emdbg/debug/remote/gdb.py
 src/emdbg/debug/remote/gdb_api_bridge.py
 src/emdbg/debug/remote/mi.py
 src/emdbg/debug/remote/px4.py
 src/emdbg/debug/remote/rpyc.py
+src/emdbg/io/README.md
 src/emdbg/io/__init__.py
 src/emdbg/io/digilent.py
+src/emdbg/patch/README.md
 src/emdbg/patch/__init__.py
 src/emdbg/patch/__main__.py
 src/emdbg/patch/operation.py
 src/emdbg/patch/set.py
 src/emdbg/patch/data/disable_uavcan_v5x.patch
 src/emdbg/patch/data/itm.h
 src/emdbg/patch/data/itm_Make.defs
 src/emdbg/patch/data/itm_nuttx_Makefile.patch
 src/emdbg/patch/data/nuttx_tracing_itm.patch
 src/emdbg/patch/data/sem_boostlog.c
 src/emdbg/patch/data/semaphore_boostlog.h
 src/emdbg/patch/data/semaphore_boostlog.patch
+src/emdbg/power/README.md
 src/emdbg/power/__init__.py
 src/emdbg/power/base.py
 src/emdbg/power/yocto.py
+src/emdbg/serial/README.md
 src/emdbg/serial/__init__.py
 src/emdbg/serial/protocol.py
 src/emdbg/serial/utils.py
```

