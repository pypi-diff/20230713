# Comparing `tmp/fugue-0.8.5.dev1.tar.gz` & `tmp/fugue-0.8.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-0.8.5.dev1.tar", last modified: Wed Jun  7 07:41:03 2023, max compression
+gzip compressed data, was "fugue-0.8.6.dev1.tar", last modified: Thu Jul 13 06:02:02 2023, max compression
```

## Comparing `fugue-0.8.5.dev1.tar` & `fugue-0.8.6.dev1.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/bag/array_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/bag/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/collections/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/collections/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/collections/yielded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/column/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/column/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/column/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/native_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/_builtins/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_builtins/creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_builtins/outputters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_builtins/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/creator/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/creator/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/outputter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/outputter/outputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/processor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/processor/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/transformer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/transformer/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/rpc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/rpc/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_contrib/seaborn/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/seaborn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_contrib/viz/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/viz/_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_ibis/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/execution/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/execution/pandas_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/nbextension/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/nbextension/description.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/nbextension/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_polars/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_polars/polars_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_polars/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_ray/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_spark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/bag_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    76338 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/builtin_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/dataframe_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/execution_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/ibis_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:01.997720 fugue-0.8.6.dev1/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.001720 fugue-0.8.6.dev1/fugue/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.001720 fugue-0.8.6.dev1/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/bag/array_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/bag/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.005720 fugue-0.8.6.dev1/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/collections/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/collections/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/collections/yielded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.005720 fugue-0.8.6.dev1/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/column/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/column/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/column/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.009720 fugue-0.8.6.dev1/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.009720 fugue-0.8.6.dev1/fugue/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.009720 fugue-0.8.6.dev1/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/native_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.009720 fugue-0.8.6.dev1/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/_builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_builtins/creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_builtins/outputters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_builtins/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/creator/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/creator/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/outputter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/outputter/outputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/processor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/processor/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/transformer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/rpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/rpc/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.001720 fugue-0.8.6.dev1/fugue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue_contrib/seaborn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/seaborn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue_contrib/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/viz/_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_ibis/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/execution/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/execution/pandas_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/nbextension/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/nbextension/description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/nbextension/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_polars/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_polars/polars_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_polars/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_ray/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/fugue_spark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/fugue_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/fugue_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/bag_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76338 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/builtin_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/dataframe_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/execution_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/ibis_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/fugue_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/setup.py
```

### Comparing `fugue-0.8.5.dev1/LICENSE` & `fugue-0.8.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/PKG-INFO` & `fugue-0.8.6.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.5.dev1
+Version: 0.8.6.dev1
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
         
@@ -148,17 +148,24 @@
         
         Fugue can be installed through pip or conda. For example:
         
         ```bash
         pip install fugue
         ```
         
+        In order to use Fugue SQL, it is strongly recommended to install the `sql` extra:
+        
+        ```bash
+        pip install fugue[sql]
+        ```
+        
         It also has the following installation extras:
         
-        *   **spark**: to support Spark as the [ExecutionEngine](https://fugue-tutorials.readthedocs.io/tutorials/advanced/execution_engine.html)
+        *   **sql**: to support Fugue SQL. Without this extra, the non-SQL part still works. Before Fugue 0.9.0, this extra is included in Fugue's core dependency so you don't need to install explicitly. **But for 0,9.0+, this becomes required if you want to use Fugue SQL.**
+        *   **spark**: to support Spark as the [ExecutionEngine](https://fugue-tutorials.readthedocs.io/tutorials/advanced/execution_engine.html).
         *   **dask**: to support Dask as the ExecutionEngine.
         *   **ray**: to support Ray as the ExecutionEngine.
         *   **duckdb**: to support DuckDB as the ExecutionEngine, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/duckdb.html).
         *   **polars**: to support Polars DataFrames and extensions using Polars.
         *   **ibis**: to enable Ibis for Fugue workflows, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/ibis.html).
         *   **cpp_sql_parser**: to enable the CPP antlr parser for Fugue SQL. It can be 50+ times faster than the pure Python parser. For the main Python versions and platforms, there is already pre-built binaries, but for the remaining, it needs a C++ compiler to build on the fly.
