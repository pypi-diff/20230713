# Comparing `tmp/vdirsyncer-0.9.2.tar.gz` & `tmp/vdirsyncer-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdirsyncer-0.9.2.tar", last modified: Sun Mar 13 19:55:09 2016, max compression
+gzip compressed data, was "dist/vdirsyncer-0.9.3.tar", last modified: Tue Mar 22 19:52:50 2016, max compression
```

## Comparing `vdirsyncer-0.9.2.tar` & `vdirsyncer-0.9.3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/
--rw-r--r--   0 untitaker  (1000) users      (100)     2138 2016-03-04 14:07:38.000000 vdirsyncer-0.9.2/README.rst
--rw-r--r--   0 untitaker  (1000) users      (100)       24 2016-03-04 14:09:12.000000 vdirsyncer-0.9.2/docs-requirements.txt
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer/
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer/cli/
--rw-r--r--   0 untitaker  (1000) users      (100)     4851 2016-03-07 11:29:41.000000 vdirsyncer-0.9.2/vdirsyncer/cli/tasks.py
--rw-r--r--   0 untitaker  (1000) users      (100)     6677 2016-03-10 20:44:43.000000 vdirsyncer-0.9.2/vdirsyncer/cli/__init__.py
--rw-r--r--   0 untitaker  (1000) users      (100)    16240 2016-03-07 12:05:42.000000 vdirsyncer-0.9.2/vdirsyncer/cli/utils.py
--rw-r--r--   0 untitaker  (1000) users      (100)     7979 2016-03-04 09:39:13.000000 vdirsyncer-0.9.2/vdirsyncer/cli/config.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2841 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/cli/fetchparams.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1482 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/metasync.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1269 2016-03-04 09:39:13.000000 vdirsyncer-0.9.2/vdirsyncer/__init__.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2239 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/repair.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer/storage/
--rw-r--r--   0 untitaker  (1000) users      (100)     7680 2016-03-09 14:50:32.000000 vdirsyncer-0.9.2/vdirsyncer/storage/base.py
--rw-r--r--   0 untitaker  (1000) users      (100)      302 2015-07-22 06:58:15.000000 vdirsyncer-0.9.2/vdirsyncer/storage/__init__.py
--rw-r--r--   0 untitaker  (1000) users      (100)     5591 2016-03-05 18:54:08.000000 vdirsyncer-0.9.2/vdirsyncer/storage/http.py
--rw-r--r--   0 untitaker  (1000) users      (100)     8721 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/storage/remotestorage.py
--rw-r--r--   0 untitaker  (1000) users      (100)    27713 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/storage/dav.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2040 2016-03-09 14:50:32.000000 vdirsyncer-0.9.2/vdirsyncer/storage/memory.py
--rw-r--r--   0 untitaker  (1000) users      (100)     5484 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/storage/singlefile.py
--rw-r--r--   0 untitaker  (1000) users      (100)     6967 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/storage/filesystem.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1767 2016-03-07 11:09:24.000000 vdirsyncer-0.9.2/vdirsyncer/exceptions.py
--rw-r--r--   0 untitaker  (1000) users      (100)    12823 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/sync.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer/utils/
--rw-r--r--   0 untitaker  (1000) users      (100)     6307 2016-01-08 22:19:31.000000 vdirsyncer-0.9.2/vdirsyncer/utils/__init__.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2486 2016-03-10 11:13:56.000000 vdirsyncer-0.9.2/vdirsyncer/utils/http.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1765 2015-12-18 20:12:53.000000 vdirsyncer-0.9.2/vdirsyncer/utils/compat.py
--rw-r--r--   0 untitaker  (1000) users      (100)     9740 2016-03-04 09:09:37.000000 vdirsyncer-0.9.2/vdirsyncer/utils/vobject.py
--rw-r--r--   0 untitaker  (1000) users      (100)      116 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer/version.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2780 2016-03-05 20:05:46.000000 vdirsyncer-0.9.2/setup.py
--rw-r--r--   0 untitaker  (1000) users      (100)      269 2016-03-04 14:07:38.000000 vdirsyncer-0.9.2/ISSUE_TEMPLATE.md
--rw-r--r--   0 untitaker  (1000) users      (100)     2904 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/PKG-INFO
--rw-r--r--   0 untitaker  (1000) users      (100)      403 2016-03-04 14:09:12.000000 vdirsyncer-0.9.2/MANIFEST.in
--rw-r--r--   0 untitaker  (1000) users      (100)     4171 2016-03-13 19:23:09.000000 vdirsyncer-0.9.2/.travis.yml
--rw-r--r--   0 untitaker  (1000) users      (100)      137 2016-03-11 12:36:35.000000 vdirsyncer-0.9.2/.gitignore
--rw-r--r--   0 untitaker  (1000) users      (100)      198 2015-07-22 06:58:15.000000 vdirsyncer-0.9.2/AUTHORS.rst
--rw-r--r--   0 untitaker  (1000) users      (100)      136 2016-03-04 14:07:38.000000 vdirsyncer-0.9.2/CONTRIBUTING.rst
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/docs/
--rw-r--r--   0 untitaker  (1000) users      (100)     3885 2016-02-24 15:44:25.000000 vdirsyncer-0.9.2/docs/conf.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1588 2016-01-16 22:29:22.000000 vdirsyncer-0.9.2/docs/keyring.rst
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/docs/_static/
--rw-r--r--   0 untitaker  (1000) users      (100)        0 2015-07-22 06:58:15.000000 vdirsyncer-0.9.2/docs/_static/.gitkeep
--rw-r--r--   0 untitaker  (1000) users      (100)     2508 2016-03-04 14:11:14.000000 vdirsyncer-0.9.2/docs/packaging.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     4081 2015-12-06 19:59:56.000000 vdirsyncer-0.9.2/docs/vdir.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     1754 2016-03-04 14:07:38.000000 vdirsyncer-0.9.2/docs/contributing.rst
--rw-r--r--   0 untitaker  (1000) users      (100)      131 2015-07-22 06:58:15.000000 vdirsyncer-0.9.2/docs/license.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     2449 2016-02-24 15:44:25.000000 vdirsyncer-0.9.2/docs/when.rst
--rw-r--r--   0 untitaker  (1000) users      (100)      817 2016-03-04 14:09:12.000000 vdirsyncer-0.9.2/docs/index.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     6709 2014-06-22 20:43:11.000000 vdirsyncer-0.9.2/docs/make.bat
--rw-r--r--   0 untitaker  (1000) users      (100)     4378 2016-03-04 09:09:37.000000 vdirsyncer-0.9.2/docs/config.rst
--rw-r--r--   0 untitaker  (1000) users      (100)      445 2016-03-04 14:07:38.000000 vdirsyncer-0.9.2/docs/contact.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     6026 2016-03-09 14:50:32.000000 vdirsyncer-0.9.2/docs/supported.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     5778 2016-03-04 09:09:37.000000 vdirsyncer-0.9.2/docs/tutorial.rst
--rw-r--r--   0 untitaker  (1000) users      (100)       31 2015-07-20 15:40:05.000000 vdirsyncer-0.9.2/docs/changelog.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     2142 2016-01-16 22:29:14.000000 vdirsyncer-0.9.2/docs/ssl-tutorial.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     3282 2016-03-04 09:09:37.000000 vdirsyncer-0.9.2/docs/problems.rst
--rw-r--r--   0 untitaker  (1000) users      (100)     6778 2014-06-22 20:43:11.000000 vdirsyncer-0.9.2/docs/Makefile
--rw-r--r--   0 untitaker  (1000) users      (100)     1084 2016-03-04 09:09:37.000000 vdirsyncer-0.9.2/LICENSE
--rw-r--r--   0 untitaker  (1000) users      (100)      196 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/setup.cfg
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/scripts/
--rw-r--r--   0 untitaker  (1000) users      (100)     1871 2016-03-13 19:22:55.000000 vdirsyncer-0.9.2/scripts/make_travisconf.py
--rw-r--r--   0 untitaker  (1000) users      (100)      862 2016-03-13 18:03:20.000000 vdirsyncer-0.9.2/scripts/travis-install.sh
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/tests/
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/tests/cli/
--rw-r--r--   0 untitaker  (1000) users      (100)     4474 2016-03-04 09:09:37.000000 vdirsyncer-0.9.2/tests/cli/test_fetchparams.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2315 2016-03-09 14:50:32.000000 vdirsyncer-0.9.2/tests/cli/test_repair.py
--rw-r--r--   0 untitaker  (1000) users      (100)      401 2016-03-04 09:39:13.000000 vdirsyncer-0.9.2/tests/cli/test_utils.py
--rw-r--r--   0 untitaker  (1000) users      (100)     5260 2016-02-15 14:45:29.000000 vdirsyncer-0.9.2/tests/cli/test_config.py
--rw-r--r--   0 untitaker  (1000) users      (100)     3867 2015-03-07 14:07:29.000000 vdirsyncer-0.9.2/tests/cli/.coverage
--rw-r--r--   0 untitaker  (1000) users      (100)      777 2015-07-22 06:58:15.000000 vdirsyncer-0.9.2/tests/cli/conftest.py
--rw-r--r--   0 untitaker  (1000) users      (100)    11135 2016-03-13 18:03:20.000000 vdirsyncer-0.9.2/tests/cli/test_main.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1635 2015-09-24 21:39:04.000000 vdirsyncer-0.9.2/tests/cli/test_discover.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2104 2016-03-09 14:50:32.000000 vdirsyncer-0.9.2/tests/test_metasync.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1465 2016-03-09 14:50:32.000000 vdirsyncer-0.9.2/tests/__init__.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/tests/storage/
--rw-r--r--   0 untitaker  (1000) users      (100)      827 2015-11-04 23:13:02.000000 vdirsyncer-0.9.2/tests/storage/test_remotestorage.py
--rw-r--r--   0 untitaker  (1000) users      (100)     9664 2016-03-13 18:03:20.000000 vdirsyncer-0.9.2/tests/storage/__init__.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/tests/storage/dav/
--rw-r--r--   0 untitaker  (1000) users      (100)     1541 2016-01-25 17:35:27.000000 vdirsyncer-0.9.2/tests/storage/dav/__init__.py
--rw-r--r--   0 untitaker  (1000) users      (100)      266 2015-12-16 18:39:53.000000 vdirsyncer-0.9.2/tests/storage/dav/test_utils.py
--rw-r--r--   0 untitaker  (1000) users      (100)     4606 2015-09-24 21:39:04.000000 vdirsyncer-0.9.2/tests/storage/dav/test_caldav.py
--rw-r--r--   0 untitaker  (1000) users      (100)      303 2015-09-24 21:39:04.000000 vdirsyncer-0.9.2/tests/storage/dav/test_carddav.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2367 2016-02-25 02:02:46.000000 vdirsyncer-0.9.2/tests/storage/test_filesystem.py
--rw-r--r--   0 untitaker  (1000) users      (100)      724 2015-09-24 21:39:04.000000 vdirsyncer-0.9.2/tests/storage/test_singlefile.py
--rw-r--r--   0 untitaker  (1000) users      (100)     3650 2015-07-22 06:58:15.000000 vdirsyncer-0.9.2/tests/storage/test_http.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/tests/storage/servers/
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/tests/storage/servers/radicale/
--rw-r--r--   0 untitaker  (1000) users      (100)      485 2015-12-18 20:12:53.000000 vdirsyncer-0.9.2/tests/storage/servers/radicale/install.sh
--rw-r--r--   0 untitaker  (1000) users      (100)     3970 2015-09-24 21:39:04.000000 vdirsyncer-0.9.2/tests/storage/servers/radicale/__init__.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/tests/storage/servers/skip/
--rwxr-xr-x   0 untitaker  (1000) users      (100)       10 2015-09-24 21:39:04.000000 vdirsyncer-0.9.2/tests/storage/servers/skip/install.sh
--rw-r--r--   0 untitaker  (1000) users      (100)      139 2015-09-24 21:39:04.000000 vdirsyncer-0.9.2/tests/storage/servers/skip/__init__.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2258 2015-09-24 21:39:04.000000 vdirsyncer-0.9.2/tests/storage/test_http_with_singlefile.py
--rw-r--r--   0 untitaker  (1000) users      (100)      313 2015-07-22 06:58:15.000000 vdirsyncer-0.9.2/tests/storage/test_memory.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1012 2016-03-11 12:36:35.000000 vdirsyncer-0.9.2/tests/conftest.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/tests/utils/
--rw-r--r--   0 untitaker  (1000) users      (100)       24 2015-07-22 06:58:15.000000 vdirsyncer-0.9.2/tests/utils/__init__.py
--rw-r--r--   0 untitaker  (1000) users      (100)     3006 2016-03-13 19:54:58.000000 vdirsyncer-0.9.2/tests/utils/test_main.py
--rw-r--r--   0 untitaker  (1000) users      (100)     5500 2016-03-04 09:09:37.000000 vdirsyncer-0.9.2/tests/utils/test_vobject.py
--rw-r--r--   0 untitaker  (1000) users      (100)    10692 2016-03-04 09:09:37.000000 vdirsyncer-0.9.2/tests/test_sync.py
--rw-r--r--   0 untitaker  (1000) users      (100)    12584 2016-03-13 19:54:58.000000 vdirsyncer-0.9.2/CHANGELOG.rst
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer.egg-info/
--rw-r--r--   0 untitaker  (1000) users      (100)       11 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer.egg-info/top_level.txt
--rw-r--r--   0 untitaker  (1000) users      (100)     2904 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer.egg-info/PKG-INFO
--rw-r--r--   0 untitaker  (1000) users      (100)        1 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer.egg-info/dependency_links.txt
--rw-r--r--   0 untitaker  (1000) users      (100)      169 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer.egg-info/requires.txt
--rw-r--r--   0 untitaker  (1000) users      (100)       52 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer.egg-info/entry_points.txt
--rw-r--r--   0 untitaker  (1000) users      (100)     2265 2016-03-13 19:55:09.000000 vdirsyncer-0.9.2/vdirsyncer.egg-info/SOURCES.txt
--rw-r--r--   0 untitaker  (1000) users      (100)       61 2016-03-11 12:36:35.000000 vdirsyncer-0.9.2/test-requirements.txt
--rw-r--r--   0 untitaker  (1000) users      (100)      567 2016-03-11 12:36:35.000000 vdirsyncer-0.9.2/.gitmodules
--rw-r--r--   0 untitaker  (1000) users      (100)     2584 2016-03-11 12:36:35.000000 vdirsyncer-0.9.2/Makefile
--rw-r--r--   0 untitaker  (1000) users      (100)     2155 2016-02-15 14:45:29.000000 vdirsyncer-0.9.2/config.example
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/
+-rw-r--r--   0 untitaker  (1000) users      (100)     2267 2016-03-20 13:58:02.000000 vdirsyncer-0.9.3/README.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)       24 2016-03-04 14:09:12.000000 vdirsyncer-0.9.3/docs-requirements.txt
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/vdirsyncer/
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/vdirsyncer/cli/
+-rw-r--r--   0 untitaker  (1000) users      (100)     4851 2016-03-07 11:29:41.000000 vdirsyncer-0.9.3/vdirsyncer/cli/tasks.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     6677 2016-03-10 20:44:43.000000 vdirsyncer-0.9.3/vdirsyncer/cli/__init__.py
+-rw-r--r--   0 untitaker  (1000) users      (100)    16240 2016-03-07 12:05:42.000000 vdirsyncer-0.9.3/vdirsyncer/cli/utils.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     7979 2016-03-04 09:39:13.000000 vdirsyncer-0.9.3/vdirsyncer/cli/config.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2841 2016-03-10 11:13:56.000000 vdirsyncer-0.9.3/vdirsyncer/cli/fetchparams.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1482 2016-03-10 11:13:56.000000 vdirsyncer-0.9.3/vdirsyncer/metasync.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1268 2016-03-15 14:36:17.000000 vdirsyncer-0.9.3/vdirsyncer/__init__.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2239 2016-03-10 11:13:56.000000 vdirsyncer-0.9.3/vdirsyncer/repair.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/vdirsyncer/storage/
+-rw-r--r--   0 untitaker  (1000) users      (100)     7680 2016-03-09 14:50:32.000000 vdirsyncer-0.9.3/vdirsyncer/storage/base.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      302 2015-07-22 06:58:15.000000 vdirsyncer-0.9.3/vdirsyncer/storage/__init__.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     5591 2016-03-05 18:54:08.000000 vdirsyncer-0.9.3/vdirsyncer/storage/http.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     8721 2016-03-10 11:13:56.000000 vdirsyncer-0.9.3/vdirsyncer/storage/remotestorage.py
+-rw-r--r--   0 untitaker  (1000) users      (100)    27709 2016-03-15 14:36:17.000000 vdirsyncer-0.9.3/vdirsyncer/storage/dav.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2040 2016-03-09 14:50:32.000000 vdirsyncer-0.9.3/vdirsyncer/storage/memory.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     5484 2016-03-10 11:13:56.000000 vdirsyncer-0.9.3/vdirsyncer/storage/singlefile.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     6967 2016-03-10 11:13:56.000000 vdirsyncer-0.9.3/vdirsyncer/storage/filesystem.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1767 2016-03-07 11:09:24.000000 vdirsyncer-0.9.3/vdirsyncer/exceptions.py
+-rw-r--r--   0 untitaker  (1000) users      (100)    12823 2016-03-10 11:13:56.000000 vdirsyncer-0.9.3/vdirsyncer/sync.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/vdirsyncer/utils/
+-rw-r--r--   0 untitaker  (1000) users      (100)     6307 2016-01-08 22:19:31.000000 vdirsyncer-0.9.3/vdirsyncer/utils/__init__.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2486 2016-03-10 11:13:56.000000 vdirsyncer-0.9.3/vdirsyncer/utils/http.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1765 2015-12-18 20:12:53.000000 vdirsyncer-0.9.3/vdirsyncer/utils/compat.py
+-rw-r--r--   0 untitaker  (1000) users      (100)    10130 2016-03-20 13:58:05.000000 vdirsyncer-0.9.3/vdirsyncer/utils/vobject.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      116 2016-03-22 19:52:44.000000 vdirsyncer-0.9.3/vdirsyncer/version.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2778 2016-03-15 14:36:17.000000 vdirsyncer-0.9.3/setup.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      269 2016-03-04 14:07:38.000000 vdirsyncer-0.9.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0 untitaker  (1000) users      (100)     3056 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/PKG-INFO
+-rw-r--r--   0 untitaker  (1000) users      (100)      403 2016-03-04 14:09:12.000000 vdirsyncer-0.9.3/MANIFEST.in
+-rw-r--r--   0 untitaker  (1000) users      (100)     6094 2016-03-15 20:05:26.000000 vdirsyncer-0.9.3/.travis.yml
+-rw-r--r--   0 untitaker  (1000) users      (100)      137 2016-03-11 12:36:35.000000 vdirsyncer-0.9.3/.gitignore
+-rw-r--r--   0 untitaker  (1000) users      (100)      198 2015-07-22 06:58:15.000000 vdirsyncer-0.9.3/AUTHORS.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)      136 2016-03-04 14:07:38.000000 vdirsyncer-0.9.3/CONTRIBUTING.rst
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/docs/
+-rw-r--r--   0 untitaker  (1000) users      (100)     3885 2016-02-24 15:44:25.000000 vdirsyncer-0.9.3/docs/conf.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1588 2016-01-16 22:29:22.000000 vdirsyncer-0.9.3/docs/keyring.rst
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/docs/_static/
+-rw-r--r--   0 untitaker  (1000) users      (100)        0 2015-07-22 06:58:15.000000 vdirsyncer-0.9.3/docs/_static/.gitkeep
+-rw-r--r--   0 untitaker  (1000) users      (100)     2766 2016-03-15 19:42:29.000000 vdirsyncer-0.9.3/docs/packaging.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     4081 2015-12-06 19:59:56.000000 vdirsyncer-0.9.3/docs/vdir.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     1926 2016-03-15 19:36:43.000000 vdirsyncer-0.9.3/docs/contributing.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)      131 2015-07-22 06:58:15.000000 vdirsyncer-0.9.3/docs/license.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     2449 2016-02-24 15:44:25.000000 vdirsyncer-0.9.3/docs/when.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)      816 2016-03-15 14:36:17.000000 vdirsyncer-0.9.3/docs/index.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     6709 2014-06-22 20:43:11.000000 vdirsyncer-0.9.3/docs/make.bat
+-rw-r--r--   0 untitaker  (1000) users      (100)     4378 2016-03-04 09:09:37.000000 vdirsyncer-0.9.3/docs/config.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)      442 2016-03-15 23:26:42.000000 vdirsyncer-0.9.3/docs/contact.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     6026 2016-03-09 14:50:32.000000 vdirsyncer-0.9.3/docs/supported.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     5777 2016-03-15 14:36:17.000000 vdirsyncer-0.9.3/docs/tutorial.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)       31 2015-07-20 15:40:05.000000 vdirsyncer-0.9.3/docs/changelog.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     2142 2016-01-16 22:29:14.000000 vdirsyncer-0.9.3/docs/ssl-tutorial.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     3282 2016-03-04 09:09:37.000000 vdirsyncer-0.9.3/docs/problems.rst
+-rw-r--r--   0 untitaker  (1000) users      (100)     6778 2014-06-22 20:43:11.000000 vdirsyncer-0.9.3/docs/Makefile
+-rw-r--r--   0 untitaker  (1000) users      (100)     1084 2016-03-04 09:09:37.000000 vdirsyncer-0.9.3/LICENSE
+-rw-r--r--   0 untitaker  (1000) users      (100)      196 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/setup.cfg
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/scripts/
+-rw-r--r--   0 untitaker  (1000) users      (100)     1986 2016-03-15 20:05:22.000000 vdirsyncer-0.9.3/scripts/make_travisconf.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      862 2016-03-13 18:03:20.000000 vdirsyncer-0.9.3/scripts/travis-install.sh
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/tests/
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/tests/cli/
+-rw-r--r--   0 untitaker  (1000) users      (100)     4474 2016-03-04 09:09:37.000000 vdirsyncer-0.9.3/tests/cli/test_fetchparams.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2315 2016-03-18 20:57:37.000000 vdirsyncer-0.9.3/tests/cli/test_repair.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      401 2016-03-04 09:39:13.000000 vdirsyncer-0.9.3/tests/cli/test_utils.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     5260 2016-02-15 14:45:29.000000 vdirsyncer-0.9.3/tests/cli/test_config.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     3867 2015-03-07 14:07:29.000000 vdirsyncer-0.9.3/tests/cli/.coverage
+-rw-r--r--   0 untitaker  (1000) users      (100)      777 2015-07-22 06:58:15.000000 vdirsyncer-0.9.3/tests/cli/conftest.py
+-rw-r--r--   0 untitaker  (1000) users      (100)    10884 2016-03-22 19:49:24.000000 vdirsyncer-0.9.3/tests/cli/test_main.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1635 2015-09-24 21:39:04.000000 vdirsyncer-0.9.3/tests/cli/test_discover.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2104 2016-03-09 14:50:32.000000 vdirsyncer-0.9.3/tests/test_metasync.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1465 2016-03-18 20:57:37.000000 vdirsyncer-0.9.3/tests/__init__.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/tests/storage/
+-rw-r--r--   0 untitaker  (1000) users      (100)      827 2015-11-04 23:13:02.000000 vdirsyncer-0.9.3/tests/storage/test_remotestorage.py
+-rw-r--r--   0 untitaker  (1000) users      (100)    11083 2016-03-20 13:58:05.000000 vdirsyncer-0.9.3/tests/storage/__init__.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/tests/storage/dav/
+-rw-r--r--   0 untitaker  (1000) users      (100)     1541 2016-01-25 17:35:27.000000 vdirsyncer-0.9.3/tests/storage/dav/__init__.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      266 2015-12-16 18:39:53.000000 vdirsyncer-0.9.3/tests/storage/dav/test_utils.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     4606 2015-09-24 21:39:04.000000 vdirsyncer-0.9.3/tests/storage/dav/test_caldav.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      303 2015-09-24 21:39:04.000000 vdirsyncer-0.9.3/tests/storage/dav/test_carddav.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2367 2016-02-25 02:02:46.000000 vdirsyncer-0.9.3/tests/storage/test_filesystem.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      724 2015-09-24 21:39:04.000000 vdirsyncer-0.9.3/tests/storage/test_singlefile.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     3650 2015-07-22 06:58:15.000000 vdirsyncer-0.9.3/tests/storage/test_http.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/tests/storage/servers/
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/tests/storage/servers/radicale/
+-rw-r--r--   0 untitaker  (1000) users      (100)      485 2015-12-18 20:12:53.000000 vdirsyncer-0.9.3/tests/storage/servers/radicale/install.sh
+-rw-r--r--   0 untitaker  (1000) users      (100)     3970 2015-09-24 21:39:04.000000 vdirsyncer-0.9.3/tests/storage/servers/radicale/__init__.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/tests/storage/servers/skip/
+-rwxr-xr-x   0 untitaker  (1000) users      (100)       10 2015-09-24 21:39:04.000000 vdirsyncer-0.9.3/tests/storage/servers/skip/install.sh
+-rw-r--r--   0 untitaker  (1000) users      (100)      139 2015-09-24 21:39:04.000000 vdirsyncer-0.9.3/tests/storage/servers/skip/__init__.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2258 2015-09-24 21:39:04.000000 vdirsyncer-0.9.3/tests/storage/test_http_with_singlefile.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      313 2015-07-22 06:58:15.000000 vdirsyncer-0.9.3/tests/storage/test_memory.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1012 2016-03-11 12:36:35.000000 vdirsyncer-0.9.3/tests/conftest.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/tests/utils/
+-rw-r--r--   0 untitaker  (1000) users      (100)       24 2015-07-22 06:58:15.000000 vdirsyncer-0.9.3/tests/utils/__init__.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     3006 2016-03-13 19:54:58.000000 vdirsyncer-0.9.3/tests/utils/test_main.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     5500 2016-03-04 09:09:37.000000 vdirsyncer-0.9.3/tests/utils/test_vobject.py
+-rw-r--r--   0 untitaker  (1000) users      (100)    10692 2016-03-04 09:09:37.000000 vdirsyncer-0.9.3/tests/test_sync.py
+-rw-r--r--   0 untitaker  (1000) users      (100)    12919 2016-03-22 19:52:29.000000 vdirsyncer-0.9.3/CHANGELOG.rst
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/vdirsyncer.egg-info/
+-rw-r--r--   0 untitaker  (1000) users      (100)       11 2016-03-22 19:52:45.000000 vdirsyncer-0.9.3/vdirsyncer.egg-info/top_level.txt
+-rw-r--r--   0 untitaker  (1000) users      (100)     3056 2016-03-22 19:52:45.000000 vdirsyncer-0.9.3/vdirsyncer.egg-info/PKG-INFO
+-rw-r--r--   0 untitaker  (1000) users      (100)        1 2016-03-22 19:52:45.000000 vdirsyncer-0.9.3/vdirsyncer.egg-info/dependency_links.txt
+-rw-r--r--   0 untitaker  (1000) users      (100)      169 2016-03-22 19:52:45.000000 vdirsyncer-0.9.3/vdirsyncer.egg-info/requires.txt
+-rw-r--r--   0 untitaker  (1000) users      (100)       52 2016-03-22 19:52:45.000000 vdirsyncer-0.9.3/vdirsyncer.egg-info/entry_points.txt
+-rw-r--r--   0 untitaker  (1000) users      (100)     2265 2016-03-22 19:52:50.000000 vdirsyncer-0.9.3/vdirsyncer.egg-info/SOURCES.txt
+-rw-r--r--   0 untitaker  (1000) users      (100)       61 2016-03-11 12:36:35.000000 vdirsyncer-0.9.3/test-requirements.txt
+-rw-r--r--   0 untitaker  (1000) users      (100)      567 2016-03-11 12:36:35.000000 vdirsyncer-0.9.3/.gitmodules
+-rw-r--r--   0 untitaker  (1000) users      (100)     2499 2016-03-15 20:08:01.000000 vdirsyncer-0.9.3/Makefile
+-rw-r--r--   0 untitaker  (1000) users      (100)     2155 2016-02-15 14:45:29.000000 vdirsyncer-0.9.3/config.example
```

### Comparing `vdirsyncer-0.9.2/README.rst` & `vdirsyncer-0.9.3/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 ==========
 vdirsyncer
 ==========
 
 - `Documentation <https://vdirsyncer.readthedocs.org/en/stable/>`_
