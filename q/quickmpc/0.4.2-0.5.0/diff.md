# Comparing `tmp/quickmpc-0.4.2.tar.gz` & `tmp/quickmpc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-mxppe0ia/quickmpc-0.4.2.tar", last modified: Mon Jun 26 03:31:31 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-o4nte57w/quickmpc-0.5.0.tar", last modified: Thu Jul 13 10:37:40 2023, max compression
```

## Comparing `quickmpc-0.4.2.tar` & `quickmpc-0.5.0.tar`

### file list

```diff
@@ -1,83 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 03:31:10.000000 quickmpc-0.4.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 03:31:10.000000 quickmpc-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 03:31:10.000000 quickmpc-0.4.2/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-26 03:31:10.000000 quickmpc-0.4.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 03:31:10.000000 quickmpc-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 03:31:10.000000 quickmpc-0.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 03:31:31.000000 quickmpc-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 03:31:10.000000 quickmpc-0.4.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-06-26 03:31:10.000000 quickmpc-0.4.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-26 03:31:10.000000 quickmpc-0.4.2/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-26 03:31:10.000000 quickmpc-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-26 03:31:10.000000 quickmpc-0.4.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-26 03:31:10.000000 quickmpc-0.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/qmpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/utils/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 03:31:10.000000 quickmpc-0.4.2/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 03:31:31.000000 quickmpc-0.4.2/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-26 03:31:31.000000 quickmpc-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 03:31:10.000000 quickmpc-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/tests/unit_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/certificates/server1.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/certificates/server1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/certificates/server2.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/certificates/server2.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/certificates/server3.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/certificates/server3.pem
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:31:31.000000 quickmpc-0.4.2/tests/unit_tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tests/unit_tests/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 03:31:10.000000 quickmpc-0.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-13 10:37:19.000000 quickmpc-0.5.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 10:37:19.000000 quickmpc-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-13 10:37:19.000000 quickmpc-0.5.0/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-13 10:37:19.000000 quickmpc-0.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 10:37:19.000000 quickmpc-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-13 10:37:19.000000 quickmpc-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-13 10:37:40.000000 quickmpc-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-13 10:37:19.000000 quickmpc-0.5.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38439 2023-07-13 10:37:19.000000 quickmpc-0.5.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-13 10:37:19.000000 quickmpc-0.5.0/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 10:37:19.000000 quickmpc-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-13 10:37:19.000000 quickmpc-0.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 10:37:19.000000 quickmpc-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/share_data_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/qmpc_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/request/qmpc_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/request/qmpc_request_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/request/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/share/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/share/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/share/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/share/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-13 10:37:40.000000 quickmpc-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 10:37:19.000000 quickmpc-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_share_data_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/request/test_qmpc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/test_qmpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/utils/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/utils/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tox.ini
```

### Comparing `quickmpc-0.4.2/.vscode/settings.json` & `quickmpc-0.5.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/LICENSE` & `quickmpc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/Pipfile.lock` & `quickmpc-0.5.0/Pipfile.lock`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8720383986928105%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'07c71127994b418ccaac592db76f34534ab83f5dfbb037deb02db3c534386bab'}}",*

 * * "'default'": "{'googleapis-common-protos': {'hashes': "*

 * *              "['sha256:0cbedb6fb68f1c07e18eb4c48256320777707e7d0c55063ae56c15db3224a61e', "*

 * *              "'sha256:b35d530fe825fb4227857bc47ad84c33c809ac96f312e13182bdeaa2abe1178a'], "*

 * *              "'version': '==1.59.1'}, 'grpcio': {'hashes': "*

 * *              "['sha256:008767c0aed4899e657b50f2e0beacbabccab51359eba547f860e7c55f2be6ba […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "58f7099bf99712610ba131af2c8131d6f5ff77bcb6cf34a64532a368df00f6d8"
+            "sha256": "07c71127994b418ccaac592db76f34534ab83f5dfbb037deb02db3c534386bab"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.7"
         },
         "sources": [
             {
@@ -83,146 +83,137 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "googleapis-common-protos": {
             "hashes": [
-                "sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44",
-                "sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f"
+                "sha256:0cbedb6fb68f1c07e18eb4c48256320777707e7d0c55063ae56c15db3224a61e",
+                "sha256:b35d530fe825fb4227857bc47ad84c33c809ac96f312e13182bdeaa2abe1178a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.59.0"
+            "version": "==1.59.1"
         },
         "grpcio": {
             "hashes": [
-                "sha256:040eb421613b57c696063abde405916dd830203c184c9000fc8c3b3b3c950325",
-                "sha256:165b05af77e6aecb4210ae7663e25acf234ba78a7c1c157fa5f2efeb0d6ec53c",
-                "sha256:200d69857f9910f7458b39b9bcf83ee4a180591b40146ba9e49314e3a7419313",
-                "sha256:22bdfac4f7f27acdd4da359b5e7e1973dc74bf1ed406729b07d0759fde2f064b",
-                "sha256:2a8e17286c4240137d933b8ca506465472248b4ce0fe46f3404459e708b65b68",
-                "sha256:2cd2e4cefb724cab1ba2df4b7535a9980531b9ec51b4dbb5f137a1f3a3754ef0",
-                "sha256:2f8ff75e61e1227ba7a3f16b2eadbcc11d0a54096d52ab75a6b88cfbe56f55d1",
-                "sha256:2fdd6333ce96435408565a9dbbd446212cd5d62e4d26f6a3c0feb1e3c35f1cc8",
-                "sha256:30e09b5e0531685e176f49679b6a3b190762cc225f4565e55a899f5e14b3aa62",
-                "sha256:3667c06e37d6cd461afdd51cefe6537702f3d1dc5ff4cac07e88d8b4795dc16f",
-                "sha256:36c8abbc5f837111e7bd619612eedc223c290b0903b952ce0c7b00840ea70f14",
-                "sha256:3709048fe0aa23dda09b3e69849a12055790171dab9e399a72ea8f9dfbf9ac80",
-                "sha256:3c1b9f8afa62ff265d86a4747a2990ec5a96e4efce5d5888f245a682d66eca47",
-                "sha256:3ea4341efe603b049e8c9a5f13c696ca37fcdf8a23ca35f650428ad3606381d9",
-                "sha256:3f9a7d88082b2a17ae7bd3c2354d13bab0453899e0851733f6afa6918373f476",
-                "sha256:49ede0528e9dac7e8a9fe30b16c73b630ddd9a576bf4b675eb6b0c53ee5ca00f",
-                "sha256:54b0c29bdd9a3b1e1b61443ab152f060fc719f1c083127ab08d03fac5efd51be",
-                "sha256:54e36c2ee304ff15f2bfbdc43d2b56c63331c52d818c364e5b5214e5bc2ad9f6",
-                "sha256:5694448256e3cdfe5bd358f1574a3f2f51afa20cc834713c4b9788d60b7cc646",
-                "sha256:5e77ee138100f0bb55cbd147840f87ee6241dbd25f09ea7cd8afe7efff323449",
-                "sha256:5eed34994c095e2bf7194ffac7381c6068b057ef1e69f8f08db77771350a7566",
-                "sha256:6604f614016127ae10969176bbf12eb0e03d2fb3d643f050b3b69e160d144fb4",
-                "sha256:68a7514b754e38e8de9075f7bb4dee919919515ec68628c43a894027e40ddec4",
-                "sha256:6972b009638b40a448d10e1bc18e2223143b8a7aa20d7def0d78dd4af4126d12",
-                "sha256:6c677581ce129f5fa228b8f418cee10bd28dd449f3a544ea73c8ba590ee49d0b",
-                "sha256:6c99a73a6260bdf844b2e5ddad02dcd530310f80e1fa72c300fa19c1c7496962",
-                "sha256:82b0ad8ac825d4bb31bff9f638557c045f4a6d824d84b21e893968286f88246b",
-                "sha256:881ecb34feabf31c6b3b9bbbddd1a5b57e69f805041e5a2c6c562a28574f71c4",
-                "sha256:8de30f0b417744288cec65ec8cf84b8a57995cf7f1e84ccad2704d93f05d0aae",
-                "sha256:b69c7adc7ed60da1cb1b502853db61f453fc745f940cbcc25eb97c99965d8f41",
-                "sha256:be1bf35ce82cdbcac14e39d5102d8de4079a1c1a6a06b68e41fcd9ef64f9dd28",
-                "sha256:be7b2265b7527bb12109a7727581e274170766d5b3c9258d4e466f4872522d7a",
-                "sha256:c02abd55409bfb293371554adf6a4401197ec2133dd97727c01180889014ba4d",
-                "sha256:c831f31336e81243f85b6daff3e5e8a123302ce0ea1f2726ad752fd7a59f3aee",
-                "sha256:cd0daac21d9ef5e033a5100c1d3aa055bbed28bfcf070b12d8058045c4e821b1",
-                "sha256:cd9a5e68e79c5f031500e67793048a90209711e0854a9ddee8a3ce51728de4e5",
-                "sha256:d5cd1389669a847555df54177b911d9ff6f17345b2a6f19388707b7a9f724c88",
-                "sha256:d81528ffe0e973dc840ec73a4132fd18b8203ad129d7410155d951a0a7e4f5d0",
-                "sha256:e860a3222139b41d430939bbec2ec9c3f6c740938bf7a04471a9a8caaa965a2e",
-                "sha256:e95c7ccd4c5807adef1602005513bf7c7d14e5a41daebcf9d8d30d8bf51b8f81",
-                "sha256:eafbe7501a3268d05f2e450e1ddaffb950d842a8620c13ec328b501d25d2e2c3",
-                "sha256:eef0450a4b5ed11feab639bf3eb1b6e23d0efa9b911bf7b06fb60e14f5f8a585",
-                "sha256:f601aaeae18dab81930fb8d4f916b0da21e89bb4b5f7367ef793f46b4a76b7b0",
-                "sha256:f7a0d0bf44438869d307f85a54f25a896ad6b4b0ca12370f76892ad732928d87",
-                "sha256:ffaaf7e93fcb437356b5a4b23bf36e8a3d0221399ff77fd057e4bc77776a24be"
+                "sha256:008767c0aed4899e657b50f2e0beacbabccab51359eba547f860e7c55f2be6ba",
+                "sha256:03a80451530fd3b8b155e0c4480434f6be669daf7ecba56f73ef98f94222ee01",
+                "sha256:0409de787ebbf08c9d2bca2bcc7762c1efe72eada164af78b50567a8dfc7253c",
+                "sha256:14e70b4dda3183abea94c72d41d5930c333b21f8561c1904a372d80370592ef3",
+                "sha256:17f47aeb9be0da5337f9ff33ebb8795899021e6c0741ee68bd69774a7804ca86",
+                "sha256:187b8f71bad7d41eea15e0c9812aaa2b87adfb343895fffb704fb040ca731863",
+                "sha256:1eadd6de258901929223f422ffed7f8b310c0323324caf59227f9899ea1b1674",
+                "sha256:38fdf5bd0a1c754ce6bf9311a3c2c7ebe56e88b8763593316b69e0e9a56af1de",
+                "sha256:4241a1c2c76e748023c834995cd916570e7180ee478969c2d79a60ce007bc837",
+                "sha256:437af5a7673bca89c4bc0a993382200592d104dd7bf55eddcd141cef91f40bab",
+                "sha256:43c50d810cc26349b093bf2cfe86756ab3e9aba3e7e681d360930c1268e1399a",
+                "sha256:4c08ee21b3d10315b8dc26f6c13917b20ed574cdbed2d2d80c53d5508fdcc0f2",
+                "sha256:4f84a6fd4482e5fe73b297d4874b62a535bc75dc6aec8e9fe0dc88106cd40397",
+                "sha256:4feee75565d1b5ab09cb3a5da672b84ca7f6dd80ee07a50f5537207a9af543a4",
+                "sha256:50f4daa698835accbbcc60e61e0bc29636c0156ddcafb3891c987e533a0031ba",
+                "sha256:59c4e606993a47146fbeaf304b9e78c447f5b9ee5641cae013028c4cca784617",
+                "sha256:5d2fc471668a7222e213f86ef76933b18cdda6a51ea1322034478df8c6519959",
+                "sha256:64bd3abcf9fb4a9fa4ede8d0d34686314a7075f62a1502217b227991d9ca4245",
+                "sha256:66f0369d27f4c105cd21059d635860bb2ea81bd593061c45fb64875103f40e4a",
+                "sha256:6b5ce42a5ebe3e04796246ba50357f1813c44a6efe17a37f8dc7a5c470377312",
+                "sha256:72836b5a1d4f508ffbcfe35033d027859cc737972f9dddbe33fb75d687421e2e",
+                "sha256:76b6e6e1ee9bda32e6e933efd61c512e9a9f377d7c580977f090d1a9c78cca44",
+                "sha256:79d4c5911d12a7aa671e5eb40cbb50a830396525014d2d6f254ea2ba180ce637",
+                "sha256:7beb84ebd0a3f732625124b73969d12b7350c5d9d64ddf81ae739bbc63d5b1ed",
+                "sha256:8219f17baf069fe8e42bd8ca0b312b875595e43a70cabf397be4fda488e2f27d",
+                "sha256:83ec714bbbe9b9502177c842417fde39f7a267031e01fa3cd83f1ca49688f537",
+                "sha256:8674fdbd28266d8efbcddacf4ec3643f76fe6376f73283fd63a8374c14b0ef7c",
+                "sha256:881575f240eb5db72ddca4dc5602898c29bc082e0d94599bf20588fb7d1ee6a0",
+                "sha256:8b3b2c7b5feef90bc9a5fa1c7f97637e55ec3e76460c6d16c3013952ee479cd9",
+                "sha256:991224fd485e088d3cb5e34366053691a4848a6b7112b8f5625a411305c26691",
+                "sha256:aa08affbf672d051cd3da62303901aeb7042a2c188c03b2c2a2d346fc5e81c14",
+                "sha256:b1f4b6f25a87d80b28dd6d02e87d63fe1577fe6d04a60a17454e3f8077a38279",
+                "sha256:b4638a796778329cc8e142e4f57c705adb286b3ba64e00b0fa91eeb919611be8",
+                "sha256:bd55f743e654fb050c665968d7ec2c33f03578a4bbb163cfce38024775ff54cc",
+                "sha256:c0bc9dda550785d23f4f025be614b7faa8d0293e10811f0f8536cf50435b7a30",
+                "sha256:c2148170e01d464d41011a878088444c13413264418b557f0bdcd1bf1b674a0e",
+                "sha256:c243b158dd7585021d16c50498c4b2ec0a64a6119967440c5ff2d8c89e72330e",
+                "sha256:c63bc5ac6c7e646c296fed9139097ae0f0e63f36f0864d7ce431cce61fe0118a",
+                "sha256:c6f36621aabecbaff3e70c4d1d924c76c8e6a7ffec60c331893640a4af0a8037",
+                "sha256:d596408bab632ec7b947761e83ce6b3e7632e26b76d64c239ba66b554b7ee286",
+                "sha256:defdd14b518e6e468466f799aaa69db0355bca8d3a5ea75fb912d28ba6f8af31",
+                "sha256:e2db108b4c8e29c145e95b0226973a66d73ae3e3e7fae00329294af4e27f1c42",
+                "sha256:f92a99ab0c7772fb6859bf2e4f44ad30088d18f7c67b83205297bfb229e0d2cf",
+                "sha256:fb34ace11419f1ae321c36ccaa18d81cd3f20728cd191250be42949d6845bb2d",
+                "sha256:fdc3a895791af4addbb826808d4c9c35917c59bb5c430d729f44224e51c92d61"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.51.3"
+            "version": "==1.56.0"
         },
         "grpcio-status": {
             "hashes": [
-                "sha256:5357dcd69e51ba3f7b86d57698bd44d2ef295528eb7219b237eb596183334d39",
-                "sha256:78442ac7d2813c56f9cc04f713efd7088596b10f88a4ddd09279211cc48402d5"
+                "sha256:9eca0b2dcda0782d3702df225918efd6d820f75f93cd5c51c7fb6a4ffbfea12c",
+                "sha256:e5f101c96686e9d4e94a114567960fdb00052aa3c818b029745e3db37dc9c613"
             ],
             "index": "pypi",
-            "version": "==1.46.3"
+            "version": "==1.56.0"
         },
         "grpcio-tools": {
             "hashes": [
-                "sha256:0395647f41561a00e5dea633b8171d0597899eb8649dc5bf6a6a0597f9848769",
-                "sha256:07c9aa1a2549569dfa2a25f495543570f4753e96b99fbd46eaf7e2f3d1948cc7",
-                "sha256:096f0901089055f467df7133403a1a1ac782b2a078552ffa51215f5d7a064643",
-                "sha256:0bb48a86591d63b34b12cea2468efc96886aa06ed404707a6fe24cd18032ad45",
-                "sha256:0c455e883e2bf0ee7cc3d0778f3b15dd7616e9a68db6fc4d36ad23d6be643035",
-                "sha256:140288c4d9d1005fcb9e88ac5c1a37973c844bdc180fc34a263efa7aceb2c8fe",
-                "sha256:14b86251ed61133f860b5182801f7d8ac5371ea7a32a60aeca96b3f6d7be56c9",
-                "sha256:15c26699c2c7188010e0dc579ef1a4fba02cfef12bfe56028f73b58feee61d30",
-                "sha256:168520ee3a12002806b7436276bdeb042e4003cc8efba2c82db82a4447d6b3df",
-                "sha256:1763fc1da10d8b505f706d8147499f199cfa55868f7372a0b7fb198378e0f9d1",
-                "sha256:1ab7aead75c794a73cfb3777fca7cd8e234fb15256cff1de506f41de453693a9",
-                "sha256:1bea61acaab74f0ba8a578e7245085fff5021e44756a68dbe83407338776422a",
-                "sha256:21a714df8b894d4d0554414393db6616e20a25d44c7356c545c23c922dcd4e17",
-                "sha256:21bbbcee52c3a1d694d4f29bafc197a16274294ee6bb33f913398f9f1bc23f2e",
-                "sha256:2270c63905fccabc50582e2a6e22700f15f87274e651a0b491771a75c9e68cdf",
-                "sha256:227e2bbc28519a384a064802e239a0231859a108220ebffe10fd9f9a63a1af16",
-                "sha256:2ab51956b500ebe5718024f083513e62f777f1812e280959e85529730f863e3c",
-                "sha256:31fee436ace5b3bd950cc3a8e68d6b84de1d6dc755959db7badc3470cdf22f70",
-                "sha256:36622a56654d2e38b9c323f06786427143e2a44356d30eca5f0e663a58f1d5b4",
-                "sha256:3721e8c5490f7c015b5961133bb5b605a3d65eb8aa873506d3291f1216e28b03",
-                "sha256:3840304ca4ca9586978c790a5433bf14a2d1cb234274dd095cd3673d08f26f07",
-                "sha256:3c6a510c29e466c489db8a3f24cad4386f5b0ca7223af93d821bc7ddfe73b172",
-                "sha256:5466fa708d9ef9980a67e72f839d24c545b0d57d976b4a1cbec150d7d90891c4",
-                "sha256:5a2a1037c0e5b9d3d417640ad233f9aae8a934f01bf54d79dea23ad53282f004",
-                "sha256:5d30bfb595e2ef767082432b17ca9238a3a59c2fd3211e19f29700448d1c9162",
-                "sha256:600ed9e6600ef4815746052833188471c07be38d14f000617791ed1ec1664d53",
-                "sha256:6533916914dc80837d4caa1cf1aec884cc0390ce0543c4091fd817b2e87a87c5",
-                "sha256:68442c23892478bd6ab324f716e0a6b611fefd98c67f18cfb4ef6c63bce3ab47",
-                "sha256:790ba7e1de54480c11b70115dfed76dcf79db929b0f808314014a58a8163d07d",
-                "sha256:7a2c6e847808141ba88e5f45bda76e3d9e5e9866379496d2289e3892fafdd201",
-                "sha256:7b29f82b0f5cf1410f8d4135c20653264a91d156a15394a7b3df5cc4ef4572eb",
-                "sha256:7cc27ec93aa105dcb86acc9eb4cb67fa85420f1bef2fccaf69955f3ee82028db",
-                "sha256:83fa1aaf052dad33000b73a865ad38e7b19ba4ecedb374cd0594824d27aab3ba",
-                "sha256:8918bf43be899b5967aeeb955bb1a557c6f753db22456505091482511021b87f",
-                "sha256:8c3a5c279b1ffbb5c90fd71d8ce94b1aa6d43b1264d086fa553acc825149bef9",
-                "sha256:8e472a2ac4e98a827fcfad719d828dda203d21e63a70f7fbeff0b472d9fb15d5",
-                "sha256:920c57d342c8f9d877679c046407cab1c98a769c196fde35c0c5a14471ebc931",
-                "sha256:9f781cc5f1bc3d70d62f2a2846ca1de588ed75513a39674dea78cb7a4c52a5e9",
-                "sha256:a1c2f0f1e13c185c381ddbe366f186a5cf6848014990ca3b8a3411dc06db9a70",
-                "sha256:a78ae1e9e478bd433999522cde57f3d6e47bfa498de98e35f827b5ea83f87c45",
-                "sha256:af9ed199b9b02a3cc66695b1d89b512084444fedc1e9240258cadcc36e1a9071",
-                "sha256:b10828c9f62cfffb9aad65c5960cac5b65b5c879b29ef7650b6f253cd1d19b37",
-                "sha256:bc630ccaf97eb68ca814305f408a8172c6b0bb5ffdaee2baf16be4da0b704161",
-                "sha256:bf1a4b9f7ba0d39b36ba4759d00a0bb51603a63cea532c5df07ca04db41ddaf9",
-                "sha256:c0f9748b8d585c01151ca8178593152f4679db9b8846f11d0e54aba64b7b72fc",
-                "sha256:c51266f343c3207fc24bf954619992bc5173c93b052de9d90ecdf1d3f42cf13a",
-                "sha256:cd3b9bec82650a47eb8c5d5c25479fcc8cd658deaa444fb8fa61118794b6a8c9",
-                "sha256:cd4084dd54bdeff97cdf648603fd4c63a496ebdf35455f6fc3ea3016231b1e41",
-                "sha256:d4dacd7bba601d00a5f9767b3ea58077ce91c2467bff977998b818f699f9a5ff",
-                "sha256:d8a73c64cd788a7ba597fa8878b4faad928d3c40981449a40e35000c2639d702",
-                "sha256:e247d3b06b441f5516e9ffbfdb83ac15648965170e184d9b5950af61e5976648",
-                "sha256:e8b37f6ef9b15349c5a575a0e0add11892bbbb107e0f21d5da45adba336daf05",
-                "sha256:eddc8509d1d22b46d57cd35284cfe4bee8af2c31693a40a4244b9b2f3795aa36",
-                "sha256:fa404d7c9cd621836220f3b9cb593eb2c475182d5c768b449407506b61f91159"
+                "sha256:02b23a12b91287ebea14b3685735d1d675e77c3cd365ec1771c3e9afbeba1ec6",
+                "sha256:0a8767e4de0f573c678313c5de075ac0e163a192bb135018e45015a22f234387",
+                "sha256:11cdd9cbf0c09c3a761c6f59dfd7128104be7cd393334efe386d4fc3f990ee1a",
+                "sha256:128bb13fe9a2681eeb08175f5fbc8e2d8953d7d0dd240e96f9244b9d2547a1aa",
+                "sha256:142530b9fdfabe04f0c7e5dacd45b6c419d39704fa439cc0aabf73ea0d8f916d",
+                "sha256:168940a4a955b6c65da978dbf62e1c36e3a311bb27f649fd201a228e2583a6d4",
+                "sha256:1bd361fcc967c21672ba855fc77ea0e7afa51664033a746df96545f84edc4670",
+                "sha256:21cf32ccffd4f1800b0dcdf58aa1fc7f626795c9da784c3d817c944edcf2d3ae",
+                "sha256:23e2ef1dc6a9bf766f091e2c52a68e54d0aff3548f94562e61fb0ac3874d514a",
+                "sha256:282176066fb082ad21c403b84f9d6b440a20482e6f52b83bb2adf54d6fdcae9f",
+                "sha256:2b7a4eb5003a29eecd71707589f93ae7e8fa2e681366a811b3f86695055d8666",
+                "sha256:2c1c43d185ebf904c3deec23c36ca2ba4e95db999cf00fc8f85eda4551622a26",
+                "sha256:2d1ee9e13ce135a6ed451b428ef14af131dc7df2551a5344ff4f8aee2d9fab99",
+                "sha256:39f5877cea514b3da9f2683dfb3ffb45ef47b05f4ff39c287d7d61c5057f48b8",
+                "sha256:3a4b06169493f9454a7f2516c5d41b566d9734e553bbc505f2a7837f7f4a2df1",
+                "sha256:3de6c08b545920a39b31ed13305f946c00b19ac1b13d26119f111b6360f22ccf",
+                "sha256:4acdc7b957abfd76581717f0ac8e4408e0a85b7d0ac8d2cdf4d964f16926b897",
+                "sha256:4d59009ed52220eb2d62f5cefa4e58dec930fb92fab27bb390c4cf1d360ac7e1",
+                "sha256:5f5c416b88d76fbdb548cfee0486928748816b700ece6e591006e5b1dc67598f",
+                "sha256:5fd4c005a4afec16578849bc522ddf3298d6d499b3d37bf51314b086c714cdd5",
+                "sha256:781cf09e4d5c9288708f6ec9c3eae64d9d5a0f4c46c7ebe70ebb7ab4f6384789",
+                "sha256:79291bfb1fe5f21d99f4839f43d3c5d44c5402c830a24dbb2811d785dd21264b",
+                "sha256:7e6bcb194b81e372411494d8ed69fab89aa3452b7275fce4f7917fbe7b04fb72",
+                "sha256:7f063443870650e55012fdb3a58ff4ce5f4042b81dad6b749333ee8146157511",
+                "sha256:80d75856f8ec949847386ad2f56a460f21c63bf82ce99ca5b6aa512c0b875fb1",
+                "sha256:8115b416ea2cad8a87dc3aadfaf26da684e003c3770b12e7219b462505bb5b85",
+                "sha256:8870ab60f8a76b4a7e43184ee03d28112b976d83c43d41cec821f47b3a297da2",
+                "sha256:8989d363ac1996238fee61c8f5663f15a8fc362cb1e758c4a686b76cb457cd70",
+                "sha256:96fe2f7f5805d88cb7f2e3e3502550b2883dfab0f9efcf3cbd444942cf2ee1da",
+                "sha256:9cffff0b4af80285fa49637d69b69d640eb775dc74b23635e4de5faad9e7e744",
+                "sha256:ac33fd2d02d24101ea389be8e05b928acb58be56403d4ebc3aecfab473fa4a25",
+                "sha256:accf713f51da74b1a18aa4b31df0ab135510704661f735a938081777b79a4c25",
+                "sha256:b12bb8c1d408ae40e4c806a3a8ebda2d107310e46696e1da13d0dc3f91fbd19d",
+                "sha256:b309659534b5d930f9ab6d521670c2dd86cb6ef7f47f37f73f96557e2ec13a49",
+                "sha256:b57f7f01eafbfe3a293f2efffb675774dbe4074c4627975ec4dc4aa5766801fb",
+                "sha256:c43b4fe8c8df4c52d3106bba2cf427f0e46bbebb80e127fbbc3134db0fead7be",
+                "sha256:c62f07452dee3f1ed23aeaef821797c5e516f79535e97fe6a6b0a0ee8db1cc91",
+                "sha256:cd69107705794e815a8b262722c6fea995911cb1dfc1310abf63b476165335d6",
+                "sha256:cdbae7312e6d132d38ec2c1611b8cafb783e0416cc5c6deae04efde5f16fb190",
+                "sha256:d9b8d1c42854d3433c058795f52b1418b53dd8c1e9811fecb1312202e803a2c5",
+                "sha256:e4cb62a521efbca4cb1ad50233aa400574b3daaf6eb26707d661a0afe8191d92",
+                "sha256:e59ab6c0bf4a8bb975553ad578d4425bd192775ae384f9406d77d31ad00f6efe",
+                "sha256:f3ab1a9fad636302f7307d143f64a9fbd11bc041652bf53bb016006e9a5ca820",
+                "sha256:f7302acaa07cf4966c926fcd6a60c8d30a697f730c38168bf83e1519b464115b",
+                "sha256:fa6d9bdd75d3625dae38372b43696e159c10aa98719b4302b1e94f1ff7878d47"
             ],
             "index": "pypi",
-            "version": "==1.46.3"
+            "version": "==1.56.0"
         },
         "natsort": {
             "hashes": [
-                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
-                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
+                "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581",
+                "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"
             ],
             "index": "pypi",
-            "version": "==8.3.1"
+            "version": "==8.4.0"
         },
         "numpy": {
             "hashes": [
                 "sha256:1dbe1c91269f880e364526649a52eff93ac30035507ae980d2fed33aaee633ac",
                 "sha256:357768c2e4451ac241465157a3e929b265dfac85d9214074985b1786244f2ef3",
                 "sha256:3820724272f9913b597ccd13a467cc492a0da6b05df26ea09e78b171a0bb9da6",
                 "sha256:4391bd07606be175aafd267ef9bea87cf1b8210c787666ce82073b05f202add1",
@@ -253,42 +244,63 @@
                 "sha256:ee5ec40fdd06d62fe5d4084bef4fd50fd4bb6bfd2bf519365f569dc470163ab0",
                 "sha256:f17e562de9edf691a42ddb1eb4a5541c20dd3f9e65b09ded2beb0799c0cf29bb",
                 "sha256:fdffbfb6832cd0b300995a2b08b8f6fa9f6e856d562800fea9182316d99c4e8e"
             ],
             "index": "pypi",
             "version": "==1.21.6"
         },
+        "pandas": {
+            "hashes": [
+                "sha256:1e4285f5de1012de20ca46b188ccf33521bff61ba5c5ebd78b4fb28e5416a9f1",
+                "sha256:2651d75b9a167cc8cc572cf787ab512d16e316ae00ba81874b560586fa1325e0",
+                "sha256:2c21778a688d3712d35710501f8001cdbf96eb70a7c587a3d5613573299fdca6",
+                "sha256:32e1a26d5ade11b547721a72f9bfc4bd113396947606e00d5b4a5b79b3dcb006",
+                "sha256:3345343206546545bc26a05b4602b6a24385b5ec7c75cb6059599e3d56831da2",
+                "sha256:344295811e67f8200de2390093aeb3c8309f5648951b684d8db7eee7d1c81fb7",
+                "sha256:37f06b59e5bc05711a518aa10beaec10942188dccb48918bb5ae602ccbc9f1a0",
+                "sha256:552020bf83b7f9033b57cbae65589c01e7ef1544416122da0c79140c93288f56",
+                "sha256:5cce0c6bbeb266b0e39e35176ee615ce3585233092f685b6a82362523e59e5b4",
+                "sha256:5f261553a1e9c65b7a310302b9dbac31cf0049a51695c14ebe04e4bfd4a96f02",
+                "sha256:60a8c055d58873ad81cae290d974d13dd479b82cbb975c3e1fa2cf1920715296",
+                "sha256:62d5b5ce965bae78f12c1c0df0d387899dd4211ec0bdc52822373f13a3a022b9",
+                "sha256:7d28a3c65463fd0d0ba8bbb7696b23073efee0510783340a44b08f5e96ffce0c",
+                "sha256:8025750767e138320b15ca16d70d5cdc1886e8f9cc56652d89735c016cd8aea6",
+                "sha256:8b6dbec5f3e6d5dc80dcfee250e0a2a652b3f28663492f7dab9a24416a48ac39",
+                "sha256:a395692046fd8ce1edb4c6295c35184ae0c2bbe787ecbe384251da609e27edcb",
+                "sha256:a62949c626dd0ef7de11de34b44c6475db76995c2064e2d99c6498c3dba7fe58",
+                "sha256:aaf183a615ad790801fa3cf2fa450e5b6d23a54684fe386f7e3208f8b9bfbef6",
+                "sha256:adfeb11be2d54f275142c8ba9bf67acee771b7186a5745249c7d5a06c670136b",
+                "sha256:b6b87b2fb39e6383ca28e2829cddef1d9fc9e27e55ad91ca9c435572cdba51bf",
+                "sha256:bd971a3f08b745a75a86c00b97f3007c2ea175951286cdda6abe543e687e5f2f",
+                "sha256:c69406a2808ba6cf580c2255bcf260b3f214d2664a3a4197d0e640f573b46fd3",
+                "sha256:d3bc49af96cd6285030a64779de5b3688633a07eb75c124b0747134a63f4c05f",
+                "sha256:fd541ab09e1f80a2a1760032d665f6e032d8e44055d602d65eeea6e6e85498cb",
+                "sha256:fe95bae4e2d579812865db2212bb733144e34d0c6785c0685329e5b60fcb85dd"
+            ],
+            "index": "pypi",
+            "version": "==1.3.5"
+        },
         "protobuf": {
             "hashes": [
-                "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7",
-                "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c",
-                "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2",
-                "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b",
-                "sha256:44246bab5dd4b7fbd3c0c80b6f16686808fab0e4aca819ade6e8d294a29c7050",
-                "sha256:447d43819997825d4e71bf5769d869b968ce96848b6479397e29fc24c4a5dfe9",
-                "sha256:67a3598f0a2dcbc58d02dd1928544e7d88f764b47d4a286202913f0b2801c2e7",
-                "sha256:74480f79a023f90dc6e18febbf7b8bac7508420f2006fabd512013c0c238f454",
-                "sha256:819559cafa1a373b7096a482b504ae8a857c89593cf3a25af743ac9ecbd23480",
-                "sha256:899dc660cd599d7352d6f10d83c95df430a38b410c1b66b407a6b29265d66469",
-                "sha256:8c0c984a1b8fef4086329ff8dd19ac77576b384079247c770f29cc8ce3afa06c",
-                "sha256:9aae4406ea63d825636cc11ffb34ad3379335803216ee3a856787bcf5ccc751e",
-                "sha256:a7ca6d488aa8ff7f329d4c545b2dbad8ac31464f1d8b1c87ad1346717731e4db",
-                "sha256:b6cc7ba72a8850621bfec987cb72623e703b7fe2b9127a161ce61e61558ad905",
-                "sha256:bf01b5720be110540be4286e791db73f84a2b721072a3711efff6c324cdf074b",
-                "sha256:c02ce36ec760252242a33967d51c289fd0e1c0e6e5cc9397e2279177716add86",
-                "sha256:d9e4432ff660d67d775c66ac42a67cf2453c27cb4d738fc22cb53b5d84c135d4",
-                "sha256:daa564862dd0d39c00f8086f88700fdbe8bc717e993a21e90711acfed02f2402",
-                "sha256:de78575669dddf6099a8a0f46a27e82a1783c557ccc38ee620ed8cc96d3be7d7",
-                "sha256:e64857f395505ebf3d2569935506ae0dfc4a15cb80dc25261176c784662cdcc4",
-                "sha256:e67f9af1b607eb3a89aafc9bc68a9d1172aae788b2445cb9fd781bd97531f1f1",
-                "sha256:f4bd856d702e5b0d96a00ec6b307b0f51c1982c2bf9c0052cf9019e9a544ba99",
-                "sha256:f4c42102bc82a51108e449cbb32b19b180022941c727bac0cfd50170341f16ee"
+                "sha256:0149053336a466e3e0b040e54d0b615fc71de86da66791c592cc3c8d18150bf8",
+                "sha256:08fe19d267608d438aa37019236db02b306e33f6b9902c3163838b8e75970223",
+                "sha256:29660574cd769f2324a57fb78127cda59327eb6664381ecfe1c69731b83e8288",
+                "sha256:2991f5e7690dab569f8f81702e6700e7364cc3b5e572725098215d3da5ccc6ac",
+                "sha256:3b01a5274ac920feb75d0b372d901524f7e3ad39c63b1a2d55043f3887afe0c1",
+                "sha256:3bcbeb2bf4bb61fe960dd6e005801a23a43578200ea8ceb726d1f6bd0e562ba1",
+                "sha256:447b9786ac8e50ae72cae7a2eec5c5df6a9dbf9aa6f908f1b8bda6032644ea62",
+                "sha256:514b6bbd54a41ca50c86dd5ad6488afe9505901b3557c5e0f7823a0cf67106fb",
+                "sha256:5cb9e41188737f321f4fce9a4337bf40a5414b8d03227e1d9fbc59bc3a216e35",
+                "sha256:7a92beb30600332a52cdadbedb40d33fd7c8a0d7f549c440347bc606fb3fe34b",
+                "sha256:84ea0bd90c2fdd70ddd9f3d3fc0197cc24ecec1345856c2b5ba70e4d99815359",
+                "sha256:aca6e86a08c5c5962f55eac9b5bd6fce6ed98645d77e8bfc2b952ecd4a8e4f6a",
+                "sha256:cc14358a8742c4e06b1bfe4be1afbdf5c9f6bd094dff3e14edb78a1513893ff5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.20.3"
+            "version": "==4.23.3"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
@@ -305,72 +317,55 @@
                 "sha256:a36d4a9dda1f19ce6e03c9a784a2921a4b726b02e1c736600ca9c22029474394",
                 "sha256:a422368fc821589c228f4c49438a368831cb5bbc0eab5ebe1d7fac9dded6567b",
                 "sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543"
             ],
             "index": "pypi",
             "version": "==1.5.0"
         },
+        "python-dateutil": {
+            "hashes": [
+                "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
+                "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==2.8.2"
+        },
+        "pytz": {
+            "hashes": [
+                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
+                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
+            ],
+            "version": "==2023.3"
+        },
         "setuptools": {
             "hashes": [
-                "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077",
-                "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.6.0"
+            "version": "==68.0.0"
+        },
+        "six": {
+            "hashes": [
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
         },
         "tqdm": {
             "hashes": [
                 "sha256:1871fb68a86b8fb3b59ca4cdd3dcccbc7e6d613eeed31f4c332531977b89beb5",
                 "sha256:c4f53a17fe37e132815abceec022631be8ffe1b9381c2e6e30aa70edc99e9671"
             ],
             "index": "pypi",
             "version": "==4.65.0"
         }
     },
     "develop": {
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
-        },
-        "autopep8": {
-            "hashes": [
-                "sha256:86e9303b5e5c8160872b2f5ef611161b2893e9bfe8ccc7e2f76385947d57a2f1",
-                "sha256:f9849cdd62108cb739dbcdbfb7fdcc9a30d1b63c4cc3e1c1f893b5360941b61c"
-            ],
-            "index": "pypi",
-            "version": "==2.0.2"
-        },
-        "cachetools": {
-            "hashes": [
-                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
-                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
-            ],
-            "markers": "python_version ~= '3.7'",
-            "version": "==5.3.0"
-        },
-        "chardet": {
-            "hashes": [
-                "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
-                "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==5.1.0"
-        },
-        "colorama": {
-            "hashes": [
-                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
-                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==0.4.6"
-        },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
@@ -380,178 +375,171 @@
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:75997740323c5f12e18f10b494bc11c03e42843129f980f17c04352cc7b09d40",
-                "sha256:eb8f0f2d37ed68223ea63e3bddf2fac99667e4362c88b3f762e434d160190d18"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.2"
+            "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
-                "sha256:326a54ace7878a5ad1538110f2145bc6a134df43fff290475fd4e7ba38a6deea",
-                "sha256:80a66cd9bd66b0679da030fc930c0a4d09237dd72f354d899427b5c6718223b9"
+                "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
+                "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "index": "pypi",
-            "version": "==2.5.5"
+            "version": "==5.0.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20",
-                "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"
+                "sha256:057e92c15bc8d9e8109738a48db0ccb31b4d9d5cfbee5a8670879a30be66304b",
+                "sha256:b7e52a1f8dec14a75ea73e0891f3060099ca1d8e6a462a4dff11c3e119ea1b31"
             ],
             "markers": "python_version < '3.8'",
-            "version": "==6.1.0"
+            "version": "==4.2.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
-        "isort": {
-            "hashes": [
-                "sha256:6be1f76a507cb2ecf16c7cf14a37e41609ca082330be4e3436a18ef74add55db",
-                "sha256:ba1d72fb2595a01c7895a5128f9585a5cc4b6d395f1c8d514989b9a7eb2a8746"
-            ],
-            "index": "pypi",
-            "version": "==5.11.5"
-        },
         "mccabe": {
             "hashes": [
-                "sha256:9a2b12ebd876e77c72e41ebf401cc2e7c5b566649d50105ca49822688642207b",
-                "sha256:cbc2938f6c01061bc6d21d0c838c2489664755cb18676f0734d7617f4577d09e"
+                "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
+                "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==0.4.0"
+            "version": "==0.7.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:0a28a76785bf57655a8ea5eb0540a15b0e781c807b5aa798bd463779988fa1d5",
-                "sha256:19ba15f9627a5723e522d007fe708007bae52b93faab00f95d72f03e1afa9598",
-                "sha256:21b437be1c02712a605591e1ed1d858aba681757a1e55fe678a15c2244cd68a5",
-                "sha256:26cdd6a22b9b40b2fd71881a8a4f34b4d7914c679f154f43385ca878a8297389",
-                "sha256:2888ce4fe5aae5a673386fa232473014056967f3904f5abfcf6367b5af1f612a",
-                "sha256:2b0c373d071593deefbcdd87ec8db91ea13bd8f1328d44947e88beae21e8d5e9",
-                "sha256:315ac73cc1cce4771c27d426b7ea558fb4e2836f89cb0296cbe056894e3a1f78",
-                "sha256:39c7119335be05630611ee798cc982623b9e8f0cff04a0b48dfc26100e0b97af",
-                "sha256:4b398d8b1f4fba0e3c6463e02f8ad3346f71956b92287af22c9b12c3ec965a9f",
-                "sha256:4e4e8b362cdf99ba00c2b218036002bdcdf1e0de085cdb296a49df03fb31dfc4",
-                "sha256:59bbd71e5c58eed2e992ce6523180e03c221dcd92b52f0e792f291d67b15a71c",
-                "sha256:5b5f81b40d94c785f288948c16e1f2da37203c6006546c5d947aab6f90aefef2",
-                "sha256:5cb14ff9919b7df3538590fc4d4c49a0f84392237cbf5f7a816b4161c061829e",
-                "sha256:61bf08362e93b6b12fad3eab68c4ea903a077b87c90ac06c11e3d7a09b56b9c1",
-                "sha256:64cc3afb3e9e71a79d06e3ed24bb508a6d66f782aff7e56f628bf35ba2e0ba51",
-                "sha256:69b35d1dcb5707382810765ed34da9db47e7f95b3528334a3c999b0c90fe523f",
-                "sha256:9401e33814cec6aec8c03a9548e9385e0e228fc1b8b0a37b9ea21038e64cdd8a",
-                "sha256:a380c041db500e1410bb5b16b3c1c35e61e773a5c3517926b81dfdab7582be54",
-                "sha256:ae9ceae0f5b9059f33dbc62dea087e942c0ccab4b7a003719cb70f9b8abfa32f",
-                "sha256:b7c7b708fe9a871a96626d61912e3f4ddd365bf7f39128362bc50cbd74a634d5",
-                "sha256:c1c10fa12df1232c936830839e2e935d090fc9ee315744ac33b8a32216b93707",
-                "sha256:ce61663faf7a8e5ec6f456857bfbcec2901fbdb3ad958b778403f63b9e606a1b",
-                "sha256:d64c28e03ce40d5303450f547e07418c64c241669ab20610f273c9e6290b4b0b",
-                "sha256:d809f88734f44a0d44959d795b1e6f64b2bbe0ea4d9cc4776aa588bb4229fc1c",
-                "sha256:dbb19c9f662e41e474e0cff502b7064a7edc6764f5262b6cd91d698163196799",
-                "sha256:ef6a01e563ec6a4940784c574d33f6ac1943864634517984471642908b30b6f7"
+                "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042",
+                "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd",
+                "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2",
+                "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01",
+                "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7",
+                "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3",
+                "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816",
+                "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3",
+                "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc",
+                "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4",
+                "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b",
+                "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8",
+                "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c",
+                "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462",
+                "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7",
+                "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc",
+                "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258",
+                "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b",
+                "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9",
+                "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6",
+                "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f",
+                "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1",
+                "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828",
+                "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878",
+                "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f",
+                "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"
             ],
             "index": "pypi",
-            "version": "==1.1.1"
+            "version": "==1.4.1"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
-        "pep8": {
+        "platformdirs": {
             "hashes": [
-                "sha256:b22cfae5db09833bb9bd7c8463b53e1a9c9b39f12e304a8d0bba729c501827ee",
-                "sha256:fe249b52e20498e59e0b5c5256aa52ee99fc295b26ec9eaa85776ffdb9fe6374"
+                "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490",
+                "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"
             ],
-            "version": "==1.7.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.6.2"
         },
-        "platformdirs": {
+        "pluggy": {
             "hashes": [
-                "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa",
-                "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.1"
+            "version": "==1.2.0"
         },
-        "pluggy": {
+        "py": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719",
+                "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==1.11.0"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
-                "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
+                "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
+                "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.10.0"
+            "version": "==2.9.1"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:071d121e9e7b33058aa1ba5de7bce9b97bfa3149cfe1acbb6587c21fc1c8eda1",
-                "sha256:f39e33a4c03beead8774f005bd3ecf0c3f2f264fa0201de965fce0aff1d34263"
+                "sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2",
+                "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "version": "==2.5.0"
         },
-        "pyproject-api": {
+        "pytest": {
             "hashes": [
-                "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
-                "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.5.1"
+            "index": "pypi",
+            "version": "==7.4.0"
         },
-        "pytest": {
+        "six": {
             "hashes": [
-                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
-                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "index": "pypi",
-            "version": "==7.2.2"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
         },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
-                "sha256:52c92a96e2c3fd47c5301e9c26f5a871466133d5376958c1ed95ef4ff4629cbe",
-                "sha256:da10ca1d809b99fae80b706b9dc9656b1daf505a395ac427d130a8a85502d08f"
+                "sha256:57b5ab7e8bb3074edc3c0c0b4b192a4f3799d3723b2c5b76f1fa9f2d40316eea",
+                "sha256:d0d28f3fe6d6d7195c27f8b054c3e99d5451952b54abdae673b71609a581f640"
             ],
             "index": "pypi",
-            "version": "==4.4.7"
+            "version": "==3.28.0"
         },
         "typed-ast": {
             "hashes": [
                 "sha256:0261195c2062caf107831e92a76764c81227dae162c4f75192c0d489faf751a2",
                 "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1",
                 "sha256:183afdf0ec5b1b211724dfef3d2cad2d767cbefac291f24d69b00546c1837fb6",
                 "sha256:211260621ab1cd7324e0798d6be953d00b74e0428382991adfddb352252f1d62",
@@ -577,51 +565,51 @@
                 "sha256:ed855bbe3eb3715fca349c80174cfcfd699c2f9de574d40527b8429acae23a66"
             ],
             "markers": "python_version < '3.8'",
             "version": "==1.5.4"
         },
         "types-protobuf": {
             "hashes": [
-                "sha256:1e59294618c9518f35f17ae1a3d866cdf7e998eb4b9907d41e9ebe5b84fde636",
-                "sha256:bf2b414d815dc387c0a041d9207db054c7cdb94591bb233d9b71a85243e05efc"
+                "sha256:7bd5ea122a057b11a82b785d9de464932a1e9175fe977a4128adef11d7f35547",
+                "sha256:c926104f69ea62103846681b35b690d8d100ecf86c6cdda16c850a1313a272e4"
             ],
             "index": "pypi",
-            "version": "==4.22.0.0"
+            "version": "==4.23.0.1"
         },
         "types-tabulate": {
             "hashes": [
-                "sha256:be2ea0de05f615ccfcbadf6206aa720e265955eb1de23e343aec9d8bf3fa9aaa",
-                "sha256:e486292c279f19247865bdabe802419740a0e74b53444e7f7a8009e08129da5d"
+                "sha256:1dd4322a3a146e9073169c74278b8f14a58eb9905ca9db0d2588df408f27cac9",
+                "sha256:a2e41cc41b6b46bfaec78f8fd8e03058fda7a31af6f203a4b235f5482f571f6f"
             ],
             "index": "pypi",
-            "version": "==0.9.0.1"
+            "version": "==0.9.0.2"
         },
         "types-tqdm": {
             "hashes": [
-                "sha256:3377b5e34396b4e1661f8df7390051490918b8be36ae0f7b6864c1d806e95ef5",
-                "sha256:8707a0dd16a1f2061e316ddc5ef07908d7465193f0d2ed24be75b55e6b9e6cbe"
+                "sha256:4894fe2b1581374ce9bca3f23d53729e4409d69b352e3d5db5829fa19482962c",
+                "sha256:972dd871b6b2b8ff32f1f0f6fdfdf5a4ba2b0b848453689391bec8bd858fb1c4"
             ],
             "index": "pypi",
-            "version": "==4.65.0.0"
+            "version": "==4.65.0.1"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
-                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.5.0"
+            "version": "==4.6.3"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
-                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
+                "sha256:0ef5be6d07181946891f5abc8047fda8bc2f0b4b9bf222c64e6e8963baee76db",
+                "sha256:635b272a8e2f77cb051946f46c60a54ace3cb5e25568228bd6b57fc70eca9ff3"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==20.21.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==20.16.2"
         },
         "zipp": {
             "hashes": [
                 "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
                 "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `quickmpc-0.4.2/README-ja.md` & `quickmpc-0.5.0/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/README.md` & `quickmpc-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/mypy.ini` & `quickmpc-0.5.0/mypy.ini`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 [mypy-quickmpc.proto.*]
 ignore_errors = True
 
 # 型ヒントが導入されていないライブラリのerrorを除外
 [mypy-numpy.*]
 ignore_missing_imports = True
 
+[mypy-pandas.*]
+ignore_missing_imports = True
+
 [mypy-nacl.*]
 ignore_missing_imports = True
 
 [mypy-grpc.*]
 ignore_missing_imports = True
 
 [mypy-pytest.*]
```

