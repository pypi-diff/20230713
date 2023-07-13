# Comparing `tmp/pyrasite-ng-2.0.1.tar.gz` & `tmp/pyrasite-ng-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrasite-ng-2.0.1.tar", last modified: Sat Oct 23 08:41:26 2021, max compression
+gzip compressed data, was "pyrasite-ng-2.0.2.tar", last modified: Thu Jul 13 13:11:51 2023, max compression
```

## Comparing `pyrasite-ng-2.0.1.tar` & `pyrasite-ng-2.0.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.333359 pyrasite-ng-2.0.1/
--rw-r--r--   0 user202729  (1000) user202729  (1000)      171 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/.coveragerc
--rw-r--r--   0 user202729  (1000) user202729  (1000)       65 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/.gitignore
--rw-r--r--   0 user202729  (1000) user202729  (1000)      592 2020-10-26 08:12:17.000000 pyrasite-ng-2.0.1/.travis.yml
--rw-r--r--   0 user202729  (1000) user202729  (1000)    35147 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/LICENSE
--rw-r--r--   0 user202729  (1000) user202729  (1000)      114 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/MANIFEST.in
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2550 2021-10-23 08:41:26.333359 pyrasite-ng-2.0.1/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1424 2021-10-23 08:39:52.000000 pyrasite-ng-2.0.1/README.rst
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.326692 pyrasite-ng-2.0.1/docs/
--rw-r--r--   0 user202729  (1000) user202729  (1000)      247 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/API.rst
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1619 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/CLI.rst
--rw-r--r--   0 user202729  (1000) user202729  (1000)      407 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/Development.rst
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1611 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/GUI.rst
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1783 2020-10-26 08:17:36.000000 pyrasite-ng-2.0.1/docs/Installing.rst
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4598 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/Makefile
--rw-r--r--   0 user202729  (1000) user202729  (1000)      777 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/MemoryViewer.rst
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2341 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/Payloads.rst
--rw-r--r--   0 user202729  (1000) user202729  (1000)      665 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/Shell.rst
--rw-r--r--   0 user202729  (1000) user202729  (1000)     7131 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/conf.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      600 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/docs/index.rst
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.320026 pyrasite-ng-2.0.1/pkgs/
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.326692 pyrasite-ng-2.0.1/pkgs/arch/
--rw-r--r--   0 user202729  (1000) user202729  (1000)      684 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pkgs/arch/PKGBUILD
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.326692 pyrasite-ng-2.0.1/pkgs/fedora/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1832 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pkgs/fedora/pyrasite.spec
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.326692 pyrasite-ng-2.0.1/pkgs/ubuntu/
--rwxr-xr-x   0 user202729  (1000) user202729  (1000)      406 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pkgs/ubuntu/make_deb.sh
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.330026 pyrasite-ng-2.0.1/pyrasite/
--rw-r--r--   0 user202729  (1000) user202729  (1000)        7 2020-10-26 08:05:03.000000 pyrasite-ng-2.0.1/pyrasite/.vimrc
--rw-r--r--   0 user202729  (1000) user202729  (1000)      992 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/__init__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2893 2021-03-03 09:56:00.000000 pyrasite-ng-2.0.1/pyrasite/injector.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1233 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/inspector.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     7635 2021-03-03 10:02:48.000000 pyrasite-ng-2.0.1/pyrasite/ipc.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     5770 2020-10-26 08:12:58.000000 pyrasite-ng-2.0.1/pyrasite/main.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.330026 pyrasite-ng-2.0.1/pyrasite/payloads/
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/__init__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      575 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/dump_memory.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)       93 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/dump_modules.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      154 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/dump_stacks.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)       23 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/force_garbage_collection.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)       22 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/helloworld.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      988 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/reverse_python_shell.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1213 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/reverse_shell.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      111 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/start_callgraph.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      129 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/payloads/stop_callgraph.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     5832 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/reverse.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     9431 2020-10-26 08:06:11.000000 pyrasite-ng-2.0.1/pyrasite/tags
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.333359 pyrasite-ng-2.0.1/pyrasite/tests/
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tests/__init__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      521 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tests/context_manager_case.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2669 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tests/test_cli.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     3213 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tests/test_code_injection.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2941 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tests/test_ipc.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2185 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tests/utils.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.333359 pyrasite-ng-2.0.1/pyrasite/tools/
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tools/__init__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     5766 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tools/memory_viewer.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2186 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/tools/shell.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.333359 pyrasite-ng-2.0.1/pyrasite/win/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     6614 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/pyrasite/win/inject_python.cpp
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2021-10-23 08:41:26.333359 pyrasite-ng-2.0.1/pyrasite_ng.egg-info/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2550 2021-10-23 08:41:26.000000 pyrasite-ng-2.0.1/pyrasite_ng.egg-info/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1387 2021-10-23 08:41:26.000000 pyrasite-ng-2.0.1/pyrasite_ng.egg-info/SOURCES.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2021-10-23 08:41:26.000000 pyrasite-ng-2.0.1/pyrasite_ng.egg-info/dependency_links.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)      198 2021-10-23 08:41:26.000000 pyrasite-ng-2.0.1/pyrasite_ng.egg-info/entry_points.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2021-10-23 08:34:30.000000 pyrasite-ng-2.0.1/pyrasite_ng.egg-info/not-zip-safe
--rw-r--r--   0 user202729  (1000) user202729  (1000)        6 2021-10-23 08:41:26.000000 pyrasite-ng-2.0.1/pyrasite_ng.egg-info/requires.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        9 2021-10-23 08:41:26.000000 pyrasite-ng-2.0.1/pyrasite_ng.egg-info/top_level.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       38 2021-10-23 08:41:26.336692 pyrasite-ng-2.0.1/setup.cfg
--rw-r--r--   0 user202729  (1000) user202729  (1000)     3029 2021-10-23 08:41:16.000000 pyrasite-ng-2.0.1/setup.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      332 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/tox.ini
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1435 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.1/winbuild.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.724306 pyrasite-ng-2.0.2/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      171 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/.coveragerc
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       65 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/.gitignore
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      592 2020-10-26 08:12:17.000000 pyrasite-ng-2.0.2/.travis.yml
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    35147 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/LICENSE
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      114 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/MANIFEST.in
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     2542 2023-07-13 13:11:51.724306 pyrasite-ng-2.0.2/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1817 2023-07-13 13:10:02.000000 pyrasite-ng-2.0.2/README.rst
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.707640 pyrasite-ng-2.0.2/docs/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      247 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/API.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1619 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/CLI.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      407 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/Development.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1611 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/GUI.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1783 2020-10-26 08:17:36.000000 pyrasite-ng-2.0.2/docs/Installing.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4598 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/Makefile
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      777 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/MemoryViewer.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     2341 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/Payloads.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      665 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/Shell.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     7131 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/conf.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      600 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/docs/index.rst
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.697640 pyrasite-ng-2.0.2/pkgs/
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.707640 pyrasite-ng-2.0.2/pkgs/arch/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      684 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pkgs/arch/PKGBUILD
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.707640 pyrasite-ng-2.0.2/pkgs/fedora/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1832 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pkgs/fedora/pyrasite.spec
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.707640 pyrasite-ng-2.0.2/pkgs/ubuntu/
+-rwxr-xr-x   0 user202729  (1000) user202729  (1000)      406 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pkgs/ubuntu/make_deb.sh
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.714306 pyrasite-ng-2.0.2/pyrasite/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        7 2020-10-26 08:05:03.000000 pyrasite-ng-2.0.2/pyrasite/.vimrc
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      992 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     2893 2021-03-03 09:56:00.000000 pyrasite-ng-2.0.2/pyrasite/injector.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1233 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/inspector.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     7635 2021-03-03 10:02:48.000000 pyrasite-ng-2.0.2/pyrasite/ipc.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     5770 2020-10-26 08:12:58.000000 pyrasite-ng-2.0.2/pyrasite/main.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.717640 pyrasite-ng-2.0.2/pyrasite/payloads/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      575 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/dump_memory.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       93 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/dump_modules.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      154 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/dump_stacks.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       23 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/force_garbage_collection.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       22 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/helloworld.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      988 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/reverse_python_shell.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1213 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/reverse_shell.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      111 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/start_callgraph.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      129 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/payloads/stop_callgraph.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     5832 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/reverse.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     9431 2020-10-26 08:06:11.000000 pyrasite-ng-2.0.2/pyrasite/tags
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.720973 pyrasite-ng-2.0.2/pyrasite/tests/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/tests/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      521 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/tests/context_manager_case.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     2669 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/tests/test_cli.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     3213 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/tests/test_code_injection.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     2941 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/tests/test_ipc.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     2185 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/tests/utils.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.720973 pyrasite-ng-2.0.2/pyrasite/tools/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/tools/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     5767 2023-07-13 13:07:04.000000 pyrasite-ng-2.0.2/pyrasite/tools/memory_viewer.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     2186 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/tools/shell.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.720973 pyrasite-ng-2.0.2/pyrasite/win/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     6614 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/pyrasite/win/inject_python.cpp
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-07-13 13:11:51.724306 pyrasite-ng-2.0.2/pyrasite_ng.egg-info/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     2542 2023-07-13 13:11:51.000000 pyrasite-ng-2.0.2/pyrasite_ng.egg-info/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1387 2023-07-13 13:11:51.000000 pyrasite-ng-2.0.2/pyrasite_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-07-13 13:11:51.000000 pyrasite-ng-2.0.2/pyrasite_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      151 2023-07-13 13:11:51.000000 pyrasite-ng-2.0.2/pyrasite_ng.egg-info/entry_points.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2021-10-23 08:34:30.000000 pyrasite-ng-2.0.2/pyrasite_ng.egg-info/not-zip-safe
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        6 2023-07-13 13:11:51.000000 pyrasite-ng-2.0.2/pyrasite_ng.egg-info/requires.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        9 2023-07-13 13:11:51.000000 pyrasite-ng-2.0.2/pyrasite_ng.egg-info/top_level.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       38 2023-07-13 13:11:51.724306 pyrasite-ng-2.0.2/setup.cfg
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     3029 2023-07-13 13:11:22.000000 pyrasite-ng-2.0.2/setup.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      332 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/tox.ini
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1435 2020-10-26 07:54:38.000000 pyrasite-ng-2.0.2/winbuild.py
```

### Comparing `pyrasite-ng-2.0.1/.travis.yml` & `pyrasite-ng-2.0.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/LICENSE` & `pyrasite-ng-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/PKG-INFO` & `pyrasite-ng-2.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,80 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyrasite-ng
-Version: 2.0.1
+Version: 2.0.2
 Summary: Inject code into a running Python process
 Home-page: https://github.com/user202729/pyrasite-ng
 Author: Luke Macken
 Author-email: lmacken@redhat.com
 License: GPLv3