-- `Source code <https://github.com/untitaker/vdirsyncer>`_
+- `Source code <https://github.com/pimutils/vdirsyncer>`_
 
 Vdirsyncer synchronizes your calendars and addressbooks between two storages_.
 The most popular purpose is to synchronize a CalDAV/CardDAV server with a local
 folder or file. The local data can then be accessed via a variety of programs_,
 none of which have to know or worry about syncing to a server.
 
 .. _storages: https://vdirsyncer.readthedocs.org/en/latest/config.html#storages
 .. _programs: https://vdirsyncer.readthedocs.org/en/stable/supported.html
 
 It aims to be for CalDAV and CardDAV what `OfflineIMAP
 <http://offlineimap.org/>`_ is for IMAP.
 
-.. image:: https://travis-ci.org/untitaker/vdirsyncer.png?branch=master
-    :target: https://travis-ci.org/untitaker/vdirsyncer
+.. image:: https://travis-ci.org/pimutils/vdirsyncer.png?branch=master
+    :target: https://travis-ci.org/pimutils/vdirsyncer
 
-.. image:: https://codecov.io/github/untitaker/vdirsyncer/coverage.svg?branch=master
-    :target: https://codecov.io/github/untitaker/vdirsyncer?branch=master
+.. image:: https://codecov.io/github/pimutils/vdirsyncer/coverage.svg?branch=master
+    :target: https://codecov.io/github/pimutils/vdirsyncer?branch=master
+
+.. image:: https://badge.waffle.io/pimutils/vdirsyncer.svg?label=ready&title=Ready
+    :target: https://waffle.io/pimutils/vdirsyncer
 
 Links of interest
 =================
 
 * Check out `the tutorial
   <https://vdirsyncer.readthedocs.org/en/stable/tutorial.html>`_ for basic
   usage.
