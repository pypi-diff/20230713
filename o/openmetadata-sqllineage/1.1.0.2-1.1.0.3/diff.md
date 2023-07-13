# Comparing `tmp/openmetadata-sqllineage-1.1.0.2.tar.gz` & `tmp/openmetadata-sqllineage-1.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata-sqllineage-1.1.0.2.tar", last modified: Wed Jul  5 07:51:15 2023, max compression
+gzip compressed data, was "openmetadata-sqllineage-1.1.0.3.tar", last modified: Thu Jul 13 09:02:39 2023, max compression
```

## Comparing `openmetadata-sqllineage-1.1.0.2.tar` & `openmetadata-sqllineage-1.1.0.3.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.429828 openmetadata-sqllineage-1.1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.393828 openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-05 07:51:15.000000 openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:51:15.429828 openmetadata-sqllineage-1.1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.393828 openmetadata-sqllineage-1.1.0.2/sqllineage/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.397827 openmetadata-sqllineage-1.1.0.2/sqllineage/build/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   146541 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/editor.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/editor.worker.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   622794 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/editor.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-05 07:49:51.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-05 07:49:51.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-05 07:49:51.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-05 07:49:51.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 07:49:51.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.393828 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.397827 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    69444 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/css/main.c1b86fee.css
--rw-r--r--   0 runner    (1001) docker     (123)   146886 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/css/main.c1b86fee.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.401828 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/333.97bcedbd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    45386 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/333.97bcedbd.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)  3567481 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/main.a8b33e0c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/main.a8b33e0c.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123) 12937453 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/main.a8b33e0c.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.413828 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    62792 2023-07-05 07:51:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.413828 openmetadata-sqllineage-1.1.0.2/sqllineage/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.413828 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.413828 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.413828 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.413828 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/swap_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/holder_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16503 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.413828 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.413828 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/cte.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/swap_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/holder_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.393828 openmetadata-sqllineage-1.1.0.2/sqllineage/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query02.sql
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query03.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query04.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query05.sql
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query06.sql
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query07.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query08.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query09.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query11.sql
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query12.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query13.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query14.sql
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query15.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query16.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query17.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query18.sql
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query19.sql
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query20.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query21.sql
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query22.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query23.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query24.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query25.sql
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query26.sql
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query27.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query28.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query29.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query30.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query31.sql
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query32.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query33.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query34.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query35.sql
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query36.sql
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query37.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query38.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query39.sql
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query40.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query41.sql
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query42.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query43.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query44.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query45.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query46.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query47.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query48.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query49.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query50.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query51.sql
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query52.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query53.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query54.sql
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query55.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query56.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query57.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query58.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query59.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query60.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query61.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query62.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query63.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query64.sql
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query65.sql
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query66.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query67.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query68.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query69.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query70.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query71.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query72.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query73.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query74.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query75.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query76.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query77.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query78.sql
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query79.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query80.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query81.sql
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query82.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query83.sql
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query84.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query85.sql
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query86.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query87.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query88.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query89.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query90.sql
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query91.sql
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query92.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query93.sql
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query94.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query95.sql
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query96.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query97.sql
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query98.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query99.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineage/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/utils/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineage/utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/config-overrides.js
--rw-r--r--   0 runner    (1001) docker     (123)  1248521 2023-07-05 07:49:49.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/App.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/api/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/app/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/app/store.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.393828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/directory/Directory.js
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/directory/DirectoryTreeItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/directory/directorySlice.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/DAG.js
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/DAGDesc.js
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/Editor.js
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/editorSlice.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:51:15.425828 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/widget/LoadError.js
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/widget/Loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-05 07:49:13.000000 openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.094144 openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-13 09:02:39.000000 openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.094144 openmetadata-sqllineage-1.1.0.3/sqllineage/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.098144 openmetadata-sqllineage-1.1.0.3/sqllineage/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   146541 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/editor.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/editor.worker.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   622794 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/editor.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-13 09:01:15.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-13 09:01:15.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-13 09:01:15.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-13 09:01:15.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 09:01:15.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.094144 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.098144 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    69444 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/css/main.c1b86fee.css
+-rw-r--r--   0 runner    (1001) docker     (123)   146886 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/css/main.c1b86fee.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.102144 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/333.97bcedbd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45386 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/333.97bcedbd.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)  3567481 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/main.a8b33e0c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/main.a8b33e0c.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123) 12937453 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/main.a8b33e0c.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.114144 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    62792 2023-07-13 09:02:37.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.114144 openmetadata-sqllineage-1.1.0.3/sqllineage/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.114144 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.114144 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.118144 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.118144 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/swap_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/holder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16422 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.118144 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.118144 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/cte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/swap_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/holder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.094144 openmetadata-sqllineage-1.1.0.3/sqllineage/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.126144 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query02.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query03.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query04.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query05.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query06.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query07.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query08.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query09.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query12.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query13.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query14.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query15.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query16.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query17.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query18.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query19.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query20.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query21.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query22.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query23.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query24.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query25.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query26.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query27.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query28.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query29.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query30.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query31.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query32.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query33.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query34.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query35.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query36.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query37.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query38.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query39.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query40.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query41.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query42.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query43.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query44.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query45.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query46.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query47.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query48.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query49.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query50.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query51.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query52.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query53.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query54.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query55.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query56.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query57.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query58.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query59.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query60.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query61.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query62.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query63.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query64.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query65.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query66.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query67.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query68.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query69.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query70.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query71.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query72.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query73.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query74.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query75.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query76.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query77.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query78.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query79.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query80.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query81.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query82.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query83.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query84.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query85.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query86.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query87.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query88.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query89.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query90.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query91.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query92.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query93.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query94.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query95.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query96.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query97.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query98.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query99.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.126144 openmetadata-sqllineage-1.1.0.3/sqllineage/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/utils/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineage/utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/config-overrides.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1248521 2023-07-13 09:01:13.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/App.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/api/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/app/store.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.094144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/directory/Directory.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/directory/DirectoryTreeItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/directory/directorySlice.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/
+-rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/DAG.js
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/DAGDesc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/Editor.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/editorSlice.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:02:39.130144 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/widget/LoadError.js
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/widget/Loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 09:00:41.000000 openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/index.js
```

### Comparing `openmetadata-sqllineage-1.1.0.2/LICENSE` & `openmetadata-sqllineage-1.1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/PKG-INFO` & `openmetadata-sqllineage-1.1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata-sqllineage
-Version: 1.1.0.2
+Version: 1.1.0.3
 Summary: OpenMetadata SQL Lineage for Analysis Tool powered by Python and sqlfluff based on sqllineage.
 Home-page: https://github.com/open-metadata/openmetadata-sqllineage
 Author: OpenMetadata Committers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openmetadata-sqllineage-1.1.0.2/README.md` & `openmetadata-sqllineage-1.1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/PKG-INFO` & `openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata-sqllineage