### Comparing `quickmpc-0.4.2/quickmpc/README.md` & `quickmpc-0.5.0/quickmpc/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-0.5.0/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _JobStatus:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _JobStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_JobStatus.ValueType], builtins.type):  # noqa: F821
+class _JobStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_JobStatus.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN: _JobStatus.ValueType  # 0
     ERROR: _JobStatus.ValueType  # 1
     RECEIVED: _JobStatus.ValueType  # 2
     PRE_JOB: _JobStatus.ValueType  # 3
     READ_DB: _JobStatus.ValueType  # 4
     COMPUTE: _JobStatus.ValueType  # 5
@@ -43,15 +43,15 @@
 COMPLETED: JobStatus.ValueType  # 6
 global___JobStatus = JobStatus
 
 class _ComputationMethod:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ComputationMethodEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ComputationMethod.ValueType], builtins.type):  # noqa: F821
+class _ComputationMethodEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ComputationMethod.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     COMPUTATION_METHOD_UNSPECIFIED: _ComputationMethod.ValueType  # 0
     COMPUTATION_METHOD_MEAN: _ComputationMethod.ValueType  # 1
     COMPUTATION_METHOD_VARIANCE: _ComputationMethod.ValueType  # 2
     COMPUTATION_METHOD_SUM: _ComputationMethod.ValueType  # 3
     COMPUTATION_METHOD_CORREL: _ComputationMethod.ValueType  # 4
     COMPUTATION_METHOD_MESH_CODE: _ComputationMethod.ValueType  # 5
