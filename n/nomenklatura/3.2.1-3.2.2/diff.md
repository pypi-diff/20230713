# Comparing `tmp/nomenklatura-3.2.1.tar.gz` & `tmp/nomenklatura-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.2.1.tar", last modified: Tue Jul 11 11:19:55 2023, max compression
+gzip compressed data, was "nomenklatura-3.2.2.tar", last modified: Thu Jul 13 09:56:37 2023, max compression
```

## Comparing `nomenklatura-3.2.1.tar` & `nomenklatura-3.2.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:19:55.553180 nomenklatura-3.2.1/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-11 11:19:55.000000 nomenklatura-3.2.1/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-11 11:19:55.000000 nomenklatura-3.2.1/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:19:55.000000 nomenklatura-3.2.1/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-11 11:19:55.000000 nomenklatura-3.2.1/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:19:55.000000 nomenklatura-3.2.1/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:19:30.000000 nomenklatura-3.2.1/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-11 11:19:55.000000 nomenklatura-3.2.1/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 11:19:55.000000 nomenklatura-3.2.1/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 11:19:55.557180 nomenklatura-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-11 11:17:51.000000 nomenklatura-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.738103 nomenklatura-3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-13 09:56:37.738103 nomenklatura-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.730101 nomenklatura-3.2.2/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.730101 nomenklatura-3.2.2/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.730101 nomenklatura-3.2.2/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.738103 nomenklatura-3.2.2/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.730101 nomenklatura-3.2.2/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:55:49.000000 nomenklatura-3.2.2/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:56:37.738103 nomenklatura-3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/setup.py
```

### Comparing `nomenklatura-3.2.1/LICENSE` & `nomenklatura-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/PKG-INFO` & `nomenklatura-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.2.1
+Version: 3.2.2
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.2.1/README.md` & `nomenklatura-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/cache.py` & `nomenklatura-3.2.2/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/cli.py` & `nomenklatura-3.2.2/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.2.2/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.2.2/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/dataset/catalog.py` & `nomenklatura-3.2.2/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/dataset/coverage.py` & `nomenklatura-3.2.2/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/dataset/dataset.py` & `nomenklatura-3.2.2/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/dataset/publisher.py` & `nomenklatura-3.2.2/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/dataset/resource.py` & `nomenklatura-3.2.2/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/dataset/util.py` & `nomenklatura-3.2.2/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/db.py` & `nomenklatura-3.2.2/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/__init__.py` & `nomenklatura-3.2.2/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/aleph.py` & `nomenklatura-3.2.2/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/common.py` & `nomenklatura-3.2.2/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.2.2/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.2.2/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/enrich/yente.py` & `nomenklatura-3.2.2/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/entity.py` & `nomenklatura-3.2.2/nomenklatura/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from followthemoney.proxy import P
 from followthemoney.types import registry
 from followthemoney.proxy import EntityProxy
 
 from nomenklatura.dataset import DS, Dataset, DefaultDataset
 from nomenklatura.publish.names import pick_name
 from nomenklatura.statement.statement import Statement
-from nomenklatura.util import BASE_ID
+from nomenklatura.util import BASE_ID, string_list
 
 if TYPE_CHECKING:
     from nomenklatura.store import View
 
 CE = TypeVar("CE", bound="CompositeEntity")
 
 
@@ -168,111 +168,14 @@
                 self.schema = model.common_schema(self.schema, stmt.schema)
             except InvalidData as exc:
                 raise InvalidData(f"{self.id}: {exc}") from exc
         if stmt.prop != BASE_ID:
             self._statements.setdefault(stmt.prop, set())
             self._statements[stmt.prop].add(stmt)
 