-Description: pyrasite (updated)
-        ==================
-        
-        This package is a fork of https://github.com/lmacken/pyrasite containing several important fixes to make pyrasite work on modern systems.
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-         * `gdb <https://www.gnu.org/s/gdb>`_ (version 7.3+ (or RHEL5+))
-         
-        On OS X you will need to have a codesigned gdb - see https://sourceware.org/gdb/wiki/BuildingOnDarwin
-        if you get errors while running with --verbose which mention codesigning.
-        
-        On Linux machines, run `echo 0 | sudo tee /proc/sys/kernel/yama/ptrace_scope` before running pyrasite.
-        
-        Compatibility
-        ~~~~~~~~~~~~~
-        
-        Pyrasite works with Python 2.4 and newer. Injection works between versions
-        as well, so you can run Pyrasite under Python 3 and inject into 2, and
-        vice versa.
-        
-        pyrasite-gui
-        ~~~~~~~~~~~~
-        
-        The graphical interface can be found here: https://github.com/lmacken/pyrasite-gui
-        
-        Authors
-        ~~~~~~~
-        
-        Created by `Luke Macken <http://twitter.com/lmacken>`_ with the help of
-        `David Malcolm <http://dmalcolm.livejournal.com>`_ and many other
-        `contributors <https://github.com/lmacken/pyrasite/contributors>`_.
-        Logo by `Adam Saunders <https://fedorahosted.org/design-team/ticket/214>`_.
-        
-        Licenses
-        ~~~~~~~~
-        
-        Code
-        ^^^^
-        
-        .. image:: https://www.gnu.org/graphics/gplv3-127x51.png
-           :target: https://www.gnu.org/licenses/gpl.txt
-        
-        Logo
-        ^^^^
-        
-        .. image:: https://creativecommons.org/images/deed/nolaw.png
-           :target: https://creativecommons.org/publicdomain/zero/1.0/
-        
 Keywords: debugging injection runtime
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+pyrasite (updated)
+==================
+
+.. image:: https://img.shields.io/pypi/v/pyrasite-ng?style=flat
+   :target: https://pypi.python.org/pypi/pyrasite-ng/
+
+This package is a fork of https://github.com/lmacken/pyrasite containing several important fixes to make pyrasite work on modern systems.
+
+Requirements
+~~~~~~~~~~~~
+
+ * `gdb <https://www.gnu.org/s/gdb>`_ (version 7.3+ (or RHEL5+))
+ 
+On OS X you will need to have a codesigned gdb - see https://sourceware.org/gdb/wiki/BuildingOnDarwin
+if you get errors while running with --verbose which mention codesigning.
+
+On Linux machines, run `echo 0 | sudo tee /proc/sys/kernel/yama/ptrace_scope` before running pyrasite.
+
+Compatibility
+~~~~~~~~~~~~~
+
+Pyrasite works with Python 2.4 and newer. Injection works between versions
+as well, so you can run Pyrasite under Python 3 and inject into 2, and
+vice versa.
+
+pyrasite-gui
+~~~~~~~~~~~~
+
+The graphical interface can be found here: https://github.com/lmacken/pyrasite-gui
+
+Bugs
+~~~~
+
+Report bug of this fork on GitHub: https://github.com/user202729/pyrasite-ng/issues
+
+Alternatively, as a workaround while waiting for the bug to be fixed,
+it's possible to use gdb to inject code into Python directly: https://stackoverflow.com/a/70312000/5267751
+
+Authors
+~~~~~~~
+
+Created by `Luke Macken <http://twitter.com/lmacken>`_ with the help of
+`David Malcolm <http://dmalcolm.livejournal.com>`_ and many other
+`contributors <https://github.com/lmacken/pyrasite/contributors>`_.
+Logo by `Adam Saunders <https://fedorahosted.org/design-team/ticket/214>`_.
+
+Licenses
+~~~~~~~~
+
+Code
+^^^^
+
+.. image:: https://www.gnu.org/graphics/gplv3-127x51.png
+   :target: https://www.gnu.org/licenses/gpl.txt
+
+Logo
+^^^^
+
+.. image:: https://creativecommons.org/images/deed/nolaw.png
+   :target: https://creativecommons.org/publicdomain/zero/1.0/
```

### Comparing `pyrasite-ng-2.0.1/README.rst` & `pyrasite-ng-2.0.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 pyrasite (updated)
 ==================
 