@@ -68,27 +68,28 @@
 COMPUTATION_METHOD_JOIN_TABLE: ComputationMethod.ValueType  # 6
 global___ComputationMethod = ComputationMethod
 
 class _ShareValueTypeEnum:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ShareValueTypeEnumEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ShareValueTypeEnum.ValueType], builtins.type):  # noqa: F821
+class _ShareValueTypeEnumEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ShareValueTypeEnum.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SHARE_VALUE_TYPE_UNSPECIFIED: _ShareValueTypeEnum.ValueType  # 0
     SHARE_VALUE_TYPE_FIXED_POINT: _ShareValueTypeEnum.ValueType  # 1
     SHARE_VALUE_TYPE_UTF_8_INTEGER_REPRESENTATION: _ShareValueTypeEnum.ValueType  # 2
 
 class ShareValueTypeEnum(_ShareValueTypeEnum, metaclass=_ShareValueTypeEnumEnumTypeWrapper): ...
 
 SHARE_VALUE_TYPE_UNSPECIFIED: ShareValueTypeEnum.ValueType  # 0
 SHARE_VALUE_TYPE_FIXED_POINT: ShareValueTypeEnum.ValueType  # 1
 SHARE_VALUE_TYPE_UTF_8_INTEGER_REPRESENTATION: ShareValueTypeEnum.ValueType  # 2
 global___ShareValueTypeEnum = ShareValueTypeEnum
 