```

### Comparing `fugue-0.8.5.dev1/README.md` & `fugue-0.8.6.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,24 @@
 
 Fugue can be installed through pip or conda. For example:
 
 ```bash
 pip install fugue
 ```
 
+In order to use Fugue SQL, it is strongly recommended to install the `sql` extra:
+
+```bash
+pip install fugue[sql]
+```
+
 It also has the following installation extras:
 
-*   **spark**: to support Spark as the [ExecutionEngine](https://fugue-tutorials.readthedocs.io/tutorials/advanced/execution_engine.html)
+*   **sql**: to support Fugue SQL. Without this extra, the non-SQL part still works. Before Fugue 0.9.0, this extra is included in Fugue's core dependency so you don't need to install explicitly. **But for 0,9.0+, this becomes required if you want to use Fugue SQL.**
+*   **spark**: to support Spark as the [ExecutionEngine](https://fugue-tutorials.readthedocs.io/tutorials/advanced/execution_engine.html).
 *   **dask**: to support Dask as the ExecutionEngine.
 *   **ray**: to support Ray as the ExecutionEngine.
 *   **duckdb**: to support DuckDB as the ExecutionEngine, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/duckdb.html).
 *   **polars**: to support Polars DataFrames and extensions using Polars.
 *   **ibis**: to enable Ibis for Fugue workflows, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/ibis.html).
 *   **cpp_sql_parser**: to enable the CPP antlr parser for Fugue SQL. It can be 50+ times faster than the pure Python parser. For the main Python versions and platforms, there is already pre-built binaries, but for the remaining, it needs a C++ compiler to build on the fly.