@@ -56,8 +59,8 @@
     <https://salt.bountysource.com/teams/vdirsyncer>`_, for one-time and
     recurring donations.
 
 
 - Flattr can be used for recurring donations:
 
   .. image:: https://api.flattr.com/button/flattr-badge-large.png
-      :target: https://flattr.com/submit/auto?user_id=untitaker&url=https%3A%2F%2Fgithub.com%2Funtitaker%2Fvdirsyncer
+      :target: https://flattr.com/submit/auto?user_id=untitaker&url=https%3A%2F%2Fgithub.com%2Fpimutils%2Fvdirsyncer
```

### Comparing `vdirsyncer-0.9.2/vdirsyncer/cli/tasks.py` & `vdirsyncer-0.9.3/vdirsyncer/cli/tasks.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/cli/__init__.py` & `vdirsyncer-0.9.3/vdirsyncer/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/cli/utils.py` & `vdirsyncer-0.9.3/vdirsyncer/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/cli/config.py` & `vdirsyncer-0.9.3/vdirsyncer/cli/config.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/cli/fetchparams.py` & `vdirsyncer-0.9.3/vdirsyncer/cli/fetchparams.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/metasync.py` & `vdirsyncer-0.9.3/vdirsyncer/metasync.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/__init__.py` & `vdirsyncer-0.9.3/vdirsyncer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 '''
 vdirsyncer is a synchronization tool for vdir. See the README for more details.
 '''
 
 from __future__ import print_function
 