+.. image:: https://img.shields.io/pypi/v/pyrasite-ng?style=flat
+   :target: https://pypi.python.org/pypi/pyrasite-ng/
+
 This package is a fork of https://github.com/lmacken/pyrasite containing several important fixes to make pyrasite work on modern systems.
 
 Requirements
 ~~~~~~~~~~~~
 
  * `gdb <https://www.gnu.org/s/gdb>`_ (version 7.3+ (or RHEL5+))
  
@@ -21,14 +24,22 @@
 vice versa.
 
 pyrasite-gui
 ~~~~~~~~~~~~
 
 The graphical interface can be found here: https://github.com/lmacken/pyrasite-gui
 
+Bugs
+~~~~
+
+Report bug of this fork on GitHub: https://github.com/user202729/pyrasite-ng/issues
+
+Alternatively, as a workaround while waiting for the bug to be fixed,
+it's possible to use gdb to inject code into Python directly: https://stackoverflow.com/a/70312000/5267751
+
 Authors
 ~~~~~~~
 
 Created by `Luke Macken <http://twitter.com/lmacken>`_ with the help of
 `David Malcolm <http://dmalcolm.livejournal.com>`_ and many other
 `contributors <https://github.com/lmacken/pyrasite/contributors>`_.
 Logo by `Adam Saunders <https://fedorahosted.org/design-team/ticket/214>`_.