-    def clean_value(
-        self,
-        prop: Property,
-        value: Optional[str],
-        cleaned: bool = False,
-        fuzzy: bool = False,
-        format: Optional[str] = None,
-    ) -> List[str]:
-        if value is None:
-            return []
-        if cleaned:
-            return [value]
-        value = prop.type.clean_text(value, fuzzy=fuzzy, format=format, proxy=self)
-        if value is None:
-            return []
-        return [value]
-
-    def claim(
-        self,
-        prop: P,
-        value: Optional[str],
-        schema: Optional[str] = None,
-        dataset: Optional[str] = None,
-        seen: Optional[str] = None,
-        lang: Optional[str] = None,
-        original_value: Optional[str] = None,
-        cleaned: bool = False,
-        quiet: bool = False,
-        fuzzy: bool = False,
-        format: Optional[str] = None,
-    ) -> None:
-        prop_name = self._prop_name(prop, quiet=quiet)
-        if prop_name is None:
-            return None
-        prop = self.schema.properties[prop_name]
-
-        # Don't allow setting the reverse properties:
-        if prop.stub:
-            if quiet:
-                return None
-            msg = gettext("Stub property (%s): %s")
-            raise InvalidData(msg % (self.schema, prop))
-
-        if lang is not None:
-            lang = registry.language.clean_text(lang)
-
-        for clean in self.clean_value(
-            prop,
-            value,
-            cleaned=cleaned,
-            fuzzy=fuzzy,
-            format=format,
-        ):
-            if original_value is None and clean != value:
-                original_value = value
-
-            stmt = Statement(
-                entity_id=self.id,
-                prop=prop.name,
-                schema=schema or self.schema.name,
-                value=clean,
-                dataset=dataset or self.default_dataset.name,
-                lang=lang,
-                original_value=original_value,
-                first_seen=seen,
-            )
-            self.add_statement(stmt)
-
-    def claim_many(
-        self,
-        prop: P,
-        values: Iterable[Optional[str]],
-        schema: Optional[str] = None,
-        dataset: Optional[str] = None,
-        seen: Optional[str] = None,
-        lang: Optional[str] = None,
-        original_value: Optional[str] = None,
-        cleaned: bool = False,
-        quiet: bool = False,
-        fuzzy: bool = False,
-        format: Optional[str] = None,
-    ) -> None:
-        for value in values:
-            self.claim(
-                prop,
-                value,
-                schema=schema,
-                dataset=dataset,
-                seen=seen,
-                lang=lang,
-                original_value=original_value,
-                cleaned=cleaned,
-                quiet=quiet,
-                fuzzy=fuzzy,
-                format=format,
-            )
-
     def get(self, prop: P, quiet: bool = False) -> List[str]:
         prop_name = self._prop_name(prop, quiet=quiet)
         if prop_name is None or prop_name not in self._statements:
             return []
         return list({s.value for s in self._statements[prop_name]})
 
     def get_statements(self, prop: P, quiet: bool = False) -> List[Statement]:
@@ -285,21 +188,30 @@
         self,
         prop: P,
         values: Any,
         cleaned: bool = False,
         quiet: bool = False,
         fuzzy: bool = False,
         format: Optional[str] = None,
+        lang: Optional[str] = None,
+        original_value: Optional[str] = None,
     ) -> None:
         prop_name = self._prop_name(prop, quiet=quiet)
         if prop_name is None:
             return
         self._statements.pop(prop_name, None)
         return self.add(
-            prop, values, cleaned=cleaned, quiet=quiet, fuzzy=fuzzy, format=format
+            prop,
+            values,
+            cleaned=cleaned,
+            quiet=quiet,
+            fuzzy=fuzzy,
+            format=format,
+            lang=lang,
+            original_value=original_value,
         )
 
     def add(
         self,
         prop: P,
         values: Any,
         cleaned: bool = False,
@@ -309,46 +221,76 @@
         lang: Optional[str] = None,
         original_value: Optional[str] = None,
     ) -> None:
         prop_name = self._prop_name(prop, quiet=quiet)
         if prop_name is None:
             return None
         prop = self.schema.properties[prop_name]