-PROJECT_HOME = 'https://github.com/untitaker/vdirsyncer'
+PROJECT_HOME = 'https://github.com/pimutils/vdirsyncer'
 DOCS_HOME = 'https://vdirsyncer.readthedocs.org/en/stable'
 
 try:
     from .version import version as __version__  # noqa
 except ImportError:  # pragma: no cover
     raise ImportError(
         'Failed to find (autogenerated) version.py. '
```

### Comparing `vdirsyncer-0.9.2/vdirsyncer/repair.py` & `vdirsyncer-0.9.3/vdirsyncer/repair.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/storage/base.py` & `vdirsyncer-0.9.3/vdirsyncer/storage/base.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/storage/http.py` & `vdirsyncer-0.9.3/vdirsyncer/storage/http.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/storage/remotestorage.py` & `vdirsyncer-0.9.3/vdirsyncer/storage/remotestorage.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/storage/dav.py` & `vdirsyncer-0.9.3/vdirsyncer/storage/dav.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,17 +507,17 @@
                 continue
 
             href = self._normalize_href(href.text)
 
             if href in hrefs:
                 # Servers that send duplicate hrefs:
                 # - Zimbra
-                #   https://github.com/untitaker/vdirsyncer/issues/88
+                #   https://github.com/pimutils/vdirsyncer/issues/88
                 # - Davmail
-                #   https://github.com/untitaker/vdirsyncer/issues/144
+                #   https://github.com/pimutils/vdirsyncer/issues/144
                 dav_logger.warning('Skipping identical href: {!r}'
                                    .format(href))
                 continue
 
             props = response.findall('{DAV:}propstat/{DAV:}prop')
             if not props:
                 dav_logger.warning('Skipping {!r}, properties are missing.'
@@ -557,15 +557,15 @@
                     <D:getcontenttype/>
                     <D:getetag/>
                 </D:prop>
             </D:propfind>
             '''
 
         # We use a PROPFIND request instead of addressbook-query due to issues
-        # with Zimbra. See https://github.com/untitaker/vdirsyncer/issues/83
+        # with Zimbra. See https://github.com/pimutils/vdirsyncer/issues/83
         response = self.session.request('PROPFIND', '', data=data,
                                         headers=headers)
         root = _parse_xml(response.content)
 
         rv = self._parse_prop_responses(root)
         for href, etag, prop in rv:
             yield href, etag
@@ -767,15 +767,15 @@
                 </D:prop>
                 <C:filter>
                 {caldavfilter}
                 </C:filter>
             </C:calendar-query>'''
 
         headers = self.session.get_default_headers()
-        # https://github.com/untitaker/vdirsyncer/issues/166
+        # https://github.com/pimutils/vdirsyncer/issues/166
         # The default in CalDAV's calendar-queries is 0, but the examples use
         # an explicit value of 1 for querying items. it is extremely unclear in
         # the spec which values from WebDAV are actually allowed.
         headers['Depth'] = 1
 
         for caldavfilter in caldavfilters:
             xml = data.format(caldavfilter=caldavfilter)
```

### Comparing `vdirsyncer-0.9.2/vdirsyncer/storage/memory.py` & `vdirsyncer-0.9.3/vdirsyncer/storage/memory.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/storage/singlefile.py` & `vdirsyncer-0.9.3/vdirsyncer/storage/singlefile.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/storage/filesystem.py` & `vdirsyncer-0.9.3/vdirsyncer/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/exceptions.py` & `vdirsyncer-0.9.3/vdirsyncer/exceptions.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/sync.py` & `vdirsyncer-0.9.3/vdirsyncer/sync.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/utils/__init__.py` & `vdirsyncer-0.9.3/vdirsyncer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/utils/http.py` & `vdirsyncer-0.9.3/vdirsyncer/utils/http.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/utils/compat.py` & `vdirsyncer-0.9.3/vdirsyncer/utils/compat.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/vdirsyncer/utils/vobject.py` & `vdirsyncer-0.9.3/vdirsyncer/utils/vobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import hashlib
 from itertools import chain, tee
 
 from . import cached_property, uniq
-from .compat import text_type
+from .compat import itervalues, text_type
 
 
 def _process_properties(*s):
     rv = set()
     for key in s:
         rv.add(key + ':')
         rv.add(key + ';')
@@ -18,15 +18,15 @@
 IGNORE_PROPS = _process_properties(
     # PRODID is changed by radicale for some reason after upload
     'PRODID',
     # X-RADICALE-NAME is used by radicale, because hrefs don't really exist in
     # their filesystem backend
     'X-RADICALE-NAME',
     # Apparently this is set by Horde?
-    # https://github.com/untitaker/vdirsyncer/issues/318
+    # https://github.com/pimutils/vdirsyncer/issues/318
     'X-WR-CALNAME',
     # REV is from the VCARD specification and is supposed to change when the
     # item does -- however, we can determine that ourselves
     # Same with LAST-MODIFIED
     'REV',
     'LAST-MODIFIED',
     # Added those because e.g. http://www.feiertage-oesterreich.at/ is
@@ -110,36 +110,43 @@
 def hash_item(text):
     return hashlib.sha256(normalize_item(text).encode('utf-8')).hexdigest()
 
 
 def split_collection(text):
     assert isinstance(text, text_type)
     inline = []
-    items = []
+    items = {}  # uid => item
+    ungrouped_items = []
 
     def inner(item, main):
         if item.name == u'VTIMEZONE':
             inline.append(item)
         elif item.name == u'VCARD':
-            items.append(item)
+            ungrouped_items.append(item)
         elif item.name in (u'VTODO', u'VEVENT', u'VJOURNAL'):
-            items.append(_Component(main.name,
-                                    main.props[:],
-                                    [item]))
+            uid = item.get(u'UID', u'')
+            wrapper = _Component(main.name, main.props[:], [])
+
+            if uid.strip():
+                wrapper = items.setdefault(uid, wrapper)
+            else:
+                ungrouped_items.append(wrapper)
+
+            wrapper.subcomponents.append(item)
         elif item.name in (u'VCALENDAR', u'VADDRESSBOOK'):
             for subitem in item.subcomponents:
                 inner(subitem, item)
         else:
             raise ValueError('Unknown component: {}'
                              .format(item.name))
 
     for main in _Component.parse(text, multiple=True):
         inner(main, main)
 
-    for item in items:
+    for item in chain(itervalues(items), ungrouped_items):
         item.subcomponents.extend(inline)
         yield u'\r\n'.join(item.dump_lines())
 
 _default_join_wrappers = {
     u'VCALENDAR': u'VCALENDAR',
     u'VEVENT': u'VCALENDAR',
     u'VTODO': u'VCALENDAR',
@@ -312,7 +319,13 @@
         for line in iterlines:
             if line.startswith((u' ', u'\t')):
                 rv += line[1:]
             else:
                 break
 
         return rv
+
+    def get(self, key, default=None):
+        try:
+            return self[key]
+        except KeyError:
+            return default
```

### Comparing `vdirsyncer-0.9.2/setup.py` & `vdirsyncer-0.9.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     #
     # Without the above pull request, `verify=False` also disables fingerprint
     # validation. This is *not* what we want, and it's not possible to
     # replicate vdirsyncer's current behavior (verifying fingerprints without
     # verifying against CAs) with older versions of urllib3.
     'requests >=2.4.1, !=2.9.0',
     'lxml >=3.1' + (
-        # See https://github.com/untitaker/vdirsyncer/issues/298
+        # See https://github.com/pimutils/vdirsyncer/issues/298
         # We pin some LXML version that is known to work with PyPy
         # I assume nobody actually uses PyPy with vdirsyncer, so this is
         # moot
         ', <=3.4.4'
         if platform.python_implementation() == 'PyPy'
         else ''
     ),
@@ -65,15 +65,15 @@
     name='vdirsyncer',
     use_scm_version={
         'write_to': 'vdirsyncer/version.py',
     },
     setup_requires=['setuptools_scm'],
     author='Markus Unterwaditzer',
     author_email='markus@unterwaditzer.net',
-    url='https://github.com/untitaker/vdirsyncer',
+    url='https://github.com/pimutils/vdirsyncer',
     description='Synchronize calendars and contacts',
     license='MIT',
     long_description=open('README.rst').read(),
     packages=find_packages(exclude=['tests.*', 'tests']),
     include_package_data=True,
     entry_points={
         'console_scripts': ['vdirsyncer = vdirsyncer.cli:main']
```

### Comparing `vdirsyncer-0.9.2/PKG-INFO` & `vdirsyncer-0.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 1.0
 Name: vdirsyncer
-Version: 0.9.2
+Version: 0.9.3
 Summary: Synchronize calendars and contacts
-Home-page: https://github.com/untitaker/vdirsyncer
+Home-page: https://github.com/pimutils/vdirsyncer
 Author: Markus Unterwaditzer
 Author-email: markus@unterwaditzer.net
 License: MIT
 Description: ==========
         vdirsyncer
         ==========
         
         - `Documentation <https://vdirsyncer.readthedocs.org/en/stable/>`_
-        - `Source code <https://github.com/untitaker/vdirsyncer>`_
+        - `Source code <https://github.com/pimutils/vdirsyncer>`_
         
         Vdirsyncer synchronizes your calendars and addressbooks between two storages_.
         The most popular purpose is to synchronize a CalDAV/CardDAV server with a local
         folder or file. The local data can then be accessed via a variety of programs_,
         none of which have to know or worry about syncing to a server.
         
         .. _storages: https://vdirsyncer.readthedocs.org/en/latest/config.html#storages
         .. _programs: https://vdirsyncer.readthedocs.org/en/stable/supported.html
         
         It aims to be for CalDAV and CardDAV what `OfflineIMAP
         <http://offlineimap.org/>`_ is for IMAP.
         
-        .. image:: https://travis-ci.org/untitaker/vdirsyncer.png?branch=master
-            :target: https://travis-ci.org/untitaker/vdirsyncer
+        .. image:: https://travis-ci.org/pimutils/vdirsyncer.png?branch=master
+            :target: https://travis-ci.org/pimutils/vdirsyncer
         
-        .. image:: https://codecov.io/github/untitaker/vdirsyncer/coverage.svg?branch=master
-            :target: https://codecov.io/github/untitaker/vdirsyncer?branch=master
+        .. image:: https://codecov.io/github/pimutils/vdirsyncer/coverage.svg?branch=master
+            :target: https://codecov.io/github/pimutils/vdirsyncer?branch=master
+        
+        .. image:: https://badge.waffle.io/pimutils/vdirsyncer.svg?label=ready&title=Ready
+            :target: https://waffle.io/pimutils/vdirsyncer
         
         Links of interest
         =================
         
         * Check out `the tutorial
           <https://vdirsyncer.readthedocs.org/en/stable/tutorial.html>`_ for basic
           usage.
@@ -64,10 +67,10 @@
             <https://salt.bountysource.com/teams/vdirsyncer>`_, for one-time and
             recurring donations.
         
         
         - Flattr can be used for recurring donations:
         
           .. image:: https://api.flattr.com/button/flattr-badge-large.png
-              :target: https://flattr.com/submit/auto?user_id=untitaker&url=https%3A%2F%2Fgithub.com%2Funtitaker%2Fvdirsyncer
+              :target: https://flattr.com/submit/auto?user_id=untitaker&url=https%3A%2F%2Fgithub.com%2Fpimutils%2Fvdirsyncer
         
 Platform: UNKNOWN
```

### Comparing `vdirsyncer-0.9.2/docs/conf.py` & `vdirsyncer-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/keyring.rst` & `vdirsyncer-0.9.3/docs/keyring.rst`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/packaging.rst` & `vdirsyncer-0.9.3/docs/packaging.rst`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 The main distribution channel is `PyPI
 <https://pypi.python.org/pypi/vdirsyncer>`_, and source tarballs can be
 obtained there. Do not use the ones from GitHub: Their tarballs contain useless
 junk and are more of a distraction than anything else.
 
 I give each release a tag in the git repo. If you want to get notified of new
 releases, `GitHub's feed
-<https://github.com/untitaker/vdirsyncer/releases.atom>`_ is a good way.
+<https://github.com/pimutils/vdirsyncer/releases.atom>`_ is a good way.
 
 Dependency versions
 ===================
 
 It is strongly discouraged to package vdirsyncer as a Python 2 application.
 Future releases will only work on Python 3.3 and newer versions.
 
@@ -36,30 +36,43 @@
 =======
 
 Everything testing-related goes through the ``Makefile`` in the root of the
 repository or PyPI package. Trying to e.g. run ``py.test`` directly will
 require a lot of environment variables to be set (for configuration) and you
 probably don't want to deal with that.
 
-You can install the testing dependencies with ``make test-install``. You
-probably don't want this since it will use pip to download the dependencies.
-Alternatively you can find the testing dependencies in
+You can install the testing dependencies with::
+
+    make install-test
+
+You probably don't want this since it will use pip to download the
+dependencies. Alternatively you can find the testing dependencies in
 ``test-requirements.txt``, again with lower-bound version requirements.
 
 You also have to have vdirsyncer fully installed at this point. Merely
 ``cd``-ing into the tarball will not be sufficient.
 
-Running the tests happens with ``make test``.
+Running the tests happens with::
+
+    make test
 
 Hypothesis will randomly generate test input. If you care about deterministic
 tests, set the ``DETERMINISTIC_TESTS`` variable to ``"true"``::
 
     make DETERMINISTIC_TESTS=true test
 
 Documentation
 =============
 
-You can find a list of dependencies in ``docs-requirements.txt``.
+Using Sphinx_ you can generate the documentation you're reading right now in a
+variety of formats, such as HTML, PDF, or even as a manpage. That said, I only
+take care of the HTML docs' formatting.
+
+You can find a list of dependencies in ``docs-requirements.txt``. Again, you
+can install those using pip with::
+
+    make install-docs
+
+Then change into the ``docs/`` directory and build whatever format you want
+using the ``Makefile`` in there (run ``make`` for the formats you can build).
 
-Change into the ``docs/`` directory and build whatever format you want. That
-said, I only take care of the HTML docs' formatting -- other targets (such as
-the generated manpage) may look like garbage.
+.. _Sphinx: www.sphinx-doc.org/
```

### Comparing `vdirsyncer-0.9.2/docs/vdir.rst` & `vdirsyncer-0.9.3/docs/vdir.rst`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/contributing.rst` & `vdirsyncer-0.9.3/docs/contributing.rst`

 * *Files 16% similar despite different names*

```diff
@@ -39,18 +39,19 @@
 Running tests, how to set up your development environment
 =========================================================
 
 For many patches, it might suffice to just let Travis run the tests. However,
 Travis is slow, so you might want to run them locally too. For this, set up a
 virtualenv_ and run this inside of it::
 
-    make install-test
-    make install-style
+    make install-dev  # install vdirsyncer from the repo into the virtualenv
+    make install-test  # install test dependencies
+    make install-style  # install dependencies for stylechecking
 
 Then you can run::
 
-    make test
+    make test  # The normal testsuite
     make style  # Stylechecker
 
 If you have any questions, feel free to open issues about it.
 
 .. _virtualenv: http://virtualenv.readthedocs.org/
```

### Comparing `vdirsyncer-0.9.2/docs/when.rst` & `vdirsyncer-0.9.3/docs/when.rst`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/index.rst` & `vdirsyncer-0.9.3/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ==========
 vdirsyncer
 ==========
 
 - `Documentation <https://vdirsyncer.readthedocs.org/en/stable/>`_
-- `Source code <https://github.com/untitaker/vdirsyncer>`_
+- `Source code <https://github.com/pimutils/vdirsyncer>`_
 
 Vdirsyncer synchronizes your calendars and addressbooks between two
 :ref:`storages <storages>`. The most popular purpose is to synchronize a
 CalDAV/CardDAV server with a local folder or file. The local data can then be
 accessed via a variety of :doc:`programs <supported>`, none of which have to
 know or worry about syncing to a server.
```

### Comparing `vdirsyncer-0.9.2/docs/make.bat` & `vdirsyncer-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/config.rst` & `vdirsyncer-0.9.3/docs/config.rst`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/supported.rst` & `vdirsyncer-0.9.3/docs/supported.rst`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/tutorial.rst` & `vdirsyncer-0.9.3/docs/tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 Configuration
 =============
 
 .. note::
 
     - The `config.example from the repository
-      <https://github.com/untitaker/vdirsyncer/blob/master/config.example>`_
+      <https://github.com/pimutils/vdirsyncer/blob/master/config.example>`_
       contains a very terse version of this.
 
     - In this example we set up contacts synchronization, but calendar sync
       works almost the same. Just swap ``type = carddav`` for ``type = caldav``
       and ``fileext = .vcf`` for ``fileext = .ics``.
 
     - Take a look at the :doc:`problems` page if anything doesn't work like
```

### Comparing `vdirsyncer-0.9.2/docs/ssl-tutorial.rst` & `vdirsyncer-0.9.3/docs/ssl-tutorial.rst`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/problems.rst` & `vdirsyncer-0.9.3/docs/problems.rst`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/docs/Makefile` & `vdirsyncer-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/LICENSE` & `vdirsyncer-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/scripts/travis-install.sh` & `vdirsyncer-0.9.3/scripts/travis-install.sh`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/cli/test_fetchparams.py` & `vdirsyncer-0.9.3/tests/cli/test_fetchparams.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/cli/test_repair.py` & `vdirsyncer-0.9.3/tests/cli/test_repair.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/cli/test_config.py` & `vdirsyncer-0.9.3/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/cli/.coverage` & `vdirsyncer-0.9.3/tests/cli/.coverage`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/cli/conftest.py` & `vdirsyncer-0.9.3/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/cli/test_main.py` & `vdirsyncer-0.9.3/tests/cli/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,14 @@
 
 import pytest
 
 import vdirsyncer.cli as cli
 from vdirsyncer.utils.compat import PY2, to_native, to_unicode
 
 
-def test_entry_points(monkeypatch, capsys):
-    monkeypatch.setattr('sys.argv', ['--help'])
-    with pytest.raises(SystemExit) as excinfo:
-        load_entry_point('vdirsyncer', 'console_scripts', 'vdirsyncer')()
-
-    assert excinfo.value.code == 0
-
-
 def test_simple_run(tmpdir, runner):
     runner.write_with_general(dedent('''
     [pair my_pair]
     a = my_a
     b = my_b
     collections = null
```

### Comparing `vdirsyncer-0.9.2/tests/cli/test_discover.py` & `vdirsyncer-0.9.3/tests/cli/test_discover.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/test_metasync.py` & `vdirsyncer-0.9.3/tests/test_metasync.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/__init__.py` & `vdirsyncer-0.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/storage/test_remotestorage.py` & `vdirsyncer-0.9.3/tests/storage/test_remotestorage.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/storage/__init__.py` & `vdirsyncer-0.9.3/tests/storage/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 
 import random
 
+import textwrap
+
 from hypothesis import given
 import hypothesis.strategies as st
 
 import pytest
 
 import vdirsyncer.exceptions as exceptions
 from vdirsyncer.storage.base import Item, normalize_meta_value
 from vdirsyncer.utils.compat import iteritems, text_type, urlquote, urlunquote
 
 from .. import EVENT_TEMPLATE, TASK_TEMPLATE, VCARD_TEMPLATE, \
-    assert_item_equals, printable_characters_strategy
+    assert_item_equals, normalize_item, printable_characters_strategy
 
 
 def get_server_mixin(server_name):
     from . import __name__ as base
     x = __import__('{}.servers.{}'.format(base, server_name), fromlist=[''])
     return x.ServerMixin
 
@@ -107,15 +109,15 @@
     def test_update(self, s, get_item):
         item = get_item()
         href, etag = s.upload(item)
         assert_item_equals(s.get(href)[0], item)
 
         new_item = get_item(uid=item.uid)
         new_etag = s.update(href, new_item, etag)
-        # See https://github.com/untitaker/vdirsyncer/issues/48
+        # See https://github.com/pimutils/vdirsyncer/issues/48
         assert isinstance(new_etag, (bytes, text_type))
         assert_item_equals(s.get(href)[0], new_item)
 
     def test_update_nonexisting(self, s, get_item):
         item = get_item()
         with pytest.raises(exceptions.PreconditionFailed):
             s.update('huehue', item, '"123"')
@@ -281,7 +283,53 @@
         x = s.get_meta('displayname')
         assert x == normalize_meta_value(x)
 
         if not getattr(self, 'dav_server', None):
             # ownCloud replaces "" with "unnamed"
             s.set_meta('displayname', value)
             assert s.get_meta('displayname') == normalize_meta_value(value)
+
+    def test_recurring_events(self, s, item_type):
+        if item_type != 'VEVENT':
+            pytest.skip('This storage instance doesn\'t support iCalendar.')
+
+        uid = u'abc123'
+        item = Item(textwrap.dedent(u'''
+        BEGIN:VCALENDAR
+        VERSION:2.0
+        BEGIN:VEVENT
+        DTSTART;TZID=Australia/Sydney:20140325T084000
+        DTEND;TZID=Australia/Sydney:20140325T101000
+        DTSTAMP:20140327T060506Z
+        UID:{uid}
+        RECURRENCE-ID;TZID=Australia/Sydney:20140325T083000
+        CREATED:20131216T033331Z
+        DESCRIPTION:
+        LAST-MODIFIED:20140327T060215Z
+        LOCATION:
+        SEQUENCE:1
+        STATUS:CONFIRMED
+        SUMMARY:test Event
+        TRANSP:OPAQUE
+        END:VEVENT
+        BEGIN:VEVENT
+        DTSTART;TZID=Australia/Sydney:20140128T083000
+        DTEND;TZID=Australia/Sydney:20140128T100000
+        RRULE:FREQ=WEEKLY;UNTIL=20141208T213000Z;BYDAY=TU
+        DTSTAMP:20140327T060506Z
+        UID:{uid}
+        CREATED:20131216T033331Z
+        DESCRIPTION:
+        LAST-MODIFIED:20140222T101012Z
+        LOCATION:
+        SEQUENCE:0
+        STATUS:CONFIRMED
+        SUMMARY:Test event
+        TRANSP:OPAQUE
+        END:VEVENT
+        END:VCALENDAR
+        '''.format(uid=uid)).strip())
+
+        href, etag = s.upload(item)
+
+        item2, etag2 = s.get(href)
+        assert normalize_item(item) == normalize_item(item2)
```

### Comparing `vdirsyncer-0.9.2/tests/storage/dav/__init__.py` & `vdirsyncer-0.9.3/tests/storage/dav/__init__.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/storage/dav/test_caldav.py` & `vdirsyncer-0.9.3/tests/storage/dav/test_caldav.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/storage/test_filesystem.py` & `vdirsyncer-0.9.3/tests/storage/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/storage/test_singlefile.py` & `vdirsyncer-0.9.3/tests/storage/test_singlefile.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/storage/test_http.py` & `vdirsyncer-0.9.3/tests/storage/test_http.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/storage/servers/radicale/__init__.py` & `vdirsyncer-0.9.3/tests/storage/servers/radicale/__init__.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/storage/test_http_with_singlefile.py` & `vdirsyncer-0.9.3/tests/storage/test_http_with_singlefile.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/conftest.py` & `vdirsyncer-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/utils/test_main.py` & `vdirsyncer-0.9.3/tests/utils/test_main.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/utils/test_vobject.py` & `vdirsyncer-0.9.3/tests/utils/test_vobject.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/tests/test_sync.py` & `vdirsyncer-0.9.3/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/CHANGELOG.rst` & `vdirsyncer-0.9.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,26 @@
 =========
 
 This changelog only contains information that might be useful to end users and
 package maintainers. For further info, see the git commit log.
 
 Package maintainers and users who have to manually update their installation
 may want to subscribe to `GitHub's tag feed
-<https://github.com/untitaker/vdirsyncer/tags.atom>`_.
+<https://github.com/pimutils/vdirsyncer/tags.atom>`_.
+
+Version 0.9.3
+=============
+
+*released on 22 March 2016*
+
+- :storage:`singlefile` and :storage:`http` now handle recurring events
+  properly.
+- Fix a typo in the packaging guidelines.
+- Moved to ``pimutils`` organization on GitHub. Old links *should* redirect,
+  but be aware of client software that doesn't properly handle redirects.
 
 Version 0.9.2
 =============
 
 *released on 13 March 2016*
 
 - Fixed testsuite for environments that don't have any web browser installed.
```

### Comparing `vdirsyncer-0.9.2/vdirsyncer.egg-info/PKG-INFO` & `vdirsyncer-0.9.3/vdirsyncer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 1.0
 Name: vdirsyncer
-Version: 0.9.2
+Version: 0.9.3
 Summary: Synchronize calendars and contacts
-Home-page: https://github.com/untitaker/vdirsyncer
+Home-page: https://github.com/pimutils/vdirsyncer
 Author: Markus Unterwaditzer
 Author-email: markus@unterwaditzer.net
 License: MIT
 Description: ==========
         vdirsyncer
         ==========
         
         - `Documentation <https://vdirsyncer.readthedocs.org/en/stable/>`_
-        - `Source code <https://github.com/untitaker/vdirsyncer>`_
+        - `Source code <https://github.com/pimutils/vdirsyncer>`_
         
         Vdirsyncer synchronizes your calendars and addressbooks between two storages_.
         The most popular purpose is to synchronize a CalDAV/CardDAV server with a local
         folder or file. The local data can then be accessed via a variety of programs_,
         none of which have to know or worry about syncing to a server.
         
         .. _storages: https://vdirsyncer.readthedocs.org/en/latest/config.html#storages
         .. _programs: https://vdirsyncer.readthedocs.org/en/stable/supported.html
         
         It aims to be for CalDAV and CardDAV what `OfflineIMAP
         <http://offlineimap.org/>`_ is for IMAP.
         
-        .. image:: https://travis-ci.org/untitaker/vdirsyncer.png?branch=master
-            :target: https://travis-ci.org/untitaker/vdirsyncer
+        .. image:: https://travis-ci.org/pimutils/vdirsyncer.png?branch=master
+            :target: https://travis-ci.org/pimutils/vdirsyncer
         
-        .. image:: https://codecov.io/github/untitaker/vdirsyncer/coverage.svg?branch=master
-            :target: https://codecov.io/github/untitaker/vdirsyncer?branch=master
+        .. image:: https://codecov.io/github/pimutils/vdirsyncer/coverage.svg?branch=master
+            :target: https://codecov.io/github/pimutils/vdirsyncer?branch=master
+        
+        .. image:: https://badge.waffle.io/pimutils/vdirsyncer.svg?label=ready&title=Ready
+            :target: https://waffle.io/pimutils/vdirsyncer
         
         Links of interest
         =================
         
         * Check out `the tutorial
           <https://vdirsyncer.readthedocs.org/en/stable/tutorial.html>`_ for basic
           usage.
@@ -64,10 +67,10 @@
             <https://salt.bountysource.com/teams/vdirsyncer>`_, for one-time and
             recurring donations.
         
         
         - Flattr can be used for recurring donations:
         
           .. image:: https://api.flattr.com/button/flattr-badge-large.png
-              :target: https://flattr.com/submit/auto?user_id=untitaker&url=https%3A%2F%2Fgithub.com%2Funtitaker%2Fvdirsyncer
+              :target: https://flattr.com/submit/auto?user_id=untitaker&url=https%3A%2F%2Fgithub.com%2Fpimutils%2Fvdirsyncer
         
 Platform: UNKNOWN
```

### Comparing `vdirsyncer-0.9.2/vdirsyncer.egg-info/SOURCES.txt` & `vdirsyncer-0.9.3/vdirsyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/.gitmodules` & `vdirsyncer-0.9.3/.gitmodules`

 * *Files identical despite different names*

### Comparing `vdirsyncer-0.9.2/Makefile` & `vdirsyncer-0.9.3/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 export TESTSERVER_BASE := ./tests/storage/servers/
 export CI := false
 export DETERMINISTIC_TESTS := false
 
 install-servers:
 	set -ex; \
 	for server in $(DAV_SERVER) $(REMOTESTORAGE_SERVER); do \
-		if [ ! -d "$(TESTSERVER_BASE)$$server/" ]; then \
+		if [ ! "$$(ls $(TESTSERVER_BASE)$$server/)" ]; then \
 			git submodule update --init -- "$(TESTSERVER_BASE)$$server"; \
 		fi; \
 		(cd $(TESTSERVER_BASE)$$server && sh install.sh); \
 	done
 
 install-test: install-servers
 	(python --version | grep -vq 'Python 3.3') || pip install enum34
@@ -39,17 +39,15 @@
 install-style:
 	pip install flake8 flake8-import-order sphinx
 	
 style:
 	flake8
 	! grep -ri syncroniz */*
 	sphinx-build -W -b html ./docs/ ./docs/_build/html/
-	python3 scripts/make_travisconf.py | \
-		diff -q .travis.yml - > /dev/null || \
-		(echo 'travis.yml is outdated. Run `make travis-conf`.' && false)
+	python3 scripts/make_travisconf.py | diff -b .travis.yml -
 
 travis-conf:
 	python3 scripts/make_travisconf.py > .travis.yml
 
 install-docs:
 	pip install -r docs-requirements.txt
```

### Comparing `vdirsyncer-0.9.2/config.example` & `vdirsyncer-0.9.3/config.example`

 * *Files identical despite different names*