```

### Comparing `fugue-0.8.5.dev1/fugue/__init__.py` & `fugue-0.8.6.dev1/fugue/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/_utils/display.py` & `fugue-0.8.6.dev1/fugue/_utils/display.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/_utils/exception.py` & `fugue-0.8.6.dev1/fugue/_utils/exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/_utils/interfaceless.py` & `fugue-0.8.6.dev1/fugue/_utils/interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/_utils/io.py` & `fugue-0.8.6.dev1/fugue/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/_utils/misc.py` & `fugue-0.8.6.dev1/fugue/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/api.py` & `fugue-0.8.6.dev1/fugue/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/bag/array_bag.py` & `fugue-0.8.6.dev1/fugue/bag/array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/bag/bag.py` & `fugue-0.8.6.dev1/fugue/bag/bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/collections/partition.py` & `fugue-0.8.6.dev1/fugue/collections/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/collections/sql.py` & `fugue-0.8.6.dev1/fugue/collections/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/collections/yielded.py` & `fugue-0.8.6.dev1/fugue/collections/yielded.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/column/expressions.py` & `fugue-0.8.6.dev1/fugue/column/expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/column/functions.py` & `fugue-0.8.6.dev1/fugue/column/functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/column/sql.py` & `fugue-0.8.6.dev1/fugue/column/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/constants.py` & `fugue-0.8.6.dev1/fugue/constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/__init__.py` & `fugue-0.8.6.dev1/fugue/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/api.py` & `fugue-0.8.6.dev1/fugue/dataframe/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/array_dataframe.py` & `fugue-0.8.6.dev1/fugue/dataframe/array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/arrow_dataframe.py` & `fugue-0.8.6.dev1/fugue/dataframe/arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/dataframe.py` & `fugue-0.8.6.dev1/fugue/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/dataframe_iterable_dataframe.py` & `fugue-0.8.6.dev1/fugue/dataframe/dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/dataframes.py` & `fugue-0.8.6.dev1/fugue/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/function_wrapper.py` & `fugue-0.8.6.dev1/fugue/dataframe/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/iterable_dataframe.py` & `fugue-0.8.6.dev1/fugue/dataframe/iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/pandas_dataframe.py` & `fugue-0.8.6.dev1/fugue/dataframe/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataframe/utils.py` & `fugue-0.8.6.dev1/fugue/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataset/api.py` & `fugue-0.8.6.dev1/fugue/dataset/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dataset/dataset.py` & `fugue-0.8.6.dev1/fugue/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/dev.py` & `fugue-0.8.6.dev1/fugue/dev.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/exceptions.py` & `fugue-0.8.6.dev1/fugue/exceptions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/execution/api.py` & `fugue-0.8.6.dev1/fugue/execution/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/execution/execution_engine.py` & `fugue-0.8.6.dev1/fugue/execution/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/execution/factory.py` & `fugue-0.8.6.dev1/fugue/execution/factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/execution/native_execution_engine.py` & `fugue-0.8.6.dev1/fugue/execution/native_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/__init__.py` & `fugue-0.8.6.dev1/fugue/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/_builtins/__init__.py` & `fugue-0.8.6.dev1/fugue/extensions/_builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/_builtins/creators.py` & `fugue-0.8.6.dev1/fugue/extensions/_builtins/creators.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/_builtins/outputters.py` & `fugue-0.8.6.dev1/fugue/extensions/_builtins/outputters.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/_builtins/processors.py` & `fugue-0.8.6.dev1/fugue/extensions/_builtins/processors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/_utils.py` & `fugue-0.8.6.dev1/fugue/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/context.py` & `fugue-0.8.6.dev1/fugue/extensions/context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/creator/convert.py` & `fugue-0.8.6.dev1/fugue/extensions/creator/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/creator/creator.py` & `fugue-0.8.6.dev1/fugue/extensions/creator/creator.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/outputter/convert.py` & `fugue-0.8.6.dev1/fugue/extensions/outputter/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/outputter/outputter.py` & `fugue-0.8.6.dev1/fugue/extensions/outputter/outputter.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/processor/convert.py` & `fugue-0.8.6.dev1/fugue/extensions/processor/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/processor/processor.py` & `fugue-0.8.6.dev1/fugue/extensions/processor/processor.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/transformer/convert.py` & `fugue-0.8.6.dev1/fugue/extensions/transformer/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/extensions/transformer/transformer.py` & `fugue-0.8.6.dev1/fugue/extensions/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/plugins.py` & `fugue-0.8.6.dev1/fugue/plugins.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/registry.py` & `fugue-0.8.6.dev1/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/rpc/base.py` & `fugue-0.8.6.dev1/fugue/rpc/base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/rpc/flask.py` & `fugue-0.8.6.dev1/fugue/rpc/flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/sql/_utils.py` & `fugue-0.8.6.dev1/fugue/sql/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/sql/_visitors.py` & `fugue-0.8.6.dev1/fugue/sql/_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/sql/api.py` & `fugue-0.8.6.dev1/fugue/sql/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/sql/workflow.py` & `fugue-0.8.6.dev1/fugue/sql/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/workflow/_checkpoint.py` & `fugue-0.8.6.dev1/fugue/workflow/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/workflow/_tasks.py` & `fugue-0.8.6.dev1/fugue/workflow/_tasks.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/workflow/_workflow_context.py` & `fugue-0.8.6.dev1/fugue/workflow/_workflow_context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/workflow/api.py` & `fugue-0.8.6.dev1/fugue/workflow/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/workflow/module.py` & `fugue-0.8.6.dev1/fugue/workflow/module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue/workflow/workflow.py` & `fugue-0.8.6.dev1/fugue/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue.egg-info/PKG-INFO` & `fugue-0.8.6.dev1/fugue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.5.dev1
+Version: 0.8.6.dev1
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
         
@@ -148,17 +148,24 @@
         
         Fugue can be installed through pip or conda. For example:
         
         ```bash
         pip install fugue
         ```
         
+        In order to use Fugue SQL, it is strongly recommended to install the `sql` extra:
+        
+        ```bash
+        pip install fugue[sql]
+        ```
+        
         It also has the following installation extras:
         