-        for value in value_list(values):
-            if not cleaned:
-                value = prop.type.clean(value, proxy=self, fuzzy=fuzzy, format=format)
-            self.claim(
+        for value in string_list(values):
+            self.unsafe_add(
                 prop,
                 value,
+                cleaned=cleaned,
+                fuzzy=fuzzy,
+                format=format,
                 quiet=quiet,
                 lang=lang,
                 original_value=original_value,
-                cleaned=True,
             )
         return None
 
     def unsafe_add(
         self,
         prop: Property,
         value: Optional[str],
         cleaned: bool = False,
         fuzzy: bool = False,
         format: Optional[str] = None,
+        quiet: bool = False,
+        schema: Optional[str] = None,
+        dataset: Optional[str] = None,
+        seen: Optional[str] = None,
         lang: Optional[str] = None,
         original_value: Optional[str] = None,
     ) -> None:
-        self.claim(
-            prop,
-            value,
-            cleaned=cleaned,
-            fuzzy=fuzzy,
-            format=format,
+        """Add a statement to the entity, possibly the value."""
+        if value is None:
+            return
+
+        # Don't allow setting the reverse properties:
+        if prop.stub:
+            if quiet:
+                return None
+            msg = gettext("Stub property (%s): %s")
+            raise InvalidData(msg % (self.schema, prop))
+
+        if lang is not None:
+            lang = registry.language.clean_text(lang)
+
+        clean: Optional[str] = value
+        if not cleaned:
+            clean = prop.type.clean_text(value, proxy=self, fuzzy=fuzzy, format=format)
+
+        if clean is None:
+            return
+
+        if original_value is None and clean != value:
+            original_value = value
+
+        stmt = Statement(
+            entity_id=self.id,
+            prop=prop.name,
+            schema=schema or self.schema.name,
+            value=clean,
+            dataset=dataset or self.default_dataset.name,
             lang=lang,
             original_value=original_value,
+            first_seen=seen,
         )
+        self.add_statement(stmt)
 
     def pop(self, prop: P, quiet: bool = True) -> List[str]:
         prop_name = self._prop_name(prop, quiet=quiet)
         if prop_name is None or prop_name not in self._statements:
             return []
         return list({s.value for s in self._statements.pop(prop_name, [])})
```

### Comparing `nomenklatura-3.2.1/nomenklatura/index/entry.py` & `nomenklatura-3.2.2/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/index/index.py` & `nomenklatura-3.2.2/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/index/tokenizer.py` & `nomenklatura-3.2.2/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/judgement.py` & `nomenklatura-3.2.2/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/__init__.py` & `nomenklatura-3.2.2/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.2.2/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.2.2/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/pairs.py` & `nomenklatura-3.2.2/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/types.py` & `nomenklatura-3.2.2/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/util.py` & `nomenklatura-3.2.2/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.2.2/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.2.2/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v1/model.py` & `nomenklatura-3.2.2/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v1/names.py` & `nomenklatura-3.2.2/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v1/train.py` & `nomenklatura-3.2.2/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v1/util.py` & `nomenklatura-3.2.2/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.2.2/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.2.2/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v2/model.py` & `nomenklatura-3.2.2/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v2/names.py` & `nomenklatura-3.2.2/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v2/train.py` & `nomenklatura-3.2.2/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/matching/v2/util.py` & `nomenklatura-3.2.2/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/publish/dates.py` & `nomenklatura-3.2.2/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/publish/edges.py` & `nomenklatura-3.2.2/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/publish/names.py` & `nomenklatura-3.2.2/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/resolver/edge.py` & `nomenklatura-3.2.2/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/resolver/identifier.py` & `nomenklatura-3.2.2/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/resolver/resolver.py` & `nomenklatura-3.2.2/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/senzing.py` & `nomenklatura-3.2.2/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/statement/serialize.py` & `nomenklatura-3.2.2/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/statement/statement.py` & `nomenklatura-3.2.2/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/store/__init__.py` & `nomenklatura-3.2.2/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/store/base.py` & `nomenklatura-3.2.2/nomenklatura/store/base.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/store/level.py` & `nomenklatura-3.2.2/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/store/memory.py` & `nomenklatura-3.2.2/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/store/util.py` & `nomenklatura-3.2.2/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/tui/app.py` & `nomenklatura-3.2.2/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/tui/comparison.py` & `nomenklatura-3.2.2/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/tui/util.py` & `nomenklatura-3.2.2/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura/util.py` & `nomenklatura-3.2.2/nomenklatura/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import os
 import Levenshtein
 from pathlib import Path
 from datetime import datetime
 from functools import lru_cache, cache
 from normality.constants import WS
 from followthemoney import model
+from collections.abc import Mapping, Sequence
 from fingerprints.fingerprint import fingerprint
 from fingerprints.cleanup import clean_strict
+from followthemoney.util import sanitize_text
 from typing import cast, Any, Mapping, Union, Iterable, Tuple, Optional, List, Set
 from urllib.parse import urlparse, urlunparse, parse_qsl, urlencode
 
 DATA_PATH = Path(os.path.join(os.path.dirname(__file__), "data")).resolve()
 QID = re.compile(r"^Q(\d+)$")
 BASE_ID = "id"
 PathLike = Union[str, os.PathLike[str]]
@@ -21,14 +23,46 @@
 def is_qid(text: Optional[str]) -> bool:
     """Determine if the given string is a valid wikidata QID."""
     if text is None:
         return False
     return QID.match(text) is not None
 
 
+def string_list(value: Any) -> List[str]:
+    """Convert a value to a list of strings."""
+    if value is None:
+        return []
+    if isinstance(value, (str, bytes)):
+        text = sanitize_text(value)
+        if text is None:
+            return []
+        return [text]
+    if not isinstance(value, Sequence):
+        value = [value]
+    texts: List[str] = []
+    for inner in value:
+        if isinstance(inner, Mapping):
+            text = inner.get("id")
+            if text is not None:
+                texts.append(text)
+            continue
+
+        try:
+            texts.append(inner.id)
+            continue
+        except AttributeError:
+            pass
+
+        text = sanitize_text(inner)
+        if text is not None:
+            texts.append(text)
+
+    return texts
+
+
 def normalize_url(url: str, params: ParamsType = None) -> str:
     """Compose a URL with the given query parameters."""
     parsed = urlparse(url)
     query = parse_qsl(parsed.query, keep_blank_values=True)
     if params is not None:
         values = params.items() if isinstance(params, Mapping) else params
         query.extend(sorted(values))
```

### Comparing `nomenklatura-3.2.1/nomenklatura/xref.py` & `nomenklatura-3.2.2/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.2.2/nomenklatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.2.1
+Version: 3.2.2
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.2.1/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.2.2/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.1/setup.py` & `nomenklatura-3.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.2.1",
+    version="3.2.2",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