+@typing_extensions.final
 class ProcedureProgress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     PROGRESS_FIELD_NUMBER: builtins.int
     COMPLETED_FIELD_NUMBER: builtins.int
@@ -114,14 +115,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_details", b"_details", "details", b"details"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["_details", b"_details", "completed", b"completed", "description", b"description", "details", b"details", "id", b"id", "progress", b"progress"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_details", b"_details"]) -> typing_extensions.Literal["details"] | None: ...
 
 global___ProcedureProgress = ProcedureProgress
 
+@typing_extensions.final
 class JobProgress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     PROGRESSES_FIELD_NUMBER: builtins.int
     job_uuid: builtins.str
@@ -135,17 +137,19 @@
         status: global___JobStatus.ValueType = ...,
         progresses: collections.abc.Iterable[global___ProcedureProgress] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "progresses", b"progresses", "status", b"status"]) -> None: ...
 
 global___JobProgress = JobProgress
 
+@typing_extensions.final
 class Stacktrace(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Frame(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         SOURCE_LOCATION_FIELD_NUMBER: builtins.int
         SOURCE_LINE_FIELD_NUMBER: builtins.int
         FUNCTION_NAME_FIELD_NUMBER: builtins.int
         source_location: builtins.str
@@ -168,14 +172,15 @@
         *,
         frames: collections.abc.Iterable[global___Stacktrace.Frame] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["frames", b"frames"]) -> None: ...
 
 global___Stacktrace = Stacktrace
 
+@typing_extensions.final
 class JobErrorInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     WHAT_FIELD_NUMBER: builtins.int
     ADDITIONAL_INFO_FIELD_NUMBER: builtins.int
     STACKTRACE_FIELD_NUMBER: builtins.int
     what: builtins.str
@@ -194,14 +199,15 @@
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_additional_info", b"_additional_info"]) -> typing_extensions.Literal["additional_info"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_stacktrace", b"_stacktrace"]) -> typing_extensions.Literal["stacktrace"] | None: ...
 
 global___JobErrorInfo = JobErrorInfo
 
+@typing_extensions.final
 class Schema(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     name: builtins.str
     type: global___ShareValueTypeEnum.ValueType
```

### Comparing `quickmpc-0.4.2/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import builtins
 import collections.abc
 import common_types.common_types_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
-import typing
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class SendSharesRequest(google.protobuf.message.Message):
     """*
     the message of SendSharesRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -51,14 +51,15 @@
         matching_column: builtins.int = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_id", b"data_id", "matching_column", b"matching_column", "piece_id", b"piece_id", "schema", b"schema", "sent_at", b"sent_at", "shares", b"shares", "token", b"token"]) -> None: ...
 
 global___SendSharesRequest = SendSharesRequest
 
+@typing_extensions.final
 class DeleteSharesRequest(google.protobuf.message.Message):
     """*
     the message of DeleteSharesRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -73,14 +74,15 @@
         dataIds: collections.abc.Iterable[builtins.str] | None = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["dataIds", b"dataIds", "token", b"token"]) -> None: ...
 
 global___DeleteSharesRequest = DeleteSharesRequest
 
+@typing_extensions.final
 class GetSchemaRequest(google.protobuf.message.Message):
     """*
     the message of GetSchemaRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -94,14 +96,15 @@
         data_id: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_id", b"data_id", "token", b"token"]) -> None: ...
 
 global___GetSchemaRequest = GetSchemaRequest
 
+@typing_extensions.final
 class GetSchemaResponse(google.protobuf.message.Message):
     """*
     the message of GetSchemaResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -113,14 +116,15 @@
         *,
         schema: collections.abc.Iterable[common_types.common_types_pb2.Schema] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["schema", b"schema"]) -> None: ...
 
 global___GetSchemaResponse = GetSchemaResponse
 
+@typing_extensions.final
 class JoinOrder(google.protobuf.message.Message):
     """*
     the message of ExecuteComputationRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -135,14 +139,15 @@
         data_ids: collections.abc.Iterable[builtins.str] | None = ...,
         debug_mode: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_ids", b"data_ids", "debug_mode", b"debug_mode"]) -> None: ...
 
 global___JoinOrder = JoinOrder
 
+@typing_extensions.final
 class Input(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SRC_FIELD_NUMBER: builtins.int
     TARGET_FIELD_NUMBER: builtins.int
     @property
     def src(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
@@ -154,14 +159,15 @@
         src: collections.abc.Iterable[builtins.int] | None = ...,
         target: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["src", b"src", "target", b"target"]) -> None: ...
 
 global___Input = Input
 
+@typing_extensions.final
 class ExecuteComputationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     METHOD_ID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     TABLE_FIELD_NUMBER: builtins.int
     ARG_FIELD_NUMBER: builtins.int
@@ -180,14 +186,15 @@
         arg: global___Input | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["arg", b"arg", "table", b"table"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["arg", b"arg", "method_id", b"method_id", "table", b"table", "token", b"token"]) -> None: ...
 
 global___ExecuteComputationRequest = ExecuteComputationRequest
 
+@typing_extensions.final
 class ExecuteComputationResponse(google.protobuf.message.Message):
     """
     the message of ExecuteComputationResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -198,15 +205,16 @@
         *,
         job_uuid: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid"]) -> None: ...
 
 global___ExecuteComputationResponse = ExecuteComputationResponse
 
-class GetComputationResultRequest(google.protobuf.message.Message):
+@typing_extensions.final
+class GetComputationRequest(google.protobuf.message.Message):
     """*
     the message of GetComputationResultRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
@@ -217,90 +225,75 @@
         self,
         *,
         job_uuid: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
 
-global___GetComputationResultRequest = GetComputationResultRequest
+global___GetComputationRequest = GetComputationRequest
 
+@typing_extensions.final
 class GetComputationResultResponse(google.protobuf.message.Message):
     """*
     the message of GetComputationResultResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     COLUMN_NUMBER_FIELD_NUMBER: builtins.int
-    STATUS_FIELD_NUMBER: builtins.int
     PIECE_ID_FIELD_NUMBER: builtins.int
-    PROGRESS_FIELD_NUMBER: builtins.int
     IS_DIM1_FIELD_NUMBER: builtins.int
     IS_DIM2_FIELD_NUMBER: builtins.int
     IS_SCHEMA_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     column_number: builtins.int
-    status: common_types.common_types_pb2.JobStatus.ValueType
     piece_id: builtins.int
-    @property
-    def progress(self) -> common_types.common_types_pb2.JobProgress: ...
     is_dim1: builtins.bool
     is_dim2: builtins.bool
     is_schema: builtins.bool
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[builtins.str] | None = ...,
         column_number: builtins.int = ...,
-        status: common_types.common_types_pb2.JobStatus.ValueType = ...,
         piece_id: builtins.int = ...,
-        progress: common_types.common_types_pb2.JobProgress | None = ...,
         is_dim1: builtins.bool = ...,
         is_dim2: builtins.bool = ...,
         is_schema: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_schema", b"is_schema", "progress", b"progress", "result_type", b"result_type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "column_number", b"column_number", "is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_schema", b"is_schema", "piece_id", b"piece_id", "progress", b"progress", "result", b"result", "result_type", b"result_type", "status", b"status"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_progress", b"_progress"]) -> typing_extensions.Literal["progress"] | None: ...