-        *   **spark**: to support Spark as the [ExecutionEngine](https://fugue-tutorials.readthedocs.io/tutorials/advanced/execution_engine.html)
+        *   **sql**: to support Fugue SQL. Without this extra, the non-SQL part still works. Before Fugue 0.9.0, this extra is included in Fugue's core dependency so you don't need to install explicitly. **But for 0,9.0+, this becomes required if you want to use Fugue SQL.**
+        *   **spark**: to support Spark as the [ExecutionEngine](https://fugue-tutorials.readthedocs.io/tutorials/advanced/execution_engine.html).
         *   **dask**: to support Dask as the ExecutionEngine.
         *   **ray**: to support Ray as the ExecutionEngine.
         *   **duckdb**: to support DuckDB as the ExecutionEngine, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/duckdb.html).
         *   **polars**: to support Polars DataFrames and extensions using Polars.
         *   **ibis**: to enable Ibis for Fugue workflows, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/ibis.html).
         *   **cpp_sql_parser**: to enable the CPP antlr parser for Fugue SQL. It can be 50+ times faster than the pure Python parser. For the main Python versions and platforms, there is already pre-built binaries, but for the remaining, it needs a C++ compiler to build on the fly.
```

### Comparing `fugue-0.8.5.dev1/fugue.egg-info/SOURCES.txt` & `fugue-0.8.6.dev1/fugue.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 fugue/__init__.py
 fugue/api.py
 fugue/constants.py
 fugue/dev.py
 fugue/exceptions.py
 fugue/plugins.py
+fugue/py.typed
 fugue/registry.py
 fugue.egg-info/PKG-INFO
 fugue.egg-info/SOURCES.txt
 fugue.egg-info/dependency_links.txt
 fugue.egg-info/entry_points.txt
 fugue.egg-info/requires.txt
 fugue.egg-info/top_level.txt
```

### Comparing `fugue-0.8.5.dev1/fugue.egg-info/requires.txt` & `fugue-0.8.6.dev1/fugue.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-triad>=0.9.0
+triad>=0.9.1
 adagio>=0.2.4
 pyarrow>=0.15.1
 pandas>=1.2.0
-qpd>=0.4.3
+qpd>=0.4.4
 fugue-sql-antlr>=0.1.6
 sqlglot
 jinja2
 
 [all]
 sqlglot
 jinja2
 fugue-sql-antlr[cpp]>=0.1.6
 pyspark>=3.1.1
-ray[data]>=2.0.0
-qpd[dask]>=0.4.3
+ray[data]>=2.1.0
+qpd[dask]>=0.4.4
 notebook
 jupyterlab
 ipython>=7.10.0
 duckdb>=0.5.0
 pyarrow>=6.0.1
 polars
 
 [all:python_version < "3.8"]
 dask[dataframe,distributed]
 ibis-framework>=2.1.1
 
 [all:python_version >= "3.8"]
 dask[dataframe,distributed]>=2022.9.0
-ibis-framework>=3.2.0
+ibis-framework<6,>=3.2.0
 
 [cpp_sql_parser]
 fugue-sql-antlr[cpp]>=0.1.6
 
 [dask]
-qpd[dask]>=0.4.3
+qpd[dask]>=0.4.4
 
 [dask:python_version < "3.8"]
 dask[dataframe,distributed]
 
 [dask:python_version >= "3.8"]
 dask[dataframe,distributed]>=2022.9.0
 
@@ -48,30 +48,30 @@
 
 [ibis]
 
 [ibis:python_version < "3.8"]
 ibis-framework>=2.1.1
 
 [ibis:python_version >= "3.8"]
-ibis-framework>=3.2.0
+ibis-framework<6,>=3.2.0
 
 [notebook]
 notebook
 jupyterlab
 ipython>=7.10.0
 
 [polars]
 polars
 
 [ray]
-ray[data]>=2.0.0
+ray[data]>=2.1.0
 duckdb>=0.5.0
 pyarrow>=6.0.1
 
 [spark]
 pyspark>=3.1.1
 
 [sql]
-qpd>=0.4.3
+qpd>=0.4.4
 fugue-sql-antlr>=0.1.6
 sqlglot
 jinja2
