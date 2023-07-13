# Comparing `tmp/qbittorrent-api-2023.7.52.tar.gz` & `tmp/qbittorrent-api-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbittorrent-api-2023.7.52.tar", last modified: Thu Jul 13 18:02:37 2023, max compression
+gzip compressed data, was "dist/qbittorrent-api-6.0.0.tar", last modified: Thu Apr 23 04:02:29 2020, max compression
```

## Comparing `qbittorrent-api-2023.7.52.tar` & `qbittorrent-api-6.0.0.tar`

### file list

```diff
@@ -1,104 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.989310 qbittorrent-api-2023.7.52/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-13 18:02:37.989310 qbittorrent-api-2023.7.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.981310 qbittorrent-api-2023.7.52/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.981310 qbittorrent-api-2023.7.52/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.981310 qbittorrent-api-2023.7.52/docs/source/apidoc/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/app.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/attrdict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/definitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/log.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/request.rst
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/rss.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/search.rst
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/sync.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/torrents.rst
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/transfer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/apidoc/version.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/behavior&configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/docs/source/spelling_wordlist
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-13 18:02:37.989310 qbittorrent-api-2023.7.52/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.977309 qbittorrent-api-2023.7.52/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.985309 qbittorrent-api-2023.7.52/src/qbittorrent_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-13 18:02:37.000000 qbittorrent-api-2023.7.52/src/qbittorrent_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-13 18:02:37.000000 qbittorrent-api-2023.7.52/src/qbittorrent_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:02:37.000000 qbittorrent-api-2023.7.52/src/qbittorrent_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:01:55.000000 qbittorrent-api-2023.7.52/src/qbittorrent_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 18:02:37.000000 qbittorrent-api-2023.7.52/src/qbittorrent_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 18:02:37.000000 qbittorrent-api-2023.7.52/src/qbittorrent_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.985309 qbittorrent-api-2023.7.52/src/qbittorrentapi/
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16455 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/_attrdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/_attrdict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/_types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/_version_support.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/_version_support.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/app.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/definitions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/log.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34725 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/rss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/sync.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    87436 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)    32667 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/torrents.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/src/qbittorrentapi/transfer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.989310 qbittorrent-api-2023.7.52/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:02:37.989310 qbittorrent-api-2023.7.52/tests/_resources/
--rw-r--r--   0 runner    (1001) docker     (123)   383556 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/_resources/kubuntu-22.04.2-desktop-amd64.iso.torrent
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/_resources/mypy_stubtest_allowlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/_resources/root_folder.torrent
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/_resources/server.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/_resources/server.key
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    24277 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    18857 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_torrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    51442 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/test_zzz_last_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-13 18:01:46.000000 qbittorrent-api-2023.7.52/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (116)     2016 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    35149 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    23199 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    17763 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    23199 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      696 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/qbittorrentapi/
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3655 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2408 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10851 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7416 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2930 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1786 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26761 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1771 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/log.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11711 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13759 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5813 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/rss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6711 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/search.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1801 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30791 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/torrents.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4224 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1525 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/setup.py
```

### Comparing `qbittorrent-api-2023.7.52/src/qbittorrentapi/exceptions.py` & `qbittorrent-api-6.0.0/qbittorrentapi/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,156 @@
-from requests.exceptions import HTTPError as RequestsHTTPError
 from requests.exceptions import RequestException
 
 
 class APIError(Exception):
-    """Base error for all exceptions from this Client."""
-
-
-class UnsupportedQbittorrentVersion(APIError):
-    """Connected qBittorrent is not fully supported by this Client."""
+    """
+    Base error for all exceptions from this Client.
+    """
+    pass
 
 
 class FileError(IOError, APIError):
-    """Base class for all exceptions for file handling."""
+    """
+    Base class for all exceptions for file handling.
+    """
+    pass
 
 
 class TorrentFileError(FileError):
-    """Base class for all exceptions for torrent files."""
+    """
+    Base class for all exceptions for torrent files.
+    """
+    pass
 
 
 class TorrentFileNotFoundError(TorrentFileError):
-    """Specified torrent file does not appear to exist."""
+    """
+    Specified torrent file does not appear to exist.
+    """
+    pass
 
 
 class TorrentFilePermissionError(TorrentFileError):
-    """Permission was denied to read the specified torrent file."""
+    """
+    Permission was denied to read the specified torrent file.
+    """
+    pass
 
 
 class APIConnectionError(RequestException, APIError):