```

### Comparing `pyrasite-ng-2.0.1/docs/CLI.rst` & `pyrasite-ng-2.0.2/docs/CLI.rst`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/docs/GUI.rst` & `pyrasite-ng-2.0.2/docs/GUI.rst`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/docs/Installing.rst` & `pyrasite-ng-2.0.2/docs/Installing.rst`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/docs/Makefile` & `pyrasite-ng-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/docs/MemoryViewer.rst` & `pyrasite-ng-2.0.2/docs/MemoryViewer.rst`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/docs/Payloads.rst` & `pyrasite-ng-2.0.2/docs/Payloads.rst`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/docs/Shell.rst` & `pyrasite-ng-2.0.2/docs/Shell.rst`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/docs/conf.py` & `pyrasite-ng-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/docs/index.rst` & `pyrasite-ng-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pkgs/arch/PKGBUILD` & `pyrasite-ng-2.0.2/pkgs/arch/PKGBUILD`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pkgs/fedora/pyrasite.spec` & `pyrasite-ng-2.0.2/pkgs/fedora/pyrasite.spec`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/__init__.py` & `pyrasite-ng-2.0.2/pyrasite/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/injector.py` & `pyrasite-ng-2.0.2/pyrasite/injector.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/inspector.py` & `pyrasite-ng-2.0.2/pyrasite/inspector.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/ipc.py` & `pyrasite-ng-2.0.2/pyrasite/ipc.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/main.py` & `pyrasite-ng-2.0.2/pyrasite/main.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/payloads/dump_memory.py` & `pyrasite-ng-2.0.2/pyrasite/payloads/dump_memory.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/payloads/reverse_python_shell.py` & `pyrasite-ng-2.0.2/pyrasite/payloads/reverse_python_shell.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/payloads/reverse_shell.py` & `pyrasite-ng-2.0.2/pyrasite/payloads/reverse_shell.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/reverse.py` & `pyrasite-ng-2.0.2/pyrasite/reverse.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/tags` & `pyrasite-ng-2.0.2/pyrasite/tags`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/tests/context_manager_case.py` & `pyrasite-ng-2.0.2/pyrasite/tests/context_manager_case.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/tests/test_cli.py` & `pyrasite-ng-2.0.2/pyrasite/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/tests/test_code_injection.py` & `pyrasite-ng-2.0.2/pyrasite/tests/test_code_injection.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/tests/test_ipc.py` & `pyrasite-ng-2.0.2/pyrasite/tests/test_ipc.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/tests/utils.py` & `pyrasite-ng-2.0.2/pyrasite/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/tools/memory_viewer.py` & `pyrasite-ng-2.0.2/pyrasite/tools/memory_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
         # Title
         self.bigtext = urwid.BigText('pyrasite ' + __version__, None)
         self.bigtext.set_font(urwid.Thin6x6Font())
         bt = urwid.Padding(self.bigtext, 'left', None)
         bt = urwid.AttrWrap(bt, 'bigtext')
 
-        # Create the object outpu
+        # Create the object output
         self.object_output = urwid.Text("", wrap='any')
         ca = urwid.AttrWrap(self.object_output, 'object_output')
 
         # Select the first object
         self.object_buttons[2].set_state(True)
 
         # ListBox
```