```

### Comparing `fugue-0.8.5.dev1/fugue_contrib/seaborn/__init__.py` & `fugue-0.8.6.dev1/fugue_contrib/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_contrib/viz/__init__.py` & `fugue-0.8.6.dev1/fugue_contrib/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_contrib/viz/_ext.py` & `fugue-0.8.6.dev1/fugue_contrib/viz/_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_dask/_io.py` & `fugue-0.8.6.dev1/fugue_dask/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_dask/_utils.py` & `fugue-0.8.6.dev1/fugue_dask/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_dask/dataframe.py` & `fugue-0.8.6.dev1/fugue_dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_dask/execution_engine.py` & `fugue-0.8.6.dev1/fugue_dask/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_dask/ibis_engine.py` & `fugue-0.8.6.dev1/fugue_dask/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_dask/registry.py` & `fugue-0.8.6.dev1/fugue_dask/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_duckdb/_io.py` & `fugue-0.8.6.dev1/fugue_duckdb/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_duckdb/_utils.py` & `fugue-0.8.6.dev1/fugue_duckdb/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_duckdb/dask.py` & `fugue-0.8.6.dev1/fugue_duckdb/dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_duckdb/dataframe.py` & `fugue-0.8.6.dev1/fugue_duckdb/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_duckdb/execution_engine.py` & `fugue-0.8.6.dev1/fugue_duckdb/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_duckdb/ibis_engine.py` & `fugue-0.8.6.dev1/fugue_duckdb/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_duckdb/registry.py` & `fugue-0.8.6.dev1/fugue_duckdb/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ibis/_utils.py` & `fugue-0.8.6.dev1/fugue_ibis/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ibis/dataframe.py` & `fugue-0.8.6.dev1/fugue_ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ibis/execution/ibis_engine.py` & `fugue-0.8.6.dev1/fugue_ibis/execution/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ibis/execution/pandas_backend.py` & `fugue-0.8.6.dev1/fugue_ibis/execution/pandas_backend.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ibis/execution_engine.py` & `fugue-0.8.6.dev1/fugue_ibis/execution_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,49 +88,42 @@
         how: str,
         on: Optional[List[str]] = None,
     ) -> DataFrame:
         _df1 = self.to_df(df1)
         _df2 = self.to_df(df2)
         key_schema, end_schema = get_join_schemas(_df1, _df2, how=how, on=on)
         on_fields = [_df1.native[k] == _df2.native[k] for k in key_schema]
+        if ibis.__version__ < "6":
+            suffixes: Dict[str, Any] = dict(suffixes=("", _JOIN_RIGHT_SUFFIX))
+        else:  # pragma: no cover
+            # breaking change in ibis 6.0
+            suffixes = dict(lname="", rname=_JOIN_RIGHT_SUFFIX)
         if how.lower() == "cross":
-            tb = _df1.native.cross_join(_df2.native, suffixes=("", _JOIN_RIGHT_SUFFIX))
+            tb = _df1.native.cross_join(_df2.native, **suffixes)
         elif how.lower() == "right_outer":
-            tb = _df2.native.left_join(
-                _df1.native, on_fields, suffixes=("", _JOIN_RIGHT_SUFFIX)
-            )
+            tb = _df2.native.left_join(_df1.native, on_fields, **suffixes)
         elif how.lower() == "left_outer":
-            tb = _df1.native.left_join(
-                _df2.native, on_fields, suffixes=("", _JOIN_RIGHT_SUFFIX)
-            )
+            tb = _df1.native.left_join(_df2.native, on_fields, **suffixes)
         elif how.lower() == "full_outer":
-            tb = _df1.native.outer_join(
-                _df2.native, on_fields, suffixes=("", _JOIN_RIGHT_SUFFIX)
-            )
+            tb = _df1.native.outer_join(_df2.native, on_fields, **suffixes)
             cols: List[Any] = []
             for k in end_schema.names:
                 if k not in key_schema:
                     cols.append(k)
                 else:
                     cols.append(
                         ibis.coalesce(tb[k], tb[k + _JOIN_RIGHT_SUFFIX]).name(k)
                     )
             tb = tb[cols]
         elif how.lower() in ["semi", "left_semi"]:
