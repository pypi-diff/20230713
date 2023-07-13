# Comparing `tmp/ez-a-sync-0.6.1.dev7.tar.gz` & `tmp/ez-a-sync-0.6.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.6.1.dev7.tar", last modified: Mon Jul 10 00:57:15 2023, max compression
+gzip compressed data, was "ez-a-sync-0.6.1.dev9.tar", last modified: Tue Jul 11 06:03:06 2023, max compression
```

## Comparing `ez-a-sync-0.6.1.dev7.tar` & `ez-a-sync-0.6.1.dev9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.192200 ez-a-sync-0.6.1.dev7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.192200 ez-a-sync-0.6.1.dev7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/TODO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1121 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/prio_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-10 00:57:15.000000 ez-a-sync-0.6.1.dev7/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-10 00:57:15.000000 ez-a-sync-0.6.1.dev7/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 00:57:15.000000 ez-a-sync-0.6.1.dev7/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-10 00:57:15.000000 ez-a-sync-0.6.1.dev7/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-10 00:57:15.000000 ez-a-sync-0.6.1.dev7/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-10 00:57:15.200200 ez-a-sync-0.6.1.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 00:57:15.196200 ez-a-sync-0.6.1.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-10 00:56:54.000000 ez-a-sync-0.6.1.dev7/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.549532 ez-a-sync-0.6.1.dev9/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.541532 ez-a-sync-0.6.1.dev9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.545532 ez-a-sync-0.6.1.dev9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-11 06:03:06.549532 ez-a-sync-0.6.1.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/TODO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.545532 ez-a-sync-0.6.1.dev9/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.545532 ez-a-sync-0.6.1.dev9/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.545532 ez-a-sync-0.6.1.dev9/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.545532 ez-a-sync-0.6.1.dev9/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.545532 ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1121 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/prio_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.549532 ez-a-sync-0.6.1.dev9/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-11 06:03:06.000000 ez-a-sync-0.6.1.dev9/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-11 06:03:06.000000 ez-a-sync-0.6.1.dev9/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 06:03:06.000000 ez-a-sync-0.6.1.dev9/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-11 06:03:06.000000 ez-a-sync-0.6.1.dev9/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-11 06:03:06.000000 ez-a-sync-0.6.1.dev9/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-11 06:03:06.549532 ez-a-sync-0.6.1.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 06:03:06.549532 ez-a-sync-0.6.1.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-11 06:02:51.000000 ez-a-sync-0.6.1.dev9/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.6.1.dev7/.github/workflows/codeql.yaml` & `ez-a-sync-0.6.1.dev9/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/.github/workflows/mypy.yaml` & `ez-a-sync-0.6.1.dev9/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/.github/workflows/pytest.yaml` & `ez-a-sync-0.6.1.dev9/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/.github/workflows/release.yaml` & `ez-a-sync-0.6.1.dev9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/LICENSE.txt` & `ez-a-sync-0.6.1.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/README.md` & `ez-a-sync-0.6.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/__init__.py` & `ez-a-sync-0.6.1.dev9/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/_bound.py` & `ez-a-sync-0.6.1.dev9/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/_flags.py` & `ez-a-sync-0.6.1.dev9/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/_helpers.py` & `ez-a-sync-0.6.1.dev9/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/_kwargs.py` & `ez-a-sync-0.6.1.dev9/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/_meta.py` & `ez-a-sync-0.6.1.dev9/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/_typing.py` & `ez-a-sync-0.6.1.dev9/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/abstract.py` & `ez-a-sync-0.6.1.dev9/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/base.py` & `ez-a-sync-0.6.1.dev9/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/config.py` & `ez-a-sync-0.6.1.dev9/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/decorator.py` & `ez-a-sync-0.6.1.dev9/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/exceptions.py` & `ez-a-sync-0.6.1.dev9/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/modified.py` & `ez-a-sync-0.6.1.dev9/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/modifiers/__init__.py` & `ez-a-sync-0.6.1.dev9/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.6.1.dev9/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.6.1.dev9/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/modifiers/limiter.py` & `ez-a-sync-0.6.1.dev9/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/modifiers/manager.py` & `ez-a-sync-0.6.1.dev9/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.6.1.dev9/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/primitives/_debug.py` & `ez-a-sync-0.6.1.dev9/a_sync/primitives/_debug.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/primitives/executor.py` & `ez-a-sync-0.6.1.dev9/a_sync/primitives/executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/event.py` & `ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/prio_semaphore.py` & `ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/prio_semaphore.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,26 +51,25 @@
         if priority not in self._context_managers:
             context_manager = self._context_manager_class(self, priority, name=self.name)
             heapq.heappush(self._waiters, context_manager)  # type: ignore [misc]
             self._context_managers[priority] = context_manager
         return self._context_managers[priority]
     
     def _wake_up_next(self) -> None:
-        if self._waiters:
+        while self._waiters:
             manager = heapq.heappop(self._waiters)
-            manager._wake_up_next()
-            self._heap_push(manager)
-    
-    def _heap_push(self, manager: "_AbstractPrioritySemaphoreContextManager[PT]") -> None:
-        if len(manager):
-            # There are still waiters, put the manager back
-            heapq.heappush(self._waiters, manager)  # type: ignore [misc]
-        else:
-            # There are no more waiters, get rid of the empty manager
-            self._context_managers.pop(manager._priority)
+            if len(manager):
+                manager._wake_up_next()
+                if len(manager):
+                    # There are still waiters, put the manager back
+                    heapq.heappush(self._waiters, manager)  # type: ignore [misc]
+                else:
+                    # There are no more waiters, get rid of the empty manager
+                    self._context_managers.pop(manager._priority)
+                break
 
 class _AbstractPrioritySemaphoreContextManager(Semaphore, Generic[PT]):
     _loop: asyncio.AbstractEventLoop
     _waiters: List[asyncio.Future]  # type: ignore [assignment]
     
     @property
     def _priority_name(self) -> str:
@@ -80,14 +79,17 @@
         self._parent = parent
         self._priority = priority
         super().__init__(0, name=name)
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} parent={self._parent} {self._priority_name}={self._priority} waiters={len(self)}>"
     
+    def _repr_no_parent_(self) -> str:
+        return f"<{self.__class__.__name__} {self._priority_name}={self._priority} waiters={len(self)}>"
+    
     def __lt__(self, other) -> bool:
         if type(other) is not type(self):
             raise TypeError(f"{other} is not type {self.__class__.__name__}")
         return self._priority < other._priority
     
     @cached_property
     def loop(self) -> asyncio.AbstractEventLoop:
```

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/primitives/locks/semaphore.py` & `ez-a-sync-0.6.1.dev9/a_sync/primitives/locks/semaphore.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/a_sync/property.py` & `ez-a-sync-0.6.1.dev9/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.6.1.dev9/ez_a_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/setup.py` & `ez-a-sync-0.6.1.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/tests/fixtures.py` & `ez-a-sync-0.6.1.dev9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/tests/test_base.py` & `ez-a-sync-0.6.1.dev9/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/tests/test_cache.py` & `ez-a-sync-0.6.1.dev9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/tests/test_decorator.py` & `ez-a-sync-0.6.1.dev9/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/tests/test_executor.py` & `ez-a-sync-0.6.1.dev9/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/tests/test_limiter.py` & `ez-a-sync-0.6.1.dev9/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/tests/test_meta.py` & `ez-a-sync-0.6.1.dev9/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.1.dev7/tests/test_semaphore.py` & `ez-a-sync-0.6.1.dev9/tests/test_semaphore.py`

 * *Files identical despite different names*