### Comparing `pyrasite-ng-2.0.1/pyrasite/tools/shell.py` & `pyrasite-ng-2.0.2/pyrasite/tools/shell.py`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite/win/inject_python.cpp` & `pyrasite-ng-2.0.2/pyrasite/win/inject_python.cpp`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/pyrasite_ng.egg-info/PKG-INFO` & `pyrasite-ng-2.0.2/pyrasite_ng.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,80 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyrasite-ng
-Version: 2.0.1
+Version: 2.0.2
 Summary: Inject code into a running Python process
 Home-page: https://github.com/user202729/pyrasite-ng
 Author: Luke Macken
 Author-email: lmacken@redhat.com
 License: GPLv3
-Description: pyrasite (updated)
-        ==================
-        
-        This package is a fork of https://github.com/lmacken/pyrasite containing several important fixes to make pyrasite work on modern systems.
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-         * `gdb <https://www.gnu.org/s/gdb>`_ (version 7.3+ (or RHEL5+))
-         
-        On OS X you will need to have a codesigned gdb - see https://sourceware.org/gdb/wiki/BuildingOnDarwin
-        if you get errors while running with --verbose which mention codesigning.
-        
-        On Linux machines, run `echo 0 | sudo tee /proc/sys/kernel/yama/ptrace_scope` before running pyrasite.
-        
-        Compatibility
-        ~~~~~~~~~~~~~
-        
-        Pyrasite works with Python 2.4 and newer. Injection works between versions
-        as well, so you can run Pyrasite under Python 3 and inject into 2, and
-        vice versa.
-        
-        pyrasite-gui
-        ~~~~~~~~~~~~
-        
-        The graphical interface can be found here: https://github.com/lmacken/pyrasite-gui
-        
-        Authors
-        ~~~~~~~
-        
-        Created by `Luke Macken <http://twitter.com/lmacken>`_ with the help of
-        `David Malcolm <http://dmalcolm.livejournal.com>`_ and many other
-        `contributors <https://github.com/lmacken/pyrasite/contributors>`_.
-        Logo by `Adam Saunders <https://fedorahosted.org/design-team/ticket/214>`_.
-        
-        Licenses
-        ~~~~~~~~
-        
-        Code
-        ^^^^
-        
-        .. image:: https://www.gnu.org/graphics/gplv3-127x51.png
-           :target: https://www.gnu.org/licenses/gpl.txt
-        
-        Logo
-        ^^^^
-        
-        .. image:: https://creativecommons.org/images/deed/nolaw.png
-           :target: https://creativecommons.org/publicdomain/zero/1.0/
-        
 Keywords: debugging injection runtime
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+pyrasite (updated)
+==================
+
+.. image:: https://img.shields.io/pypi/v/pyrasite-ng?style=flat
+   :target: https://pypi.python.org/pypi/pyrasite-ng/
+
+This package is a fork of https://github.com/lmacken/pyrasite containing several important fixes to make pyrasite work on modern systems.
+
+Requirements
+~~~~~~~~~~~~
+
+ * `gdb <https://www.gnu.org/s/gdb>`_ (version 7.3+ (or RHEL5+))
+ 
+On OS X you will need to have a codesigned gdb - see https://sourceware.org/gdb/wiki/BuildingOnDarwin
+if you get errors while running with --verbose which mention codesigning.
+
+On Linux machines, run `echo 0 | sudo tee /proc/sys/kernel/yama/ptrace_scope` before running pyrasite.
+
+Compatibility
+~~~~~~~~~~~~~
+
+Pyrasite works with Python 2.4 and newer. Injection works between versions
+as well, so you can run Pyrasite under Python 3 and inject into 2, and
+vice versa.
+
+pyrasite-gui
+~~~~~~~~~~~~
+
+The graphical interface can be found here: https://github.com/lmacken/pyrasite-gui
+
+Bugs
+~~~~
+
+Report bug of this fork on GitHub: https://github.com/user202729/pyrasite-ng/issues
+
+Alternatively, as a workaround while waiting for the bug to be fixed,
+it's possible to use gdb to inject code into Python directly: https://stackoverflow.com/a/70312000/5267751
+
+Authors
+~~~~~~~
+
+Created by `Luke Macken <http://twitter.com/lmacken>`_ with the help of
+`David Malcolm <http://dmalcolm.livejournal.com>`_ and many other
+`contributors <https://github.com/lmacken/pyrasite/contributors>`_.
+Logo by `Adam Saunders <https://fedorahosted.org/design-team/ticket/214>`_.
+
+Licenses
+~~~~~~~~
+
+Code
+^^^^
+
+.. image:: https://www.gnu.org/graphics/gplv3-127x51.png
+   :target: https://www.gnu.org/licenses/gpl.txt
+
+Logo
+^^^^
+
+.. image:: https://creativecommons.org/images/deed/nolaw.png
+   :target: https://creativecommons.org/publicdomain/zero/1.0/
```

### Comparing `pyrasite-ng-2.0.1/pyrasite_ng.egg-info/SOURCES.txt` & `pyrasite-ng-2.0.2/pyrasite_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrasite-ng-2.0.1/setup.py` & `pyrasite-ng-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     # These imports are not used, but make
     # tests pass smoothly on python2.7
     import multiprocessing
     import logging
 except Exception:
     pass
 
-version = '2.0.1'
+version = '2.0.2'
 
 f = open('README.rst')
 long_description = f.read()
 f.close()
 
 requirements = ['urwid']
 if sys.version_info[0] == 3:
```

### Comparing `pyrasite-ng-2.0.1/winbuild.py` & `pyrasite-ng-2.0.2/winbuild.py`

 * *Files identical despite different names*