-            tb = _df1.native.semi_join(
-                _df2.native, on_fields, suffixes=("", _JOIN_RIGHT_SUFFIX)
-            )
+            tb = _df1.native.semi_join(_df2.native, on_fields, **suffixes)
         elif how.lower() in ["anti", "left_anti"]:
-            tb = _df1.native.anti_join(
-                _df2.native, on_fields, suffixes=("", _JOIN_RIGHT_SUFFIX)
-            )
+            tb = _df1.native.anti_join(_df2.native, on_fields, **suffixes)
         else:
-            tb = _df1.native.inner_join(
-                _df2.native, on_fields, suffixes=("", _JOIN_RIGHT_SUFFIX)
-            )
+            tb = _df1.native.inner_join(_df2.native, on_fields, **suffixes)
         return self.to_df(tb[end_schema.names], schema=end_schema)
 
     def union(self, df1: DataFrame, df2: DataFrame, distinct: bool = True) -> DataFrame:
         _df1 = self.to_df(df1)
         _df2 = self.to_df(df2)
         tb = _df1.native.union(_df2.native, distinct=distinct)
         return self.to_df(tb, df1.schema)
```

### Comparing `fugue-0.8.5.dev1/fugue_ibis/extensions.py` & `fugue-0.8.6.dev1/fugue_ibis/extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_notebook/__init__.py` & `fugue-0.8.6.dev1/fugue_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_notebook/env.py` & `fugue-0.8.6.dev1/fugue_notebook/env.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_notebook/nbextension/main.js` & `fugue-0.8.6.dev1/fugue_notebook/nbextension/main.js`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_polars/polars_dataframe.py` & `fugue-0.8.6.dev1/fugue_polars/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_polars/registry.py` & `fugue-0.8.6.dev1/fugue_polars/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ray/_constants.py` & `fugue-0.8.6.dev1/fugue_ray/_constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ray/_utils/cluster.py` & `fugue-0.8.6.dev1/fugue_ray/_utils/cluster.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ray/_utils/io.py` & `fugue-0.8.6.dev1/fugue_ray/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ray/dataframe.py` & `fugue-0.8.6.dev1/fugue_ray/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     get_column_names,
     get_num_partitions,
     is_df,
     rename,
 )
 
 from ._constants import _ZERO_COPY
-from ._utils.dataframe import build_empty, get_dataset_format
+from ._utils.dataframe import build_empty, get_dataset_format, materialize, to_schema
 
 
 class RayDataFrame(DataFrame):
     """DataFrame that wraps Ray DataSet. Please also read
     |DataFrameTutorial| to understand this Fugue concept
 
     :param df: :class:`ray:ray.data.Dataset`, :class:`pa:pyarrow.Table`,
@@ -48,25 +48,25 @@
             schema = _input_schema(schema).assert_not_empty()
         if df is None:
             schema = _input_schema(schema).assert_not_empty()
             super().__init__(schema)
             self._native = build_empty(schema)
             return
         if isinstance(df, rd.Dataset):
-            fmt = get_dataset_format(df)
+            fmt, df = get_dataset_format(df)
             if fmt is None:  # empty:
                 schema = _input_schema(schema).assert_not_empty()
                 super().__init__(schema)
                 self._native = build_empty(schema)
                 return
             elif fmt == "pandas":
                 rdf = rd.from_arrow_refs(df.to_arrow_refs())
             elif fmt == "arrow":
                 rdf = df
-            else:
+            else:  # pragma: no cover
                 raise NotImplementedError(
                     f"Ray Dataset in {fmt} format is not supported"
                 )
         elif isinstance(df, pa.Table):
             rdf = rd.from_arrow(df)
             if schema is None:
                 schema = df.schema
@@ -152,16 +152,15 @@
         data = self.native.limit(1).to_pandas().values.tolist()
         if len(data) == 0:
             raise FugueDatasetEmptyError
         return data[0]
 
     def persist(self, **kwargs: Any) -> "RayDataFrame":
         # TODO: it mutates the dataframe, is this a good bahavior
-        if not self.native.is_fully_executed():  # pragma: no cover
-            self.native.fully_executed()
+        self._native = materialize(self._native)
         return self
 
     def count(self) -> int:
         return self.native.count()
 
     def as_arrow(self, type_safe: bool = False) -> pa.Table:
         return pa.concat_tables(_get_arrow_tables(self.native))
@@ -222,19 +221,20 @@
         return pdf.as_local()  # type: ignore
 
     def _apply_schema(
         self, rdf: rd.Dataset, schema: Optional[Schema], internal_schema: bool
     ) -> Tuple[rd.Dataset, Schema]:
         if internal_schema:
             return rdf, schema
-        if get_dataset_format(rdf) is None:  # empty
+        fmt, rdf = get_dataset_format(rdf)
+        if fmt is None:  # empty
             schema = _input_schema(schema).assert_not_empty()
             return build_empty(schema), schema
-        if schema is None or schema == rdf.schema(fetch_if_missing=True):
-            return rdf, rdf.schema(fetch_if_missing=True)
+        if schema is None or schema == to_schema(rdf.schema(fetch_if_missing=True)):
+            return rdf, to_schema(rdf.schema(fetch_if_missing=True))
 
         def _alter(table: pa.Table) -> pa.Table:  # pragma: no cover
             return ArrowDataFrame(table).alter_columns(schema).native  # type: ignore
 
         return (
             rdf.map_batches(
                 _alter, batch_format="pyarrow", **_ZERO_COPY, **self._remote_args()
@@ -259,20 +259,23 @@
 @as_local_bounded.candidate(lambda df: isinstance(df, rd.Dataset))
 def _rd_as_local(df: rd.Dataset) -> bool:
     return pa.concat_tables(_get_arrow_tables(df))
 
 
 @get_column_names.candidate(lambda df: isinstance(df, rd.Dataset))
 def _get_ray_dataframe_columns(df: rd.Dataset) -> List[Any]:
-    fmt = get_dataset_format(df)
-    if fmt == "pandas":
-        return list(df.schema(True).names)
-    elif fmt == "arrow":
-        return [f.name for f in df.schema(True)]
-    raise NotImplementedError(f"{fmt} is not supported")  # pragma: no cover
+    if hasattr(df, "columns"):  # higher version of ray
+        return df.columns(fetch_if_missing=True)
+    else:  # pragma: no cover
+        fmt, _ = get_dataset_format(df)
+        if fmt == "pandas":
+            return list(df.schema(True).names)
+        elif fmt == "arrow":
+            return df.schema(fetch_if_missing=True).names
+        raise NotImplementedError(f"{fmt} is not supported")  # pragma: no cover
 
 
 @rename.candidate(lambda df, *args, **kwargs: isinstance(df, rd.Dataset))
 def _rename_ray_dataframe(df: rd.Dataset, columns: Dict[str, Any]) -> rd.Dataset:
     if len(columns) == 0:
         return df
     cols = _get_ray_dataframe_columns(df)
```