-    @typing.overload
+    def HasField(self, field_name: typing_extensions.Literal["is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_schema", b"is_schema", "result_type", b"result_type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["column_number", b"column_number", "is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_schema", b"is_schema", "piece_id", b"piece_id", "result", b"result", "result_type", b"result_type"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["result_type", b"result_type"]) -> typing_extensions.Literal["is_dim1", "is_dim2", "is_schema"] | None: ...
 
 global___GetComputationResultResponse = GetComputationResultResponse
 
-class GetDataListRequest(google.protobuf.message.Message):
+@typing_extensions.final
+class GetComputationStatusResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TOKEN_FIELD_NUMBER: builtins.int
-    token: builtins.str
-    def __init__(
-        self,
-        *,
-        token: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["token", b"token"]) -> None: ...
-
-global___GetDataListRequest = GetDataListRequest
-
-class GetDataListResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    RESULT_FIELD_NUMBER: builtins.int
-    result: builtins.str
+    STATUS_FIELD_NUMBER: builtins.int
+    PROGRESS_FIELD_NUMBER: builtins.int
+    status: common_types.common_types_pb2.JobStatus.ValueType
+    @property
+    def progress(self) -> common_types.common_types_pb2.JobProgress: ...
     def __init__(
         self,
         *,
-        result: builtins.str = ...,
+        status: common_types.common_types_pb2.JobStatus.ValueType = ...,
+        progress: common_types.common_types_pb2.JobProgress | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "progress", b"progress"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "progress", b"progress", "status", b"status"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_progress", b"_progress"]) -> typing_extensions.Literal["progress"] | None: ...
 
-global___GetDataListResponse = GetDataListResponse
+global___GetComputationStatusResponse = GetComputationStatusResponse
 
+@typing_extensions.final
 class GetElapsedTimeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     job_uuid: builtins.str
     token: builtins.str
@@ -310,54 +303,75 @@
         job_uuid: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
 
 global___GetElapsedTimeRequest = GetElapsedTimeRequest
 
+@typing_extensions.final
 class GetElapsedTimeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ELAPSED_TIME_FIELD_NUMBER: builtins.int
     elapsed_time: builtins.float
     def __init__(
         self,
         *,
         elapsed_time: builtins.float = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["elapsed_time", b"elapsed_time"]) -> None: ...
 
 global___GetElapsedTimeResponse = GetElapsedTimeResponse
 
-class GetJobErrorInfoRequest(google.protobuf.message.Message):
+@typing_extensions.final
+class GetJobErrorInfoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOB_UUID_FIELD_NUMBER: builtins.int
+    JOB_ERROR_INFO_FIELD_NUMBER: builtins.int
+    @property
+    def job_error_info(self) -> common_types.common_types_pb2.JobErrorInfo: ...
+    def __init__(
+        self,
+        *,
+        job_error_info: common_types.common_types_pb2.JobErrorInfo | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "job_error_info", b"job_error_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "job_error_info", b"job_error_info"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_job_error_info", b"_job_error_info"]) -> typing_extensions.Literal["job_error_info"] | None: ...
+
+global___GetJobErrorInfoResponse = GetJobErrorInfoResponse
+
+@typing_extensions.final
+class AddShareDataFrameRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    BASE_DATA_ID_FIELD_NUMBER: builtins.int
+    ADD_DATA_ID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
-    job_uuid: builtins.str
+    base_data_id: builtins.str
+    add_data_id: builtins.str
     token: builtins.str
     def __init__(
         self,
         *,
-        job_uuid: builtins.str = ...,
+        base_data_id: builtins.str = ...,
+        add_data_id: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["add_data_id", b"add_data_id", "base_data_id", b"base_data_id", "token", b"token"]) -> None: ...
 
-global___GetJobErrorInfoRequest = GetJobErrorInfoRequest
+global___AddShareDataFrameRequest = AddShareDataFrameRequest
 
-class GetJobErrorInfoResponse(google.protobuf.message.Message):
+@typing_extensions.final
+class AddShareDataFrameResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    JOB_ERROR_INFO_FIELD_NUMBER: builtins.int
-    @property
-    def job_error_info(self) -> common_types.common_types_pb2.JobErrorInfo: ...
+    DATA_ID_FIELD_NUMBER: builtins.int
+    data_id: builtins.str
     def __init__(
         self,
         *,
-        job_error_info: common_types.common_types_pb2.JobErrorInfo | None = ...,
+        data_id: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "job_error_info", b"job_error_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "job_error_info", b"job_error_info"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_job_error_info", b"_job_error_info"]) -> typing_extensions.Literal["job_error_info"] | None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["data_id", b"data_id"]) -> None: ...
 
-global___GetJobErrorInfoResponse = GetJobErrorInfoResponse
+global___AddShareDataFrameResponse = AddShareDataFrameResponse
```

### Comparing `quickmpc-0.4.2/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,31 +35,36 @@
         self.ExecuteComputation = channel.unary_unary(
             '/libctomanage.LibcToManage/ExecuteComputation',
             request_serializer=libc__to__manage__pb2.ExecuteComputationRequest.SerializeToString,
             response_deserializer=libc__to__manage__pb2.ExecuteComputationResponse.FromString,
         )
         self.GetComputationResult = channel.unary_stream(
             '/libctomanage.LibcToManage/GetComputationResult',
-            request_serializer=libc__to__manage__pb2.GetComputationResultRequest.SerializeToString,
+            request_serializer=libc__to__manage__pb2.GetComputationRequest.SerializeToString,
             response_deserializer=libc__to__manage__pb2.GetComputationResultResponse.FromString,
         )