-    """Base class for all communications errors including HTTP errors."""
+    """
+    Base class for all communications errors including HTTP errors.
+    """
+    pass
 
 
 class LoginFailed(APIConnectionError):
-    """This can technically be raised with any request since log in may be attempted for
-    any request and could fail."""
+    """
+    This can technically be raised with any request since log in may be attempted for any request and could fail.
+    """
+    pass
 
 
-class HTTPError(RequestsHTTPError, APIConnectionError):
+class HTTPError(APIConnectionError):
     """
-    Base error for all HTTP errors.
-
-    All errors following a successful connection to qBittorrent are returned as HTTP
-    statuses.
+    Base error for all HTTP errors. All errors following a successful connection to qBittorrent are returned as HTTP statuses.
     """
-
-    http_status_code = None
+    pass
 
 
 class HTTP4XXError(HTTPError):
-    """Base error for all HTTP 4XX statuses."""
+    """
+    Base error for all HTTP 4XX statuses.
+    """
+    pass
 
 
 class HTTP5XXError(HTTPError):
-    """Base error for all HTTP 5XX statuses."""
+    """
+    Base error for all HTTP 5XX statuses.
+    """
+    pass
 
 
 class HTTP400Error(HTTP4XXError):
-    """HTTP 400 Status."""
-
-    http_status_code = 400
+    pass
 
 
 class HTTP401Error(HTTP4XXError):
-    """HTTP 401 Status."""
-
-    http_status_code = 401
+    pass
 
 
 class HTTP403Error(HTTP4XXError):
-    """HTTP 403 Status."""
-
-    http_status_code = 403
+    pass
 
 
 class HTTP404Error(HTTP4XXError):
-    """HTTP 404 Status."""
-
-    http_status_code = 404
-
-
-class HTTP405Error(HTTP4XXError):
-    """HTTP 405 Status."""
-
-    http_status_code = 405
+    pass
 
 
 class HTTP409Error(HTTP4XXError):
-    """HTTP 409 Status."""
-
-    http_status_code = 409
+    pass
 
 
 class HTTP415Error(HTTP4XXError):
-    """HTTP 415 Status."""
-
-    http_status_code = 415
+    pass
 
 
 class HTTP500Error(HTTP5XXError):
-    """HTTP 500 Status."""
-
-    http_status_code = 500
+    pass
 
 
 class MissingRequiredParameters400Error(HTTP400Error):
-    """Endpoint call is missing one or more required parameters."""
+    """
+    Endpoint call is missing one or more required parameters.
+    """
+    pass
 
 
 class InvalidRequest400Error(HTTP400Error):
-    """One or more endpoint arguments are malformed."""
+    """
+    One or more endpoint arguments are malformed.
+    """
+    pass
 
 
 class Unauthorized401Error(HTTP401Error):
-    """Primarily reserved for XSS and host header issues."""
+    """
+    Primarily reserved for XSS and host header issues.
+    """
+    pass
 
 
 class Forbidden403Error(HTTP403Error):
-    """Not logged in, IP has been banned, or calling an API method that isn't public."""
+    """
+    Not logged in, IP has been banned, or calling an API method that isn't public.
+    """
+    pass
 
 
 class NotFound404Error(HTTP404Error):
-    """This should mean qBittorrent couldn't find a torrent for the torrent hash."""
-
-
-class MethodNotAllowed405Error(HTTP405Error):
-    """HTTP method is not supported for the API endpoint."""
+    """
+    This should mean qBittorrent couldn't find a torrent for the torrent hash.
+    It is also possible this means the endpoint doesn't exist in qBittorrent...but that also means this Client has a bug.
+    """
+    pass
 
 
 class Conflict409Error(HTTP409Error):
-    """Returned if arguments don't make sense specific to the endpoint."""
+    """
+    Returned if arguments don't make sense specific to the endpoint.
+    """
+    pass
 
 
 class UnsupportedMediaType415Error(HTTP415Error):
-    """``torrents/add`` endpoint will return this for invalid URL(s) or files."""
+    """
+    torrents/add endpoint will return this for invalid URL(s) or files.
+    """
+    pass
 
 
 class InternalServerError500Error(HTTP500Error):
-    """Returned if qBittorrent errors internally while processing the request."""
+    """
+    Returned if qBittorent craps on itself while processing the request...
+    """
+    pass
```