### Comparing `fugue-0.8.5.dev1/fugue_ray/execution_engine.py` & `fugue-0.8.6.dev1/fugue_ray/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_ray/registry.py` & `fugue-0.8.6.dev1/fugue_ray/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_spark/_utils/convert.py` & `fugue-0.8.6.dev1/fugue_spark/_utils/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_spark/_utils/io.py` & `fugue-0.8.6.dev1/fugue_spark/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_spark/_utils/misc.py` & `fugue-0.8.6.dev1/fugue_spark/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_spark/_utils/partition.py` & `fugue-0.8.6.dev1/fugue_spark/_utils/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_spark/dataframe.py` & `fugue-0.8.6.dev1/fugue_spark/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_spark/execution_engine.py` & `fugue-0.8.6.dev1/fugue_spark/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_spark/ibis_engine.py` & `fugue-0.8.6.dev1/fugue_spark/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_spark/registry.py` & `fugue-0.8.6.dev1/fugue_spark/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_test/bag_suite.py` & `fugue-0.8.6.dev1/fugue_test/bag_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_test/builtin_suite.py` & `fugue-0.8.6.dev1/fugue_test/builtin_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_test/dataframe_suite.py` & `fugue-0.8.6.dev1/fugue_test/dataframe_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_test/execution_suite.py` & `fugue-0.8.6.dev1/fugue_test/execution_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/fugue_test/ibis_suite.py` & `fugue-0.8.6.dev1/fugue_test/ibis_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/setup.cfg` & `fugue-0.8.6.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fugue-0.8.5.dev1/setup.py` & `fugue-0.8.6.dev1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,66 +27,66 @@
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="distributed spark dask sql dsl domain specific language",
     url="http://github.com/fugue-project/fugue",
     install_requires=[
-        "triad>=0.9.0",
+        "triad>=0.9.1",
         "adagio>=0.2.4",
         "pyarrow>=0.15.1",
         "pandas>=1.2.0",
         # sql dependencies
-        "qpd>=0.4.3",
+        "qpd>=0.4.4",
         "fugue-sql-antlr>=0.1.6",
         "sqlglot",
         "jinja2",
     ],
     extras_require={
         "sql": [
-            "qpd>=0.4.3",
+            "qpd>=0.4.4",
             "fugue-sql-antlr>=0.1.6",
             "sqlglot",
             "jinja2",
         ],
         "cpp_sql_parser": ["fugue-sql-antlr[cpp]>=0.1.6"],
         "spark": ["pyspark>=3.1.1"],
         "dask": [
             "dask[distributed,dataframe]; python_version < '3.8'",
             "dask[distributed,dataframe]>=2022.9.0; python_version >= '3.8'",
-            "qpd[dask]>=0.4.3",
+            "qpd[dask]>=0.4.4",
         ],
-        "ray": ["ray[data]>=2.0.0", "duckdb>=0.5.0", "pyarrow>=6.0.1"],
+        "ray": ["ray[data]>=2.1.0", "duckdb>=0.5.0", "pyarrow>=6.0.1"],
         "duckdb": [
             "duckdb>=0.5.0",
             "pyarrow>=6.0.1",
             "numpy",
         ],
         "polars": ["polars"],
         "ibis": [
             "ibis-framework>=2.1.1; python_version < '3.8'",
-            "ibis-framework>=3.2.0; python_version >= '3.8'",
+            "ibis-framework>=3.2.0,<6; python_version >= '3.8'",
         ],
         "notebook": ["notebook", "jupyterlab", "ipython>=7.10.0"],
         "all": [
             "sqlglot",
             "jinja2",
             "fugue-sql-antlr[cpp]>=0.1.6",
             "pyspark>=3.1.1",
             "dask[distributed,dataframe]; python_version < '3.8'",
             "dask[distributed,dataframe]>=2022.9.0; python_version >= '3.8'",
-            "ray[data]>=2.0.0",
-            "qpd[dask]>=0.4.3",
+            "ray[data]>=2.1.0",
+            "qpd[dask]>=0.4.4",
             "notebook",
             "jupyterlab",
             "ipython>=7.10.0",
             "duckdb>=0.5.0",
             "pyarrow>=6.0.1",
             "ibis-framework>=2.1.1; python_version < '3.8'",
-            "ibis-framework>=3.2.0; python_version >= '3.8'",
+            "ibis-framework>=3.2.0,<6; python_version >= '3.8'",
             "polars",
         ],
     },
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
@@ -96,15 +96,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     python_requires=">=3.7",
-    package_data={"fugue_notebook": ["nbextension/*"]},
+    package_data={"fugue": ["py.typed"], "fugue_notebook": ["nbextension/*"]},
     entry_points={
         "fugue.plugins": [
             "ibis = fugue_ibis[ibis]",
             "duckdb = fugue_duckdb.registry[duckdb]",
             "duckdb_ibis = fugue_duckdb.ibis_engine[duckdb,ibis]",
             "spark = fugue_spark.registry[spark]",
             "spark_ibis = fugue_spark.ibis_engine[spark,ibis]",
```