-        self.GetDataList = channel.unary_unary(
-            '/libctomanage.LibcToManage/GetDataList',
-            request_serializer=libc__to__manage__pb2.GetDataListRequest.SerializeToString,
-            response_deserializer=libc__to__manage__pb2.GetDataListResponse.FromString,
+        self.GetComputationStatus = channel.unary_unary(
+            '/libctomanage.LibcToManage/GetComputationStatus',
+            request_serializer=libc__to__manage__pb2.GetComputationRequest.SerializeToString,
+            response_deserializer=libc__to__manage__pb2.GetComputationStatusResponse.FromString,
+        )
+        self.GetJobErrorInfo = channel.unary_unary(
+            '/libctomanage.LibcToManage/GetJobErrorInfo',
+            request_serializer=libc__to__manage__pb2.GetComputationRequest.SerializeToString,
+            response_deserializer=libc__to__manage__pb2.GetJobErrorInfoResponse.FromString,
         )
         self.GetElapsedTime = channel.unary_unary(
             '/libctomanage.LibcToManage/GetElapsedTime',
             request_serializer=libc__to__manage__pb2.GetElapsedTimeRequest.SerializeToString,
             response_deserializer=libc__to__manage__pb2.GetElapsedTimeResponse.FromString,
         )
-        self.GetJobErrorInfo = channel.unary_unary(
-            '/libctomanage.LibcToManage/GetJobErrorInfo',
-            request_serializer=libc__to__manage__pb2.GetJobErrorInfoRequest.SerializeToString,
-            response_deserializer=libc__to__manage__pb2.GetJobErrorInfoResponse.FromString,
+        self.AddShareDataFrame = channel.unary_unary(
+            '/libctomanage.LibcToManage/AddShareDataFrame',
+            request_serializer=libc__to__manage__pb2.AddShareDataFrameRequest.SerializeToString,
+            response_deserializer=libc__to__manage__pb2.AddShareDataFrameResponse.FromString,
         )
 
 
 class LibcToManageServicer(object):
     """*
     LibcToManage service
     """
@@ -90,27 +95,33 @@
 
     def GetComputationResult(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetDataList(self, request, context):
+    def GetComputationStatus(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetJobErrorInfo(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetElapsedTime(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetJobErrorInfo(self, request, context):
+    def AddShareDataFrame(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_LibcToManageServicer_to_server(servicer, server):
@@ -133,31 +144,36 @@
         'ExecuteComputation': grpc.unary_unary_rpc_method_handler(
             servicer.ExecuteComputation,
             request_deserializer=libc__to__manage__pb2.ExecuteComputationRequest.FromString,
             response_serializer=libc__to__manage__pb2.ExecuteComputationResponse.SerializeToString,
         ),
         'GetComputationResult': grpc.unary_stream_rpc_method_handler(
             servicer.GetComputationResult,
-            request_deserializer=libc__to__manage__pb2.GetComputationResultRequest.FromString,
+            request_deserializer=libc__to__manage__pb2.GetComputationRequest.FromString,
             response_serializer=libc__to__manage__pb2.GetComputationResultResponse.SerializeToString,
         ),
-        'GetDataList': grpc.unary_unary_rpc_method_handler(
-            servicer.GetDataList,
-            request_deserializer=libc__to__manage__pb2.GetDataListRequest.FromString,
-            response_serializer=libc__to__manage__pb2.GetDataListResponse.SerializeToString,
+        'GetComputationStatus': grpc.unary_unary_rpc_method_handler(
+            servicer.GetComputationStatus,
+            request_deserializer=libc__to__manage__pb2.GetComputationRequest.FromString,
+            response_serializer=libc__to__manage__pb2.GetComputationStatusResponse.SerializeToString,
+        ),
+        'GetJobErrorInfo': grpc.unary_unary_rpc_method_handler(
+            servicer.GetJobErrorInfo,
+            request_deserializer=libc__to__manage__pb2.GetComputationRequest.FromString,
+            response_serializer=libc__to__manage__pb2.GetJobErrorInfoResponse.SerializeToString,
         ),
         'GetElapsedTime': grpc.unary_unary_rpc_method_handler(
             servicer.GetElapsedTime,
             request_deserializer=libc__to__manage__pb2.GetElapsedTimeRequest.FromString,
             response_serializer=libc__to__manage__pb2.GetElapsedTimeResponse.SerializeToString,
         ),
-        'GetJobErrorInfo': grpc.unary_unary_rpc_method_handler(
-            servicer.GetJobErrorInfo,
-            request_deserializer=libc__to__manage__pb2.GetJobErrorInfoRequest.FromString,
-            response_serializer=libc__to__manage__pb2.GetJobErrorInfoResponse.SerializeToString,
+        'AddShareDataFrame': grpc.unary_unary_rpc_method_handler(
+            servicer.AddShareDataFrame,
+            request_deserializer=libc__to__manage__pb2.AddShareDataFrameRequest.FromString,
+            response_serializer=libc__to__manage__pb2.AddShareDataFrameResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         'libctomanage.LibcToManage', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
@@ -244,33 +260,50 @@
                              call_credentials=None,
                              insecure=False,
                              compression=None,
                              wait_for_ready=None,
                              timeout=None,
                              metadata=None):
         return grpc.experimental.unary_stream(request, target, '/libctomanage.LibcToManage/GetComputationResult',
-                                              libc__to__manage__pb2.GetComputationResultRequest.SerializeToString,
+                                              libc__to__manage__pb2.GetComputationRequest.SerializeToString,
                                               libc__to__manage__pb2.GetComputationResultResponse.FromString,
                                               options, channel_credentials,
                                               insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetDataList(request,
-                    target,
-                    options=(),
-                    channel_credentials=None,
-                    call_credentials=None,
-                    insecure=False,
-                    compression=None,
-                    wait_for_ready=None,
-                    timeout=None,
-                    metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/libctomanage.LibcToManage/GetDataList',
-                                             libc__to__manage__pb2.GetDataListRequest.SerializeToString,
-                                             libc__to__manage__pb2.GetDataListResponse.FromString,
+    def GetComputationStatus(request,
+                             target,
+                             options=(),
+                             channel_credentials=None,
+                             call_credentials=None,
+                             insecure=False,
+                             compression=None,
+                             wait_for_ready=None,
+                             timeout=None,
+                             metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/libctomanage.LibcToManage/GetComputationStatus',
+                                             libc__to__manage__pb2.GetComputationRequest.SerializeToString,
+                                             libc__to__manage__pb2.GetComputationStatusResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetJobErrorInfo(request,
+                        target,
+                        options=(),
+                        channel_credentials=None,
+                        call_credentials=None,
+                        insecure=False,
+                        compression=None,
+                        wait_for_ready=None,
+                        timeout=None,
+                        metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/libctomanage.LibcToManage/GetJobErrorInfo',
+                                             libc__to__manage__pb2.GetComputationRequest.SerializeToString,
+                                             libc__to__manage__pb2.GetJobErrorInfoResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetElapsedTime(request,
                        target,
                        options=(),
@@ -284,22 +317,22 @@
         return grpc.experimental.unary_unary(request, target, '/libctomanage.LibcToManage/GetElapsedTime',
                                              libc__to__manage__pb2.GetElapsedTimeRequest.SerializeToString,
                                              libc__to__manage__pb2.GetElapsedTimeResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetJobErrorInfo(request,
-                        target,
-                        options=(),
-                        channel_credentials=None,
-                        call_credentials=None,
-                        insecure=False,
-                        compression=None,
-                        wait_for_ready=None,
-                        timeout=None,
-                        metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/libctomanage.LibcToManage/GetJobErrorInfo',
-                                             libc__to__manage__pb2.GetJobErrorInfoRequest.SerializeToString,
-                                             libc__to__manage__pb2.GetJobErrorInfoResponse.FromString,
+    def AddShareDataFrame(request,
+                          target,
+                          options=(),
+                          channel_credentials=None,
+                          call_credentials=None,
+                          insecure=False,
+                          compression=None,
+                          wait_for_ready=None,
+                          timeout=None,
+                          metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/libctomanage.LibcToManage/AddShareDataFrame',
+                                             libc__to__manage__pb2.AddShareDataFrameRequest.SerializeToString,
+                                             libc__to__manage__pb2.AddShareDataFrameResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `quickmpc-0.4.2/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -27,28 +27,32 @@
         libc_to_manage_pb2.GetSchemaResponse,
     ]
     ExecuteComputation: grpc.UnaryUnaryMultiCallable[
         libc_to_manage_pb2.ExecuteComputationRequest,
         libc_to_manage_pb2.ExecuteComputationResponse,
     ]
     GetComputationResult: grpc.UnaryStreamMultiCallable[
-        libc_to_manage_pb2.GetComputationResultRequest,
+        libc_to_manage_pb2.GetComputationRequest,
         libc_to_manage_pb2.GetComputationResultResponse,
     ]
-    GetDataList: grpc.UnaryUnaryMultiCallable[
-        libc_to_manage_pb2.GetDataListRequest,
-        libc_to_manage_pb2.GetDataListResponse,
+    GetComputationStatus: grpc.UnaryUnaryMultiCallable[
+        libc_to_manage_pb2.GetComputationRequest,
+        libc_to_manage_pb2.GetComputationStatusResponse,
+    ]
+    GetJobErrorInfo: grpc.UnaryUnaryMultiCallable[
+        libc_to_manage_pb2.GetComputationRequest,
+        libc_to_manage_pb2.GetJobErrorInfoResponse,
     ]
     GetElapsedTime: grpc.UnaryUnaryMultiCallable[
         libc_to_manage_pb2.GetElapsedTimeRequest,
         libc_to_manage_pb2.GetElapsedTimeResponse,
     ]
-    GetJobErrorInfo: grpc.UnaryUnaryMultiCallable[
-        libc_to_manage_pb2.GetJobErrorInfoRequest,
-        libc_to_manage_pb2.GetJobErrorInfoResponse,
+    AddShareDataFrame: grpc.UnaryUnaryMultiCallable[
+        libc_to_manage_pb2.AddShareDataFrameRequest,
+        libc_to_manage_pb2.AddShareDataFrameResponse,
     ]
 
 class LibcToManageServicer(metaclass=abc.ABCMeta):
     """*
     LibcToManage service
     """
 
@@ -75,30 +79,36 @@
         self,
         request: libc_to_manage_pb2.ExecuteComputationRequest,
         context: grpc.ServicerContext,
     ) -> libc_to_manage_pb2.ExecuteComputationResponse: ...
     @abc.abstractmethod
     def GetComputationResult(
         self,
-        request: libc_to_manage_pb2.GetComputationResultRequest,
+        request: libc_to_manage_pb2.GetComputationRequest,
         context: grpc.ServicerContext,
     ) -> collections.abc.Iterator[libc_to_manage_pb2.GetComputationResultResponse]: ...
     @abc.abstractmethod
-    def GetDataList(
+    def GetComputationStatus(
+        self,
+        request: libc_to_manage_pb2.GetComputationRequest,
+        context: grpc.ServicerContext,
+    ) -> libc_to_manage_pb2.GetComputationStatusResponse: ...
+    @abc.abstractmethod
+    def GetJobErrorInfo(
         self,
-        request: libc_to_manage_pb2.GetDataListRequest,
+        request: libc_to_manage_pb2.GetComputationRequest,
         context: grpc.ServicerContext,
-    ) -> libc_to_manage_pb2.GetDataListResponse: ...
+    ) -> libc_to_manage_pb2.GetJobErrorInfoResponse: ...
     @abc.abstractmethod
     def GetElapsedTime(
         self,
         request: libc_to_manage_pb2.GetElapsedTimeRequest,
         context: grpc.ServicerContext,
     ) -> libc_to_manage_pb2.GetElapsedTimeResponse: ...
     @abc.abstractmethod
-    def GetJobErrorInfo(
+    def AddShareDataFrame(
         self,
-        request: libc_to_manage_pb2.GetJobErrorInfoRequest,
+        request: libc_to_manage_pb2.AddShareDataFrameRequest,
         context: grpc.ServicerContext,
-    ) -> libc_to_manage_pb2.GetJobErrorInfoResponse: ...
+    ) -> libc_to_manage_pb2.AddShareDataFrameResponse: ...
 
 def add_LibcToManageServicer_to_server(servicer: LibcToManageServicer, server: grpc.Server) -> None: ...
```

### Comparing `quickmpc-0.4.2/quickmpc/qmpc_server.py` & `quickmpc-0.5.0/quickmpc/request/qmpc_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,98 +4,116 @@
 import json
 import logging
 import os
 import struct
 import time
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass, field, InitVar
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple
 from urllib.parse import urlparse
 
 import google.protobuf.json_format
 import grpc
 import numpy as np
+import pandas as pd
 import tqdm  # type: ignore
 from grpc_status import rpc_status  # type: ignore
 
-from .exception import ArgumentError, QMPCJobError, QMPCServerError
-from .proto.common_types.common_types_pb2 import (JobErrorInfo, JobStatus,
-                                                  Schema, ShareValueTypeEnum)
-from .proto.libc_to_manage_pb2 import (DeleteSharesRequest,
-                                       ExecuteComputationRequest,
-                                       GetComputationResultRequest,
-                                       GetComputationResultResponse,
-                                       GetDataListRequest,
-                                       GetElapsedTimeRequest,
-                                       GetJobErrorInfoRequest, Input,
-                                       JoinOrder, SendSharesRequest)
-from .proto.libc_to_manage_pb2_grpc import LibcToManageStub
-from .share import Share
-from .utils.if_present import if_present
-from .utils.make_pieces import MakePiece
-from .utils.overload_tools import Dim1, Dim2, Dim3, methoddispatch
-from .utils.parse_csv import format_check
-
-abs_file = os.path.abspath(__file__)
-base_dir = os.path.dirname(abs_file)
+import quickmpc.pandas as qpd
+from quickmpc.exception import ArgumentError, QMPCJobError, QMPCServerError
+from quickmpc.proto.common_types.common_types_pb2 import (ComputationMethod,
+                                                          JobErrorInfo, Schema)
+from quickmpc.proto.libc_to_manage_pb2 import (AddShareDataFrameRequest,
+                                               DeleteSharesRequest,
+                                               ExecuteComputationRequest,
+                                               GetComputationRequest,
+                                               GetComputationResultResponse,
+                                               GetElapsedTimeRequest, Input,
+                                               JoinOrder, SendSharesRequest)
+from quickmpc.proto.libc_to_manage_pb2_grpc import LibcToManageStub
+from quickmpc.request.qmpc_request_interface import QMPCRequestInterface
+from quickmpc.request.response import (AddShareDataFrameResponse,
+                                       ExecuteResponse,
+                                       GetComputationStatusResponse,
+                                       GetElapsedTimeResponse,
+                                       GetJobErrorInfoResponse,
+                                       GetResultResponse, SendShareResponse)
+from quickmpc.share import Share
+from quickmpc.utils import if_present, MakePiece
 
 logger = logging.getLogger(__name__)
 
 
+def _create_grpc_channel(endpoint: str) -> grpc.Channel:
+    channel: grpc.Channel = None
+    o = urlparse(endpoint)
+    if o.scheme == 'http':
+        # insecureなchannelを作成
+        channel = grpc.insecure_channel(o.netloc)
+    elif o.scheme == 'https':
+        # secureなchannelを作成
+        credential: grpc.ChannelCredentials \
+            = grpc.ssl_channel_credentials()
+        channel = grpc.secure_channel(o.netloc, credential)
+    else:
+        logger.error(f'仕様を満たさない形式のendpointが渡された: {endpoint}')
+        raise ArgumentError(
+            "endpointsにサポートされてないプロトコルが指定されています．http/httpsのいずれかを指定してください．")
+
+    return channel
+
+
 @dataclass(frozen=True)
-class QMPCServer:
+class QMPCRequest(QMPCRequestInterface):
+    """QuickMPCサーバと通信を行う
+
+    Attributes
+    ----------
+    __endpoints: List[url]
+        QuickMPCサーバのURL
+    __token: str
+        QuickMPCサーバへの通信を担う
+    """
+
     endpoints: InitVar[List[str]]
+
     __client_stubs: Tuple[LibcToManageStub] = field(init=False)
     __client_channels: Tuple[grpc.Channel] = field(init=False)
     __party_size: int = field(init=False)
-    token: str
-    retry_num: int = 10
-    retry_wait_time: int = 5
+    __token: str = field(init=False)
+    # TODO: retry manager的なのを作る
+    __retry_num: int = 10
+    __retry_wait_time: int = 5
 
     def __post_init__(self, endpoints: List[str]) -> None:
-        chs = [QMPCServer.__create_grpc_channel(ep) for ep in endpoints]
+        chs = [_create_grpc_channel(ep) for ep in endpoints]
         stubs = [LibcToManageStub(ch) for ch in chs]
-        object.__setattr__(self, "_QMPCServer__client_channels", chs)
-        object.__setattr__(self, "_QMPCServer__client_stubs", stubs)
-        object.__setattr__(self, "_QMPCServer__party_size", len(endpoints))
-
-    @staticmethod
-    def __create_grpc_channel(endpoint: str) -> grpc.Channel:
-        channel: grpc.Channel = None
-        o = urlparse(endpoint)
-        if o.scheme == 'http':
-            # insecureなchannelを作成
-            channel = grpc.insecure_channel(o.netloc)
-        elif o.scheme == 'https':
-            # secureなchannelを作成
-            credential: grpc.ChannelCredentials \
-                = grpc.ssl_channel_credentials()
-            channel = grpc.secure_channel(o.netloc, credential)
-        else:
-            logger.error(f'仕様を満たさない形式のendpointが渡された: {endpoint}')
-            raise ArgumentError(
-                "endpointsにサポートされてないプロトコルが指定されています．http/httpsのいずれかを指定してください．")
-
-        return channel
+        object.__setattr__(self, "_QMPCRequest__client_channels", chs)
+        object.__setattr__(self, "_QMPCRequest__client_stubs", stubs)
+        object.__setattr__(self, "_QMPCRequest__party_size", len(endpoints))
+        token = os.environ["QMPC_TOKEN"] \
+            if "QMPC_TOKEN" in os.environ else "token_demo"
+        object.__setattr__(self, "_QMPCRequest__token", token)
 
     def __retry(self, f: Callable, *request: Any) -> Any:
         for ch in self.__client_channels:
             # channelの接続チェック
             is_channel_ready = False
-            for _ in range(self.retry_num):
+            for _ in range(self.__retry_num):
                 try:
-                    grpc.channel_ready_future(ch).result(self.retry_wait_time)
+                    grpc.channel_ready_future(ch).result(
+                        self.__retry_wait_time)
                     is_channel_ready = True
                     break
                 except grpc.FutureTimeoutError as e:
                     logger.error(e)
             if not is_channel_ready:
-                raise RuntimeError("channel の準備が出来ません")
+                raise QMPCServerError("channel の準備が出来ません")
 
-        for _ in range(self.retry_num):
+        for _ in range(self.__retry_num):
             # requestを送る
             try:
                 return f(*request)
             except grpc.RpcError as e:
                 logger.error(f'{e.details()} ({e.code()})')
 
                 # エラーが詳細な情報を持っているか確認
@@ -115,253 +133,197 @@
 
                 # MC で Internal Server Error が発生している場合
                 # 例外を rethrow する
                 if e.code() == grpc.StatusCode.UNKNOWN:
                     raise QMPCServerError("backend server return error") from e
             except Exception as e:
                 logger.error(e)
-            time.sleep(self.retry_wait_time)
-        raise RuntimeError(f"All {self.retry_num} times it was an error")
+            time.sleep(self.__retry_wait_time)
+        raise QMPCServerError(f"All {self.__retry_num} times it was an error")
 
     @staticmethod
     def __futures_result(
-            futures: Iterable, enable_progress_bar=True) -> Tuple[bool, List]:
+            futures: Iterable, enable_progress_bar=True) -> List:
         """ エラーチェックしてfutureのresultを得る """
-        is_ok: bool = True
-        response: List = []
         try:
             if enable_progress_bar:
                 futures = tqdm.tqdm(futures, desc='receive')
             response = [f.result() for f in futures]
-        except (QMPCJobError, QMPCServerError):
+        except Exception:
             raise
-        except Exception as e:
-            is_ok = False
-            logger.error(e)
-
-        return is_ok, response
-
-    @staticmethod
-    def __stream_result(stream: Iterable, job_uuid: str, party: int,
-                        path: Optional[str]) -> Dict:
-        """ エラーチェックしてstreamのresultを得る """
-        is_ok: bool = True
-        res_list = []
-        for res in stream:
-            if path and res.status == JobStatus.Value('COMPLETED'):
-                file_title = "dim1"
-                if res.HasField("is_dim2"):
-                    file_title = "dim2"
-                elif res.HasField("is_schema"):
-                    file_title = "schema"
-
-                file_path = f"{path}/" + \
-                    f"{file_title}-{job_uuid}-{party}-{res.piece_id}.csv"
-
-                with open(file_path, 'w') as f:
-                    writer = csv.writer(f)
-                    writer.writerow([res.column_number])
-                    writer.writerow(res.result)
-                progress = res.progress if res.HasField('progress') else None
-                res = GetComputationResultResponse(
-                    column_number=res.column_number,
-                    status=res.status,
-                    piece_id=res.piece_id,
-                    progress=progress,
-                )
-            res_list.append(res)
-        res_dict: Dict = {"is_ok": is_ok, "responses": res_list}
-        return res_dict
-
-    @methoddispatch(is_static_method=True)
-    @staticmethod
-    def __convert_schema(_):
-        raise ArgumentError("不正な引数が与えられています．")
-
-    @__convert_schema.register(Dim1)
-    @staticmethod
-    def __convert_schema_dummy(schema: List):
-        raise ArgumentError("不正な引数が与えられています．")
-
-    @__convert_schema.register((Dim1, str))
-    @staticmethod
-    def __convert_schema_str(schema: List[str]) -> List[Schema]:
-        return [
-            Schema(name=name,
-                   type=ShareValueTypeEnum.SHARE_VALUE_TYPE_FIXED_POINT)
-            for name in schema]
+        return response
 
-    @__convert_schema.register((Dim1, Schema))
-    @staticmethod
-    def __convert_schema_typed(
-            schema: List[Schema]) -> List[Schema]:
-        return schema
-
-    @methoddispatch()
-    def send_share(self, _):
-        raise ArgumentError("不正な引数が与えられています．")
-
-    @send_share.register(Dim2)
-    @send_share.register(Dim3)
-    def __send_share_impl(self, secrets: List,
-                          schema: List[Union[str, Schema]],
-                          matching_column: int,
-                          piece_size: int) -> Dict:
+    def send_share(self, df: pd.DataFrame, piece_size: int = 1_000_000) \
+            -> SendShareResponse:
+        """ Shareをコンテナに送信 """
         if piece_size < 1000 or piece_size > 1_000_000:
             raise RuntimeError(
                 "piece_size must be in the range of 1000 to 1000000")
-
-        if matching_column <= 0 or matching_column > len(schema):
-            raise RuntimeError(
-                "matching_column must be in the "
-                "range of 1 to the size of schema")
-
-        typed_schema: List[Schema] = QMPCServer.__convert_schema(schema)
-
-        # TODO parse_csv経由でsend_shareをすると同じチェックをすることになる．
-        if not format_check(secrets, schema):
+        if df.isnull().values.sum() != 0:
             raise RuntimeError("規定されたフォーマットでないデータです．")
+        sort_index_name = "__qmpc_sort_index__"
+        if sort_index_name not in df.columns:
+            raise RuntimeError("規定されたフォーマットでないデータです．"
+                               "quickmpc.pandas.read_csvで読み込んだデータか，"
+                               f"columnsに{sort_index_name}が含まれたデータ"
+                               "でなければならないです．")
+
+        # TODO: 無駄に一度tableを再構成しているのでparse関数を書き直す
+        df = df.sort_values(by=sort_index_name)
+        df = df.drop(sort_index_name, axis=1)
+        table = [df.columns.values.tolist()] + \
+                [row.tolist() for row in df.values]
+        secrets, schema = qpd.parse(table, matching_column=1)
 
-        """ Shareをコンテナに送信 """
-        sorted_secrets = sorted(
-            secrets, key=lambda row: row[matching_column - 1])
         # pieceに分けてシェア化
         pieces: list = MakePiece.make_pieces(
-            sorted_secrets, int(piece_size / 10))
+            secrets, int(piece_size / 10))
         data_id: str = hashlib.sha256(
-            str(sorted_secrets).encode() + struct.pack('d', time.time())
+            str(secrets).encode() + struct.pack('d', time.time())
         ).hexdigest()
 
         # リクエストパラメータを設定して非同期にリクエスト送信
         sent_at = str(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
         futures: list = []
         with ThreadPoolExecutor() as executor:
             for piece_id, p in enumerate(tqdm.tqdm(pieces, desc='sharize')):
                 shares = Share.sharize(p, self.__party_size)
                 for stub, s in zip(self.__client_stubs, shares):
                     req = SendSharesRequest(data_id=data_id,
                                             shares=json.dumps(s),
-                                            schema=typed_schema,
+                                            schema=schema,
                                             piece_id=piece_id,
                                             sent_at=sent_at,
-                                            matching_column=matching_column,
-                                            token=self.token)
+                                            matching_column=1,
+                                            token=self.__token)
                     futures.append(executor.submit(self.__retry,
                                                    stub.SendShares,
                                                    req))
-        is_ok, _ = QMPCServer.__futures_result(futures)
-        return {"is_ok": is_ok, "data_id": data_id}
+        QMPCRequest.__futures_result(futures)
+        return SendShareResponse(data_id)
 
-    def delete_share(self, data_ids: List[str]) -> Dict:
-        """ Shareを削除 """
-        req = DeleteSharesRequest(dataIds=data_ids, token=self.token)
-        # 非同期にリクエスト送信
-        with ThreadPoolExecutor() as executor:
-            futures = [executor.submit(self.__retry, stub.DeleteShares, req)
-                       for stub in self.__client_stubs]
-        is_ok, _ = QMPCServer.__futures_result(futures)
-        return {"is_ok": is_ok}
-
-    def execute_computation(self, method_id: int,
-                            data_ids: List[str],
-                            inp: Tuple[List, List],
-                            *, debug_mode: bool = False) -> Dict:
+    def __execute_computation(self, method_id: ComputationMethod.ValueType,
+                              data_ids: List[str],
+                              columns: Tuple[List, List],
+                              *, debug_mode: bool = False)  \
+            -> ExecuteResponse:
         """ 計算リクエストを送信 """
-        join_order_req = JoinOrder(
-            data_ids=data_ids,
-            debug_mode=debug_mode)
-        input_req = Input(
-            src=inp[0],
-            target=inp[1])
         req = ExecuteComputationRequest(
             method_id=method_id,
-            token=self.token,
-            table=join_order_req,
-            arg=input_req,
+            token=self.__token,
+            table=JoinOrder(data_ids=data_ids,
+                            debug_mode=debug_mode),
+            arg=Input(src=columns[0],
+                      target=columns[1]),
         )
 
         # 非同期にリクエスト送信
         with ThreadPoolExecutor() as executor:
             # JobidをMCから貰う関係で単一MC（現在はSP（ID=0）のみ対応）にリクエストを送る
             futures = [
                 executor.submit(self.__retry,
                                 self.__client_stubs[0].ExecuteComputation,
                                 req)]
 
-        is_ok, response = QMPCServer.__futures_result(futures)
-        job_uuid = response[0].job_uuid if is_ok else None
+        response = QMPCRequest.__futures_result(futures)
+        return ExecuteResponse(response[0].job_uuid)
 
-        return {"is_ok": is_ok, "job_uuid": job_uuid}
+    def sum(self, data_ids: List[str], columns: List[int],
+            *, debug_mode: bool = False) -> ExecuteResponse:
+        return self.__execute_computation(
+            ComputationMethod.COMPUTATION_METHOD_SUM,
+            data_ids, (columns, []), debug_mode=debug_mode)
+
+    def mean(self, data_ids: List[str], columns: List[int],
+             *, debug_mode: bool = False) -> ExecuteResponse:
+        return self.__execute_computation(
+            ComputationMethod.COMPUTATION_METHOD_MEAN,
+            data_ids, (columns, []), debug_mode=debug_mode)
+
+    def variance(self, data_ids: List[str], columns: List[int],
+                 *, debug_mode: bool = False) \
+            -> ExecuteResponse:
+        return self.__execute_computation(
+            ComputationMethod.COMPUTATION_METHOD_VARIANCE,
+            data_ids, (columns, []), debug_mode=debug_mode)
+
+    def correl(self, data_ids: List[str], inp1: List[int], inp2: List[int],
+               *, debug_mode: bool = False) \
+            -> ExecuteResponse:
+        return self.__execute_computation(
+            ComputationMethod.COMPUTATION_METHOD_CORREL,
+            data_ids, (inp1, inp2), debug_mode=debug_mode)
+
+    def meshcode(self, data_ids: List[str], inp1: List[int],
+                 *, debug_mode: bool = False) \
+            -> ExecuteResponse:
+        return self.__execute_computation(
+            ComputationMethod.COMPUTATION_METHOD_MESH_CODE,
+            data_ids, (inp1, []), debug_mode=debug_mode)
+
+    def join(self, data_ids: List[str],
+             *, debug_mode: bool = False) -> ExecuteResponse:
+        return self.__execute_computation(
+            ComputationMethod.COMPUTATION_METHOD_JOIN_TABLE,
+            data_ids, ([], []), debug_mode=debug_mode)
 
-    def get_data_list(self) -> Dict:
-        # 非同期にリクエスト送信
-        with ThreadPoolExecutor() as executor:
-            futures = [executor.submit(self.__retry,
-                                       stub.GetDataList,
-                                       GetDataListRequest(token=self.token))
-                       for stub in self.__client_stubs]
-        is_ok, response = QMPCServer.__futures_result(futures)
-        results = [eval(r.result) for r in response] if is_ok else None
+    @staticmethod
+    def __stream_result(stream: Iterable, job_uuid: str, party: int,
+                        output_path: Optional[str]) -> Dict:
+        """ エラーチェックしてstreamのresultを得る """
+        is_ok: bool = True
+        res_list = []
+        for res in stream:
+            if output_path:
+                file_title = "dim1"
+                if res.HasField("is_dim2"):
+                    file_title = "dim2"
+                elif res.HasField("is_schema"):
+                    file_title = "schema"
 
-        return {"is_ok": is_ok, "results": results}
+                file_path = f"{output_path }/" + \
+                    f"{file_title}-{job_uuid}-{party}-{res.piece_id}.csv"
 
-    def get_elapsed_time(self, job_uuid: str) -> Dict:
-        # リクエストパラメータを設定
-        req = GetElapsedTimeRequest(
-            job_uuid=job_uuid,
-            token=self.token
-        )
-        # 非同期にリクエスト送信
-        with ThreadPoolExecutor() as executor:
-            futures = [executor.submit(self.__retry,
-                                       stub.GetElapsedTime,
-                                       req)
-                       for stub in self.__client_stubs]
-        is_ok, response = QMPCServer.__futures_result(futures)
-        elapsed_time = max([res.elapsed_time
-                            for res in response]) if is_ok else None
-        return {"is_ok": is_ok, "elapsed_time": elapsed_time}
+                with open(file_path, 'w') as f:
+                    writer = csv.writer(f)
+                    writer.writerow([res.column_number])
+                    writer.writerow(res.result)
+                res = GetComputationResultResponse(
+                    column_number=res.column_number,
+                    piece_id=res.piece_id,
+                )
+            res_list.append(res)
+        res_dict: Dict = {"is_ok": is_ok, "responses": res_list}
+        return res_dict
 
     def get_computation_result(self, job_uuid: str,
-                               path: Optional[str]) -> Dict:
+                               output_path: Optional[str] = None) \
+            -> GetResultResponse:
         """ コンテナから結果を取得 """
         # リクエストパラメータを設定
-        req = GetComputationResultRequest(
+        req = GetComputationRequest(
             job_uuid=job_uuid,
-            token=self.token
+            token=self.__token
         )
         # 非同期にリクエスト送信
         with ThreadPoolExecutor() as executor:
             futures = [executor.submit(self.__retry,
-                                       QMPCServer.__stream_result,
+                                       QMPCRequest.__stream_result,
                                        stub.GetComputationResult(req),
-                                       job_uuid, party, path)
+                                       job_uuid, party, output_path)
                        for party, stub in enumerate(self.__client_stubs)]
-        is_ok, response = QMPCServer.__futures_result(
-            futures, enable_progress_bar=False)
+        response = QMPCRequest.__futures_result(futures,
+                                                enable_progress_bar=False)
         results_sorted = [sorted(res["responses"], key=lambda r: r.piece_id)
                           for res in response]
-        # NOTE: statusは0番目(piece_id=1)の要素にのみ含まれている
-        statuses = [res[0].status for res in results_sorted] \
-            if results_sorted else None
-        all_completed = all([
-            s == JobStatus.Value('COMPLETED') for s in statuses
-        ]) if statuses is not None else False
-
-        progresses = None
-        if results_sorted is not None:
-            progresses = [
-                res[0].progress if res[0].HasField("progress") else None
-                for res in results_sorted
-            ]
 
         results: Optional[Any] = None
         schema = None
         is_table = False
-        if not path and all_completed:
+        if not output_path:
             for res in results_sorted:
                 is_dim2 = False
                 column_number = 0
                 result: Any = []
                 schema_1p = []
                 for r in res:
                     if r.HasField("is_schema"):
@@ -388,31 +350,89 @@
                 result = Share.convert_type(result, schema)
                 if results is None:
                     results = []
                 results.append(result)
 
         results = if_present(results, Share.recons)
         results = if_present(results, Share.convert_type, schema)
-        if is_table:
-            results = {"schema": schema, "table": results}
-        return {"is_ok": is_ok, "statuses": statuses,
-                "results": results, "progresses": progresses}
+        if is_table and schema:
+            columns = [s.name for s in schema]
+            return GetResultResponse(pd.DataFrame(results, columns=columns))
+        return GetResultResponse(pd.DataFrame(results))
+
+    def get_computation_status(self, job_uuid: str) \
+            -> GetComputationStatusResponse:
+        # リクエストパラメータを設定
+        req = GetComputationRequest(
+            job_uuid=job_uuid,
+            token=self.__token
+        )
+        # 非同期にリクエスト送信
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry,
+                                       stub.GetComputationStatus,
+                                       req)
+                       for stub in self.__client_stubs]
+        response = QMPCRequest.__futures_result(futures,
+                                                enable_progress_bar=False)
+        statuses = [res.status for res in response]
+        progresses = [res.progress if res.HasField("progress") else None
+                      for res in response]
 
-    def get_job_error_info(self, job_uuid: str) -> Dict:
+        return GetComputationStatusResponse(statuses, progresses)
+
+    def get_job_error_info(self, job_uuid: str) -> GetJobErrorInfoResponse:
         # リクエストパラメータを設定
-        req = GetJobErrorInfoRequest(
+        req = GetComputationRequest(
             job_uuid=job_uuid,
-            token=self.token
+            token=self.__token
         )
         # 非同期にリクエスト送信
         with ThreadPoolExecutor() as executor:
             futures = [executor.submit(self.__retry, stub.GetJobErrorInfo, req)
                        for stub in self.__client_stubs]
-        is_ok, response = QMPCServer.__futures_result(
+        response = QMPCRequest.__futures_result(
             futures, enable_progress_bar=False)
 
         job_error_info = [
             res.job_error_info if res.HasField("job_error_info") else None
             for res in response
         ]
+        return GetJobErrorInfoResponse(job_error_info)
 
-        return {"is_ok": is_ok, "job_error_info": job_error_info}
+    def get_elapsed_time(self, job_uuid: str) -> GetElapsedTimeResponse:
+        # リクエストパラメータを設定
+        req = GetElapsedTimeRequest(
+            job_uuid=job_uuid,
+            token=self.__token
+        )
+        # 非同期にリクエスト送信
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry,
+                                       stub.GetElapsedTime,
+                                       req)
+                       for stub in self.__client_stubs]
+        response = QMPCRequest.__futures_result(futures)
+        elapsed_time = max([res.elapsed_time for res in response])
+        return GetElapsedTimeResponse(elapsed_time)
+
+    def delete_share(self, data_ids: List[str]) -> None:
+        req = DeleteSharesRequest(dataIds=data_ids, token=self.__token)
+        # 非同期にリクエスト送信
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry, stub.DeleteShares, req)
+                       for stub in self.__client_stubs]
+        QMPCRequest.__futures_result(futures)
+
+    def add_share_data_frame(self, base_data_id: str, add_data_id: str) \
+            -> AddShareDataFrameResponse:
+        req = AddShareDataFrameRequest(base_data_id=base_data_id,
+                                       add_data_id=add_data_id,
+                                       token=self.__token)
+        # 非同期にリクエスト送信
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(self.__retry,
+                                       stub.AddShareDataFrame, req)
+                       for stub in self.__client_stubs]
+        response = QMPCRequest.__futures_result(futures)
+        data_id = response[0].data_id
+        return AddShareDataFrameResponse(data_id)
```

### Comparing `quickmpc-0.4.2/quickmpc/restore.py` & `quickmpc-0.5.0/quickmpc/share/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import csv
 import glob
 from typing import Any
 
+import google.protobuf.json_format
 import numpy as np
 from natsort import natsorted
 
-import google.protobuf.json_format
-from .proto.common_types.common_types_pb2 import Schema
-from .share import Share
-from .utils.if_present import if_present
+from quickmpc.proto.common_types.common_types_pb2 import Schema
+from quickmpc.share.share import Share
+from quickmpc.utils import if_present
 
 
 def get_meta(job_uuid: str, path: str):
     file_name = glob.glob(f"{path}/dim?-{job_uuid}-*")[0]
     with open(file_name, 'r') as f:
         reader = csv.reader(f)
         # 1列目のデータを取得
```

### Comparing `quickmpc-0.4.2/quickmpc/share.py` & `quickmpc-0.5.0/quickmpc/share/share.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import logging
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import (Any, Callable, ClassVar, List,
                     Optional, Sequence, Tuple, Union)
 
 import numpy as np
 
-from .exception import ArgumentError
-from .proto.common_types.common_types_pb2 import Schema, ShareValueTypeEnum
-from .utils.overload_tools import (DictList, DictList2, Dim1,
-                                   Dim2, Dim3, methoddispatch)
-from .utils.random import ChaCha20, RandomInterface
+from quickmpc.exception import ArgumentError
+from quickmpc.proto.common_types.common_types_pb2 import (Schema,
+                                                          ShareValueTypeEnum)
+from quickmpc.qmpc_logging import get_logger
+from quickmpc.share.random import ChaCha20, RandomInterface
+from quickmpc.utils import (DictList, DictList2, Dim1,
+                            Dim2, Dim3, methoddispatch)
 
-logger = logging.getLogger(__name__)
+logger = get_logger()
 
 
 @dataclass(frozen=True)
 class Share:
     __share_random_range: ClassVar[Tuple[Decimal, Decimal]] =\
         (Decimal(-(1 << 64)), Decimal(1 << 64))
```

### Comparing `quickmpc-0.4.2/quickmpc/utils/make_pieces.py` & `quickmpc-0.5.0/quickmpc/utils/make_pieces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 import operator
 from dataclasses import dataclass
 from typing import List
 
-from ..exception import ArgumentError
-from .overload_tools import Dim1, Dim2, methoddispatch
+from quickmpc.exception import ArgumentError
+from quickmpc.utils.overload_tools import Dim1, Dim2, methoddispatch
 
 
 @dataclass(frozen=True)
 class MakePiece:
 
     @methoddispatch(is_static_method=True)
     @staticmethod
```

### Comparing `quickmpc-0.4.2/quickmpc/utils/overload_tools.py` & `quickmpc-0.5.0/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/quickmpc/utils/parse_csv.py` & `quickmpc-0.5.0/quickmpc/pandas/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import csv
-import logging
 from dataclasses import dataclass
 from hashlib import sha512
 from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
-from ..exception import ArgumentError
-from ..proto.common_types.common_types_pb2 import Schema, ShareValueTypeEnum
-from .overload_tools import Dim1, methoddispatch
+from quickmpc.exception import ArgumentError
+from quickmpc.proto.common_types.common_types_pb2 import (Schema,
+                                                          ShareValueTypeEnum)
+from quickmpc.qmpc_logging import get_logger
+from quickmpc.utils import Dim1, methoddispatch
+
+logger = get_logger()
 
-logger = logging.getLogger(__name__)
 
 SUPPORT_TAGS: Dict[str, ShareValueTypeEnum.ValueType] = {
     'id': ShareValueTypeEnum.Value('SHARE_VALUE_TYPE_FIXED_POINT'),
 }
 
 ShareValueType = Union[float, int]
```

### Comparing `quickmpc-0.4.2/quickmpc/utils/random.py` & `quickmpc-0.5.0/quickmpc/share/random.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import math
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import ClassVar, List
-import math
 
 from nacl.utils import random, randombytes_deterministic
 
-from ..exception import ArgumentError
-from .overload_tools import methoddispatch
+from quickmpc.exception import ArgumentError
+from quickmpc.utils import methoddispatch
 
 
 # 乱数生成のインタフェース
 class RandomInterface(ABC):
     @abstractmethod
     def get(self, a, b) -> int:
         ...
```

### Comparing `quickmpc-0.4.2/tests/unit_tests/conftest.py` & `quickmpc-0.5.0/tests/unit_tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 yieldのタイミングで全てのTestが開始
 """
 import glob
 import os
 
 import pytest
 
-from .local_server import serve
+from tests.unit_tests.local_server import serve
 
 
 @pytest.fixture(scope='session')
 def run_server1():
     """ run server """
     server = serve(1)
     server.start()
 
     """ test start """
     yield
 
     """ test end """
-    for file in glob.glob("./tests/unit_tests/dim1-uuid*"):
+    for file in glob.glob("./tests/unit_tests/dim1-*.csv"):
         os.remove(file)
 
     server.stop(0)
 
 
 @pytest.fixture(scope='session')
 def run_server2():
```

### Comparing `quickmpc-0.4.2/tests/unit_tests/local_server.py` & `quickmpc-0.5.0/tests/unit_tests/local_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,62 +44,70 @@
                 and request.table.data_ids[0] == "UnregisteredDataId":
             # QMPCServerError
             # MC で Internal Server Error が発生している場合を再現
             context.set_code(grpc.StatusCode.UNKNOWN)
             return libc_to_manage_pb2.ExecuteComputationResponse()
 
         res = libc_to_manage_pb2.ExecuteComputationResponse(
-            job_uuid="jobjobjob"
+            job_uuid="job_uuid"
         )
         return res
 
     def GetComputationResult(self, request, context):
         yield libc_to_manage_pb2.GetComputationResultResponse(
             result=["1"],
-            status=common_types_pb2.COMPLETED,
             piece_id=1,
             column_number=2,
             is_dim1=True,
         )
         yield libc_to_manage_pb2.GetComputationResultResponse(
             result=["2"],
-            status=common_types_pb2.COMPLETED,
             piece_id=2,
             column_number=2,
             is_dim1=True,
         )
 
-    def GetDataList(self, request, context):
-        res = libc_to_manage_pb2.GetDataListResponse(
-            result="[]"
-        )
-        return res
-
     def GetJoinTable(self, request, context):
         res = libc_to_manage_pb2.GetJoinTableResponse(
             is_ok=True,
             result="['1']",
             schema=["s"]
         )
         return res
 
+    def GetComputationStatus(self, request, context):
+        res = libc_to_manage_pb2.GetComputationStatusResponse(
+            status=common_types_pb2.COMPLETED,
+        )
+        return res
+
     def GetJobErrorInfo(self, request, context):
         res = libc_to_manage_pb2.GetJobErrorInfoResponse(
             job_error_info=JobErrorInfo(
                 what="QMPCJobError",
                 stacktrace=Stacktrace()
             )
         )
         return res
 
     def GetElapsedTime(self, request, context):
-        pass
+        res = libc_to_manage_pb2.GetElapsedTimeResponse(
+            elapsed_time=1,
+        )
+        return res
 
     def GetSchema(self, request, context):
-        pass
+        res = libc_to_manage_pb2.GetSchemaResponse()
+        return res
+
+    def AddShareDataFrame(self, request, context):
+        res = libc_to_manage_pb2.AddShareDataFrameResponse(
+            data_id="data_id"
+        )
+        return res
 
 
 def serve(num: int):
     """ server setting """
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=10))
     libc_to_manage_pb2_grpc.add_LibcToManageServicer_to_server(
         LibToManageServiceServicer(), server)
```

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_files/edge_data.csv` & `quickmpc-0.5.0/tests/unit_tests/pandas/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_files/string_data.csv` & `quickmpc-0.5.0/tests/unit_tests/pandas/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_make_pieces.py` & `quickmpc-0.5.0/tests/unit_tests/utils/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_over_load.py` & `quickmpc-0.5.0/tests/unit_tests/utils/test_over_load.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_parse.py` & `quickmpc-0.5.0/tests/unit_tests/pandas/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import math
 import os
 from typing import List
 
 import numpy as np
 import pytest
 
-from quickmpc import Schema, ShareValueTypeEnum
-from quickmpc.utils.parse_csv import parse, parse_csv
+from quickmpc.pandas.parser import parse, parse_csv
+from quickmpc.proto.common_types.common_types_pb2 import (Schema,
+                                                          ShareValueTypeEnum)
 
 
 def schema_fp(name: str):
     return Schema(name=name,
                   type=ShareValueTypeEnum.SHARE_VALUE_TYPE_FIXED_POINT)
```

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_qmpc.py` & `quickmpc-0.5.0/tests/unit_tests/request/test_qmpc_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,158 +1,166 @@
-from typing import Any, Dict
+import io
+from typing import List, Optional
 
+import pandas as pd
 import pytest
 
-from quickmpc.exception import ArgumentError, QMPCJobError, QMPCServerError
-from quickmpc.qmpc_server import QMPCServer
-
-
-def send_share_param(secrets=[[1, 2, 3]],
-                     schema=["attr1", "attr2", "attr3"],
-                     matching_column=1,
-                     piece_size=1_000_000):
-    return (secrets, schema, matching_column, piece_size)
-
-
-def execute_computation_param(method_id=1,
-                              data_ids=["data_id1", "data_id2"],
-                              src=[0],
-                              target=[1]):
-    return (method_id, data_ids, (src, target))
-
-
-class TestQMPC:
-    qmpc: QMPCServer = QMPCServer(
-        ["http://localhost:50001",
-         "http://localhost:50002",
-         "http://localhost:50003"],
-        "token_demo"
-    )
+import quickmpc.pandas as qpd
+from quickmpc.exception import QMPCServerError
+from quickmpc.proto.common_types import common_types_pb2
+from quickmpc.request.qmpc_request import QMPCRequest
+
+
+def to_string_io(data: List[List]) -> io.StringIO:
+    text_data = "\n".join([",".join(map(str, row)) for row in data])
+    return io.StringIO(text_data)
+
+
+def data_frame(values: List[List] = [[1, 2, 3], [3, 4, 5]],
+               columns: Optional[List[str]] = None,
+               exist_sort_index: bool = True
+               ) -> pd.DataFrame:
+    if columns is None:
+        columns = [f"c{i}" for i in range(len(values[0]))] \
+            if len(values) > 0 else []
+    if columns and exist_sort_index:
+        columns[-1] = "__qmpc_sort_index__"
+    return pd.DataFrame(values, columns=columns)
+
+
+def send_share_param(df: pd.DataFrame = data_frame(), piece_size: int = 1000):
+    return (df, piece_size)
+
+
+class TestQMPCRequest:
+    qmpc_request = QMPCRequest([
+        "http://localhost:50001",
+        "http://localhost:50002",
+        "http://localhost:50003"
+    ])
 
     @pytest.mark.parametrize(
         ("params"), [
+            # 通常ケース
             (send_share_param()),
-            (send_share_param(secrets=[[1], [2], [3]], schema=["a1"])),
-            (send_share_param(secrets=[[0, 0, 0]])),
-            (send_share_param(secrets=[[1e10, 1e10, 1e10]])),
-            (send_share_param(secrets=[[-1e10, -1e10, -1e10]])),
-            (send_share_param(secrets=[[1e-10, 1e-10, 1e-10]])),
-            (send_share_param(secrets=[[-1e-10, -1e-10, -1e-10]])),
+            (send_share_param(df=data_frame([[0, 0, 0]]))),
+            # 境界ケース
+            (send_share_param(df=data_frame([[1e10, 1e10, 1e10]]))),
+            (send_share_param(df=data_frame([[-1e10, -1e10, -1e10]]))),
+            (send_share_param(df=data_frame([[1e-10, 1e-10, 1e-10]]))),
+            (send_share_param(df=data_frame([[-1e-10, -1e-10, -1e-10]]))),
+            (send_share_param(df=data_frame([[-1e-10, -1e-10, -1e-10]]))),
+            # quickmpc.pandasのread_csv経由
+            (send_share_param(df=qpd.read_csv(
+                to_string_io([["id", "c"], ["a", 1]]), index_col="id"))),
         ]
     )
     def test_send_shares(self, params,
                          run_server1, run_server2, run_server3):
-        """ serverにシェアを送れるかのTest"""
-        response: Dict[str, Any] = self.qmpc.send_share(*params)
-        assert (response["is_ok"])
+        self.qmpc_request.send_share(*params)
 
     @pytest.mark.parametrize(
         ("params", "expected_exception"), [
             # piece_sizeが範囲外
-            (send_share_param(piece_size=500), RuntimeError),
-            (send_share_param(piece_size=10000000), RuntimeError),
-            # matching_columnが範囲外
-            (send_share_param(matching_column=-1), RuntimeError),
-            (send_share_param(matching_column=4), RuntimeError),
+            (send_share_param(piece_size=500),
+             RuntimeError),
+            (send_share_param(piece_size=10000000),
+             RuntimeError),
             # empty
-            (send_share_param(secrets=[]), TypeError),
+            (send_share_param(df=data_frame([])),
+             RuntimeError),
             # schemaに同じものが含まれる
-            (send_share_param(schema=["a1", "a1", "a2"]), RuntimeError),
+            (send_share_param(df=data_frame(columns=["a1", "a1", "a2"])),
+             RuntimeError),
             # 列数が異なる
-            (send_share_param(secrets=[[1, 1, 2], [2, 3]]), RuntimeError),
-            # 文字列が含まれる
-            (send_share_param(secrets=[["a", 2, 3]]), ArgumentError),
+            (send_share_param(df=data_frame([[1, 1, 2], [2, 3]])),
+             RuntimeError),
             # Noneが含まれる
-            (send_share_param(secrets=[[None, 2, 3]]), TypeError),
+            (send_share_param(df=data_frame([[None, 2, 3]])),
+             RuntimeError),
+            # __qmpc_sort_index__が含まれない
+            (send_share_param(df=data_frame([[1, 2], [3, 4]],
+                                            exist_sort_index=False)),
+             RuntimeError),
+            # __qmpc_sort_index__しかない
+            (send_share_param(df=data_frame([[0], [1]])),
+             RuntimeError),
+            # pandasのread_csv経由
+            (send_share_param(df=pd.read_csv(to_string_io([["id", "c"],
+                                                           ["a", 1]]))),
+             RuntimeError),
         ]
     )
     def test_send_shares_errorhandring(self, params, expected_exception,
                                        run_server1, run_server2, run_server3):
         with pytest.raises(expected_exception):
-            self.qmpc.send_share(*params)
+            self.qmpc_request.send_share(*params)
 
-    def test_delete_shares(self, run_server1, run_server2, run_server3):
-        """ serverにシェア削除要求を送れるかのTest"""
-        response: Dict[str, Any] = self.qmpc.delete_share([])
-        assert (response["is_ok"])
+    def test_sum(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.sum(["data_id1"], [1, 2, 3])
 
-    @pytest.mark.parametrize(
-        ("params"), [
-            execute_computation_param(method_id=1, target=[]),
-            execute_computation_param(method_id=2, target=[]),
-            execute_computation_param(method_id=3, target=[]),
-            execute_computation_param(method_id=4),
-            execute_computation_param(method_id=5),
-            execute_computation_param(method_id=6),
-        ]
-    )
-    def test_execute_computation(self, params,
-                                 run_server1, run_server2, run_server3):
-        """ serverに計算リクエストを送れるかのTest"""
-        response: Dict[str, Any] = self.qmpc.execute_computation(*params)
-        assert (response["is_ok"])
+    def test_mean(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.mean(["data_id1"], [1, 2, 3])
 
-    @pytest.mark.parametrize(
-        ("params", "expected_exception"), [
-            # QMPCJobErrorとして例外がthrowされるか
-            (execute_computation_param(src=[1000000000]),
-             QMPCJobError),
-            # QMPCServerErrorとして例外がthrowされるか
-            (execute_computation_param(data_ids=["UnregisteredDataId", "id2"]),
-             QMPCServerError),
-        ]
-    )
-    def test_execute_computation_errorhandring(self, params,
-                                               expected_exception,
-                                               run_server1,
-                                               run_server2,
-                                               run_server3):
-        with pytest.raises(expected_exception):
-            self.qmpc.execute_computation(*params)
+    def test_variance(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.variance(["data_id1"], [1, 2, 3])
 
-    def test_get_computation_resultRequest(self, run_server1,
-                                           run_server2, run_server3):
-        """ serverから結果を得られるかのTest """
-        job_uuid: str = "uuid"
-        response: Dict[str, Any] = self.qmpc.get_computation_result(
-            job_uuid, None)
-        assert (response["is_ok"])
-
-    def test_get_data_list(self, run_server1, run_server2, run_server3):
-        """ serverにシェアを送れるかのTest"""
-        response: Dict[str, Any] = self.qmpc.get_data_list()
-        assert (response["is_ok"])
+    def test_correl(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.correl(["data_id1"], [1, 2, 3], [4])
 
-    def test_get_job_error_info(self, run_server1, run_server2, run_server3):
-        # 例外がthrowされないことをテスト
-        response: Dict[str, Any] = self.qmpc.get_job_error_info("test")
+    def test_meshcode(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.meshcode(["data_id1"], [1, 2, 3])
 
-        assert (response["is_ok"])
-        for res in response["job_error_info"]:
-            assert (res.what == "QMPCJobError")
-
-    qmpc_failed: QMPCServer = QMPCServer(
-        # 通信失敗する場合をテストする用のサーバー
-        ["http://localhost:50011",
-         "http://localhost:50012",
-         "http://localhost:50013"],
-        "token_demo",
+    def test_join(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.join(["data_id1"])
+
+    def test_get_computation_result(self,
+                                    run_server1, run_server2, run_server3):
+        self.qmpc_request.get_computation_result("job_uuid", None)
+
+    def test_get_computation_status(self,
+                                    run_server1, run_server2, run_server3):
+        response = self.qmpc_request.get_computation_status("test")
+        assert response.job_statuses == [
+            common_types_pb2.COMPLETED for _ in range(3)]
+
+    def test_get_job_error_info(self, run_server1, run_server2, run_server3):
+        response = self.qmpc_request.get_job_error_info("test")
+        for res in response.job_error_info:
+            assert res.what == "QMPCJobError"
+
+    def test_get_elapsed_time(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.get_elapsed_time("job_uuid")
+
+    def test_delete_share(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.delete_share(["data_id"])
+
+    def test_add_share_data_frame(self, run_server1, run_server2, run_server3):
+        self.qmpc_request.add_share_data_frame("id1", "id2")
+
+
+class TestQMPCRequestFailed:
+    # 通信失敗する場合をテストする用のサーバー
+    qmpc_request_failed = QMPCRequest(
+        ["http://localhost:33333",
+         "http://localhost:44444",
+         "http://localhost:55555"],
         10,
         0
     )
 
     @pytest.mark.parametrize(
         ("function", "argument"), [
-            (qmpc_failed.send_share, send_share_param()),
-            (qmpc_failed.delete_share, [[]]),
-            (qmpc_failed.execute_computation, execute_computation_param()),
-            (qmpc_failed.get_data_list, []),
-            (qmpc_failed.get_elapsed_time, ["uuid"]),
-            (qmpc_failed.get_computation_result, ["uuid", None]),
-            (qmpc_failed.get_job_error_info, ["uuid"]),
+            (qmpc_request_failed.send_share, send_share_param()),
+            (qmpc_request_failed.delete_share, ["data_id"]),
+            (qmpc_request_failed.sum, (["data_id"], [1])),
+            (qmpc_request_failed.get_elapsed_time, (["uuid"])),
+            (qmpc_request_failed.get_computation_result, ["uuid", None]),
+            (qmpc_request_failed.get_job_error_info, ["uuid"]),
+            (qmpc_request_failed.add_share_data_frame, ["id1", "id2"]),
         ]
     )
     def test_retry(self, function, argument, caplog,
                    run_server1, run_server2, run_server3):
-        # 10回の retry に失敗したら "All 10 times it was an error" が log に出るかをテスト
-        _ = function(*argument)
-        assert "channel の準備が出来ません" in caplog.text
+        with pytest.raises(QMPCServerError) as e:
+            _ = function(*argument)
+        assert str(e.value) == "channel の準備が出来ません"
```

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_random.py` & `quickmpc-0.5.0/tests/unit_tests/share/test_random.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from decimal import Decimal
 
 import pytest
 
-from quickmpc.utils.random import ChaCha20, RandomInterface
+from quickmpc.share.random import ChaCha20, RandomInterface
 
 
 class TestCsprng:
     rnd: RandomInterface = ChaCha20()
 
     @pytest.mark.parametrize(
         ("lower", "upper"),
```

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_share_recons.py` & `quickmpc-0.5.0/tests/unit_tests/share/test_share_recons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from decimal import Decimal
 
 import numpy as np
 import pytest
 
 from quickmpc.exception import ArgumentError
-from quickmpc.share import Share
+from quickmpc.share.share import Share
 
 
 class TestQMPC:
 
     @staticmethod
     def isclose(val, true_val):
         ok: bool = True
```

### Comparing `quickmpc-0.4.2/tests/unit_tests/test_share_sharize.py` & `quickmpc-0.5.0/tests/unit_tests/share/test_share_sharize.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from decimal import Decimal
 from typing import List
 
 import numpy as np
 import pytest
 
 from quickmpc.exception import ArgumentError
-from quickmpc.share import Share
+from quickmpc.share.share import Share
 
 
 def sharize_params(secrets=[1], party_size=3):
     return (secrets, party_size)
 
 
 class TestQMPC:
```