-Version: 1.1.0.2
+Version: 1.1.0.3
 Summary: OpenMetadata SQL Lineage for Analysis Tool powered by Python and sqlfluff based on sqllineage.
 Home-page: https://github.com/open-metadata/openmetadata-sqllineage
 Author: OpenMetadata Committers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openmetadata-sqllineage-1.1.0.2/openmetadata_sqllineage.egg-info/SOURCES.txt` & `openmetadata-sqllineage-1.1.0.3/openmetadata_sqllineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/setup.py` & `openmetadata-sqllineage-1.1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/__init__.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 
 NAME = "openmetadata-sqllineage"
-VERSION = "1.1.0.2"
+VERSION = "1.1.0.3"
 DEFAULT_LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {"default": {"format": "%(levelname)s: %(message)s"}},
     "handlers": {
         "console": {
             "level": "WARNING",
```

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/asset-manifest.json` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/editor.worker.js` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/editor.worker.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/editor.worker.js.map` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/editor.worker.js.map`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/favicon.ico` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/index.html` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/index.html`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/logo192.png` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/logo192.png`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/logo512.png` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/logo512.png`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/css/main.c1b86fee.css` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/css/main.c1b86fee.css`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/css/main.c1b86fee.css.map` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/css/main.c1b86fee.css.map`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/333.97bcedbd.chunk.js` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/333.97bcedbd.chunk.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/333.97bcedbd.chunk.js.map` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/333.97bcedbd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/main.a8b33e0c.js` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/main.a8b33e0c.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/main.a8b33e0c.js.LICENSE.txt` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/main.a8b33e0c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/js/main.a8b33e0c.js.map` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/js/main.a8b33e0c.js.map`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf` & `openmetadata-sqllineage-1.1.0.3/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/cli.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/cli.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/holders.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/holders.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/models.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/models.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/__init__.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/analyzer.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/analyzer.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/base.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/base.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/source.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/source.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/swap_partition.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/swap_partition.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/handlers/target.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/handlers/target.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/holder_utils.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/holder_utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/models.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/models.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlfluff/utils.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlfluff/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,36 +266,34 @@
 ) -> List[BaseSegment]:
     """
     Filter segments for a given segment's segments if they are not negligible
     :param segment: segment to be processed
     :param check_bracketed: process segment if it is of type "bracketed"
     :return: a list of segments
     """
-    if segment.type == "bracketed" and is_union(segment):
-        result = []
+    if segment.type == "bracketed":
         for sgmt in segment.segments:
             if sgmt.type == "set_expression":
-                result = [sgmt]
-        return result
-    elif segment.type == "bracketed" and check_bracketed:
+                return [sgmt]
+
+    if segment.type == "bracketed" and check_bracketed:
         segments = [
             sg
             for sg in segment.iter_segments(expanding=["expression"], pass_through=True)
         ]
         result = []
         for sgmnt in segments:
             if sgmnt.type == "column_reference":
                 result.append(sgmnt)
             else:
                 for sg in sgmnt.segments:
                     if not is_segment_negligible(sg):
                         result.append(sg)
         return result
-    else:
-        return [sgmnt for sgmnt in segment.segments if not is_segment_negligible(sgmnt)]
+    return [sgmnt for sgmnt in segment.segments if not is_segment_negligible(sgmnt)]
 
 
 def get_identifier(col_segment: BaseSegment) -> str:
     """
     :param col_segment: column segment
     :return: the table identifier name
     """
```

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/__init__.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/__init__.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/analyzer.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/analyzer.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/base.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/base.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/cte.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/cte.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/source.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/source.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/swap_partition.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/swap_partition.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/handlers/target.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/handlers/target.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/holder_utils.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/holder_utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/models.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/models.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/core/parser/sqlparse/utils.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/core/parser/sqlparse/utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query01.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query01.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query02.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query02.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query04.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query04.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query05.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query05.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query06.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query06.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query07.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query07.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query08.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query08.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query09.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query09.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query10.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query10.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query11.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query11.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query12.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query12.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query13.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query13.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query14.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query14.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query15.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query15.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query16.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query16.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query17.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query17.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query18.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query18.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query19.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query19.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query20.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query20.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query21.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query21.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query23.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query23.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query24.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query24.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query25.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query25.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query26.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query26.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query27.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query27.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query28.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query28.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query29.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query29.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query30.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query30.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query31.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query31.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query32.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query32.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query33.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query33.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query34.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query34.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query35.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query35.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query36.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query36.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query37.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query37.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query38.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query38.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query39.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query39.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query40.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query40.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query41.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query41.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query42.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query42.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query43.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query43.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query44.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query44.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query45.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query45.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query46.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query46.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query47.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query47.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query48.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query48.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query49.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query49.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query50.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query50.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query51.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query51.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query53.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query53.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query54.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query54.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query56.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query56.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query57.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query57.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query58.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query58.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query59.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query59.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query60.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query60.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query61.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query61.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query62.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query62.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query63.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query63.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query64.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query64.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query65.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query65.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query66.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query66.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query67.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query67.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query68.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query68.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query69.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query69.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query70.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query70.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query71.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query71.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query72.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query72.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query73.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query73.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query74.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query74.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query75.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query75.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query76.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query76.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query77.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query77.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query78.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query78.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query79.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query79.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query80.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query80.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query81.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query81.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query82.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query82.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query83.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query83.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query84.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query84.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query85.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query85.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query86.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query86.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query87.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query87.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query88.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query88.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query89.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query89.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query90.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query90.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query91.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query91.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query92.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query92.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query93.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query93.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query94.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query94.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query95.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query95.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query97.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query97.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query98.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query98.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/data/tpcds/query99.sql` & `openmetadata-sqllineage-1.1.0.3/sqllineage/data/tpcds/query99.sql`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/drawing.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/drawing.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/io.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/io.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/runner.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/runner.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineage/utils/helpers.py` & `openmetadata-sqllineage-1.1.0.3/sqllineage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/package-lock.json` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/package-lock.json`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/package.json` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/package.json`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/favicon.ico` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/index.html` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/index.html`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/logo192.png` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/logo192.png`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/public/logo512.png` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/public/logo512.png`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/App.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/App.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/api/client.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/api/client.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/directory/Directory.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/directory/Directory.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/directory/DirectoryTreeItem.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/directory/DirectoryTreeItem.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/directory/directorySlice.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/directory/directorySlice.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/DAG.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/DAG.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/DAGDesc.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/DAGDesc.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/Editor.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/Editor.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/editor/editorSlice.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/editor/editorSlice.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/widget/LoadError.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/widget/LoadError.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/features/widget/Loading.js` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/features/widget/Loading.js`

 * *Files identical despite different names*

### Comparing `openmetadata-sqllineage-1.1.0.2/sqllineagejs/src/index.css` & `openmetadata-sqllineage-1.1.0.3/sqllineagejs/src/index.css`

 * *Files identical despite different names*

